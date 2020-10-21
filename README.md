# Operator-DevisionDemo
형변환 연산자

package org.opentutorials.javatutorials.operator;

public class DivisionDemo {

	public static void main(String[] args) {
		
		
		//형변환 + 연산자
		
		int a = 10;
		int b = 3;
		
		float c = 10.0F;
		float d = 3.0F;
		
		System.out.println(a/b);
		//a = 10 정수(int)
		//b = 3 정수(int)
		//a/b = 3.333.. 실수가 되는데
		//정수라는 데이터타입끼리 연산을 했을땐 값도 정수로 나오게되면서
		//소수점자리의 값은 손실이 된다.(0.333..사라진다)
		//그래서 값은 3으로 나오게 된다.
		
		System.out.println(c/d);
		//c = 10.0F라는 플로트 형식의 실수이다.
		//d = 3.0F라는 플로트 형식의 실수이다.
		//연산하는 값이 둘다 실수였기 때문에
		//결과값도 아무런 문제없이 실수가 나오게 된다.(3.333..)
		//소수점아래의 값도 잃어버리지 않게 된다.
		
		System.out.println(a/d);
		//a = 10이라는 정수 데이터타입이고
		//d = 3.0F이라는 실수 데이터타입이다.
		//a/d 나누면 어떻게 형변환이 될까?
		//두개의 값을 같은 형식의 형으로 컨버팅해준다 자바는.
		//더 정밀하게 더 넓은 수로 그렇지않은데이터형식이 형변환된다.
		//정수와 실수는 실수가 더 조밀하고 정밀한 숫자가 된다.
		//내부에서 10이라는 정수를 10.0으로 형변환이 자동으로 이루어진다.
		//그래서 값이 실수의 형태로 3.333이라는 값이 나온다.
		
