# Hacker-rank-Solution-
I have written this code in CPP at hackerank on between the sets
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int na1,na2;
    cin>>na1>>na2;
    int arr1[na1];
    int arr2[na2];
    vector<int>v;
    for(int i=0;i<na1;i++)
    {
        cin>>arr1[i];
    }
    for(int i=0;i<na2;i++)
    {
        cin>>arr2[i];
    }
    int fac=1;
    while(fac<=100)
    {
        int count1=0;
        int count2=0;
        for(int i=0;i<na1;i++)
        {
            if((fac%arr1[i])==0)
            {
                count1++;
            }
        }
        for(int i=0;i<na2;i++)
        {
            if((arr2[i]%fac)==0)
            {
                count2++;
            }
        }
        if((count1==na1)&&(count2==na2))
        {
            v.push_back(fac);
        }
        fac++;
    }
    
    cout<<v.size()<<endl;
    
    return 0;
}
