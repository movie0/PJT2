

##### 상속(inheritance)

- class에서 이름 뒤에 괄호는 상속이다.  
- python의 모든 객체는 object를 상속받는다.  
- python3부터는 (object)는 생략가능하다. 즉 지금까지 class를 정의할 때 object를 내부적으로 상속하고 있었다.

  
                                                            * 상속을 사용하면 확장이 용이하며, 유지보수가 편해진다.





```bash
class Parent:
    x = 'parent'
    
    @classmethod
    def output(cls):
        return cls.x
    
    @staticmethod
    def prn():
        return Parent.x
    
# Parent를 Child에 상속
class Child(Parent):
    x = 'child'
    
    def display(self):
        print(Parent.output())
        print(Child.output())
```

