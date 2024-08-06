#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;

number(int no)
{
	int num,health=3;
	while(num!=no && health>0)
	{
		cin>>num;
		health--;
		if(num>no)
		{
			cout<<"Guess Lower"<<endl;
			
		}
		else if(num<no)
		{
			cout<<"Guess higher "<<endl;
			
		}
	
	}
	
	if(num==no)
	{
		cout<<"Correct guess"<<endl;
	}
	else if(num!=no && health==0)
	{
		cout<<" You Lost \n Correct ans is "<<no<<endl;
	}
}
int main()
{
	cout<<"Guess Game \n Total no of guess =3"<<endl;
	srand((unsigned int) time(NULL));
    int no=(rand() % 100)+1;
    cout<<"Guess the number (1-100):";
    number(no);
}# codesoft
