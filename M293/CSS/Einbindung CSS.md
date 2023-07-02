## Internes Stylesheet
```html
<!DOCTYPE html>
<html>
<head>
    <title>Beispiel für internes Stylesheet</title>
    <style>
        body {
            background-color: lightblue;
        }
        h1 {
            color: navy;
        }
        p {
            color: red;
        }
    </style>
</head>
<body>
    <h1>Willkommen auf meiner Webseite!</h1>
    <p>Dies ist ein Absatz.</p>
</body>
</html>
```
## Externes Stylesheet

#### index.html

```html
<!DOCTYPE html>
<html>
	<head>
	    <title>Beispiel für internes Stylesheet</title>
	    <link rel='stylesheet' type='text/css' href='styles.css'>
	</head>
	<body>
	    <h1>Willkommen auf meiner Webseite!</h1>
	    <p>Dies ist ein Absatz.</p>
	</body>
</html>
```

#### style.css

```css
body {
    background-color: lightblue;
}
h1 {
    color: navy;
}
p {
    color: red;
}
```

## Inline-Style
```html
<!DOCTYPE html>
<html>
	<body>
	    <h1 style='color:navy;'>Willkommen auf meiner Webseite!</h1>
	    <p style='color:red;'>Dies ist ein Absatz.</p>
	</body>
</html>
```

## Wann wird welche Methode verwendet?

- **Externes Stylesheet:** meisten Projekte, insbesondere für größere Websites und Anwendungen
- **Internes Stylesheet:**  die nur auf einer einzigen Seite gelten(nicht zu viel benutzen)
- **Inline-Style:** nur für einmalige/Spezifische Sachen(nicht zu viel benutzen)