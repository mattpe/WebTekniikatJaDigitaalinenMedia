# JavaScript: Opiskelu ja tehtävien palautus

## Materiaalien opiskelu ennen tunteja

JavaScript-materiaalit opiskellaan nk. flipped classroom -metodilla. Tämä tarkoittaa sitä, että materiaaleihin perehdytään etukäteen ja tunneilla keskitytään tehtävien tekemiseen opettajan avustuksella.

Tehtäviä voi ja kannattaa tehdä myös etukäteen, sillä niitä kaikkia ei ehkä ehdi tuntien aikana tekemään. Tehtävät palautetaan OMAan alla olevan ohjeen mukaisesti. Myöhässä palautetuista tehtävistä vähennetään niistä annettavia pisteitä tai jätetään arvioimatta kokonaan.

## Tehtävien tallentaminen kotihakemistoon

Tee tehtävien palautusta varten alihakemisto _users.metropolia.fi_ -palvelimella olevaan public_html kotihakemistoosi ja siirrä koodisi sinne. Siirron voit tehdä monella tapaa, esim. suoraan WebStorm tai VSCode -kehitysympäristöistä, erillisellä SCP-tiedostonsiirto-ohjelmalla (kuten WinSCP, Cyberduck, Filezilla, tms.) tai Metropolian verkkolevyjen weppi-käyttöliittymällä [Webdiskillä](https://webdisk.metropolia.fi/).

- yhteyden muodostaminen:
  - Protokolla: SFTP, portti 22
  - osoite: shell.metropolia.fi
- web-sivujen kansio:
  - public_html ja sen alikansiot
- osoite web sivuille:
  - users.metropolia.fi/~tunnus/[kansio][/][tiedosto]
- Tarvittaessa säädä oikeudet tiedostoille ja kansioille
  - oikea hiiren nappi/properties (tai info)/permissions
  - 755 (tai 0755)
  - puttyllä/terminaalilla:
    - (mäkillä: ssh tunnus@shell.metropolia.fi)
    - chmod -R 755 public_html/kansion_nimi

Lisätietoja kotisivuista [tietohallinnon ohjeesta](https://wiki.metropolia.fi/display/tietohallinto/Kotisivu-%2C+Shell-+ja+MySQL-palvelut).

## Tehtävään vastaaminen OMAssa

1. Jos tehtävät toimivat, etkä halua/tarvitse opettajalta palautetta, palauta:
    1. **Klikattava linkki**, joka johtaa _users.metropolia.fi_:llä oleviin tiedostoihisi.
    1. Laita HTML-tiedoston nimeen (ainakin osaksi) tehtävän numero.
    1. Listaa palautuskenttään ne tehtävät, jotka teit kokonaan ja ne jotka teit osittain. **Testaa ohjelma huolella ja laita vastaukseen kommentti, jos ei toimi.**
    1. Kirjoita myös kokonaan tehtyjen tehtävien pistemäärä ja niiden yhteispisteet
      -Pistemäärät löytyvät tehtävien ohjeista
1. Jos haluat opettajalta palautetta tai apua, palauta **klikattava linkki**, joka johtaa users.metropolia.fi:llä oleviin tiedostoihisi ja pyydä opettaja paikalle.
1. Jos olet sairaana tms. toimi kohdan A mukaan.

**_HUOM!_ Jos vastauksessasi oleva linkki ei ole klikattava, tehtävää ei arvioida.**
