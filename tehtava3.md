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
	**micro uusitiedosto.md**
Jonka jälkeen lisään sen repositoryyn kaikille komenoilla **git pull** , **git add uusitiedosto.md** , **git commit** ja **git push**. Nyt kaikki muutokset näkyvät githubissa:

![Image](https://imgur.com/DKbO0Bp.png)

## c) Kaikki kirjataan. Näytä omalla git-varastollasi esimerkit komennoista 'git log','git diff' ja 'git blame'. Selitä tulokset

Git log näyttää kaikki gitissä suoritetut commitit ja niiden kommentit

![Image](https://imgur.com/8tO3Cjp.png) 

git diff näyttää erot githubin ja oman gitin välillä ennen committaamista

![Image](https://imgur.com/zs7t69s.png)

git blame:illä voidaan katsoa, kuka on muokannut viimeksi vaikka jotain tiedostoa, ja milloin. Esimerkiksi tässä edellisessä tehtävässäni luoma uusitiedosto.md blame näyttää minut ja ajan jolloin viimeksi olen sitä muokannut:

![image](https://imgur.com/cG37U5j.png)  

## d) Huppis! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset 'git reset --hard'. Huomaa, että tässä toiminossa ei ole peruutusnappia. 

Tee kuvitteelisen tyhmän muutoksen gittiin, jossa lisään uusitiedosto.md:seen jotakin esimerkiksi ohjelman salaisuuksia joita ei tulisi olla julkisessa repositoryssa.

![Image](https://i.imgur.com/mSgKuSG.png)

Sen jälkeen lisään sen gittiin, mutta en aja committia vaan teen komennon **git reset --hard**

![Image](https://i.imgur.com/tf1axg4.png)

Nyt gitti on palauttanut itsensä jälkimmäiseen commit versioonsa, ja uusitiedostosta on poistunut tekemäni virheet

![Image](https://i.imgur.com/SzyfCt7.png)

## e) Tee uusi salt-tila (formula,moduli,infraa koodina)(eli uusi tiedosto esim. srv/salt/terontila/init.sls)Voit tehdä yksinkertaisen parin funktion (pkg,file..)tilan, tai edistyneemmin asentaa ja konfiguroida minkä vaan uuden ohjelman: demonin, työpöytäohjelman tai komentokehotteesta toimivan ohjelman. 

Aloitan salt-tilan luomisen tekemällä /srv/salt/kimintila/ kansion komenolla **sudo mkdir -p /srv/salt/kimintila**. Sen jälkeen luon sinne init.sls tiedoston komenolla **sudoedit /srv/salt/kimintila/init.sls** Teen salt- tilan joka lisää käyttäjän Lehtonen, sekä luo tekstitiedoston "heikimi" tmp kansioon.

![Image](https://i.imgur.com/C6l4rjP.png)

Testaan vielä että se toimii ajamalla komennon
	sudo salt '*' state.apply kimintila

![Image](https://imgur.com/wMWRAIF.png)

Saltti onnistui tekemään muutokset.  

