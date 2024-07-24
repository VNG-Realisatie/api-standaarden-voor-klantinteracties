---
layout: page-with-side-nav
title: Productvisie Klantinteracties
date: 24-07-2024
---

# Productvisie Klantinteracties

Onder de naam 'Klantinteracties' beschrijven we een te ontwikkelen product of producten waarmee een beperkte set gegevens die te maken hebben met contact tussen inwoners en ondernemers en de gemeente in API-specificaties wordt beschreven. Mogelijk leidt het resultaat van dit ontwikkeltraject uiteindelijk tot één of meerdere standaarden.

Hieronder wordt vanuit drie perspectieven beschreven waarom we aan Klantinteracties werken, voor wie we dat doen en welke aandachtspunten daarbij gelden:
1. Ontwikkelingen in het domein van interacties met klanten;
2. doelgroep van de specificatie en beoogd implementerende systemen;
3. bijdrage van het ontwikkelproces aan de API-referentiearchitectuur.

## Ontwikkelingen in het domein

Het woord klantinteractie valt uiteen in twee woorden: ‘klant’ en ‘interactie’. Samen beschrijven die heel precies met welk doel deze specificatie ontwikkeld wordt: het op uniforme wijze beschikbaar stellen van informatie over inwoners en ondernemers die contact hebben met de gemeente – of korter, haar ‘klanten’, en over hun interacties met de gemeente. Dit zodat gemeenten enerzijds via opgegeven (voorkeurs)kanalen met hun klanten contact kunnen opnemen, en anderzijds inzage geboden kan worden in (de inhoud van) eerdere interacties tussen klanten en de gemeente.

Een traject voor het specificeren van gegevens over contact tussen klant en gemeente komt niet uit de lucht vallen. Al bij het ontwikkelen van de API-standaarden voor Zaakgericht werken constateerden we dat gestandaardiseerde beschikbaarheid van deze gegevens niet afhankelijk zou moeten zijn van het antwoord op de vraag of die klant ‘toevallig’ betrokken is bij een lopende zaak. Ook de inhoud van een mail die over levering van een product dat niet zaakgericht wordt verstrekt, of de inhoud van gesprek dat niet het aanmaken van een zaak rechtvaardigt kan voor een klant immers heel relevant zijn.

Maar met alleen het ‘uit zaken lichten’ van gegevens die met klantinteracties te maken hebben, zijn we er niet. Met deze specificatie willen ook aansluiten bij veranderde verwachtingen van inwoners en ondernemers over overheidsdienstverlening en nieuwe, onder invloed daarvan bij gemeenten ontstane behoeften. Deze behoefteverandering is onder meer terug te zien in het ontstaan van nieuwe uitgangspunten voor (communicatie over) dienstverlening. Die ontstaan bijvoorbeeld naar aanleiding van diepgaand gebruikersonderzoek naar gemeentelijke inwonerportalen of maken een omnichannel-aanpak mogelijk.

