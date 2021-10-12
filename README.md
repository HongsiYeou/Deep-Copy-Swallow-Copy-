<h1>DeepCopy(깊은 복사)?</h1>
<hr>
프로그래밍을 하다 보면 객체를 복사했음에도 불구하고 복사가 되지 않은 경우가 있다.
    
    public animal(String name){
        this.name = name;
    }

    Animal a = new Animal();
    Animal b = a;
> b 와 a의 주소를 비교하면 같은 값이 나옵니다. (a의 주소를 b에게 넣었기 떄문에);

이를 *Swallow Copy(얕은 복사)* 라고 하며 서로 같은 주소를 사용하게 되어
b 인스턴스에 값을 수정하면 같은주소를 사용하는 a또한 변경됩니다.

```
    b.name("여우");
    System.out.println("b에 들어있는 동물은?? : "+b.Name);
    System.out.println("a에 들어있는 동물은?? : "+a.Name);
```
> b에 들어있는 동물은?? : 여우
> a에 들어있는 동물은?? : 여우


