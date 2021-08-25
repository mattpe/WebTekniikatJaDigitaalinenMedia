# Ohjelmointiympäristö

Tervetuloa opiskelemaan ohjelmointia JavaScript-kielellä!

JavaScript on selaimessa ajattava ohjelmointikieli, jolla voidaan tuottaa dynaamista, ohjelmallisesti luotua sisältöä web-sivuille.

Työkaluina kurssilla käytetään Visual Studio Code -editoria tai WebStorm-kehitintä (voit valita itse tai opettajan esimerkin mukaan) ja Chrome-selainta.

## Visual Studio Code (VSCode)

Saatavilla ilmaiseksi: [Visual Studio Code](https://code.visualstudio.com/)

- avointa lähdekoodia by Microsoft (älä sekoita kaupalliseen Visual Studio IDE -kehitysympäristöön)
- laajasti laajenteita saatavilla (JavaScript-tuki sisäänrakennettuna)
- kevyt, saatavilla useille alustoille
- hyvä [dokumentaatio ja ohjeistus](https://code.visualstudio.com/docs/editor/codebasics)
- monen JS-kehittäjän valinta

### VSCode - Peruskäyttä

Aktiivinen **projekti** on käytännössä sivupaneelissa auki oleva kansio (_File -> Open folder..._).

Näppäriä näppäinoikoteitä (for finnish keyboard layout, check _File -> Preferences -> Keyboard shortcuts_ for more)

- Multiline comment: _ctrl-'_
- Delete line: _ctrl-shift-k_
- Move line(s): _alt-up/down_
- Copy line(s): _alt-shift-up/down_
- Auto format code: _alt-shift-f_
- Open integrated console: _ctrl-ö_
- [Command palette](https://code.visualstudio.com/docs/getstarted/tips-and-tricks#_command-palette): _ctrl-shift-p_
- Quick find/open files: _ctrl-p_
- Split editor: _ctrl-§_

[Visual Studio Code Tips and Tricks](https://code.visualstudio.com/docs/getstarted/tips-and-tricks)

## Web-selain koodin ajamiseen ja testaamiseen

- Chrome & [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/) (_ctrl-shift-j_ tai _option-cmd-j_)
- pidä selaimen kehitystyökalut ja konsoli auki **aina** kun testaat koodiasi

## Using a local web server for development

- code behaves just like published on a 'real' server in the internet (no direct access to computer's filesystem)
- no need for upload the code to the server (or even refresh the browser) all the time
- no need to publish incomplete, buggy versions of your code
- development can be done in offline mode too
- the url address of the local web server is always `http(s)://localhost:[PORT]` when connecting from the same local computer (ip address `127.0.0.1` works too)
  - `[PORT]` number is defined in the web server settings, something like 8080, 8081, 3000, 3001, 5000, 5050 or 18001 might be the default setting
- [Live Server by Ritwick Dey](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) is a popular extension for VSCode to get an easy to use local dev enviroment

## Webstorm

Webstorm on maksullinen työkalu, mutta voit hankkia ilmaisen opiskelijalisenssin sivulla https://www.jetbrains.com/student/ ja sen jälkeen ladata [tuotteen](https://www.jetbrains.com/webstorm/).

Pääset alkuun ohjelmien kirjoittamisessa seuraavan ohjeen avulla:

1. Luo uusi projekti (File/New/Project). Voit valita projektin tyypiksi Empty project. Nimeä projekti haluamallasi tavalla.
2. Varmista, että JavaScript versioksi on valittu EcmaScript 6
    1. Avaa File/Settings (win) tai WebStorm/Preferences (mac)
    1. Valitse vasemmalta Languages & Frameworks/JavaScript ja valitse listasta ECMAScript 6 ja ruksaa 'Prefer strict mode', jos se on vaihtoehtona.
    1. Valitse vasemmalta Editor/Code Style. CodeStyle-kolmiosta klikkaamalla aukeaaa lista kieliä. Valitse JavaScript
    1. Oikealla on linkki 'Set from'. Valitse 'Predefined style' ja sieltä 'Google JavaScript Style Guide'. Nyt voit muotoilla koodin automaattisesti näppäinyhdistelmällä _alt-ctrl-l_ tai _alt-cmd-l_ 
    1. Avaa File/Settings for new projects ja tee kohdat i-iv uudestaan, jotta kaikissa uusissa projekteissa on samat asetukset.
2. Lisää projektiin HTML-tiedosto, jolla on haluamasi nimi, vaikkapa `esimerkki.html`.
3. Aseta tiedoston sisällöksi alla oleva ohjelmakoodi. Varsinainen JavaScript-koodi koostuu tässä yhdestä `console.log()`-lauseesta, joka tulostaa `Hei, maailma!`-tekstin.
Voit korvata sen haluamallasi ohjelmalla.

    ```javascript
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>JavaScript-kokeilu</title>
    </head>
    <body>
        <script>
            'use strict';
            
            console.log('Hei, maailma!');
    
        </script>
    </body>
    </html>
    ```

4. Tallenna tiedosto Ctrl-S-näppäinyhdistelmällä.

5. Paina työskentelyalueen oikeassa laidassa kelluvan selainpalkin painiketta (ks. kuva). Sivu avataan ja JavaScript-koodi
suoritetaan valitsemassasi selaimessa. Tässä materiaalissa käytetään Chrome-selainta.

    ![selainpalkki](img/selainpalkki.png)

6. Kun Chrome-selain avautuu, paina F12-näppäintä tai alt-ctrl-i tai alt-cmd-i, jolloin selaimessa aukeaa kehittäjäpaneeli. Kehittäjäpaneelissa
näet ohjelman tuottamat konsolitulosteet (kuten tässä `Hei, maailma!`-tekstin) ja pääset tarkastelemaan ohjelman
mahdollisesti tuottamia virheilmoituksia. Ks. kuva alla.
    ![konsolituloste](img/konsolituloste.png)

Tässä kuvatulla tavalla voit opiskella ohjelmoinnin perusasiat.  Myöhemmin tarkastellaan keinoja, joissa JavaScript-ohjelma saadaan reagoimaan käyttäjän verkkosivulla antamiin syötteisiin ja päivittämään verkkosivulla olevia HTML-elementtejä joko käyttäjän syötteiden tai ulkoisista tietolähteistä haettujen tietojen avulla.
