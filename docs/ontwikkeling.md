---
layout: page-with-side-nav
title: Projectinformatie
date: 24-07-2024
---

# Ontwikkeling

Informatie over het Klantinteracties-ontwikkelproject.

## Ontwikkeling gestopt

De op deze website gepubliceerde klantinteractiesmaterialen werden ontwikkeld als onderdeel van een onderzoekstraject naar nieuwe patronen voor API-specificaties. Het was de bedoeling dit traject af te ronden met een praktijkbeproeving van deze patronen aan de hand van de klantinteracties-casus. Daaruit zou later eventueel een gemeentelijke standaard kunnen ontstaan. Uiteindelijk bleek het voor zo'n toets in praktijkomstandigheden te vroeg.

Op dit moment (juli 2024) hebben andere vraagstukken prioriteit, waardoor er niet aan klantinteracties gewerkt kan worden. Het hier en in de [GitHub-repository](https://github.com/VNG-Realisatie/klantinteracties/) gepubliceerde materiaal geldt derhalve als halfproduct, dat 'as is, where is' onder de voorwaarden van de [EUPL](https://eupl.eu/1.2/nl/) te gebruiken is.

## Ontwikkelupdate 20 april 2023

Benieuwd naar de stand van zaken? Bekijk [deel 1](./assets/project/20230420-toelichting-inzichten-klantinteracties-deel-1.pdf) en [deel 2](./assets/project/20230420-toelichting-inzichten-klantinteracties-deel-2.pdf) van de tijdens de laatste ontwikkelbijeenkomst op donderdag 20 april getoonde presentatie.

## Online toelichting Klantinteracties 23 juni 2022

Op 23 juni 2022 is tijdens de 'Week van de dienstverlening' een korte toelichting gegeven bij de ontwikkelingen rondom de API-standaarden voor Klantinteracties.

### Presentatie

De tijdens de bijeenkomst getoonde [Powerpointpresentatie](./assets/project/20220623-presentatie-klantinteracties.pptx).

### Video-opname

De video-opname is niet publiek toegankelijk gepubliceerd, maar na inloggen beschikbaar via de [Pleio-omgeving bij de 'Week van de dienstverlening'](https://weekvandedienstverlening.pleio.nl/events/view/7bcb43f5-5773-4d9a-b98d-aa1fa413a37c/api-standaarden-voor-klantinteracties-wat-en-waarom-ook-alweer-en-wat-gaat-er-gebeuren).

### Q & A

_Onderstaande vragen en vervolgvragen (**in vet**) zijn tijdens de bijeenkomst in de chat gesteld en achteraf (*in cursief*) beantwoord._

* **Qua definitie van klant: kan het niet ook een vestiging van een organisatie zijn?**<br/><br/>
*Jazeker, maar een vestiging is wat mij betreft een onderdeel van een organisatie of een kenmerk van een persoon (in geval die namens zijn eenmanszaak handelt).*

* **Zijn meerdere mail-adressen mogelijk ? En zijn ook Social Media (Twitter/Facebook-accounts) mogelijk?**<br/><br/>
*Zoals toegelicht zijn klantgegevens bedoeld als ‘default’ contactgegevens voor die klant. Voor gebruik tijdens specifieke interacties (een aanvraag bijvoorbeeld) kunnen afwijkende contactgegevens worden opgegeven. Deze gelden als kenmerk van die interactie, en niet als kenmerk van de klant. Als we dit patroon volgen is het vast kunnen leggen van één e-mailadres bij de klant volgens mij voldoende.*<br/>
*Voor het vastleggen van gebruikersnamen op sociale media van klanten zijn nog geen user stories ingediend. Als dat gewenst is, graag zo’n user story via https://github.com/VNG-Realisatie/klantinteracties/issues/new/choose :).*

* **Hoe vrij is de api in het zelf opnemen van elementen? welke vrijheid heeft de gemeente zelf?**<br/><br/>
*De Klanten API omvat gegevens die (zoveel mogelijk) door de klant zelf (kunnen) worden verstrekt. De standaard is dus niet bedoeld voor het bijhouden van kenmerken of eigenschappen van de klant door de gemeente.*<br/><br/>
[reactie bij opmerking hierboven]<br/>**Om een standaard goed te kunnen laten werken is het juist niet de bedoelding om als gemeente eigen elementen toe te voegen. Dat wil niet zeggen dat een gemeente geen goede bijdragen kan hebben maar die zouden we dan graag in de standaard opnemen zodat andere gemeenten hier ook van kunnen profiteren.**<br/><br/>
*Mee eens :)*<br/><br/>
[reactie bij twee opmerkingen hierboven over ‘vrije kenmerken’]<br/>**M.i. nog wel punt van overdenking want binnen verschillende domeinen zijn denk ik verschillende behoeften wat betreft 'klant+ gegevens'.**<br/><br/>
*Dat denk ik ook. Daarom beperken we ons binnen de Klanten API-standaard tot contactgegevens en -voorkeuren. De behoeften daaromtrent zijn (naar mijn inschatting) domeinonafhankelijk.*

* **Ik denk dat het handig zou zijn om adres als lijsten te kunnen opgeven met een type aanduiding. Idem voor contactgegevens zoals e-mail, telefoonnummer, social media accounts, …**<br/><br/>
*Voor adressen, social media-accounts en telefoonnummers lijkt me dit ook handig. Ik kan me bijvoorbeeld voorstellen dat het zinvol is om bijvoorbeeld een mobiel en een vast telefoonnummer vast te leggen. Voor e-mailadressen zie ik de noodzaak daarvoor niet meteen – ik kan zo snel ook geen voorbeelden bedenken van andere organisaties waar ik meerdere e-mailadressen kan opgeven om die in verschillende situaties te gebruiken. Een eventueel voorbeeld is welkom als user story :).*<br/><br/>
[reactie bij opmerking hierboven]<br/>**Je ziet ook vaak telefoon werk of telefoon privé.**<br/><br/>
*Mee eens. Belangrijk hierbij op te merken is dat we een persoon die handelt namens zichzelf zien als een andere klant dan dezelfde persoon die handelt namens een organisatie – bijvoorbeeld omdat zij of hij daar werkt. Omdat ‘zakelijke’ nummers vaak ook privé worden gebruikt lijkt me het overigens alsnog nuttig om het mogelijk te maken zakelijke telefoonnummers vast te leggen. Teruggrijpend op de vraag hierboven zie ik dat nut voor e-mailadressen minder.*

