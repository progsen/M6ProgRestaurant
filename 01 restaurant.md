## opdracht

wat we gaan maken is een restaurant website
op deze website kan je het dag menu zien voor lunch en dinner

elke dag veranderd het menu, dit wordt gekozen uit een standaard aanbod aan gerechten

iemand met de juiste login link kan het dagmenu aanpassen


## docker maken

- gebruik de lessen van m5prog om een docker te maken, let op:
    - zorg ervoor dat de docker M6ProgProject heet
    - de database m6prog heet
    - je de wachtwoorden aanpast
    - je het test

- zet in workbench een nieuwe connection naar deze docker

## Eind Opdracht docker maken:
- maak nu ook een andere docker aan M6ProgEindOpdracht
    - zorg ervoor dat de docker M6ProgEindOpdracht heet
    - de database m6prog heet
    - je de wachtwoorden aanpast
    - je het test

- zet in workbench een nieuwe connection naar deze docker

## tabellen maken

- maak een ERD:
    > vergeet niet al je tabellen een ID te geven met AI (auto increment)
    - drankje
        - heet ja nee
        - alcohol ja nee
        - naam
        - prijs
        - imagelink
    - gerechttype  (voor,hoofd,na)
        - naam
    - gerecht
        - gerechttype_id
        - naam
        - ingredienten lijst
        - prijs
        - imagelink
        
    - menu
        - dag
        - lunch ja/nee
        - voorgerechtid
        - hoofdgerechtid
        - nagerechtid
        - intro tekst

    - teksten
        - paginanaam
        - tekstnaam
        - tekst
## SQL bewaren

- doe een forward engereering en bewaard de SQL
    - noem deze file createdb.sql

## paginas maken

- maak de volgende paginas aan:
    - index.php
    - dagmenu.php
    - drankjes.php
    - menuinstellen.php
    - onderdelen/header.php
    - onderdelen/footer.php
## Navigatie

- elke pagina include de header en footer

## index.php

- hier staat een intro tekst
- contact gegevens (ficief adres)

## Dagmenu.php

- hier staat een korte uitleg tekst over dat dit restaurant een dagmenu heeft
- het lunch menu wordt getoond
- het dinner menu wordt getoond
- een link naar drankjes.php

> Het kan zijn dat je nu veel HTML gaat herhalen, maak functions met php om dat beter te doen
## Drankjes

- hier komen de drankjes te staan, verdeeld over de 3 catagorien

### TEKSTEN

- maak een data.sql file aan
- maak inserts voor de teksten tabel, gebruik de volgende gegevens voor teksten
HOME
- introtekst:
    > Welkom bij restaurant het goede menu, bij ons kunt u elke dag genieten van een speciaal samengesteld menu. Geniet van onze rustieke sfeer terwijl u een heerlijke lunch of dinner nuttigd
- contact:
    > Zomerzonlaan 6347
    > postcode 9876ZU
    > College van Media stad
    > Nederland

DAGMENU
- menuuitleg:
    > Geen keuze stress bij ons menu, u kunt hier zien wat het dagmenu is. speciaal uitgekozen voor maximaal genieten van de dag!. 

- drankjeslink:
    > click hier voor een overzicht de drankjes die wij in ons resaurant serveren 

## teksten uit db

- we hebben nu teksten in de DB
- zorg dat je die ook op de site gebruikt
    - kan je nog meer teksten in de database zetten?

## Klaar?
- commit naar je github