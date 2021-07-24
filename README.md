# Prime-Factorization-Number

```C++
#include<bits/stdc++.h>

using namespace std;

int main()
{
    int num,n,i;
    cin>>num;
    n=num;
    vector <int> fact;
    for (i=2;i<=n;)
    {
        if (n%i==0)
        {
            fact.push_back (i);
            n=n/i;
            i=2;
        }
        else
            i++;
    }
    for (int j=0;j<fact.size();j++)
    {
        cout<<fact[j]<<" ";
    }
    cout <<" = " <<num;
}
```
