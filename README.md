# Hacker-rank-Solution-
I have written code for Bill Division on hacker rank in c++
#include <bits/stdc++.h>

using namespace std;
int main()
{
    int arrs,arrel,paid,refund;
    cin>>arrs>>arrel;
    int arr[arrs];
    for(int i=0;i<arrs;i++)
    {
        cin>>arr[i];
    }
    cin>>paid;
    int sum =0;
    for(int i=0;i<arrs;i++)
    {
        if(i!=arrel)
        {
            sum+=arr[i];
        }
    }
    if(sum/2==paid)
    {
        cout<<"Bon Appetit";
    }else 
    {
        refund=paid-(sum/2);
        cout<<refund;
    }
    return 0;
}
