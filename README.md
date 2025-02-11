# selection_sort

#include<bits/stdc++.h>
using namespace std;

int main(){
int n,i,j,index;
int arr[600];
cout<<"ENTER SIZE ";
cin>>n;
for(i=0;i<n;i++){
    cin>>arr[i];
}


for( i=0;i<n-1;i++){
 index =i;
for ( j=i+1;j<n;j++ ){

    if(arr[j]<arr[index]){

        index=j;

    }
}
swap(arr[index],arr[i]);

}

for(i=0;i<n;i++){

    cout<<arr[i]<<"  ";
}

}
