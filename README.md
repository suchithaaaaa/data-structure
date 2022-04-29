# data-structure
**  singly linked list**
#include&lt;iostream&gt;
#include&lt;conio.h&gt;
#include&lt;stdlib.h&gt;
using namespace std;
int
cost[10][10],qu[10],front,rare,visit[10],visited[10
];
int main()
{
int m,n,j,i,v,k;
cout &lt;&lt;&quot;Enter no of vertices:&quot;;
cin &gt;&gt; n;
cout &lt;&lt;&quot;Enter no of edges:&quot;;
cin &gt;&gt; m;
cout &lt;&lt;&quot;\nEDGES \n&quot;;
for(k=1; k&lt;=m; k++)
{
cin &gt;&gt;i&gt;&gt;j;
cost[i][j]=1;
}
cout &lt;&lt;&quot;Enter initial vertex to traverse from:&quot;;

cin &gt;&gt;v;
cout &lt;&lt;&quot;Visitied vertices:&quot;;
cout &lt;&lt;v&lt;&lt;&quot; &quot;;
visited[v]=1;
k=1;
while(k&lt;n)
{
for(j=1; j&lt;=n; j++)
if(cost[v][j]!=0 &amp;&amp; visited[j]!=1 &amp;&amp; visit[j]!=1)
{
visit[j]=1;
qu[rare++]=j;
}
v=qu[front++];
cout&lt;&lt;v &lt;&lt;&quot; &quot;;
k++;
visit[v]=0;
visited[v]=1;
}
return 0;
}
<br>
