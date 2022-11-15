# tehtävänanto

Tämä tiedosto sisältää raporttini Tero Karvisen [Palvelinten hallinta](https://terokarvinen.com/2022/palvelinten-hallinta-2022p2/) -kurssin h3-tehtävään.

> a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita ‘#’ tekee otsikon, sisennys merkitsee koodinpätkän.

Tämä h3report.md -tiedosto on raporttini h3-tehtävänantoon, tehty Markdownilla.

> b) Offline. Tee paikallinen offline-varasto git:llä. Varaston nimessä tulee olla sana "cat" (kissa). Aiemmin tehty varasto ei siis kelpaa. Aseta itsellesi sähköpostiosoite ja nimi. Näytä varastollasi muutosten teko ja niiden katsominen lokista.

Tein uuden git-varaston nimeltä catrepo. Tähän käytin seuraavaa komentoa:

    git init catrepo
    
Uuteen varastoon asetan itselleni sähköpostiosoitteen ja nimen seuraavilla komennoilla:

    git config --global user.email "palvelinkurssi@gmail.com"

    git config --global user.name "Nelli Laajaranta"

komennon --global -osuus määrittelee jatkossa kyseiset käyttäjätiedot oletuksena jokaiselle projektille tällä käyttäjällä.
Laittamalla --global sijaan --local määrittelee käyttäjätiedot vain kyseiseen varastoon.

Loin varastoon nano-tekstieditorilla myös readme.md -tiedoston, johon tein muutoksia komennolla:

    nano README.md

tämän jälkeen muutokset lisätään gitiin komennolla:

    git add . && git commit

Seuraavaksi tarkistin muutokset git lokista:

    git log --patch
    
    git log -komennon tulokset:
    ![alt text](https://github.com/nellilaajaranta/carrepo/blob/main/pictures/offline%20git.jpg"offlinegit")
  
    
    
