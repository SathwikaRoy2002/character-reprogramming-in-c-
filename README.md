# character-reprogramming-in-c++
#include <bits/stdc++.h>
#pragma GCC optimize("Ofast")
#pragma GCC optimize("unroll-loops")
#pragma GCC target("avx2")
#pragma GCC optimize("Os")
using namespace std;
#define ll long long
#define ccc ios::sync_with_stdio(0); cin.tie(0); cout.tie(0);
int main(int argc, char const *argv[])
{
    ccc
    string str;
    cin>>str;
    int u,d,l,r,i;
    u=d=l=r=0;
    for(i=0;i<str.length();i++)
    {
        if(str[i]=='U')
            u++;
        else if(str[i]=='D')
            d++;
        else if(str[i]=='L')
            l++;
        else
        r++;
    }
    cout<<2*(min(u,d)+min(l,r));
    return 0;
}
