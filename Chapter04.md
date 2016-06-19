## CHAPTER 4. 들여 쓸 때 좋은 코딩 습관
<pre>
중괄호위치
함수의 시작이나 블록의 시작점과 끝점을 알려주는 {  }(중괄호)는 들여쓰기가 굉장히 중요!
</pre>
<code>
첫 번째 Style : 중괄호를 문장과 한 줄에 쓰는 방법
void main(){
int i,j;
for(i=2; j<=9; i++){
for(j=1; j<=9; j++){
printf(“%d x %d = %2d”, &i,&j,&i*j);}
printf(“\n”);}
}
</code>
두 번째 Style : 중괄호를 문장과 다른 줄에 쓰는 방법
void main()
{
int i,j;
for(i=2; j<=9; i++){
for(j=1; j<=9; j++){
printf(“%d x %d = %2d”, &i,&j,&i*j);
}
printf(“\n”);
}
}