* **In een DSO-verzoek kan de indiener ook afwijkende persoonsgegevens en correspondentiegegevens indienen. Hoe verhoudt dat zich tot de klanten-api?**<br/><br/>
*Deze vraag is tijdens de bijeenkomst beantwoord en wordt in de video beantwoord vanaf minuut 16:00.*

* **De vraag is denk ik of het van belang is om In de klantregistratie vast te kunnen leggen dat een klant gemachtigde is namens iemand anders.**<br/><br/>
*De Klanten API omvat gegevens die (zoveel mogelijk) door de klant zelf (kunnen) worden verstrekt. Machtigingsgegevens voldoen niet aan dat criterium. Bovendien ‘hangt’ zo’n machtiging aan een basisregistratiesubject, en zou die ook daar in de buurt moeten worden vastgelegd. Ten slotte loopt er een groot project rondom machtigen bij het ministerie van Binnenlandse Zaken en zou ik een oplossing voor dit – landelijke en niet gemeentelijke – probleem het liefst ook op dat niveau zien.*<br/><br/>
[als vervolg op de vorige opmerking]<br/>**M.i. is dit context-gerelateerd dwz niet voor een generieke klantenregistratie.**<br/><br/>
*Mee eens dus :)*

* &quot;**Iedereen die contact heeft/kan-hebben met de gemeente**&quot; **is m.i. ruimer dan wat meestal met 'klant' wordt aangeduid. Bijv. wikipedia:** "**Een klant is de afnemer van een goed of dienst van een leverancier.**" **Terminologie nog punt van aandacht dus...**<br/><br/> 
*De gekozen definitie wijkt inderdaad wat af van hetgeen gebruikelijk is, daarom is die ook zo belangrijk. Eerder hebben we voorgesteld dat ‘klant’ ‘betrokkene’ bij ‘zaak’ vervangt in alle gevallen waar zo’n betrokkene niet voor de gemeente werkt. Dit betekent dat ook een persoon die niet de aanvraag heeft ingediend die heeft geleid tot een zaak, maar daarbij wel betrokken is (bijvoorbeeld omdat de zaak een bezwaar tegen een aan haar of hem verleende vergunning betreft), wordt opgevoerd als ‘klant’. Dit maakt de brede definitie noodzakelijk.*

