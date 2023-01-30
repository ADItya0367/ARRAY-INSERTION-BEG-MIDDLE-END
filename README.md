# ARRAY-INSERTION-BEG-MIDDLE-END
Here i had provided the code that how insertion operation is performed in an array at the beginning ending and at the middle .


#include<iostream>
#include<conio.h>
using namespace std;
class A
{
    public:
    void func()
    {
        int pos,ele,i;
        
        int arr[7]={1,2,3,4,5};
        int size=sizeof(arr)/sizeof(arr[0]);
        cout<<"the elements of the array are "<<endl;
        for(i=0;i<5;i++)
        cout<<arr[i]<<endl;
        cout<<"enter the elements-"<<endl;
        
        cin>>ele;
        cout<<"enter the position"<<endl;
        cin>>pos;
        size=size+1;
        for(i=size-1;i>=pos-1;i--)
        {
            arr[i+1]=arr[i];
            arr[pos-1]=ele;
            
        }
        for(i=0;i<size;i++)
        cout<<arr[i]<<endl;
    }
};
int main()
{
    A obj;
    obj.func();
    return 0;
}
                           
  //PLEASE DROP A STAR IF SATISFIED !!
