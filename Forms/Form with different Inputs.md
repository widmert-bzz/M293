````html
<form action='https://it.bzz.ch/demo/formdata/index.php' method='post'>
  <div>
    <label for='price'>Price</label>
    <input id='price' name='price' type='number' min='0.05' max='99.95' step='0.05'>
  </div>
  <div>
    <label for='release'>Erscheinungsdatum</label>
    <input id='release' name='release' type='date'>
  </div>
  <div>
    <label for='edition'>Auflage</label>
    <input id='edition' name='edition' type='range' min='1' max='9'>
  </div>
  <div>
    <button type='submit'>Absenden</button>
    <button type='reset'>Zurücksetzen</button>
  </div>
</form>
```