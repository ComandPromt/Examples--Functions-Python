# Examples--Functions-Python

# Replace Last

~~~python

def replace_last(string, find, replace):

    reversed = string[::-1]
    
    replaced = reversed.replace(find[::-1], replace[::-1], 1)
    
    return replaced[::-1]
    
texto = replace_last("a--aaasasda-, "-", "")

print(texto)
~~~

# Simple Translator

~~~python
from deep_translator import GoogleTranslator
from unidecode import unidecode
import os
import codecs

def replace_last(string, find, replace):

    reversed = string[::-1]
    
    replaced = reversed.replace(find[::-1], replace[::-1], 1)
    
    return replaced[::-1]

word = 'gato';

start='spanish';

idiomas = ["english","fr","ks"];

cars = ["Ford", "Volvo", "BMW"]; 

indice=0;

f = open("datos.txt","w")

for i in idiomas:
        
    texto=""
    
    for b1 in a:
    
        texto+=str(b1)+",";
    
        translated_word = GoogleTranslator(source=start, target=idiomas[indice]).translate(str(b1));
        
        a=translated_word.encode('utf-8')
        
        b=a.decode()
    
        print(translated_word)
    
    texto=texto+replace_last(texto, ",", "")+'\n';

    f.write(texto)
    
    indice=indice+1;
    
f.close()
~~~
