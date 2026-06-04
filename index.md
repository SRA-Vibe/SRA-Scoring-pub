# Alpha² – SRA Scoring – tietosuojaseloste

> **Huom:** Alpha² on itsenäisen kehittäjän tekemä sovellus. Se ei ole
> Reserviläisurheiluliiton (ResUL) tai SRA:n virallinen tai hyväksymä
> sovellus, vaikka se on yhteensopiva SRA 8.1 -kilpailusääntöjen kanssa.

Päivitetty: 4.6.2026

Tämä seloste kuvaa, miten **Alpha² – SRA Scoring** -sovellus käsittelee
henkilötietoja. Sovellus toimii kokonaan käyttäjän laitteella eikä
lähetä tietoja verkkoon. Sovelluksessa ei ole mainoksia, ei käyttäjä-
seurantaa eikä kolmansien osapuolten työkaluja.

> Laitteen aloitusnäytöllä sovellus näkyy nimellä **Alpha²**.
> *Alpha² – SRA Scoring* on Play Storen virallinen julkaisunimi.
> Nämä ovat sama sovellus.

## Rekisterinpitäjä

Sovelluksen kehittäjä: Niitti (yksityishenkilö, sovelluksen kehittäjä)
Yhteydenotot: sra.scoring@gmail.com

Tietosuojaa koskevissa virallisissa pyynnöissä (esim. rekisteröidyn
oikeuksien käyttäminen, tietosuojavaltuutetun toimiston kyselyt)
rekisterinpitäjä toimittaa täydet yhteystietonsa erikseen pyynnöstä.

## Mitä tietoja sovellus käsittelee

Sovellus tallentaa seuraavat tiedot käyttäjän laitteen sisäiseen
tietokantaan:

**Käyttäjäprofiili:**
- Etu- ja sukunimi
- Seura
- Mahdollinen SRA-jäsennumero
- Mahdollinen SRA-status (ampuja, tuomari, kouluttaja, ylituomari)
- Oletusluokka (Vakio, Avoin, TST)

**Kilpailutiedot:**
- Kilpailun nimi, päivämäärä ja järjestäjä
- Kilpailun rastit, niiden määritykset ja maalit
- Kilpailuun lisättyjen ampujien nimet, seurat ja luokat
- Pisteet, ajat, osumat ja erikoistilat (DNF, DNS, ZEROED, DQ)
- Auditointitiedot: kuka kirjasi mitäkin (käyttäjäprofiilin nimi)

**Muut:**
- Sovelluksen asetukset (esim. oletusluokka, viimeisin
  varmuuskopiointi-aika)

## Tietojen sijainti ja siirrot

Kaikki tiedot tallentuvat **vain käyttäjän laitteen sisäiseen
tietokantaan**. Sovellus ei lähetä tietoja sovelluksen kehittäjälle,
SRA:lle, mainostajille, analytiikka- tai muillekaan ulkopuolisille
tahoille. Sovellus ei käytä Internet-yhteyttä.

Käyttäjä voi viedä omaa dataa JSON-muotoon valitsemaansa paikkaan
(esim. pilvitallennukseen tai muulle laitteelle). Vientipaikan
tietosuojakäytännöistä vastaa kyseinen palvelu, ei Alpha².

## Diagnostiikka- ja kaatumisloki

Jos sovellus kaatuu, se kirjoittaa laitteelle paikallisen
diagnostiikkalokin vianetsintää varten. Loki sisältää **vain teknisiä
tietoja**: sovelluksen version, Android-version, laitteen mallin,
aikaleiman ja virheen teknisen kuvauksen (stack trace). **Loki ei
sisällä kilpailutietoja, ampujien nimiä eikä muuta henkilödataa.**

Loki tallentuu vain laitteelle eikä sitä lähetetä automaattisesti
mihinkään. Voit halutessasi viedä lokin sovelluksen
Varmuuskopiointi-näkymän "Vie diagnostiikkaloki" -toiminnolla ja jakaa
sen kehittäjälle vianselvitystä varten — tämä tapahtuu täysin omasta
aloitteestasi. Loki poistuu samalla kun poistat sovelluksen tai
tyhjennät sen tiedot.

## Käsittelyn oikeusperuste

Tietojen käsittely perustuu käyttäjän suostumukseen, jonka käyttäjä
antaa täyttäessään profiilin sovelluksen aloituskyselyssä, ja
käyttäjän omaan käyttötarkoitukseen (kilpailujen pisteytys).

## Säilytysaika

