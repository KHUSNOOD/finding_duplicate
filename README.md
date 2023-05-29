#include<iostream>
using namespace std;
void dupli(int a[],int b[]){
    int dup=0;
    for(int i=0; i<11; i++){
        if(a[i]==a[i+1] && a[i]!=dup){
            b[a[i]]++;
            dup=a[i];
        }
    }
    for(int i=0; i<=20; i++){
        if(b[i]==1 && i!=0){
            cout<<i<<" ";
        }
    }
}
int main(){
    int a[]={3,6,8,8,10,12,15,15,15,20};
    int b[20];
    dupli(a,b);
    // for(int i=0; i<20; i++){
    //     cout<<b[i]<<" ";
    // }
    return 0;
}
