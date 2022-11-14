class Person{
String? name;  // 멤버변수, name 이 인스턴스
int? age;
String? sex;

Person({String? name, int? age, String? sex}){ // argument 에 {}를 할 경우 NullSafety 적용
this.name = name;
this.age = age;
this.sex = sex;
}
}



void main(){ // return 불가능

Person p1 = new Person(age:30); // 변수와 생성자
Person p2 = new Person(sex: 'male'); // 이와 같이 생성자 argument에 넣으려면 Person 변수 선언 시 argument 에 {} 해줘야 함.

print(p1.age); // 변수 출력
print(p2.sex);

}

addNumber(int num1, int num2){ // argument 에 꼭 int(타입)가 없어도 됨.
return num1 + num2;
}