# CTCI
#include <iostream>
#include<string>
using namespace std;

bool isUnique(string s)
{
    if (s.length()>256)
    return false;
bool check[256];
for(int i=1;i<s.length();i++)
{
    int val = s.at(i);
    if(check[val])
    return false;
check[val]=true;
}
return true;
}


int main() {
    char s[257];
    bool check;
    check = isUnique(s);
    if(check)
    cout<<"unique";
    else
    cout<<"not unique";
    
    
   
	// your code goes here
	return 0 ;
}
