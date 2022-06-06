---
marp: true
theme: uncover
_class: lead
paginate: true
backgroundColor: #fff
---
![height: auto](images/html5-logo.png)

---

# Indice

---

# HTML, CSS e Javascript

- Nascono negli anni '90 per sviluppare siti web
- Sono tuttora **gli unici linguaggi accettati** da tutti i browser (per standard definito)

---

### HTML

- Definisce la struttura della pagina
- Utilizza dei **tag** per definire le varie parti
- I sorgenti hanno estensione `.html` (ad esempio, `index.html`)

<!-- fit -->

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Untitled</title>
    <link rel="stylesheet" type="text/css" href="theme.css" />
  </head>
  <body></body>
</html>
```

---

### CSS

- Definisce la parte grafica della pagina
- Utilizza degli `identificatori` e delle `proprietà`
- Può essere definito nella pagina HTML (attraverso il tag `<style>`) o in un file `.css`

```css
p:first-letter {
  display: block;
  margin: 5px 0 0 5px;
  float: left;
  color: #000;
  font-size: 60px;
}
```

---

### JavaScript

- Definisce il "comportamento" della pagina (eliminazione o aggiunta di elementi, eventi...)
- Tra questi linguaggi, è l'unico di **programmazione**
- Può essere definito nella pagina HTML (attraverso il tag `<script>`) o in un file `.js`

<!-- fit -->

```js
const username = "david123";
if (username.length > 4 && username.length < 16) {
  console.log("Username is valid!");
} else {
  console.log("Username must be between 5 and 15 characters!");
}
```

---

# HTML

---

### Tag in HTML

- Una pagina HTML è composta da varie porzioni di codice chiamate **tag**
- Ogni tag ha un nome unico, che viene usato per aprire e chiudere la relativa porzione di codice
- Per aprire e chiudere un tag si usa la sintassi, rispettivamente, `<nome>` e `</nome>`, dove `nome` è il nome del tag
- Un tag può essere annidato all'interno di un altro tag, definendo una gerarchia (ad esempio, `<p> <span> Ciao! </span> </p>`)

---

### Attributi dei tag

- Un tag può contenere degli **attributi**, che definiscono alcuni parametri del tag
- Si usa la sintassi `<tag attributo="valore">`
- Sono molto importanti, in quanto permettono di fornire molte informazioni riguardo al tag

---

### Struttura di una pagina HTML

- Tutte le pagine HTML hanno una struttura di base fissa, composta da:
  ```html
  <!DOCTYPE html>
  <head>
    ...
  </head>
  <body>
    ...
  </body>
  ```

---

- Il tag **`<!DOCTYPE html>`** informa il browser sul tipo di file
- Il tag **`<head>`** contiene le informazione relative a **ciò che l'utente non vede nella pagina**, come ad esempio il collegamento di altri file, metadati per motori di ricerca o il nome della tab nel browser
- Il tag **`<body>`** contiene **tutti gli elementi con cui l'utente può interagire**

---

# Alcuni tag utili

---

### Tag `<hn>`

- Per definire il titolo della pagina o di una sua sezione si utilizza il tag `<hn>`, dove n è un numero tra 1 e 6 (più è basso il numero, più il titolo sarà grande)
- Permette di definire una gerarchia tra parti della pagina
- Esempio:

```html
<h1>Titolo della pagina</h1>
<h2>Sottotitolo</h2>
```

---

### Tag `<p>`

- Rappresenta un paragrafo
- Normalmente contiene solo testo
- **I ritorni a capo non vengono visualizzati dall'utente** 
```html
<p>Questo è un paragrafo.
Anche se sono andato a capo, nella pagina finale non si vedrà
</p>
```

---

### Tag `<br>`

- Permette di inserire una riga vuota
- Utile per separare il testo all'interno di un tag (come il tag `<p>`)

```html
<p>
  Prima riga
  <br />
  Seconda riga
</p>
```

---
### Esercizio

Crea una pagina web composta da un titolo, un paragrafo di due caporiga separati.
