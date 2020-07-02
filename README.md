#include <iostream>
#include <string>
#include <algorithm>
using namespace std;

int main()
{
    int counter=0 ;

    string name;
    cin >> name;
    sort(name.begin(), name.end());
    string temp="";
    temp = name;

    for (int i = 0; i <temp.length()  ; i++)
    {


        if (name[i]==name[i+1])
            counter++;
    }

    int final = temp.length() - counter;
    if (final%2==0)
    {
        cout <<"CHAT WITH HER!" << endl;
    }
    else
        cout <<"IGNORE HIM!" << endl;
}
