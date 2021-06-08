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
my_bicycle=Bicycle()

my_bicycle.wheel_size=26
my_bicycle.color='black'

my_bicycle.move(30)
my_bicycle.turn('좌')
my_bicycle.stop()

```