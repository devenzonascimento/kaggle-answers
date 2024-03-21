# 1
```py
def select_second(L):
    
    if len(L) < 2:
        return None
    return L[1]

q1.check()
```
# 2
```py
def losing_team_captain(teams):
    
    return teams[-1][1]

q2.check()
```
# 3
```py
def purple_shell(racers):
    
    temp = racers[0]
    racers[0] = racers[-1]
    racers[-1] = temp
    
q3.check()
```
# 4
```py
a = [1, 2, 3]
b = [1, [2, 3]]
c = []
d = [1, 2, 3][1:]

lengths = [3, 2, 0, 2]

q4.check()
```
# 5
```py
def fashionably_late(arrivals, name):
    
    order = arrivals.index(name)
    return order >= len(arrivals) / 2 and order != len(arrivals) - 1

q5.check()
```
