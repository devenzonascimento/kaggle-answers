# 1
```py
def sign(x):
    if x > 0:
        return 1
    elif x < 0:
        return -1
    else:
        return 0
    
q1.check()
```

# 2
```py
def to_smash(total_candies):
    
    print("Splitting", total_candies, "candy" if total_candies == 1 else "candies")
    
    return total_candies % 3

to_smash(91)
to_smash(1)
```
# 3
```py
def prepared_for_weather(have_umbrella, rain_level, have_hood, is_workday):

    return have_umbrella or rain_level < 5 and have_hood or not rain_level > 0 and is_workday

have_umbrella = False
rain_level = 0.0
have_hood = False
is_workday = False


actual = prepared_for_weather(have_umbrella, rain_level, have_hood, is_workday)
print(actual)

q3.check()
```
# 4
```py
def is_negative(number):
    if number < 0:
        return True
    else:
        return False

def concise_is_negative(number):
    return number < 0
q4.check()
```

# 5a
```py
def wants_all_toppings(ketchup, mustard, onion):
    
    return ketchup and mustard and onion

q5.a.check()
```

# 5b
```py
def wants_plain_hotdog(ketchup, mustard, onion):
    
    return not (ketchup or mustard or onion)

q5.b.check()
```

# 5c
```py
def exactly_one_sauce(ketchup, mustard, onion):
    
    return (ketchup and not mustard) or (mustard and not ketchup)

q5.c.check()
```

# 6
```py
def exactly_one_topping(ketchup, mustard, onion):

    return (ketchup + mustard + onion) == 1

q6.check()
```