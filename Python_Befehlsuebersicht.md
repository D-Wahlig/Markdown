# Python Befehlsübersicht


### Textausgabe mit dem Befehl: print


#### In Python 2
```python
print "Hello World"
print "Ergebnis: %d" % int1
print Ergebnis: %f" % float1

```

#### In Python 3
```python
print ("Hello World")
print (f"Ergebnis: {int1}")


---

### Variablen und Datentypen

```python
a = 1                           #Ganzzahl
b = 1.2                         #Kommazahl
c = c                           #Char
d = Text                        #String
e = True **ODER** e = False     #Boolean
f = g = 5                       #Zuweiseung eines Wertes an mehrere Variablen
h = 1,2 **ODER** h = (1,2)      #Tuple
i = [1,2,3]                     #Liste
j = {1,2,3}                     #Set

del a #löscht Variable a

```


**Wichtig!**  
Variablen dürfen nicht mit einer Zahl beginnen.  
Variablen dürfen keine Sonderzeichen beinhalten.  
Variablen dürfen nicht nach Befehlen benannt werden.  
True **ODER** False sollten keine Werte zugewiesen werden auch wenn es möglich ist.  
Im interaktiven Modus sollte quit nicht als Variablenname verwendet werden und keine Funktion mit dem Namen quit() angelegt werden.  

---


## Kontrollstrukturen

### if, elif und else

```python
a = 10
b = 11

if a < b:                   #VWenn a < b dann
    print "Wahr"            #wird "Wahr" ausgeführt

elif b < a:                 #Sonst wird geprüft ob b < a
    print "Falsch"          #wenn das stimmt wird "Falsch" ausgegeben

elif a == b:                #Stimmen die ersten beiden nicht wird geprüft ob a == b ist
    print "Gleich"          #wenn ja, wird "Gleich" ausgegeben

else:                       #Sollte keine der oben stehenden Prüfungen wahr ergeben
    print "Fehler"          #printen wir "Fehler"

```

### for-Schleife

```python
a = [1,2,3,4,5,6,7,8,9,10]                              #Erstellen einer Liste mit 10 Inhalten

for number in a:                                        #Solange ein Wert in a steht
    print "Wir sind gerade an Stelle: %d" % number      #Ausgabe an welcher Stelle in a die Schleife ist
                                                        #Nach 10 durchläufen endet die Schleife
```

### while-Schleife

```python
a = 100                     #Festlegen von a

while a > 1:                Solange a größer 1
    print a                 Ausgabe a
    a-=1                    reduzieren von a um 1
```

## Funktion def

```python
def name(uebergabewert):                                #Erstellenn der Definition "name"
    if uebergabewert != 1:                              #if-Verzweigung innerhalb der Funktion
            print "Übergebener Wert ist ungleich 1."    
    else:
        print "Übergebener Wert gleich 1."

uebergabewert = 5

name(uebergabewert)                                     #Aufruf der Funktion mit einem Übergabewert

```

### Iterativ

Die Wiederholung wird von 1 nach n durchgeführt.

```python
n = 10

for i in range(1, n):
    print i

```

### Rekursiv

Die Wiederholung wird von n nach 1 durchgeführt.

```python
n = 10

def func(n):
    if n < 2:
        return 1

    return fib(n - 1) + fib(n - 2)

print fib(n)

```

---

## Datenstrukturen

### Liste

```python
a = []                                          #Leere Liste
a = [1, 2.1,"a"]                                

```

Frei veränderbarer Inhalt mit festem Index.
Kann mit .append() erweitert werden.


### Tuple

```python
a = 1, 2.3, "a"

```

Lässt seine Werte, nach der Erstellung, nicht verändern, nur anfügen.


### Dict

```python
a = {"key" : "value", "key2" : "value2"}

```

Frei veränderbarer Inhalt mit variablem Index.

### Set

```python
a = {1, 2, 3}
b = {3, 4, 5}

a - b                   #{1, 2}

a & b                   #{3}

a | b                   #{1, 2, 3, 4, 5}

```
Kann verwendet werden, um Dopplungen aus Listen zu entfernen.

Unveränderbarer Inhalt ohne Index.


#### Unterschiede

Eine Liste kann man verändern mit:
a[n] = Wert                             #n steht hier als Platzhalter für einen existierenden Index

Bei Tuplen und sets kommt hiereine Fehlermeldung

Der .append Befehl funktioniert nur bei Listen.


## Command-line Arguments

```python
#!/usr/bin/env python3

"""Hier steht der Text wenn -h 
oder --help beim Aufruf angegeben wurde
"""

import argparse


params = argparse.ArgumentParser(description = __doc__, formatter_class = argparse.RawDescriptionHelpFormatter)

params.add_argument(-o, --option, action = 'store_true', dest = 'opt' help = 'Hier steht die Beschreibung des optionalen Argumentes')

params.add_argument('command', action = 'store', help = 'Hier steht die Beschreibung des positionellen Argumentes')

params.add_argument('optcommand', action = 'store', nargs = '?', help = 'Hier steht die Beschreibung des optionalen positionellen Argumentes')

# Parsen der Kommandozeilen Argumente
args = params.parse_args()

```

## Input

```python
words = sys.stdin.read()                #Standard Input wird gelesen und in words gespeichert


words = open("file.txt", "r")           #file.txt wird zum lesen geöffnet 
words = words.read()                    #Inhalt von file.txt wird in words gespeichert

```






















