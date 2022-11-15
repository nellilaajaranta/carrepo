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
   
![kuva got log-komennon tuloksesta](https://github.com/nellilaajaranta/carrepo/blob/main/pictures/offline%20git.jpg)
  
 Kuvassa näkyy bit log-komennon tulokset.
 
 > c) Doh! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.

Seuraavaksi tein tyhmän muutoksen gitiin. Muokkasin readme-tiedostoon turhaa sekä lisäsin sen commitoitavaksi.

![kuva muutoksesta](https://github.com/nellilaajaranta/carrepo/blob/main/pictures/useless%20line.jpg)

![git status](https://github.com/nellilaajaranta/carrepo/blob/main/pictures/addeduseless.jpg)

Tämän turhan lisäyksen saa pois palaamalle aikaisempaan versioon. Tämä tapahtuu seuraavalla komennolla:

        git reset --hard
        
 Nyt readme-tiedosto on palautunut vanhaan versioon, jossa turhaa tekstiä ei enää ole.
    
 > d) Online. Tee uusi varasto GitHubiin (tai Gitlabiin tai mihin vain vastaavaan palveluun). Varaston nimessä ja lyhyessä kuvauksessa tulee olla sana "car" (auto). Aiemmin tehty varasto ei kelpaa. (Muista tehdä varastoon tiedostoja luomisvaiheessa, suosittelen tekemään README.md ja vapaista lisensseistä itse tykkään GPLv3 eli GNU General Public License, version 3)

Loin uuden GitHub-varaston nimeltä carrepo, jossa tämä tehtäväraporttikin sijaitsee. [Linkki](https://github.com/nellilaajaranta/carrepo)


