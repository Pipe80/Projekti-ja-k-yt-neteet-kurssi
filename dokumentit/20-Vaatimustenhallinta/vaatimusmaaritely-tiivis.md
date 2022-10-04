# Tiivistetty vaatimusmäärittely

|  |  |
|:-:|:-:|
| Dokumentti | Tiivistetty vaatimusmääritelmä |
| Laatija: | Pirjo M |
| Versio: |1.5 |
| Päivämäärä: | 4.10.2022 |

## Johdanto

Asiakkaana on WIMMA Lab-koulutusympäristö, joka on kehittämässä toimintaansa laajemmaksi. Asiakkaan toimeksiantona on tuottaa palveluna Foorumi-ratkaisu, WIMMA Lab-kotisivujen osaksi. Foorumin pohjana käytetään ns. Conduit-ohjelmistoa, joka on ennalta valittu asiakkaan puolesta.
Code Cerub vastaa tämän jälkeen palvelun tukemisesta ja siihen liittyvästä ylläpidosta. Projektin tavoitteena on muokata ja tuottaa Conduit-ohjelmistosta sopiva versio asiakkaan tarpeeseen. Ylläpito jatkuu erillisen sopimuksen pohjalta.
Asiakkaan edustajana toimii  WIMMA Labilla työskentelevä Kari Pitkäniemi, joka toivoo Forum-keskustelupalstan käyttöön saamista ~4 kk jälkeen projektin alkamisesta.

## Kohderyhmä 

Foorumilla voi keskustella ja kommentoida toisten aloittamia keskusteluja. Foorumille voi kirjautua ja esim. seurata muita käyttäjiä sekä tykätä toisten keskusteluista. Käyttäjäryhmänä nuoret, aikuiset ja kohderyhmään kuuluvat henkilöt, opiskelijat.


## Sidosryhmäkartta

```plantuml
@startmindmap
+ Wimma lab foorumi
++ Ohjelmoija
+++ Testaaja
++++ Asiakas
-- Toimivuus
--- Sisältö
--- Sivuston sijainti
-- Tietoturva-aukot
--- Hakkerit
--- Sivuston turvallisuus, salasanat
@endmindmap
```

**Tarkennettut sidosryhmätprofiilit** 

| ID |  Nimi | Kuvaus | Motivaatio |
|:-:|:-:|:-:|:-:|
| SR-001 | [Asiakas profiili Jonne](pohjat/pohja-profiilikuvaus.md) | Nuori 16-22V | Selkeä tarve palvelulle ja tarvitsee palvelua usein |
| SR-002 | [Asiakas profiili Anne](pohjat/pohja-profiilikuvaus4.md) | Aikuinen 22-45V | Tarve satunnainen, mutta yleisin asiakas  |
| SR-003 | [Sidosryhmä - Rahoittaja Roope](pohjat/pohja-profiilikuvaus3.md) | Pääomasijoittaja | Palvelun tuottamat tuotot |
| SR-004 | [Sidosryhmä - Hakkeri Harri](pohjat/pohja-profiilikuvaus2.md) | Nuori hakkeri | Kerätä tietoa ja haavoittuvuuksia  |
| SR-005 | [Sidosryhmä - Palveluntuottaja N5589](pohjat/pohja-profiilikuvaus5.md) | Keski-ikäinen täti-ihminen | Palvelun ylläpitäjä  |

## Palveluun liittyviä asiakaspolkuja

Kuinka saada asiakkaat sivustolle? Mainonta, sosiaalinen media, verkostot, esim. ystäväpiirit.
Kuinka saada sivustosta turvallinen? Kirjautuminen, vahva salasana, testaus.
Palvelun helppokäyttöissys

Houkutteleva visuaalinen sivuston ulkoasu. 
Helppokäyttöisyys, esim. yksinkertaiset napit, selkeät ohjetekstit, värimaailma.
Turvallisuus - palvelun käyttö on turvallista ja asiakas on tyytyväinen.

