# 1
```py
def prettify_graph(graph):
    graph.set_title("Results of 500 slot machine pulls")
    
    graph.set_ylim(0)
    
    graph.set_ylabel("Balance")
    
graph = jimmy_slots.get_graph()
prettify_graph(graph)
graph
```
# 2
```py
from learntools.python.luigi_analysis import full_dataset

def best_items(racers):

    winner_item_counts = {}

    for i in range(len(racers)):

        racer = racers[i]

        if racer['finish'] == 1:

            for j in racer['items']:

                if j not in winner_item_counts:

                    winner_item_counts[j] = 0

                winner_item_counts[j] += 1

        if racer['name'] is None:

            print("WARNING: Encountered racer with unknown name on iteration {}/{} (racer = {})".format(
                i+1, len(racers), racer['name'])
                 )

    return winner_item_counts

best_items(full_dataset)
```
# 3
```py
def hand_total(hand):

    total = 0

    aces = 0
    for card in hand:
        
        if card in ['J', 'Q', 'K']:
            
            total += 10
            
        elif card == 'A':
            
            aces += 1
            
        else:

            total += int(card)
    
    total += aces

    while total + 10 <= 21 and aces > 0:

        total += 10
        aces -= 1
        
    return total

def blackjack_hand_greater_than(hand_1, hand_2):
    
    total_1 = hand_total(hand_1)
    
    total_2 = hand_total(hand_2)
    
    return total_1 <= 21 and (total_1 > total_2 or total_2 > 21)

q3.check()
```



