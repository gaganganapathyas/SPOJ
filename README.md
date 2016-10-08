#include<stdio.h>
int rev(int);
int main()
{
 int N,a,b,i,revsum;
 scanf("%d",&N);
 for(i=1;i<=N;i++)
  { 
   scanf("%d %d",&a,&b);
   revsum = rev(rev(a)+rev(b));
   printf("%d\n",revsum);
  }
 return 0;
}
int rev(int num)
 {
  int revn=0,rem;
  while(num>0)
   {
    rem=num%10;
    num=num/10;
    revn=revn*10+rem;
   }
   return revn;
 }
        
    
# SPOJ
All the SPOJ Problems