```plantuml
Step1: Asiakas löytää sivuille 
Step2: Asiakas tutustuu palveluun
Step3: Asiakas saa palvelusta ensivaikutelman
Step4: Asiakas tekee päätöksen, jääkö sivuille
Step5: Asiakas käyttää palvelua
Step6: Asiakas poistuu palvelusta

[*] --> Step1
Step1 --> Step2
Step2 --> Step3
Step3 --> Step4
Step4 --> Step6
Step4 --> Step5
Step5 --> Step6
```

## Palvelun ominaisuudet (Features)


>*Kaikki palveluun/ohjelmistoon liittyvät toiminnot (Functions) voidaan kirjaan alkuvaiheessa ns. toiminnallisina vaatimuksina (Functional Requirements), mutta näistä osa niistä osoittautuu melko varmasti palvelun kannalta oleellisiksi ominaisuuksiksi (Features). Tärkeimmät ominaisuudet on tunnistettava riittävästi alkuvaiheessa, koska niiden pohjalta ohjataan tuotekehitystä projektin edetessä.* 

>*Mietitään seuraavaksi miltä ovat palvelun tärkeimmät toiminnalliset ominaisuudet? Kirjataan ne tässä vaiheessa ne taulukkoon ja luodaan niiden pohjalta myös hahmotelma MindMap-kuvauksen muotoon. Kuvan avulla palvelun eri osa-alueet saattava hahmottua selkeämmin.* 
>*Mieti esimerkisi tilannetta, että sinulta kysytään mitä kehittämällasi palvelulla voi käytännössä tehdä? Saat aikaa vastata 15 sekuntia. Mitä vastaat?*
>*Mitä tärkeimpiä toimintoja nostatat esiin?* 
>*Mitkä ominaisuudet tekevätä tuotteestasi on paremman kuin muilla?*

**Pääominaisuudet ja toiminnot**

![](../assets/work-to-do.png)

**HUOMIO** harjoituksessa ei tarvitse määritellä itsenäistä ominaisuutta tarkemmin!

| Ominaisuus (Feature) | Toiminto (Function) |
|:-:|:-:|
| *[Sisäinen sähköposti](pohjat/pohja-ominaisuus.md)* | |
|| Asiakas_A voi lähettää postia ulkopuoliselle henkilölle Mahdollinen_Asiakas_C |
|| Asiakas_A voi saada postia palvelun sisäiseltä käyttäjältä Asiakas_B |
| *[laskutus](pohjat/pohja-ominaisuus.md)* ||
|| Ylläpito_henkilö voi poistaa laskun Asiakaalta_A |
|| Ylläpito_henkilö voi luoda uuden laskun Asiakkaalle_A | 
| *[Pelitilanteen hallinta](pohjat/pohja-ominaisuus.md)* | |
|| Pelaaja_B kykenee tallettamaan tilanteen |
|| Asiakas_B voi jakaa pelitilanteen Asiakkaalle_A |
| *[Suorasoitto](pohjat/pohja-ominaisuus.md)* ||
|| Asiakas_A voi soittaa tuntemalleen henkilölle Asiakas_B |
|| Asiakas_A voi soittaa tuntemattomalle henkilölle, jos soitto on sallittu |


>Jokainen ominaisuus kannattaa kuvata itsenäisenä dokumenttina, koska niihin liittyy paljon tarkentavaa tietoa. Tutustu esimerkkinä [FEAT0001](20-Vaatimustenhallinta/ominaisuus-FEA0001.md). Kuvauksen tekemiseen käytetään tarvittaessa seuraavaa [pohjaa](pohja/../pohjat/pohja-ominaisuus.md). 


**Kirjataan ominaisuudet vielä MindMap-muotoon ja samalla linkitetään niihin liittyvät toiminnot**

![](../assets/work-to-do.png)

