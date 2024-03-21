# 0a
```py
a = ""
length = 0
q0.a.check()
```
# 0b
```py
b = "it's ok"
length = 7
q0.b.check()
```
# 0c
```py
c = 'it\'s ok'
length = 7
q0.c.check()
```
# 0d
```py
d = """hey"""
length = 3
q0.d.check()
```
# 0e
```py
e = '\n'
length = 1
q0.e.check()
```
# 1
```py
def is_valid_zip(zip_code):
    
    return len(zip_code) == 5 and zip_code.isdigit()

q1.check()
```
# 2
```py
def word_search(doc_list, keyword):
    
    indices = [] 
    
    for i, doc in enumerate(doc_list):
        
        tokens = doc.split()
         
        normalized = [token.rstrip('.,').lower() for token in tokens]
        
        if keyword.lower() in normalized:
            
            indices.append(i)
            
    return indices

q2.check()
```
# 3
```py
def multi_word_search(documents, keywords):
    
    keyword_to_indices = {}
    
    for keyword in keywords:
        
        keyword_to_indices[keyword] = word_search(documents, keyword)
        
    return keyword_to_indices

q3.check()
```



