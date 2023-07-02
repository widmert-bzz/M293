## Universalselektor

- *
- Keywords(z.b main)
- Kombination

```css
/* Grüner, gepunkteter Rahmen für alle Elemente */
* { 
  margin: 5px;
  padding: 3px;
  border: 2px dotted green;
  text-align: center; 
}

/* Nur ein Rahmen, kein Universal- sondern normaler Typselektor */
main { 
	border: 3px solid red; 
}

/* Rahmen um alle Kindselemente im main-Element */
main * { 
	border: 2px solid blue; 
}
```

## Attributselektor
der Attributname muss zwischen eckigen Klammern [] gesetzt werden

![[Pasted image 20230702172905.png]]

```css
/* Styling für alle Elemente mit dem Attribut title */
[title] {
  border: 4px solid black;
}

/* Styling for alle a-Element mit dem Attribut title */
a[title] { 
  text-decoration: none;
  color: red;
  font-weight: bold;
  border: 2px dotted red;
}
```

### Attributselektor mit einem bestimmten Attributwert

| Selektor | Bezeichnung | Auswahl | Beispiel |  
| -------- | -------- | -------- | -------- |  
| `[attr=wert]` | Attributselektor (Attributwert) |jedes Element, bei dem das Attribut `attr` den Wert `wert` enthält| `<elm arrt=wert'>` |  
| `[attr~=wert]` | Attributselektor (Attributwert) mit Tilde (`~`) |jedes Element, bei dem im Attribut `attr` der Wert `wert` als allein stehendes Wort vorkommt| `<elem attr='abc wert xyz'>` |
| `[attr "Verkettungszeichen" =wert]` | Attributselektor (Attributwert) mit Verkettungszeichen (alt gr + 7) | jedes Element, bei dem im Attribut `attr` der Wert `valx` am Anfang als eine durch Bindestrich getrennte Zeichenfolge steht| `<elem attr='valx-valy'>` |


#### Beispiele

```CSS
/* Styling für alle HTML-Elemente wo title den Attributwert deprecated besitzt */
[title=deprecated] {
  color: red;
  text-decoration: line-through;
}

/* Styling von HTML-Elemente wo title im Attributwert das Wort "bzzlab" enthält */
[title~=bzzlab] { 
	font-weight: bold; 
	color: red; 
}

/* Styling von HTML-Elemente wo title im Attributwert das Wort "bzzlab" enthält */
[title~=bzzlab] { 
	font-weight: bold; 
	color: red; 
}
```

### Attributselektor mit einem bestimmten Teilwert (Teilübereinstimmung)

| Selektor | Bezeichnung | Auswahl | Beispiel |  
| -------- | -------- | -------- | -------- |  
| `[attr^=wert]` | Attributselektor (Teilwert) |jedes Element, bei dem das Attribut `attr` mit der Textfolge `wert` anfängt| `<elem attr=“werter”>` |  
| `[attr$=wert]` | Attributselektor (Teilwert) |jedes Element, bei dem das Attribut `attr` mit der Textfolge `wert` endet| `<elem attr=“endwert”>` |
| `[attr*=wert]` | Attributselektor (Teilwert) | jedes Element, bei dem das Attribut `attr` die Textfolge `wert` enthält| `<elem attr=“bewertung”>` |


#### Beispiele

```CSS
/* Styling alle a-Elemente wo das Attribut href mit http:// beginnt */
a[href^="http://"] {
	text-decoration: none;
	border-bottom: 2px dotted red;
	color: red;
}

/* Styling für a-Elemente wo das Attribut href mit .pdf endet */
a[href$=".pdf"] {
	text-decoration: none;
	color: red;
	padding: 1px;
	border: 2px dotted red;
}

/* Styling für a-Elemente wo im Attribut href die Textfolge mydomain enthalten ist */
a[href*=mydomain] { 
	font-weight: bold; 
	color: red; 
}
```