#include<stdio.h>
void main()
{
	int a,b,c,t,max,min,mid;
	printf("Please enter the three integers that you want compare:\n");
	scanf("%d%d%d",&a,&b,&c);
	t=a>b;
	switch(t){
    	case 0:
		max=b; break;
    	case 1:
		max=a; break;
	}
	t=max>c;
	switch(t){
    	case 0:
		max=c; break;
	}
	t= a<b;
	switch(t){
    	case 0:
		min=b; break;
    	case 1:
		min=a; break;
	}
	t=min>c;
	switch(t){
	    case 1:
	    min=c; break; 
	    
	}
	t= a <max && a> min;
	switch(t){
	    case 1 :
	    mid=a;
	    case 0 :
	    mid=b;
	}
	t=c<max && c>min;
	switch(t){
	    case 1 :
	    mid = c;
	}
	
	
	
	
	printf("max=%d\n",max);
	printf("midlle=%d\n",mid);
	printf("min=%d\n",min);
}
