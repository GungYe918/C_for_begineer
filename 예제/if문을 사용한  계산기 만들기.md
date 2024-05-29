#if 문을 사용하여 계산기를 만드는 과정이다.

>1. 두 정수의 덧셈을 계산한다고 가정, 2개의 변수를 담을 #int 형 변수 2개와, 연산기호를 담을 #char 형 변수를 선언한다.
>2. #if 문의 조건을 연산기호에 따라 설정한 뒤 각 연산기호에 맞는 문구를 출력하도록 코딩한다.
>3. 컴파일 후 실행한다.

다음은 #if 문을 사용하여 2개의 정수에 관하 사칙연산을 수행하는 코드이다.

```C
#include <stdio.h>
int main(void)
{
	int a, b;
	char operand;

	printf("두 정수를 입력하시오: ");
	scanf("%d, %d\n", &a, &b);
	printf("연산기호를 입력하시오: ");
	scanf("%c", &operand);

	if(operand == '+')
	{
		printf("%d + %d = %d", a, b, a+b);
	}
	else if(operand == '-')
	{
		printf("%d - %d = %d",a, b, a-b);
	}
	else if(operand == '*')
	{
		printf("%d * %d = %d", a,  b, a*b);
	}
	else if(operand == '/')
	{
		printf("%d / %d = %d", a, b, a/b);	
	}
	else
	{
		printf("Invaild operand! choose the right operand");
	}
	return 0;
}
```

a = 4, b =2, operand = '+'로 설정하고 출력한 결과는 다음과 같다.

```C
4 + 2 = 6

done
```

###### 참고문서
- [[2-1 변수의 자료형|변수의 자료형]]
- [[3-2. 형식지정자에 관하여|형식지정자]]
- [[3-1. 숫자, 문자를 입력하려면?|숫자 또는 문자를 입력하려면?]]
- [[4-1. if문|if문]]

<br>



