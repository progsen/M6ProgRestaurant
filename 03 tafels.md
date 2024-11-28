## opdracht

We gaan nu een tafel reserverings systeem maken

- zet al je werk uit de M6ProgProject over naar de M6ProgEindOpdracht docker


- rol je sql files uit:
    - createdb.sql
    - data.sql
    
## tafel tabel
- breidt je ERD uit met:

    - tafel
        - idtafel
        - tafelnummer
        - maxPersonen

    - reservering
        - reserverinUUID (PRIMARY KEY,varchar(45), UNIEK)
            > dus geen ID nodig voor deze tabel
        - datum
        - tafelnummer
        - reserveringstijd
        - aantal personen
        - opNaam

- laat de SQL genereren, sla die op in reserveren.sql

## paginas maken

- maak de volgende paginas aan:
    - reserveren.php

## reserveren.php

- zet hier een datum input neer (zie html inputs)
- zet hier een dropdown input neer met tijden:
    - 11:00
    - 12:00
    - 13:00

    - 16:00
    - 17:00
    - 18:00
    - 19:00
    - 20:00

- aantal personen input
- voeg een tekst input toe
- voeg een submit knop toe

## functionaliteit:

- een gebruiker moet:
    - een datum tijd kunnen selecteren 
    - een naam kunnen invoeren
- als de gebruiker op submit clickt:
    - checked reserveren.php (als het een POST is):
        - is er een tafel vrij om die tijd (met gereserveerdDoor op NULL)
            - VRIJ: insert een nieuwe reservering
            - NIET: toon een foutboodschap, en de reservering pagina, met de data zoals die al was ingevuld
>HINTS:
```
Het vrije tafel probleem is een probleem wat goed op te lossen is in:
- OF een storedprocedure (snelst), 
    - je hebt een where IN () nodig
- OF via code (langzamer)


```

## reservering aanpassen

- als je op de reservering link clickt:
    - kom je op reserveren.php
    - wordt je reservering in de database gezocht
        - en wordt deze in de input velden neergezet
    - komt er een edit en annuleren knop

- druk je op annuleren:
    - dan wordt je reservering gedelete uit de database


- druk je op edit:
    - dan wordt je reservering geupdate:
        - met nieuwe datum/tijd etc,
        - ALS DAT KAN!

## extra beter

- als je bij reserveren komt, laat alleen de tijden zien van die dag die nog vrij zijn! 


## Klaar?
- commit naar je github