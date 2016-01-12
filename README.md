# prime-no.-betwen-given-range
void main()
{
int n1,n2,i,j,f,t,count=0;
scanf("%d %d ",&n1,&n2);
if(n2<2)
printf("no prime no.");
t=n1;
if(n1%2==0)
n1++;
for(i=n1;i<=n2;i=i+2)
{
f=0;
for(j=2;j<=i;j<=i/2;j++)
{
if((i%j)==0)
{
f=1;
break;
}
}
if(f==0)
{
printf("%d\n",i);
count++;
}
}
printf("%d",t);
}
