#Markdown

Markdown ist keine eigene Sprache, hat aber ähnlichkeiten zu Programmiersprachen. Während die "Sprache" in Markdown beliebig ist gibt es Formatierungssyntaxe die unikat sind. Dabei ist die oberste Priorität von Markdown, Leserlichkeit. Es soll von jedem, der die gleiche Sprache spricht, gelesen und verstanden werden können ohne dass dieser von Klammern, Befehlen und Kommandos überflutet wird.  

---

##Horizontale Linien

Mit mindestens 3 -(also ---) kann man eine horizontale Linie erstellen, dabei gibt es kein maximum wie viele "-" man macht. Man kann statt - auch * verwenden.



##Text

Text wird einfach geschrieben, wobei es die Möglichkeit gibt HTML Tags zur Textdarstellung zu verwenden.  
Zwei Leerzeichen für einen Zeilenumbruch.  Aber nur am Ende einer Zeile...  
Man kann auch Worte *betonen*, in dem man ein * vor und nach dem zu betonenden Wort setzt.  
Man kann Worte auch mit einem _ betonen.  
Worte mit * oder _ zu betonen hat den gleichen Effekt, wie den <i\>Tag von HTML zu verwenden.  
Benutzt man *\* oder __ **betont** man ein Wort, wie mit dem <b\> Tag von HTML.  
Mit dem \\ kann man einzelne Symbole escapen, muss mir noch einfallen wie das auf deutsch heisst...


----------------

##Zitate

>Zitate werden mit einem ">" eingeleitet.  
Man muss nichtmahl für jede Zeile ein eigenes machen sondern nur für das Erste.

>Dennoch ist es eleganter es in JEDER Zeile zu machen.



--------------------

##Ungeordnete Liste

Bei ungeordneten Listen wird nur ein Aufzählungszeichen verwendet. Man leitet eine ungeordnete Liste mit *, + oder - ein.

* Punkt 1

+ Punkt 2

- Punkt 3

-------------

##Geordnete Liste

Bei geordneten Listen werden die Aufzählungen nummeriert. Dabei ist es egal welche Zahlenfolge verwendet wird, wichtig ist aber eine Zahl mit Punkt zu schreiben.  
  

1. Geordneter Listenpunkt

2. Geordneter Listenpunkt

1. Geordneter Listenpunkt

---------------

##Code Blöcke

Code Blöcke werden durch eine Einrückung von 4 Leerzeilen oder einem Tab eingeleitet.

    Hier könnte Ihr Code stehen.
    Es ist sogar Zeilenübergreifend

Zumindest solange man die Einrückung beachtet...


------------

##Überschriften

Überschriften werden per Doppelkreuz eingeleitet, dabei gibt die Anzahl der Doppelkreuze die Ebene der Überschrift an:

# Überschrift Ebene 1

Überschrift Ebene 1, aber alternative Schreibweise.
=

## Überschrift Ebene 2

Überschrift Ebene 2, aber alternative schreibweise.
-

### Überschrift Ebene 3

#### Überschrift Ebene 4

##### Überschrift Ebene 5

###### Überschrift Ebene 6

-------------------

##HTML Tags

Man kann HTML Tags in Markdown verwenden. Sie haben den gleichen Syntax:

<b>Fett</b>  
<i>Kursiv</i>  
<u>Unterstrichen</u>  
<s>Durchgestrichen</s>  
 
---------

##Links

Es gibt zwei Arten von Links:

Links und das andere Links.

Inline

Bei einem Inline Link schreibt man in [eckigen Klammern] die Bezeichnung des Links und in (runden Klammern) die URL und optional in "Anführungszeichen" den Titel, wenn man mit der Maus über den Link fährt.

Bsp. :  
[Google](https://www.google.de "Google Suchmaschiene")


und Referenzen

Bei referenzen wird auf eine ID verwiesen unter welcher der Link zu finden ist.

Bsp. :

[Google][1]

[1]: https://www.google.de "Google Suchmaschiene"


---------------------

##Bild

Ein Bild funktioniert wie ein Link nur dass es mit einem ! eingeleitet wird.

![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg "Markdown-Logo")

-------------



