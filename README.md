#include <bits/stdc++.h>

using namespace std;

int main()
{
    int t;
    cin>>t;
    int test=1;
    while(t)
    {
        int x,cnt=0;
        char arr[105];
        cin>>x;
        for(int i=0; i<x; i++)
        {
            cin>>arr[i];
        }
        for(int j=0; j<x; j++)
        {
            if(arr[j]=='.')
            {
                cnt++;
                j=j+2;
            }
            else
                continue;
        }
        cout<<"Case "<<test<<": "<<cnt<<endl;
        t--;
        test++;
    }
    return 0;
}
