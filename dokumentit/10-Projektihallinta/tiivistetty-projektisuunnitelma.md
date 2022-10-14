# Tiivistetty projektisuunnitelma

|  |  |
|:-:|:-:|
| Dokumentti | Tiivistetty projektisuunnitelma |
| Laatija: | Pirjo M |
| Versio: | 1.8|
| Päivämäärä: |6.10.2022 |

![](https://cdn.pixabay.com/photo/2018/08/06/21/32/darknet-3588402_1280.jpg)

## 1. Toimeksianto 
## 1.1 Tausta ja lähtökohdat

KCodeCerub Oy on saanut asiakkaakseen WIMMA Lab-koulutusympäristön, joka on nyt laajentamassa toimintaansa. WIMMA Labin toimintaa pyritään avaamaan eri sidosryhmille ja siihen tarvitaan uusia sähköisiä palveluja. Toimeksianto CodeCerub Oy:lle on kehittää WIMMA Labin käyttöön soveltuva Foorumi-palvelu, joka liitetään osaksi kotisivuja. Foorumin toteutuksen pohjana hyödynnetään (Open Source) avoimen lähdekoodin perustuvaa Conduit-ohjelmistoa, jo on asiakkaan esittämä vaatimus. Syynä tähän on tiukka aikataulu. Asiakkaalla on vahva oletus, että tämä säästää aikaa kehitykseltä ja voidaan keskittyä nopeampaan käyttöönottoon.
Projekti toteutetaan Jyväskylän ammattikorkeakoulun järjestämän <TTC2070> ‑opintojakson puitteissa.

## 1.2 Tavoitteet ja tehtävät

Projektina on toteuttaa WIMMA Labin käyttöön soveltuva Foorumi-palvelu, joka liitetään osaksi kotisivuja.
Projektin tavoite on muokata ja kehittää nykyisestä Conduit-ohjelmistosta paremmin asiakkaan tarpeeseen sopiva versio. Tärkeimpinä toimintoina asiakas edellyttää käyttöliittymän sulavaa integrointia WIMMA Lab-kotisivun kanssa ja saumatonta liittämistä osaksi kotisivuja. Lisäksi tietosuojan vaikutukset on otettava huomioon palvelun tuotannossa.

Asiakkaan edustajana toimii ohjaaja Kari Pitkäniemi

Johtoryhmään kuuluvat seuraavat henkilöt:
Pirjo M (N5589)
WIMMA Labin tekninen arkkitehti Teemu K
WIMMA Labin edustaja Kari Pitkäniemi.
Tuoteomistaja Marko Rintamäki

Tietoturvan osalta edellytetään Kyberturvallisuus keskuksen jakamia tunnettuja hyviä käytänteitä. 
Nämä lähteet toimivat myös lähteinä vaatimusmäärittelylle.  ![](https://www.kyberturvallisuuskeskus.fi/fi/toimintamme/saantely-ja-valvonta/tietoturva)

## 1.3 Rajaus ja liittymät

Projektin tehtävänä on toteuttaa Conduit-ohjelmiston pohjalle Foorumi-ratkaisu asiakkaan toiveiden mukaan. 
Palvelun ylläpitovastuu jää tuotteen toimituksen jälkeen Code Cerub:ille. Toimeksiantoon eivät liity muut ratkaisut Foorumin ulkopuolella.

## 1.4 Oikeudet

Eri osapuolten oikeudet on määritelty projektisopimuksessa.

## 1.5 Termit ja määritelmät

CASE = Computer aided software engineering, tietokoneavusteinen systeemityö
JAMK = Jyväskylän ammattikorkeakoulu
SWOT-kuvaus = Strengths, Weaknesses, Opportunities, Threats eli suomeksi Vahvuudet, Heikkoudet, Mahdollisuudet ja Uhat
IT = Information technology

## 1.6 Projektiin liittyvät haasteet
![SWOT](assets/swot.jpg)

ps. pöllöt löytyi, olin täyttänyt vahingossa laajaa projektisuunnitelmaa, damned.

## 2. Projektiorganisaatio

## 2.1 Organisaation esittely

**Projektiorganisaation rakenne MindMap-muodossa**

```plantuml
@startmindmap
+ Conduit
++ N5589
+++ Teemu K
+++  Marko Rintamäki
-- CodeCerub
--- Asiakkaan edustaja Kari Pitkäniemi
++ Laadunvalvonta organisaatio
+++ Testipäällikkö
+++ Testaaja
+++ Käytettävyystestaaja
@endmindmap
```
![Tiimin esittely](https://gitlab.labranet.jamk.fi/fi-a2022-ttc2070/ht1-N5589-/core/-/blob/master/dokumentit/10-Projektihallinta/esittely.md)

## 2.2 Vastuut ja päätöksentekoprosessi

>Tähän kirjataan kaikkien projektiorganisaatioon kuuluvien (esim. johtoryhmä, projektipäällikkö, sihteeri, ryhmä, >ohjaajat) vastuut sekä päätöksentekoprosessi (esim. projektipäällikkö valmistelee ja esittää johtoryhmän päätettäväksi…)

>”Projektiryhmä suorittaa johtoryhmän projektille asettam[]at tehtävät käytettävissä olevien resurssien puitteissa. >Projektin aikana ryhmän päällikön ja sihteerin roolit kiertävät ryhmän sisällä siten, että jokainen ryhmän jäsen toimii >kerran kummassakin roolissa.”

>”Johtoryhmän muodostavat siihen valitut projektiryhmän, ohjaajien ja toimeksiantajan edustajat. Johtoryhmän kokouksiin >voidaan tarvittaessa kutsua myös muita henkilöitä, esim. asiantuntijoita.Johtoryhmän kokoonpano on esitelty >projektisopimuksen liitteessä <X>.” 

>Tukiryhmän tehtävänä on antaa projektiryhmälle sisällöllistä opastusta tehtävän suorittamiseksi. Kappaleessa tulee >esitellä projektin muut sidosryhmät (asiakas, ulkopuoliset konsultit, jne.) henkilötasolla. Asiakkaan mukana olevista >henkilöistä tulee mainita ainakin nimi, yhteystiedot, toimenkuva sekä rooli projektissa.


## 2.3. Projektin vaiheet ja taloudelliset tavoitteet

>tehtäväkokonaisuudet, osittelu ja vaiheistus, välitulokset, aikataulut ja resurssissuunnitelmat, budjetti

## 2.4. Laadun varmistus

>menetelmät, standardit, hyväksymismenettely, muutosten hallinta, dokumentointi, katselmoinnit, riskien hallinta, muut täydentävät suunnitelmat

## 2.5. Tiedonvälitys ja projektin etenemisen seuranta

>projektin aloitus, työtilat ja viestintävälineet, palaverikäytäntö ja yhteydenpito, raportointi ja tiedotus, projektikansio

## 2.6. Projektin päättyminen

>luovutus, käyttöönotto, ylläpito, projektin aineiston taltiointi, arkistointi, loppuraportti, projektin virallinen päättäminen

## 3. Projektin ajalliset tavoitteet	

## 3.1 Osittaminen ja vaiheistus

>Projektin etenemistä voidaan kuvata ns. GANTT-kaaviolla. Sen avulla voidaan esittää eri vaiheiden eteneminen aikajanalla, samalla voidaan osoittaa projektin eri vaiheisiin liittyvät kriittiset pisteet / etapit. Ohjelmistoprojekteissa karkea etenemisjärjestystä voi kuvata ohjelmistojen [SDLC](https://en.wikipedia.org/wiki/Systems_development_life_cycle )-mallilla.
Tästä voidaan nostaa esiin muutama oleellisia vaiheita kuten:

* Määrittely
* Suunnittelu
* Toteutus
* Testaus
* Luovutus

![](../assets/work-to-do.png)

**Esitetään vaiheet yksinkertaisen GANTT diagrammin avulla**

```plantuml
Project starts the 2022-9-10
[Projekti aktiivinen] Starts 2022-9-12 and ends 2022-12-1
[Määrittely vaihe] Starts 2022-9-12 and ends 2022-9-18
[Suunittelu] Starts 2022-9-19 and ends 2022-10-2
[Toteutus+suunnittelu] Starts 2022-10-3 and ends 2022-11-3
[Testaus+korjaus] Starts 2022-11-4 and ends 2022-11-20
[Hyväksyntätestaus] Starts 2022-11-21 and ends 2022-11-26
[Luovutus] Starts 2022-11-27 and ends 2022-12-1
```

![](../assets/work-to-do.png)

Päivitä linkit omaan projektiin liittyviksi!

* [Etappi 0](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/2)
* [Etappi 1](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/3)
* [Etappi 2](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/4)
* [Etappi 3](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/5)
* [Etappi 4](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 5](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 6](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 7](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)

* [Etappi 8](https://gitlab.labranet.jamk.fi/fi-a2022-ttc2070/ht1-N5589-/core/-/milestones/11#tab-issues)
* [Etappi 9](https://gitlab.labranet.jamk.fi/fi-a2022-ttc2070/ht1-N5589-/core/-/milestones/12#tab-issues)
* [Etappi 10](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 11](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 12](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 13](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 14](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 15](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)
* [Etappi 16](https://gitlab.labranet.jamk.fi/jamkit/project-templates/opf-core-template-v2/-/milestones/6)


>Projektin osittamisella tarkoitetaan projektin jakamista selkeisiin osakokonaisuuksiin ja niitä vastaaviin toteutuskokonaisuuksiin (osaprojekteihin, vaiheisiin, tehtäväkokonaisuuksiin ja tehtäviin). >Tutkimus- ja kehitysprojektien etenemiselle on tyypillistä lopputuloksen muodostuminen ja tavoitteen tarkentuminen vaihe vaiheelta. Projektin osituksen tulee perustua tähän lähtökohtaan (koskee myös >IT-instituutin opiskelijaprojekteja). 
>Projektin elinkaari voidaan jakaa erityyppisiin vaiheisiin. Kussakin vaiheessa tuotetaan määrätyt tuotteet, kuten selvitys, suunnitelmat, prototyyppi, laite jne. Kunkin vaiheen loppuun sovitaan arviointi, hyväksyntä tai katselmointi. Ohjelmistoprojekti jakautuu tyypillisesti seitsemään vaiheeseen: perustaminen, esitutkimus, analyysi, suunnittelu, toteutus, testaus ja lopettaminen. Joskus esitutkimus on oma projektinsa, joskus analyysi sisällytetään suunnitteluun jne. Testaus ei välttämättä ole oma vaiheensa, vaan se sisältyy kaikkiin vaiheisiin. Usein edetään inkrementaalisesti eli ensin suunnitellaan ja toteutetaan yksi asia kokonaisuudessaan ennen kuin edetään seuraavaan asiakokonaisuuteen. Ei ole yhtä ainutta ”oikeaa” vaihejakoa, mutta jos toimeksiantajalla on oma menetelmänsä ja siihen liittyvät mallipohjat, niin opiskelijaprojekteissa käytetään ensisijaisesti niitä. Yhä useammin käytetään ketterää sovelluskehitystä eli ohjelmisto tehdään 1-4 viikon sprinteissä.

>Mitä tavoitteita  / vaiheita projekti sisältää? (Lyhyt kuvaus kustakin)> <Mitä tuloksia kustakin vaiheesta syntyy? >

Seuraavassa käydään jokainen vaihe, niiden vaatimat aikaresurssit ja tulokset läpi lyhyesti. Vaiheet ja niiden tehtävät kuvataan tarkemmin vaihesuunnitelmissa. Parhaillaan meneillään olevasta vaiheesta tulee olla tiedossa tarkasti kuka tekee ja kuinka paljon työtä tämän vaiheen tehtävien suorittamiseksi. Myöhempien vaiheiden työmääräarviot voidaan esittää alkuvaiheessa karkealla tasolla, jota sitten projektin edetessä tarkennetaan yksityiskohtaiselle tasolle. Tämä tapahtuu jokaisen vaiheen lopussa, jolloin suunnitellaan tarkemmin seuraava vaihe.

Huom.: Seuraavassa on esitetty käynnistys- ja lopetusvaiheet. Kaikista projektin vaiheista, niiden kestoista ja työmääristä laaditaan myös nk. Gantt-kaavio (liitteenä), jossa näkyy myös vaiheiden väliset riippuvuudet ja tärkeimmät etapit (esim. johtoryhmän kokouspäivämäärät).

>Projektin eteneminen kannataa jakaa ns. tavoitteisiin/etappeihin. Näiden tehtävän on osoittaa ajanhetkeä, jollon jokin oleellinen projektin vaihe on tarkoitus saavuttaa. Projektille määritellyt etapit voidaan linkittää dokumentaation kanssa yhteen käyttäen apuna Issue/Milestone linkkejä avulla. *Katso esimerkit alla*




* [Etappi 0](https://gitlab.labranet.jamk.fi/jamkit/project-templates/fi-opf-2021-core-template-v2/-/milestones/1)

>esim. ryhmän webbisivut, tutustutaan tarkemmin toimeksiantoon, aloitetaan kohdealueeseen perehtyminen ja laaditaan projektisuunnitelma yhteistyössä toimeksiantajan edustajien kanssa. 
>Projektin käynnistämiseen kuuluu olennaisesti projektisuunnittelu ja suunnitteludokumenttien laatiminen sekä yhteydenpitokäytänteiden luominen toimeksiantajayrityksen kanssa. Vaiheen aikana tehdään
>Etappiin mennessä muodostetaan johtoryhmä, pidetään johtoryhmän kokous sekä allekirjoitetaan projektisopimus.

* [Etappi Z](https://gitlab.labranet.jamk.fi/jamkit/project-templates/fi-opf-2021-core-template-v2/-/milestones/3)

>Esimerkkinä Etappi Z , jossa tavoitteet on asetettu ennakkon esimerkkeinä: projektisuunnitelman hyväksyminen, tavoitteiden tarkistaminen

* [Etappi X](https://gitlab.labranet.jamk.fi/jamkit/project-templates/fi-opf-2021-core-template-v2/-/milestones)

>Sovittu etappi X, jossa suoritettaa esimerkisi katselmointi ja esitetään tilanneraportti

* [Etappi Y](https://gitlab.labranet.jamk.fi/jamkit/project-templates/fi-opf-2021-core-template-v2/-/milestones)


* [Etappi Z](https://gitlab.labranet.jamk.fi/jamkit/project-templates/fi-opf-2021-core-template-v2/-/milestones)

>”Lopettamisvaihe sisältää projektin päättämiseen liittyvät toimenpiteet. Vaiheen aikana projektiryhmä laatii projektin loppuraportin ja esityksen johtoryhmälle. Vaiheen aikana luovutetaan projektin tulos toimeksiantajalle, pidetään viimeinen johtoryhmän kokous viikolla X sekä puretaan projektin organisaatio. Lopettamisvaiheen tuloksena on projektin loppuraportti.”

## 3.2 Projektin alustavat kustannusarvio

![](../assets/work-to-do.png)

Kustannusarvion esittäminen taulukon avulla: 

![](kustannusarvio.jpg)

## 4. Laadunvarmistus

>Projektissa sovellettavat työmenetelmät, välineet, ohjeet ja standardit

>Tässä kappaleessa luetellaan kaikki käytettävät menetelmät, työkalut ja standardit versionumeroineen. Usein toimeksiantajalla on jokin menetelmä, jota projektiryhmän olisi syytä noudattaa. Toimeksiantaja voi määrittää myös noudatettavat dokumenttien ulkoasustandardit. Muussa tapauksessa projektiryhmä räätälöi IT-instituutin tarjoamista mallipohjista itselleen soveltuvan ja toimeksiantajan hyväksymän mallin.

>Opintojakso asettaa siis tietyt vaatimukset projektin seurantatyökaluille ja raportoinnille, jotka tulee ottaa huomioon. Opintojaksolla ei kuitenkaan pakoteta tiettyä tapaa käyttää työkaluja, joten niiden käytöstä on syytä tehdä suunnitelma tähän kohtaan.

>Projektin tiedon- ja versionhallinnan perusteet tulee selvittää, jotta kaikki projektin sidosryhmät tietävät dokumenttien uusimpien versioiden sijainnin. Projektisuunnitelmasta ja kaikista muistakin projektin keskeisistä dokumenteista tulee useita versioita, joihin pitää lisätä versiohistoria, jotta projektin kehityksen seuraaminen jälkikäteen on mahdollista. Mikäli jokin yksittäinen laite tai ohjelmisto nousee projektin toteutuksen kannalta kriittiseen asemaan, on tälle hyvä nimetä vastuuhenkilö, joka tuntee ko. laitteen tai ohjelmiston ryhmästä parhaiten. Ohessa on lista asioista, jotka kannattaa suunnitella ja dokumentoida: 

## 4.1 Väli- ja lopputulosten hyväksymismenettely

>Tähän kirjataan se hyväksymismenettely, mikä projektissa on sovittu.

## 4.2 Muutosten hallinta

>Kuvataan muutosten hallintaproseduuri projektinkäytäntöihin tai projektin tuloksiin liittyvien muutosten osalta.

## 4.3 Dokumentointi

>Kirjataan minne dokumentit tallennetaan/arkistoidaan, miten ne jaetaan ja kuka on vastuussa eri dokumenteista.

## 4.4 Riskien hallinta

>Listataan riskit, arvioidaan niiden vakavuus ja todennäköisyys ja koetetaan miettiä toimenpiteet kuinka vakavimmat/todennäköisimmät riskit voitaisiin ehkäistä jo ennalta. Lisäksi olisi hyvä olla suunnitelma kuinka toimitaan, jos riski toteutuu.
>Kirjataan alla olevaan taulukkoon projektiin kohdistuvat riskit ja pidetään niitä yllä tarpeen mukaan. Jokaiselle riskille annetaan yksilöllinen tunniste esim. RIS007, koska tämä helpottaa niiden käsittelyä eri tilanteissa.

Liitä seuraava osio tähän mukaan: [Riskienhallintataulukko](riskitaulukko.md)

## 4.5 Katselmointikäytäntö

>Luetellaan ja alustavasti aikataulutetaan projektin tuloskatselmukset laaditun toteutussuunnitelman pohjalta. Esitetään luettelomaisesti, mitä katselmuksia pidetään, alustava ajankohta, käsiteltävät asiat, osallistujat sekä käytännöt katselmointimateriaalin toimittamisesta (mitä, milloin, miten).

## 4.6 Projektisuunnitelmaa täydentävät suunnitelmat

>Tässä kohdassa mainitaan, mitä täydentäviä suunnitelmia on käytettävissä tai aiotaan projektin kuluessa laatia (esim. viestintä-, riskienhallinta-, testaus- ja käyttöönottosuunnitelma).

* [Projektisopimus](..//10-Projektinhallinta/projektisuunnitelma.md)
* [Vaatimusmäärittely](../20-Vaatimustenhallinta/vaatimusmaarittely.md)
* [Julkaisusuunnitelma](../40-Julkaisusuunnittelu/julkaisusuunnitelma.md)
* [Yleistestisuunnitelma](../40-Julkaisusuunnittelu/julkaisusuunnitelma.md)
* [Viestintäsuunnitelma](..//10-Projektinhallinta/viestintasuunnitelma.md)
* [Riskihallintasuunnitelma](../10-Projektinhallinta/riskihallinta-suunnitelma.md)
* [Muu annettu dokumentaatio]()


## 4.7 Suunnitelmien tarkistus- ja päivitysajankohdat 

>Projektisuunnitelman avulla reagoidaan poikkeamiin ja ympäristömuutoksiin, joten sitä päivitetään projektin aikana. Tähän kohtaan kirjataan ne ajankohdat, jolloin suunnitelman ajantasaisuus ainakin on tarkistettava.

## 4.8 Projektin keskeyttämiskriteerit

Oikeaoppiseen projektisuunnitelmaan kuuluu myös projektin keskeyttämiskriteerit. Näitä ei kuitenkaan opiskelijaprojekteissa käytetä, koska projekteissa käytetään tietty tuntimäärä tuloksen tekoon ja tulos luovutetaan sellaisena, kun se opintojakson päättyessä on. Projektiryhmä tekee kuitenkin jatkokehityssuunnitelman, josta mahdollinen uusi projekti jatkaa.

## 5. Tiedonvälitys ja projektin etenemisen seuranta (viestintäsuunnitelma)

## 5.1 Viestintäsuunnitelma

>Viestintäsuunnitelman tarkoituksena on määritellä X projektin yhteydessä käytetyt viestintämenetelmät ja kanavat. Selkeällä ja yhdenmukaisella viestinnällä varmistetaan >informaation kulku ja vaikutetaan projektin laatutavoitteiden toteutumiseen. Suunnitelma voidaan laatia osana projektisuunnitelmaa tai siihen voidaan viitata omana [alasivunaan](../10-Projektihallinta/viestintasuunnitelma.md)

>Listaa projektissa sovitut työtilat ja viestintävälineet, palaverikäytäntö ja yhteydenpito, raportointi ja tiedotus.

## 6. Projektin päättyminen

## 6.1 Lopputuotteen luovutus, käyttöönotto

>Projektin lopputuote tulee myös dokumentoida järkevällä tasolla. Osana lopputuotetta saattaa olla asiakkaalle tarjottavaa käyttöönottokoulutusta ja mahdollisesti asennus- tai käyttöönotto­palvelua. Mikäli koulutuksen rooli projektin kannalta on huomattava (esimerkiksi ohjelmiston käyttäjät eivät ole olleet mukana projektissa ja eivät tiedä miten järjestelmä toimii) tulee projektisuunnitelmaan liittää suunnitelma asiakkaalle tarjottavasta koulutuksesta. Lisäksi jos on tarpeen, tulee projektisuunnitelmaan liittää myös asennussuunnitelma ja käyttöönottosuunnitelma.

## 6.2 Projektin tuottaman aineiston taltiointi, arkistointi ja säilytysaika

>”Projektiryhmien dokumentaatiosta jäävä osa tallennetaan X-järjestelmään” 
>Toimeksiantajan kanssa tulee tarvittaessa voida sopia, mitkä dokumentit voidaan jättää opiksi seuraaville projekteille. 
>Tyypillisesti eri suunnitelmat ja loppuraportti sopivin osin ovat tällaisia dokumentteja. 

## 6.3 Projektin virallinen päättäminen

>On tärkeää määritellä milloin, mihin tai miten projekti päättyy. Projektin päätös voi olla tietty päivämäärä, tietty tuotteen valmiusaste, tietty työtuntimäärä, tietty kulutettu rahasumma, kun asiakas ottaa tuotteen käyttöön, takuuaika on umpeutunut tai kun asiakas hyväksyy tuotteen.

>”Projekti päättyy p.k.vvvv, jolloin projektisopimuksen voimassaoloaika päättyy.”

## 6.4 Lopetustilaisuus

>Yleensä projektit päätetään yhteiseen päätösseminaariin. Tähän kirjataan osallistujat ja ajankohta. 

* Saunailta :)?


## 6.5 Projektin loppuraportti

>Projektin loppuraportti laaditaan viimeiseen johtoryhmän kokoukseen mennessä.

