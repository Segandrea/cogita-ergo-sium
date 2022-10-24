# Cogita

Repository relativo al primo corso ["Come costruire una WebApp"](https://www.youtube.com/watch?v=WO5qoXu9fwo)
dell'associazione [./Cogita](https://www.cogita.it)

## Prima lezione

In questa lezione vengono indicati i programmi necessari e suggeriti per la
realizzazione di un'applicazione web.

### Strumenti consigliati

* Editor suggerito: [Visual Studio Code](https://code.visualstudio.com/)
* Runtime per Javascript: [Node.js](https://nodejs.org/)
* Package manager:
  * Per la gestione degli strumenti: [npm](https://www.npmjs.com/)
  * Per la gestione delle dipendenze: [yarn](https://yarnpkg.com/)
* Altri pacchetti da npm: create-react-app

**Suggerimento**: usare Ubuntu o altra distro linux (I use arch btw)

### Setup

1. Installare Visual Studio Code
2. Installare Node.js
3. Installare Yarn con `npm install -g yarn`
4. Installare create-react-app con `npm install -g create-react-app`
5. Inizializzare il progetto con `create-react-app cogita-ergo-sium`

**Suggerimento**: in caso di problemi con le dipendenze eseguire
dalla root del progetto `rm -rf node_modules && yarn install`.

## Seconda lezione

Nella lezione vengono trattati html e css.
Inoltre viene anche data una rapida occhiata a come é strutturato il progetto.

### Mamma che bello html

(**Disclaimer**: Non sono serio qui sotto)

Html é un bellissimo linguaggio di **PROGRAMMAZIONE**.
É inutile che diciate che é solo un linguaggio di markup, dentro al tag
`<script></script>` che cosa ci mettete? Il *codice Javascript*!
E allora HTML altro non é che un ***superset di Javascript*** e dunque é un
***linguaggio di programmazione***.

### Mamma che bello css

Se non si é capito dai titoli, mi annoiano sia html che css, non
replicheró quello che viene detto nel video in quanto comunque non é sufficiente
ad avere una conoscenza adeguata di nessuna delle due cose.

Lascio peró un link a un sito che sicuramente sa spiegarlo meglio di quanto
potrei fare io: [w3schools](https://www.w3schools.com/)

### Mamma che bello react

Struttura del progetto creato nella lezione precedente con il
comando `create-react-app` :

```
.
├── package.json
├── package-lock.json
├── .gitignore
├── .git/
│   └── ...
├── node_modules/
│   └── ...
├── public/
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
├── README.md
└── src/
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    ├── reportWebVitals.js
    └── setupTests.js
```

* In `public/` ci sono gli asset statici dell'applicazione tipo il logo, le immagini
 e il file html che contiene la pagina iniziale autogenerata.
* In `src/` ci sono invece i file relativi al codice javascript (`App.js`, `index.js`
 in particolare) e al css (`App.css`, `index.css`) che si occupano di popolare
 e abbellire l'html autogenerato in `public/index.html`.

Per buildare e lanciare l'applicazione in modalitá development in modo da poterla
visitare nel browser basta dare il comando `yarn start` da terminale.
NB. In questo modo si rimane in *watch* sul progetto.
Questo vuol dire che ogni volta che si effettua una modifica e si salva un file,
la pagina web si aggiorna automaticamente modificando il contenuto esposto in
base alle modifiche effettuate.
