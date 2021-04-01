# Hacker-rank-Solution-
I have written code for Marc's Cakewalk question on hacker rank in c++
#include<iostream>
#include<set>
#include<limits>
#include<cmath>
#include<algorithm>

using namespace std;
#define ll long long int
int main()
{
    ios_base::sync_with_stdio(0);
    cin.tie(0);
    cout.tie(0);
    
    multiset<int,greater<int>>set1;
    int n;
    cin>>n;
    int val;
    for(auto i=0;i<n;i++)
    {
        cin>>val;
        set1.insert(val);
    }
    int m=0;
    ll miles=0;
    for(auto itr=set1.begin();itr!=set1.end();itr++)
    {
        miles+=(*(itr)*(pow(2,m)));
        m++;
    }
    cout<<miles<<endl;
    return 0;
}
