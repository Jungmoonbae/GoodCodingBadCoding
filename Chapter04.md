## CHAPTER 4. 들여 쓸 때 좋은 코딩 습관

1.중괄호위치
함수의 시작이나 블록의 시작점과 끝점을 알려주는 {  }(중괄호)는 들여쓰기가 굉장히 중요!

<pre>
<code>

첫 번째 Style : 중괄호를 문장과 한 줄에 쓰는 방법
void main(){
int i,j;
 for(i=2; j<=9; i++) {
   for(j=1; j<=9; j++) {
     printf(“%d x %d = %2d”, I, j, i*j); }
  printf(“\n”); } }
  
  
두 번째 Style : 중괄호를 문장과 다른 줄에 쓰는 방법
void main()
{
int i,j;
for(i=2; j<=9; i++)
{
for(j=1; j<=9; j++)
{
printf(“%d x %d = %2d”, I, j, i*j);
}
printf(“\n”);
}
}

세 번째 Style : 첫 번째와 두 번째를 혼합한 방법
void main()
{
int i,j;
  for(i=2; j<=9; i++) {
    for(j=1; j<=9; j++) {
     printf(“%d x %d = %2d”, i, j, i*j);
    }
   printf(“\n”);
  }
}



</code>
</pre>

2.중괄호위치를 통일 시켜라
 중괄호의 위치를 통일 시켜주어야 한다.
 문장이 길어질수록 통일된 중괄호가 도움이된다.

<pre>
<code>

몸체를 들여 쓰지 않는 경우
void main()
{
printf(“들여쓰기 예제\n”);
}

몸체만 들여 쓴 경우
void main()
{
 printf(“들여쓰기 예제\n”);
}

중괄호까지  들여 쓴 경우
void main()
   {
   printf(“들여쓰기 예제\n”);
   }

</code>
</pre>

3. 내부블록을 들여 써라
 함수 내에 블록이 존재한다면 ?
 함수의 몸체를 이루는 문장이 시작되는 지점에 맞추어 중괄호를 써준다.
 그리고 블록을 이루는 문장은 중괄호보다 더 들여써주면 좋다.

<pre>
<code>

int main()
{
int a=1;
if(a==1){
int a=2;
printf(“블록 내에서 a는 %d”, a);
}
printf(“블록 밖에서 a는 %d”, a);
return 0;
}



int main()
{
  int a=1;
  
  if(a==1){
    int a=2;
    printf(“%d”, a);
  }
  printf(“%d”, a);
return 0;
}
</code>
</pre>
