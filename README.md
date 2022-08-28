# cpp-program-5
yogi is a young coder who likes music a lot....



#include<cstdio>
#include<iostream>
#include<algorithm>

using namespace std;
pair<int,int> v[109];
class LoveForMusic
{int n,k;
public:
void Instruments()
 {cin>>n;
  cin>> k;
for(int i=0;i<n;i++)
{
cin>>v[i].first;
v[i].second=i;
}
sort(v,v+n);
int rem=k,ans=0;
for(int i=0;i<n;i++)
{
if(rem-v[i].first>=0)
{
ans++;
rem-=v[i].first;
}
}
cout<<ans<<endl;
for(int i=0;i<ans;i++)
{
cout<<v[i].second+1<<" ";
}
}
};
int main()
{LoveForMusic Learning;
Learning.Instruments();
return 0;
}