```plantuml
@startmindmap
+ Tuote X, eli tuotettava ratkaisu
++ Ominaisuus A - sisäinen sähköposti
+++ Asiakas_A voi lähettää postia toiselle henkilölle
+++ Asiakas_A voi saada postia toiselta henkilöltä
++ Ominaisuus B - Laskutus
+++ Ylläpito-henkilö voi poistaa laskun Asiakaalta
+++ Ylläpito-henkilö voi luoda uuden laskun Asiakkaalle
-- Ominaisuus C - Dokumentin jakotoiminto
--- Toiminto 5 - Asiakas_B voi jakaa kuvatiedoston
--- Toiminto 6 - Asiakas_A voi kommentoida dokumenttia
-- Ominaisuus D - Pelitilanteen talletus
--- Toiminto 7 - Pelaaja_C kykenee tallettamaan tilanteen valitulla hetkellä
--- Toiminto 8 - Pelaaja_C voi poistaa aiemman talletukse
@endmindmap
```

# Toiminnalliset vaatimukset (Functional Requirements)

>Kuten huomasit yksittäinen toiminto (Function) liittyy yleensä laajempaan kokonaisuuteen eli ominaisuuteen (Feature). Määrittelyn alkaessa kaikki tunnistetut toiminnot voi kirjata ns. toiminnallisina vaatimuksina esimerkiksi taulukon muotoon. Tämän jälkeen voidaan tunnistaa niistä tärkeimmät ominaisuudet ja liittää niihin esiin tulleet toiminnot. 

Kaikkia vaatimuksia (myös ei-toiminnalliset vaatimukset) koskevat seuraavat ehdot:

![](../assets/work-to-do.png)

* *Vaatimus on yksilöllinen ja identifioitu*
* *Vaatimus on oltava mitattavissa*
* *Vaatimuksen on oltava yksiselitteinen ja selkeä*
* *Vaatimukseen ei tule sisällyttää useampia vaatimuksia*
* *Vaatimus kannattaa perustella, jos tarpeen*
* *Vaatimuksen ei saa ylikirjoittaa aiemmin määriteltyä vaatimusta*
* *Edustaako kirjattu vaatimus itseasiassa ominaisuutta?*

| ID | Toiminnallisen vaatimuksen kuvaus | ominaisuus	|				
|:-:|:-:|:-:|
| [FUNCREQ-C0001]() | Palveluun kirjautumisessa voidaan käyttää Facebook-tunnuksia | [Kirjautumis-ominaisuus](pohjat/pohja-ominaisuus.md) |
| [FUNCREQ-C0002]() | Käyttöliittymää voidaan ohjata tarvittaessa äänikomennoilla | [Ääniohjaustuki-ominaisuus](pohjat(pohjat/pohja-ominaisuus.md)) |
| [FUNCREQ-C0003]() | Käyttäjä voi vaihtaa kirjautumisikkunassa kielen | [Kirjatumis-ominaisuus]() |
| [FUNCREQ-C0004]() | ... | ... |

## Käyttöliittymänäkymä/mockup 

![](../assets/work-to-do.png)

>*Eri ominaisuuksien ja niihin liittyvien toiminnallisuuksien selkeyttämiseksi voidaan hyödyntää myös erilaisia kuvauksia. Kuvausten avulla pyritään hahmottamaan miltä tuotteen tulisi näyttää tai mitä on otettava huomioon käyttöliittymätoteutuksessa? Tähän tarkoitukseen voi soveltaa nykyaikaisia ns. MockUp/prototyyppityökaluja. Näiden välineiden avulla voidaan luoda helposti käyttöliittymästä nopea kokeiluverso, jota voidaan koekäyttää eri kohderyhmillä.* 
>*Ominaisuuksien toteutuksiin liittyvät prototyyppi kuvaukset kannataa liittää ominaisuuksien määrittelydokumentteihin, jolloin ne löytyvät asian mukaisesta paikasta. Tutustu esimerkkinä [Feature-FEA0001](20-Vaatimustenhallinta/ominaisuus-FEA0001.md)
>*Perinteisesti käyttöliittymä hahmotelmat ja kuvaukset on tehty piirtämällä käyttöliittymästä staattisia kuvia ja näitä on käytetty suunnittelun apuna. Tämä onnistuu myös soveltamalla apuna PlantUML-kuvauksia. (ks. alla) Kannattaa kuitenkin tutustua ja kokeilla arjolla olevia prototyyppi/MockUp-työkaluja tähän tarkoitukseen.*  

 * [Lisää tähän linkki prototyyppiin / MockUp-toteutukseen]()
 * Kokeile myös upottaa prototyyppi IFRAMEn muodossa? 