* **Is in de tweede situatie [waarbij voor een klant geen identificerende gegevens worden vastgelegd] wel sprake van een klant, of alleen van NAW-gegevens bij het formulier van degene die dat formulier heeft ingediend?**<br/><br/>
*Interessante vraag. Stel iemand doet een melding en wil op de hoogte gehouden worden van de behandeling daarvan. Die melding wordt geregistreerd als productaanvraag. Je kan in dit geval inderdaad twee routes kiezen:*<br/><br/>1. *Contactgegevens worden vastgelegd bij de klant, de contactgegevens bij de productaanvraag waarin die melding is geregistreerd blijft leeg.*<br/>2. *Er ontstaat geen klant, de contactgegevens worden in de contactgegevens bij de bij de productaanvraag waarin die melding is geregistreerd.*<br/><br/>*Het tweede is conceptueel zuiverder: het gaat hier immers om contactgegevens die alleen voor de duur van de interactie (kunnen) worden gebruikt: precies waar de contactgegevens bij de aanvraag voor bedoeld zijn. Aan de andere kant kan ik me ook voorstellen dat deze route vraagt om het kunnen vastleggen van meer contactgegevens bij de productaanvraag.*<br/><br/>*Een andere consequentie van de tweede optie is dat het niet langer logisch lijkt de relatie tussen een zaak en iemand die bij die zaak betrokken is, maar niet aanleiding heeft gegeven tot het starten daarvan als klant te registreren. Diens contactgegevens zou je dan immers eerder op de relatie persoon – zaak verwachten.*<br/><br/>*Het lijkt me noodzakelijk om dit in een aantal casussen verder uit te werken.*

* **Patroon is dus: Klant ophalen (bsn) -> bestaat niet? aanmaken; bestaat wel aanvullen/gegevens ophalen.**<br/><br/>
*Klopt.*

* **De situatie van meerdere klanten wil je in een CRM systeem helemaal vermijden! Zo niet kan je geen "totaal" klantbeeld maken.**<br/><br/>
*Helemaal mee eens. Dubbele ‘geïdentificeerde’ klanten zijn inderdaad ongewenst (en komen als het goed is ook niet voor). Maar als je een klant niet identificeert, kan je niet weten of er sprake is van een dubbele klant, of iemand die je nog helemaal niet kent. Vergelijk het met het als ‘gast’ afrekenen bij een webwinkel waar je ook een account hebt. De winkel kan op basis van naam en adres wel aannemen dat de bestelling is gedaan door iemand met dezelfde naam en adres in een account, maar niet met voldoende zekerheid om die bestelling ook daadwerkelijk aan dat account te kunnen koppelen.*<br/><br/>
[reactie bij opmerking hierboven]<br/>**Dat lukt je niet als de klant zich niet identificeert (denk aan het inloggen op een site waar je iets wil bestellen).**<br/><br/>
*Precies.*

* **Het email-adres is ook context-afhankelijk, naast wellicht een defauilt-mailadres.**<br/><br/>
*Klopt. Dat zou je ook moeten kunnen ‘overrulen’ voor gebruik tijdens een specifieke interactie.*

* **Mag een zaakafhandelcomponent dan een 'niet herbruikbaar' klant record aanmaken om de contact gegevens in de context van een zaak in te kunnen opslaan?**<br/><br/>
*Ja, dat zou die component volgens het voorstel hierboven mogen doen. Maar wellicht moeten we daar naar aanleiding van de twee hierboven beschreven routes nog eens naar kijken.*

* **Als de klant zich voor één product zeg Vergunning identificeert en bij een melding openbare ruimte NIET. Wat ziet hij dan terug in zijn mijn-omgeving ? Alleen de vergunning, of ook de Melding Openbare ruimte ?**<br/><br/>
*Deze vraag is tijdens de bijeenkomst beantwoord en wordt in de video beantwoord vanaf minuut 31:45.*<br/><br/>
[reactie bij opmerking hierboven]<br/>**lijkt mij alleen die hij met identificatie heeft gedaan. Die andere  kan niet :)**<br/><br/>
*Klopt!*

