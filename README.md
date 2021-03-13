# Hacker-rank-Solution-
I have written code for apple and orange question on hacker rank in c++
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int starth,endh,applet,oranget,napp,norange;
    cin>>starth>>endh>>applet>>oranget>>napp>>norange;
    int nap[napp];
    for(int i=0;i<napp;i++)
    {
        cin>>nap[i];
    }
    int nor[norange];
       for(int i=0;i<norange;i++)
    {
        cin>>nor[i];
    }
    int acount=0;
    int ocount=0;
    
    for(int i=0;i<napp;i++)
    {
        if(((applet+nap[i])>=starth)&&((applet+nap[i])<=endh))
        {
            acount++;
        }
        
        
    }
    for(int i=0;i<norange;i++)
    {
        if(((oranget+nor[i])<=endh)&&((oranget+nor[i])>=starth))
        {
            ocount++;
        }
    }
    cout<<acount<<endl;
    cout<<ocount<<endl;
}