Tiedot säilyvät niin kauan kuin käyttäjä pitää sovelluksen
asennettuna ja tietoja sovelluksen sisällä. Sovelluksen
poistaminen laitteelta poistaa kaikki sovelluksen tallentamat tiedot
samalla.

Käyttäjä voi milloin tahansa poistaa yksittäisiä tietoja sovelluksen
kautta tai poistaa koko datan poistamalla sovelluksen.

## Käyttäjän oikeudet

Koska tiedot ovat käyttäjän laitteella, käyttäjä hallitsee niitä
itse:

- **Tarkastusoikeus:** kaikki tallennettu data näkyy sovelluksessa.
- **Vienti:** "Varmuuskopiointi" -toiminto vie koko datan
  JSON-tiedostoksi.
- **Korjausoikeus:** profiili- ja kilpailutietoja voi muokata
  sovelluksessa.
- **Poisto-oikeus:** yksittäisiä tietoja voi poistaa sovelluksen
  kautta. Koko datan saa pois poistamalla sovelluksen.

## Tietojen poistaminen

Tämä koskee sovellusta **Alpha² – SRA Scoring** (kehittäjä: Niitti).

Sovellus toimii kokonaan laitteellasi. Kehittäjä **ei kerää, vastaanota,
siirrä eikä säilytä** tietojasi millään palvelimella, joten kehittäjällä
ei ole sinusta dataa, jota voisi erikseen pyytää poistettavaksi. Hallitset
tietojasi itse laitteella seuraavasti.

**Miten poistat tietosi**

- **Yksittäiset tiedot:** poista kilpailuja, ampujia tai muita tietoja
  suoraan sovelluksessa.
- **Kaikki sovelluksen data kerralla:** Android-asetukset → Sovellukset →
  *Alpha²* → Tallennustila → **Tyhjennä tiedot**. Tämä poistaa kaikki
  sovelluksen tallentamat tiedot välittömästi.
- **Koko sovellus ja sen data:** poista sovellus (*uninstall*). Tämä
  poistaa kaikki sovelluksen tallentamat tiedot laitteelta.
- **Itse tekemäsi varmuuskopiot:** jos olet vienyt dataa JSON-tiedostoksi
  (Varmuuskopiointi-toiminto), poista kyseiset tiedostot itse siitä
  paikasta, johon tallensit ne (esim. laitteen muisti tai pilvitallennus).

**Mitä poistetaan ja mitä säilytetään**

- **Poistetaan:** kaikki sovelluksen tallentamat tiedot — käyttäjäprofiili
  (nimi, seura, mahdollinen SRA-jäsennumero, oletusluokka), kilpailut,
  rastit, ampujat, pisteet, ajat, erikoistilat ja asetukset.
- **Säilytetään:** ei mitään kehittäjän tai palvelimen toimesta. Koska
  tiedot ovat vain laitteellasi eikä niitä lähetetä mihinkään, tietojen
  tyhjennys tai sovelluksen poisto poistaa ne **välittömästi ja
  pysyvästi**. Palvelinpuolen säilytysaikaa ei ole (kehittäjä ei säilytä
  kopiota).

## Lapset

Sovellus on tarkoitettu kilpailujen pisteytystyökaluksi SRA-ampujille
ja toimitsijoille. Sitä ei ole suunnattu eikä markkinoida lapsille.
SRA-toimintaan voi osallistua myös alle 18-vuotias, mutta tällöin
edellytetään huoltajan allekirjoittama kirjallinen osallistumislupa;
sovellus ei kerää tätä lupaa eikä käsittele alaikäisyyteen liittyviä
erityistietoja. Jos alaikäinen on kilpailussa mukana, hänen nimensä ja
tuloksensa tallentuvat samalla tavalla kuin muidenkin osallistujien —
tiedot pysyvät järjestäjän laitteella eikä niitä lähetetä verkkoon.

## Tietoturva

Tiedot tallentuvat Android-järjestelmän sovelluskohtaiseen
yksityiseen tallennustilaan. Tämän tallennustilan suojaus perustuu
laitteen lukitukseen (PIN/sormenjälki/kasvotunnistus). Sovellus
suosittelee laitteen lukituksen pitämistä päällä.

Sovellus ei salli automaattista Android Auto Backup -varmuuskopiointia
Google Driveen.

## Muutokset selosteeseen

Selostetta päivitetään tarvittaessa. Päivitetty versio julkaistaan
samassa osoitteessa. Käyttäjälle ei lähetetä erillistä ilmoitusta
muutoksista, mutta merkittävät muutokset esitellään sovelluksen
julkaisutiedotteissa Play Storessa.

## Yhteydenotot

Tietosuojaa koskevissa kysymyksissä: sra.scoring@gmail.com
