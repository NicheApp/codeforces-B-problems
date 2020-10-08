# Here we will discuss codeforces 1000-1300 level problems (50 ques) 
# Ques - 1 
### https://codeforces.com/contest/1288/problem/B
MY soln-
#include <bits/stdc++.h>
using namespace std;

int main()
{ typedef long long ll;
	int t; 
cin>>t; 
while(t--){ 
ll a,b,mx,mn,count=0; 
cin>>a>>b; 
if(b<9) 
{cout<<0<<endl;continue;} 
mx=b; 
mn=a; 
while(mx!=0) 
{ 
mx/=10; 
count++; 	
}
if(b<(pow(10,count)-1)) 
{
	cout<<mn*(count-1)<<endl; 
}else 
{ 
cout<<mn*count<<endl; 	
	
} 


} 
    return 0; 
} 
