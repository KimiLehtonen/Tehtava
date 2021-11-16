# h3 Versionhallinta

Tein tehtävän windows 10 pöytäkoneellani, käyttäyen virtualboxissa debian 11 bullseyeta ja raportissa markdownia.

## z) Lue ja tiivistä artikkeli muutamalla ranskalaisella viivalla. Tässä z-alakohdassa ei tarvitse siis tehdä testejä tietokoneella.

 Commonmark contributors: Markdown Reference (huomaa ainakin otsikot risuaidoilla, kappalejako tyhjällä rivillä, sisennys (tab) koodia, lista, linkki, kuva.

- Markdown on simppeli tapa luoda tekstiä hyvän näköisessä muodossa. 
- hashtagillä otsikot, tyhjä rivi tekee kappalejaon, lista viivalla ja linkit suluissa

## a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti.

Loin ensikisi uuden repositoryn gittiin, jonka jälkeen loin sinne tämän .md päätteisen tiedoston jota teen nyt micro nimisellä ohjelmalla.

## b) Pull first. Tee useita muutoksia git-varastoosi. Tee muutama muutos, jossa yksi commmit koskee useamapaa tiedostoa. Anna hyvät kuvaukset (commit message), yksi enganninkielinen ause imperatiivisessa (määräysmuodossa)"add top level menu to Foobar synchronizer"

Ensimmäisenä muutoksena varastooni, on tämän tehtävän kirjoittaminen joka siis muokkaa git-varastoni tehtava3.md tiedostoa. Toisena muutoksena luon uuden Markdown tiedoston komenolla
	micro uusitiedosto.md
Jonka jälkeen lisään sen repositoryyn kaikille komenoilla **git add uusitiedosto.md** , **git commit** ja **git push**. Nyt muutokset näkyvät kaikille githubissa:

![Image](https://imgur.com/DKbO0Bp.png)

## c) Kaikki kirjataan. Näytä omalla git-varastollasi esimerkit komennoista 'git log','git diff' ja 'git blame'. Selitä tulokset

Git log näyttää kaikki gitissä suoritetut commitit ja niiden kommentit

![Image](https://imgur.com/8tO3Cjp.png) 

git diff näyttää erot githubin ja oman gitin välillä ennen committaamista

![Image](https://imgur.com/zs7t69s.png)

git blame:illä voidaan katsoa, kuka on muokannut viimeksi vaikka jotain tiedostoa, ja milloin. Esimerkiksi tässä edellisessä tehtävässäni luoma uusitiedosto.md blame näyttää minut ja ajan jolloin viimeksi olen sitä muokannut:

![image](https://imgur.com/cG37U5j.png)  

