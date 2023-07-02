
## Kombinieren von Selektoren

### Nachfahrenselektor
Wählt alle Element die innerhalb des erstgenannten Element sind
```css
div p {
    color: red;
}
```
### Kindselektor
wählen nur direkte Kinder eines bestimmten Elements aus (also nicht tiefer liegende Elemente)
```css
div > p {
    color: blue;
}
```
### Nachfolgerselektor
wählen nur unmittelbare nachfolgende Element aus
```css
h1 + p {
    font-size: 18px;
}
```
### Geschwisterselektor
ist ähnlich wie der Nachfolgerselektor, aber nicht nur nachfolgendes Element, sonder auch alle Elemente die dasselbe Elternelement haben
```css
h1 ~ p {
    font-size: 18px;
}
```
### Gruppenselektor
gleicher Still auf verschiedene Elemente
```css
h1, h2, p {
    color: green;
}
```


## Übersicht

| Selektor | Bezeichnung | Auswahl | HTML-Beispiel |  
| -------- | -------- | -------- | -------- |  
| element {…} | Typselektor |HTML-Element mit dem Namen _element_| `<body>` |  
| .klname | Klassenselektor | Element mit der Klasse _klname_ | `<p class='klname'>` |
| `#elemid` |ID-Selektor| Element mit der ID _elemid_ | `<p id='elemid'>` |


## Klassenselektor
#### HTML

```html
<p class='hinweis'>Ein Absatztext ...</p>
```

#### CSS

```css
/*alle <p> mit der Klasse hinweis*/
p.hinweis { 
	color: red;
}
/*alle elemente mit der Klasse hinweis*/
.hinweis {
	color: red;
}
```


## ID-Selektor

id kann nur einmalig sein

#### HTML

```html
<p id='text'>Ein Absatztext ...</p>
```

#### CSS

```css
#text {
	color: red;
}
```

## Element-Selektor

nur Elemente(keywords)

#### CSS

```css
h1 {
	color: red;
}
```

