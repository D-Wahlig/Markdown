# Python Befehlsübersicht

Auf dieser Seite werden Befehle von Programmiersprachen am Beispiel von Python erklärt.

---

## Textausgabe mit dem Befehl: print

Mit dem print Befehl kann eine __beliebig__ lange Zeichenkette ausgegeben werden.   
Hier ein Beispiel: print "Hello World!" - Damit lassen wir das Programm Hello World! ausgeben. Somit ist es möglich dem Nutzer helfen zu verstehen was das Programm, mit dem er arbeitet, macht und bei Eingabeaufforderungen weiß, was er eingeben soll. Mit einem print kann nicht nur Text ausgegeben werden, es ist auch möglich Variablen auszugeben, um zu prüfen ob eine Berechnung fehlerfrei durchgeführt wurde. 

---

## Datentypen
 
Jegliche Eingaben werden einem Datentyp zugeordnet. Es gibt folgende Datentypen:  

- int(Intager), also eine Ganzzahl. - es gibt auch long(längere Ganzzahlen)
- double, eine Kommazahl. - oder float(32 Bit statt 64 Bit reservierter Speicher)
- char(character), einzelnes Zeichen
- string, Zeichenkette
- boolean, für Wahr(True) oder Falsch(False)

---

## Variablen

Variablen werden als Speicher für Werte verwendet, welche das Programm später wieder verwenden oder weiter verarbeiten  soll.  


Eine Variable deklarieren heißt, ihr einen **Datentyp** zuzuweisen; sie zu definieren heißt, ihr einen **Wert** zuzuweisen.  
In Python müssen Variablen nicht deklariert werden, sondern können direkt definiert werden. Bsp. : *a = 5*  
Variablen können auch deklariert werden: *b = int(7)* - dabei wird die Variable gleichzeitig definiert.  




Mit Variablen ist es möglich zu rechnen:  
Definieren wir uns hierfür die Variablen a mit dem Wert 5 und b mit dem Wert 7: *a = 5, b = 7*  
Nun haben wir unseren zwei Variablen Werte zugewiesen; d. H. sie definiert.

Zum Rechnen selbst werden Rechenoperatoren verwendet:  
\+ für Addition, - für Subtraktion, * für Multiplikation, / für Division; diese sollten schon bekannt sein.  
Dann gibt es da noch:  
% für Modulo - dieser berechnet den Rest einer Division  
 
Kommen wir nun zum rechnen selbst:  
Wir haben nun a den Wert 5 und b den Wert 7 zugewiesen, jetzt wollen wir diese addieren:

Also benutzen wir den + Operator und schreiben:  
 *a + b*   
Nun haben wir zwar a mit b addiert, aber das Ergebnis geht verloren.
Wollen wir nur das Ergebnis einmal anzeigen, können wir es mit dem print Befehl ausgeben:  
*print a + b* - somit wird uns nur 12 angezeigt.  
Wollen wir nun aber das Ergebnis ebenfalls speichern fügen wir eine weitere Variable hinzu, aber da wir ihr keinen Wert selbst zuweisen wollen, sondern das Ergebnis in ihr speichern, verwenden wir den Zuweisungsoperator *=*. Also:  
*c = a + b*  
Nun wird das Ergibnis von a + b in c gespeichert. Also sollte jetzt in c der Wert 12 stehen.  
Überprüfen wir das doch mit einem print: *print c*  
Und siehe da, wir erhalten das Ergebns 12.