# Examples--Functions-Python

~~~python

def replace_last(string, find, replace):

    reversed = string[::-1]
    
    replaced = reversed.replace(find[::-1], replace[::-1], 1)
    
    return replaced[::-1]
    
texto = replace_last("a--aaasasda-, "-", "")

print(texto)
~~~
