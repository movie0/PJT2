# 객체지향 프로그래밍


```python
class Bicycle():

    def move(self, speed):
        print('자전거: 시속 {}킬로미터로 전진'.format(speed))
    
    def turn(self, direction):
        print('자전거: {}회전'.foramt(direction))
    
    def stop(self):
        print('자전거({}, {})'.foramt(self.wheel_size, self.color))
```

```python
my_bicycle = Bicycle()

my_bicycle.wheel_size = 26
my_bicycle.color = 'black'

my_bicycle.move(30)
my_bicycle.turn('좌')
my_bicycle.stop()

```


```python
class Car():
    instance_count = 0

    #초기화 함수(인스턴스 메서드)
    def __init__(self, size, color):
        self.size = size
        self.color = color
        Car.instance_count = Car.instance_count + 1

    def move(self, speed):
        print('자동차{},{}가 '.format(self.size, self.color), end='')
        print('시속 {}킬로미터로 전진'.format(self.speed))

    def auto_cruise(self):
        print('자율주행모드')
        self.move(self.speed)

    @staticmethod
    def check_type(model_code):
        if model_code >= 20 :
            print('이 자동차는 전기차입니다')
        elif (model_code >= 10) & (model_code < 20):
            print('이 자동차는 가솔린차입니다')
        else :
            print('이 자동차는 디젤차입니다')

    @classmethod
    def count_instance(cls):
        print('자동차 객체의 개수: {}'.format(cls.instance_count))
    
```