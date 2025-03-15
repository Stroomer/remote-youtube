
# Remote-Youtube

De Remote-Youtube applicatie is een mooi voorbeeld van een NodeJS project die onder andere gebruik maakt van Socket.io. De applicatie is gemaakt door Emiel Seine, docent bij de afdeling CMD van het GLU. Het biedt bezoekers van het GLU (bijvoorbeeld bij opendagen) de mogelijkheid om met behulp van je eigen telefoon de controle over een virtuele TV te nemen. Jouw mobiel wordt dan een afstandbediening en je kan ermee zappen.

In dit voorbeeld laten we je zien hoe je het project lokaal kan testen binnen de browser. 




## Downloaden
Download de bestanden die je nodig hebt om het voorbeeld te bekijken.

- Ga naar de map waar jouw projecten staan.
- Open een terminal. 
- Maak een map aan:

```bash
  mkdir voorbeeld-remote-controller
```

- Navigeer binnen de terminal naar de map die je hebt aangemaakt in de vorige stap.

```bash
  cd voorbeeld-remote-controller
```

- Clone de repo in de huidige map.

```bash
  git clone https://github.com/Stroomer/remote-youtube .
```

- Pak de bestanden uit (Extract All).
- Klaar!

## Installatie

- Maak een keuze voor Mac of Pc, open de gekozen map.
- Open het project in VSCode.

```bash
  code .
```

- Open package.json.
- Installeer de pakketjes uit package.json.

```bash
  npm install
```

- Start de applicatie in Node.

```bash
  node index.js
```

- Controleer of "server started" in de terminal zichtbaar is.
- Druk ctrl-c om het Node-proces af te breken.
- Installeer nodemon.

```bash
  npm i nodemon --save-dev
```

- Herstart de Node-applicatie met behulp van nodemon.

```bash
  nodemon index.js
```

- Open index.js.
- Zoek naar: const serverIP = results.en0;
- En vervang het: const serverIP = results.en0 || results['Wi-Fi'];
- Open een nieuwe tab in de browser (de TV) en vul onderstaande adres in:

```bash
  http://192.168.2.8:3000/
```
- Doe het volume op laag, maar niet helemaal uit.
- Klik op het rode vlak om de tv te starten.
- Open nog een tab in de browser (de afstandbediening) en schuif deze tab naast de tab met de tv.

```bash
  http://192.168.2.8:3000/remote.html
```
- Druk op een van de knoppen van de afstandbediening.

Klaar!