**Alla esimerkki yksinkertaisesta PlantUML:n avulla muodostetusta käyttöliittymän dialogista**

```plantuml
salt
{
  Just plain text
  [This is my button]
  ()  Unchecked radio
  (X) Checked radio
  []  Unchecked box
  [X] Checked box
  "Enter text here   "
  ^This is a droplist^
}
```

## Ketterän kehittämisen käyttötarinat - User Story 

![](../assets/work-to-do.png)

>*Nykyaikaisessa ohjelmistokehityksessä on yleistynyt tapa käyttää tarkkojen vaatimusten sijaan eri sidosryhmiltä kerättyjä kuvauksia tarvittavista toiminnoista. Näitä kuvauksia nimitetään käsitteellä käyttötarina eli *User Story*. Kannattaa tutustu aiheeseen [User Story](https://en.wikipedia.org/wiki/User_story). Käyttötarinat ovat kehitystiimin kannalta erittäin oleellisia, koska ne kuvaavat toimintoja, joita palvelulta odotetaan. Käytännössä User Storyjen avulla ohjataa koko kehitystiimin tavoitteellista työskentelyä projektin aikana.*

>Käyttötarina kuvauksen yleinen muoto on: 

* Englanniksi: As a <-role-> I can <-capability->, so that <-receive benefit->*

* Vapaasti suomennettuna: Palvelun käyttäjän <-roolissa X-> voin tarvittaessa suorittaa <-toiminnon->, koska <-perustelu->* 

>*Yksittäinen käyttötarina (User Story) voidaan kirjata esim Gitlab-palvleussa ns. Issuen muotoon. User Storyt voi alkuvaiheessa kerätä myös taulukkoon/listaan ja siirtää ne sopivalla hetkellä Issue-muotoon.*

**Esimerkki, jossa on linkitys issueen**

* *Käyttäjänä haluan, että voin luoda raportin tekemistäni ostoista viimeisen kuukauden ajalta, koska se helpottaa oman talouteni hallintaa* #14

## Tietojärjestelmiä yleisesti koskevista vaatimuksista

>Laajoja tietojärjestelmiä/ohjelmistoja suunniteltaessa vaatimuksia voidaan kirjata eri näkökulmista. Tietojärjestelmien suunnittelussa voi käyttää analogiana kuvaa jäävuoresta, josta pinnalla näkyy osa, mutta iso osa (90%) on piilossa veden alla. Tämä pätee tietojärjestelmän vaatimuksiin. Korkealta tasolta katsottuna näyttää kokonaisuus ehkä selkeältä, mutta yksityiskohtiin mentäessä työ hankaloituu. 

![](https://openclipart.org/image/400px/29153)

>Vaatimusmäärittelyn työstäminen voidaan nähdä kahden eri näkökulman kannalta.

**Ongelma kenttä (Problem Domain) vs Ratkaisu kentttä (Solution Domain)**

>Eli on tunnettava riittävän tarkasti ongelmakenttä (Asiakkaan/toimeksiantajan tarve), että voidaan kehittää siihen sopiva ratkaisu (esim. ohjelmistopalvelu)

>Tietojärjestelmän vaatimusten eri muotoja voivat olla olla esimerkiksi
>* Asiakasvaatimukset (Customer Needs)
>* Liiketoimintavaatimukset (Business Requirements/Needs)
>* Järjestelmävaatimukset (System Requirements)
>* Ali-järjestelmän vaatimukset (Sub-System Requirement)
>* Komponenttitason vaatimukset (Component Requirements)

>Opintojakson kannalta keskitytään tunnistamaan toiminnalliset vaatimukset, ei-toiminnalliset vaatimukset (suorituskyky, tietoturva ja saavutettavuus)

* [Vaatimusmäärittelystä Wikipediassa](https://en.wikipedia.org/wiki/Requirements_analysis)

*Vaatimusten jäljitettävyydestä*

>Eri vaatimusten eri muodoilla voidaan tarkastella kehitettävää tuotetta eri näkökulmista, mutta eri tasojen välillä olevilla vaatimuksilla voi olla yhteys. 
Näitä yhteyksiä kutsutaan vaatimusten jäljitettävyydeksi (Traceablity). 

> * *Asiakasvaatimus CUST001* -> *Ominaisuus FEA001* --> *Toiminnallinen vaatimus Y*
> * *Asiakasvaatimus CUST001* -> *Liiketoiminnan vaatimus BISREQ100* -> *Ominaisuus FEA001*
> * *Tietoturvavaatimus SEC001* -> *Ominaisuus FEA001*

>Vahvan jäljitettävyyden avulla voidaan tarkastella yksittäisten muutosten vaikutusta koko tuotteeseen. Tässä tilanteessa voidaan yksittäistä vaatimusta "törmäyttää" ja nähdään minne kaikkialle vaikutus ulottuu (Impact analysis).
>Tämän vaatii vaatimusmäärittelytyön tueksi tarkoitukseen sopia työkaluja (Requirement Management Tools)

## Palveluun liittyvät tekniset vaatimukset

>Kokonaisvaltaisia ohjelmisto palveluja määriteltäessa on tärkeä tunnistaa ja määritellä palvelun tuottamiseksi tarvittavat teknologiat, laitteistot tai muut tärkeät osa-järjestelmät. Esimerkkinä tarvittava palvelinympäristö, tietokanta, varmistusjärjestelmät ja muut palvelun toiminnan kannalta oleelliset tarpeet.

*Esimerkkinä on kirjattu muutamia laitteistovaatimuksia (Hardware Requirements)*

| ID | Kuvaus | 
|:-:|:-:|
| HWREQ-0001 | Palvelun on oltava skaalattavissa HA-proxy ratkaisun varassa | |
| HWREQ-0002 | Palvelimen muistikapasiteeti >32GB  ||
| HWREQ-0003 | Palvelimen fyysinen sijainti on oltava EU-aluella| |
| HWREQ-0004 |... ||

## Laadulliset vaatimukset (Non-functional Requirements)

>Laadulliset vaatimukset tarkastelevat palvelua ns. ei-toiminnallisesta näkökulmasta. Kuulostaa ehkä äkkiseltään hankalalta, mutta mieti seuraavia kysymyksiä?

* *Miten tuottesta saadaan kehitettyä riittävän turvallinen? Onko joitain vaatimuksia, jotka on täytettävä tästä johtuen? (tietoturva-security)*
* *Mitkä asiat on huolehdittava, että tuote on hyväksyttävissä viranomaisten käyttöön? (yhteensopivuus-conformance)*
* *Miten paljon käyttäjiä palvelussa voi olla yhtäaikaa(suorituskyky-performance)
* *Onko palvelun tarkoitus joskus toimia laajemmalle käyttäjäkunnalle(skaalautuvuus-scalability)*
* *Miten voidaan varmistaa, että palvelu on saavutettavissa kaikkien käyttäjien kannalta?(skaalautuvuus-scalability)*
* *Onko tarvetta eri kieliversioille?(saavutettavuus-accessability)*
* *Mitä on otettava huomioon palvelua jatkokehitettäessä? (ylläpidettävyys-maintainability)*
* *Mitä teknologioita voidaan käyttää?(ylläpidettävyys-maintainability)*

>[Ei-toiminnalliset vaatimuksia](https://en.wikipedia.org/wiki/Non-functional_requirement) on useita eri tyyppejä, mutta opintojen kannalta tärkeimmiksi on valittu: suorituskyky, tietoturva ja saavutettavuus 
>* Suorituskyky (Performance Requirement)
>* Tietoturva (Security Requirement)
>* Saavutettavuus (Accessability Requirement)

### Suorituskykyvaatimukset (Performance Requirements)



>Millaisia vaatimuksia palveluun kohdistuu suorituskyvyn näkökulmasta?
>Mitä tarkoittaa suorituskyvyn testaus, eli [load testing](https://en.wikipedia.org/wiki/Load_testing) Tutustu myös K6-työkaluun? [K6-Load Tester](https://k6.io/)

| ID | Kuvaus |
|:-:|:-:|
| PERFREQ-0000 | Kirjautuminen on mahdollista yhtäaikaa x käyttäjällä |					
| PERFREQ-0001 | Palvelun maksimi käyttäjä määrä on ? |
| PERFREQ-0002 | Palvelun kotisivu aukeaa < Xs ||

### Tietoturvavaatimukset (Security Requirements)

![](../assets/work-to-do.png)

>Millaisia vaatimuksia palveluun kohdistuu tietoturvan näkökulmasta? 
> Tutustu [VAHTI 1/2013 Sovelluskehityksen tietoturvaohje](https://www.suomidigi.fi/ohjeet-ja-tuki/vahti-ohjeet/vahti-12013-sovelluskehityksen-tietoturvaohje)
> Tarkista esimerkkinä [TRAFICOMin tietoturvamerkki](https://tietoturvamerkki.fi/fi/vaatimukset/)


| ID |  Kuvaus |
|:-:|:-:|
| SECURITY-REQ-0001 | Salasanassa on käytettävä vähintään MD5-tason salausta, koska vaatimus [CONSTRAIN-000]() sitä edellyttää |
| SECURITY-REQ-0002 | Jokainen tapahtuma palvelussa on kirjattava käyttölogiin, että niitä voidaan tarkastella myöhemmin | 
| SECURITY-REQ-0003 | ... |

### Saavutettavuusvaatimukset (Accessablity Requirements)

![](../assets/work-to-do.png)

>Mitä tarkoitetaan saavutettavuudella? Millaisia asioita/ohjeistuksia on otettava huomioon palvelua toteutettaessa? Tutustu lähteeseen: [https://www.saavutettavuusvaatimukset.fi/](https://www.saavutettavuusvaatimukset.fi/)

| ID  |  Kuvaus |
|:-:|:-:|
| ACCESSREQ-0000 | Palvelun käyttöliittymässä on mahdollista valita selkeä kontrastinen teema |	
| ACCESSREQ-0001 | Käyttöliittymän Fonttikokoa on voitava muuttaa päävalikon kautta |
| ACCESSREQ-0002 |  ... |

## Rajaukset ja reunaehdot (Constraints and limitations)

>Eri ohjelmistojena/palvelujen toteutusta ja käyttöä ohjaavat usein lait ja säädökset. Näiden edellyttämät vaatimukset kirjataan vaatimusmäärittelyyn rajauksina. Rajausten (Constraints) vaikutus voi koskea koko palvelua palvelun jonkin osa-kokonaisuuden toteuttamista. Tästä syystä eri rajoitteet on tunnistettava ajoissa, koska vaikutus saataa olla varsin ratkaiseva pitemmällä tähtäimella. Esimerkkinä tästä on viime vuonna voimaan tullut [EU GDPR-säädös](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation).
Kannattaa tutkia esimerkiksi https://www.sfs.fi/aihealueet/terveydenhuolto/laakinnalliset_laitteet tai http://docs.jhs-suositukset.fi/jhs-suositukset/JHS190/JHS190.html

| ID |  Rajaus/reunaehto | Mihin vaikuttaa |
|:-:|:-:|:-:|
| CONSTRAIN-000  |  Palvelun kirjautumisprosessin on noudatettava JUHTA-hyväksyttyjä käytänteitä  | [Feature Kirjautuminen](pohjat/pohja-ominaisuus.md) |
| CONSTRAIN-001 |  Palvelussa on huomioitava JHS:n suosituksest lokihallinasta | [Feature - Lokihallinta](pohjat/pohja-ominaisuus.md)|
| CONSTRAIN-002 |  ... | ... |

## Ohjelmistoarkkitehtuuri

>Vaatimusmäärittelyn osaksi voidaan tarvittaessa liittää teknillisiä kuvauksia, joiden avulla voidaan tarkentaa eri vaatimuksia. Yksi tärkeä dokumentti voi olla esimerkiksi tekninen arkkitehtuuri. Tämä kuvaus voidaan lyhyessä muodossaan liittää osaksi vaatimusmäärittelyä, mutta yleensä se on varsin laaja itsenäinen dokumentaation osa. Arkkitehtuuri ratkaisujen kuvaamiseksi voidaan laatia yödyntäen apuna UML-kuvauskielen eri diagrammeja. Esimerkkinä alla on  sijoittelunäkymä ([Deployment Diagram](https://plantuml.com/deployment-diagram)). Sijoittelunäkymän avulla voidaan kuvata miten palvelun eri palvelut sijaitsevat ja miten ne kytkeytyvät toisiinsa.

Ohjelmistoarkkitehtuurin kuvaus on itsessään laaja osa-alue ja käytännössä se edellyttää laajempaa dokumentaatiota.

* [Tähän linkki erilliseen ohjelmistoarkkitehtuurin kuvaukseen](../30-Suunnittelu-ja-toteutus/arkkitehtuuri-ja-tekninentoteutus.md)

```plantuml
@startuml
actor User
node "Client_Host" as WIN10{
node "Browser"{
}
}

cloud "Network" as net{
queue "https"{
}
}

node "Uno Server / Ubuntu 20.04" as AWS{ 
node "Frontend_Container"{ 
}
node "Backend_Container" {
}
database "MariaDB_Container" {
}
node "Logger_Container" {
}

}
User -- Browser
Browser -- https
https -- Frontend_Container
Frontend_Container -- Backend_Container
Backend_Container -- MariaDB_Container
Logger_Container -- Frontend_Container
Logger_Container -- Backend_Container
Logger_Container -- MariaDB_Container

@enduml
```

## Standardit ja lähteet

>Kirjataan käytetyt lähteet alla olevaan taulukkoon.

| ID | Nimi | Linkki | Kuvaus |  
|:-:|:-:|:-:|:-:|
| REF1 | JHS 165 ICT | [JHS Suositukset - vaatimusmäärittelylle](http://www.jhs-suositukset.fi/c/document_library/get_file?uuid=b8118ad7-8ee4-459a-a12b-f56655e4ab9d&groupId=14) | Vaatimusmäärittelyn suositus |
| REF2 | ISO 9241-11  | [Käytettävyys](https://fi.wikipedia.org/wiki/K%C3%A4ytett%C3%A4vyys)  | Usability | 
| REF3 |  EN 301 549 | [Saavutettavuus](https://fi.wikipedia.org/wiki/Saavutettavuus) | Availability |
| REF4 |  GDPR | [GDPR Asetus](https://europa.eu/youreurope/business/dealing-with-customers/data-protection/data-protection-gdpr/index_fi.htm) | General_Data_Protection_Regulation |
| REF5 | KATAKRI V11 | [Katakri](https://www.defmin.fi/files/1870/KATAKRI_versio_II.pdf) | Kansallinen turvallisuusauditointikriteeristö |


