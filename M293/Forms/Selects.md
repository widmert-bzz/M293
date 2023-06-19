#### Eine Auswahl:
```html
<select name='anreise' size='5'>
      <option>Auto</option>
      <option>Zug</option>
      <option>Bus</option>
      <option>Fahrrad</option>
      <option>Schiff</option>
</select>
```
#### Mehrere Auswahlen:
```html
<select name='anreise[]' size='5' multiple>
  <option>Auto</option>
  <option>Zug</option>
  <option>Bus</option>
  <option>Fahrrad</option>
  <option>Schiff</option>
</select>
```

Add "selected" statement to option tag to pre-select

#### Groups:
```html
<select name='Namen' size='6'>
      <optgroup label='Namen mit A'>
        <option label='Anna'>Anna</option>
        <option label='Achim'>Achim</option>
        <option label='August'>August</option>
      </optgroup>
      <optgroup label='Namen mit B'>
        <option label='Berta'>Berta</option>
        <option label='Barbara'>Barbara</option>
        <option label='Bernhard'>Bernhard</option>
      </optgroup>
    </select>
```