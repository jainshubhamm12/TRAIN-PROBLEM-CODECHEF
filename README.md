# TRAIN-PROBLEM-CODECHEF

#include<iostream>
using namespace std;

int main(){
	
	int t;

	cin>>t;
	int t1= t;
	string s[t];
	int a[t];
	int res[t];
	int i=0;
	while(t-->0){
		cin>>a[i];
		i++;
	}
	i=0;
int temp;
int seatno;	
while(i<t1){
		temp=a[i];
		seatno=temp%8;
		
		if(seatno==1)
		{	res[i]=temp+3;	
			s[i]="LB";
	i++;
	continue;
	}
	if(seatno==2)
		{	res[i]=temp+3;	
			s[i]="MB";
				i++;
	continue;
	}
	
	if(seatno==3 )
		{	res[i]=temp+3;	
				s[i]="UB";
				i++;
	continue;
	}
	
		if(seatno==4)
		{	res[i]=temp-3;	
			s[i]="LB";
				i++;
	continue;
	}
	if(seatno==5)
		{	res[i]=temp-3;	
	s[i]="MB";
	i++;
	continue;
	}
	if(seatno==6)
		{	res[i]=temp-3;	
	s[i]="UB";
	i++;
	continue;
	}
	if(seatno==7)
		{res[i]=temp+1;	
	s[i]="SU";
	i++;
	continue;
		}
	
	if(seatno==0)
{	res[i]=temp-1;
	s[i]="SL";
	i++;
	continue;
	}
	
	
	}	

for(int j =0;j<t1;j++){
	cout<<res[j]<<s[j]<<endl;

}
}
