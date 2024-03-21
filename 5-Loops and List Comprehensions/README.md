# 1
```py
def has_lucky_number(nums):
    
    return any([num % 7 == 0 for num in nums])

q1.check()
```
# 2
```py
def elementwise_greater_than(L, thresh):
    
    return [ele > thresh for ele in L]

q2.check()
```
# 3
```py
def menu_is_boring(meals):
    
    for i in range(len(meals)-1):
        if meals[i] == meals[i+1]:
            return True
    return False

q3.check()
```
# 4
```py
def estimate_average_slot_payout(n_runs):
    
    payouts = [play_slot_machine()-1 for i in range(n_runs)]
    
    avg_payout = sum(payouts) / n_runs
    
    return avg_payout

estimate_average_slot_payout(10000000)
```