* **Waar blijft het e-mailadres in ZGW API als het e-maildres specifiek is voor de zaak?**<br/><br/>
*Dat zou moeten worden als kenmerk van (en bij) de zaak.*<br/><br/>
[reactie bij opmerking hierboven]<br/>**vermoed dat je dat vastlegt op de relatie tussen Klant en Zaak als zijnde zaakspecifiek voorkeurskanaal**<br/><br/>
*Voorkeurskanaal zou ik contactgegevens noemen :) – maar klopt!*

* **DigiD is geen must voor identificatie. Er zijn ook andere mogelijkheden van identificatie: denk aan telefoonnummer, social media ids, ...**<br/><br/>
*Telefoonnummers en social media-id’s zijn veelal bij meerdere mensen bekend, en op zichzelf geen goede middelen om iemands identiteit vast te stellen en tegen te authentiseren. Tegelijkertijd is vragen in te loggen via DigiD of met een identiteitsbewijs fysiek langs te komen niet altijd haalbaar of gewenst. Waar nu precies de grens ligt tussen bescherming tegen mogelijke ongeoorloofd(e) handelen of gegevensverstrekking en het zo laagdrempelig mogelijk aanbieden van producten en diensten is een heel interessant vraagstuk dat ook buiten de toepassing van de Klanten API relevant is en nader onderzoek verdient.*<br/><br/>
[reactie bij opmerking hierboven]<br/>**Als je deze kan koppelen aan de klant, kan je altijd een klantbeeld opbouwen. Natuurlijk rekening houdend met AVG en wetgeving**<br/><br/>
*Koppelen aan een (bestaande, geïdentificeerde) klant moet zeker kunnen, maar die klantgegevens verstrekken van persoonlijke informatie op basis van (alleen) het noemen van een telefoonnummer of social media-id lijkt me niet haalbaar en gewenst.*

* **Ik ben bang dat we niet gaan toekomen aan wat mijn belangrijkste vraag voor deze sessie was:**<br/>
**Komen er ook documentrelaties? Opdat vastgelegd kan worden welke documenten in welke contactmoment zijn ingediend of verzonden**<br/><br/>
*Daar is een (nu gesloten) user story voor: https://github.com/VNG-Realisatie/klantinteracties/issues/138. Functionaliteit lijkt bij nader inzien praktisch. Aanvullingen met argumentatie daarvoor zijn welkom.*

* **Onderscheid van productaanvragen API t.o.v. ZGW API's mag wat mij betreft duidelijker. Ik zie niet heel snel de toegevoegde waarde. Maar dat kan ook aan mij liggen.**<br/><br/>
*Ligt niet aan jou. We moeten dit beter beschrijven. Staat op de planning, maar we nemen eerst de vragen rondom klanten op.*<br/><br/>
[reactie bij opmerking hierboven]<br/>**Productaanvraag is in terminologie van de klant. Zaak is ambtelijke term van de gegevensverzameling en procesafhandeling voor het leveren van het formele product. Kan 1:1 of 1:N of N:N zijn**<br/><br/>
*Precies, dat is een heel mooi begin van het antwoord :)*

* **Betreft naamgeving 'productaanvraag': blijf ik een lastige vinden. Persoonlijk vind ik een klantvraag of een verzoek meer passend. Een verzoek is iets wat de klant vraagt aan de gemeente, bv. wat zijn de openingstijden (informatieverzoek), maar ook een productverzoek(aanvraag)**<br/><br/>
**Vanuit sociaal domein is het een hulpvraag, waarbij pas bij het ondersteuningsplan en inzetten van instrumenten er sprake is van productaanvragen.**<br/><br/>
**Naamgeving hierin is dus erg lastig en wellicht zelfs domeinspecifiek.**<br/><br/>
*Goede suggesties. We gaan hier nog eens naar kijken.*

* **Naast productaanvragen ook ongevraagde (of uit initiatief gemeente) producten. bekendste de woz aanslag. in kader van integraal klantbeeld. hoe nemen we deze qua klantbeeld?**<br/><br/>
*Als zaak :). Maar vanuit het oogpunt van consistentie zou ik die zaak dan ophangen aan het product dat met die zaak wordt geleverd. Dan bied je de klant dus een overzicht van ‘aangevraagde’ en ‘niet-aangevraagde’ producten.*
