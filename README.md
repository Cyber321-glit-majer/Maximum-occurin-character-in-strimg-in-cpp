# Maximum-occurin-character-in-strimg-in-cpp
**CODE**
```

** #include<bits/stdc++.h>**
using namespace std;
int main()
{
    string s="hekkkklllo";
    int max=0;
    char cnt[26]={0};
    char res;
    for(int i=0;i<s.size();i++)
    {
        cnt[s[i]-'a']++;
    }
    for(int i=0;i<26;i++)
    {
        if(cnt[i]>max)
        {
            max=cnt[i];
            res='a'+i;
        }
    }
    cout<<res;
    
}
