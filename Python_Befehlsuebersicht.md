# Python Befehlsübersicht


## Textausgabe mit dem Befehl: print

```python
print "Hello World"
print "Ergebnis: %d" % int1
print Ergebnis: %f" % float1

```

---

## Variablen und Datentypen

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
Variablen dürfen nicht nach Funktionen benannt werden.  
True **ODER** False sollten keine Werte zugewiesen werden auch wenn es möglich ist.  
Im interaktiven Modus sollte quit nicht als Variablenname verwendet werden und keine Funktion mit dem Namen quit() angelegt werden.  

---

## if, elif und else

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

## for-Schleife

```python
a = [1,2,3,4,5,6,7,8,9,10]                              #Erstellen einer Liste mit 10 Inhalten

for number in a:                                        #Solange ein Wert in a steht
    print "Wir sind gerade an Stelle: %d" % number      #Ausgabe an welcher Stelle in a die Schleife ist
                                                        #Nach 10 durchläufen endet die Schleife
```

## while-Schleife

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