Een goede verbinding met de hedendaagse gemeentelijke dienstverleningspraktijk proberen we op twee manieren te waarborgen:
1. We werken bij de ontwikkeling nauw samen met gemeenten en hun leveranciers, valideren bij hen onze inzichten, en sluiten aan bij de ontwikkeling van [MijnZaken-services](https://vng.nl/artikelen/mijnzaken-service-track-trace-voor-de-overheidsdienstlevering);
2. we beproeven en illustreren de beoogde werking van de specificatie aan de hand van heel concrete en van gemeentelijke behoefte afgeleide casussen.

## Doelgroep en systemen

De voor de hand liggende doelgroep voor API-specificaties zijn mensen en organisaties die zo'n specificatie in IT-systemen moeten toepassen: ontwikkelaars, (informatie)architecten, domein- en productmanagers die werken voor gemeenten en hun leveranciers. Hen proberen we met de documentatie op deze pagina's bij implementatie zo goed mogelijk te ondersteunen. We ontwikkelen daartoe naast API-specificaties een informatiemodel en illustreren de werking van de specificatie in casussen en functionaliteit.

Contact tussen de gemeente en haar klanten vindt op allerlei plaatsen binnen de gemeentelijke organisatie plaats. Dit contact wordt door veel verschillende IT-systemen ondersteund. Zo overlapt het toepassingsgebied van Klantinteracties deels met toepassingsbied van gemeentelijke CRM- of KCC-ondersteunende systemen. Belangrijk te benadrukken is dat dat deze specificatie niet beoogt de functionaliteit die deze systemen doorgaans leveren volledig af te dekken. We maken met andere woorden geen CRM- of KCC-specificatie. Onderdelen als kennisbanken, dashboards of andere rapportagetooling zijn voor de werking en waarde van deze systemen zeer belangrijk, maar vallen buiten de beoogde doelen – en dus het bereik – van Klantinteracties. Behalve deze ‘frontoffice’-systemen ligt implementatie ook voor de hand in taakspecifieke en generieke afhandelsystemen die het leveren van producten en diensten aan klanten ondersteunen. Ook voor deze systemen geldt uiteraard dat Klantinteracties slechts een klein deel bestrijkt van de totale functionaliteit die deze systemen leveren.

Inwoners en ondernemers moeten van deze specificatie uiteindelijk de vruchten plukken. Zij krijgen, doordat hun gemeente deze specificatie toepast, via meer kanalen toegang tot een completere set informatie over interacties met de gemeente. Ook medewerkers van gemeentelijke klantcontactcentra zijn belangrijke belanghebbenden. Dankzij Klantinteracties-specificatie krijgen zij toegang tot een completer, actueler klantbeeld. Hierdoor kunnen zij inwoners en ondernemers sneller, beter en vaker zonder ruggenspraak met vakafdelingen kunnen helpen. Medewerkers van deze afdelingen vormen een laatste groep die baat heeft bij een specificatie voor klantinteracties. Zij hoeven minder vragen zelf te beantwoorden omdat informatie over contact dat zij met klanten hebben (voor zover gewenst en toegestaan) eenvoudig door die klanten zelf of medewerkers van het klantcontactcentrum kan worden ingezien.

## API-referentiearchitectuur (ARA)

In de tweede helft van 2022 zijn we gestart met de ontwikkeling van een API-referentiearchitectuur (ARA). Deze is gericht op het ontwikkelen van bruikbare, doelmatige en goed op elkaar aansluitende API-standaarden. Een aantal vraagstukken die we hierbij tegenkwamen zijn tijdens vruchtbare werksessies met gemeenten en hun leveranciers diepgaand besproken. Het team dat ARA ontwikkelt werkt ook aan de Klantinteracties. Te ontwikkelen API-specificaties gelden daarmee als belangrijke 'testcase' voor inzichten die bij de ontwikkeling van ARA zijn opgedaan.

ARA-inzichten zijn reden om bij de ontwikkeling van Klantinteracties aan een drietal onderwerpen extra aandacht te besteden:
1. Weloverwogen kiezen van domeingrenzen, nadrukkelijke aandacht voor mogelijke (consistentie)problematiek bij het overschrijden daarvan en eventuele mitigerende maatregelen;
2. expliciet beschrijven van keuzes gemaakt ten aanzien van API-ontwerporiëntatie (gegevens- of handeling gedreven) en API-architectuur (REST ‘volgens het boekje’ versus een meer vrije interpretatie, of iets heel anders als GraphQL);
3. illustreren van implementatie van deze specificatie volgens verschillende patronen (gegevens in één centraal register, decentrale implementatie met façade-API, …).

Ontwerpbeslissingen waarvan de gevolgen raken aan generieke ontwerpuitgangspunten voor API-specificaties leggen we voor aan vertegenwoordigers van gemeenten en leveranciers in de ARA-klankbordgroep.