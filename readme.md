# Discord boti loomine

| Sisukord | |
-----------|--------------
| [Koodi allalaadimine](#githubi-repo-allalaadimine) | Koodi alla laadimise jaoks ei ole vaja GitHubi kontot |
| [Discordi mooduli allalaadimine](#discordi-mooduli-alla-laadimine) | |
| [Discordi konto loomine](#discordi-konto-loomine-kui-sul-pole-veel-seda) | Kui sul on juba discordi konto, siis võid selle vahele jätta (peaasi et parooli tead või mingil muul moel saad sisse) |
| [Discordi serveri loomine](#discordi-serveri-loomine) | _<span style="color:red">Ilmselt pole vaja</span>_ |
| [Boti loomine](#Boti-loomine) |  
| [Boti kutsumine serverisse](#boti-kutsumine-serverisse) |
| [Boti jooksutamine (ellu äratamine)](#boti-ellu-äratamine-ehk-koodi-jooksutamine) |



## Githubi repo allalaadimine
Selleks, et kood alla laadida vajuta selle lehe ülaosas olevale rohelisele nupule "_Code_"
![Github koodi allalaadimine](images/1.png "Githubist koodi alla laadimine")  

Seejärel vali HTTPS ning kopeeri link.
![Githubi koodi allalaadimine](images/2.png "Githubist koodi allalaadimine")
Ava PyCharm.  
Kui PyCharm küsib litsentsi aktiveerimist, siis vali _License server_ ning aseta antud link serveri aadressi alla.
```
http://license1.intra.ttu.ee:1111
```
![PyCharmi aktiveerimine](images/3.png "Pycharmi aktiveerimine")

Kui see on tehtud, siis peaks avanema projekti avamise vaade  Sealt vali _Clone Repository_.
![PyCharmiga Repo Kloonimine](images/21.png "PyCharmiga Repo Kloonimine")

Peale seda aseta link, mille GitHubist kopeerisid ning vajuta _Clone_
![PyCharmiga Repo kloonimine link](images/22.png "PyCharmiga Repo kloonimine link")

PyCharm ilmselt küsib, kas usaldada antud projekti, vajuta _Trust Project_.
![PyCharmi projekti usaldamine](images/23.png "Pycharmi projekti usaldamine")

Kui kõik läks hästi, siis peaks kood olema alla laetud ning seda peaks olema näha (kõige laguses see avab muidugi selle õpetuse faili (`readme.md`), kuid vasakul paneelil saate failides ning kaustades sorada).
![PyCharmi projekti vaade](images/24.png "PyCharmi projekti vaade")

<details>
  <summary><b>Kui GITiga (lingiga ehk HTTPS) allalaadimine ebaõnnestub</b></summary>  

  Kui gitiga allalaadimine ebaõnnestus, siis võib ka ZIP failina koodi alla laadida. Selleks vali _Download ZIP_
  ![Githubi koodi allalaadimine](images/2.png "Githubist koodi allalaadimine")  
  Nüüd kui kood on alla laetud mine allalaetud failide kausta ning paki ZIP fail lahti (Parem klõps ja _extract all..._)
  ![ZIP faili lahti pakkimine](images/4_cropped.png "ZIP faili lahti pakkimine")  
  Nüüd kui see tehtud, siis ava PyCharm ning projektide alt vali _Open_
  ![Kausta avamine PyCharmis](images/28.png "Kausta avamine PyCharmis")
  Leia üles kaust, kuhe te failid ekstraktisite ning avage see.
  ![Kausta leidmine PyCharmis](images/29.png "Kausta leidmine PyCharmis")
  Jällegi, vajutage, et usaldate projekti.
  ![Projekti usaldamine PyCharmis](images/30.png "Projekti usaldamine PyCharmis")
</details>



## Discordi mooduli alla laadimine
Selleks et meie kood saaks discoridga suhelda on head arendajad loonud python'i jaoks mooduli, mille abil saab discordi boti programmeerida. Kuna antud moodul pole veel alla laetud, siis peate te seda ise tegema.
Selleks avage PyCharmis terminal (vasakus all servas).
![PyCharmis terminali avamine](images/25.png "PyCharmis terminali avamine")
Peale seda asetage järgnev rida terminali ning vajutage _Enter_.
```
pip install discord
```
![Pip-ga discordi mooduli alla laadimine](images/26.png "Pip-ga discordi mooduli alla laadimine")

Peale seda peaksid punased jooned _game.py_ faili ülaosast kaduma (kui ei kao, siis kutsuge juhendaja).



## Discordi konto loomine (kui sul pole veel seda)
Selleks, et boti luua, peab olema discordi konto, selle tegemiseks mine lehele [https://discord.com/register](https://discord.com/register).  
Konto kasutajanimeks võid kasutada ükskõik mida (ei pea olema sinu päris nimi).
![Discordi konto loomine](images/5.png "Discordi konto loomine")



## Discordi serveri loomine  
_<span style="color:red">Ilmselt ei lähe vaja ju?</span>_  

Selleks mine tagasi discordi ning vajuta suurt plussi vasakul servas.  
Peale seda vali, et teed serveri enda jaoks (_Create My Own_) ning see on ainult sulle endale ja sõpradele (_For me and my friends_).  
![Serveri valimine](images/10.png "Serveri valimine")
![Kes kasutavad serverit](images/11.png "Kes kasutavad serverit")

Vali serverile mingi nimi (võid ka pildi panna, aga see ei ole oluline)  
![Serverile nime lisamine](images/12.png "Serverile nime lisamine")

Nüüd on server valmis  
![Serveri vaade](images/13.png "Serveri vaade")



## Boti loomine
Mine lehele [https://discord.com/developers/applications](https://discord.com/developers/applications) ning loo uus rakendus (_New Application_).  
![Discordi rakenduse loomine](images/6.png "Discordi rakenudse loomine")
Anna enda botile mingi nimi.  
![Botile nime andmine](images/7.png "Botile nime andmine")

Selleks, et boti kasutada saaks, tuleb temale juurdepääs saada. Selleks on vaja boti tokenit. Seega mine "Bot"-i alla ning vajuta "Reset Token".
![Boti tokeni leidmine](images/8.png "Boti tokeni leidmine")  

Token-i resettimise käigus ilmselt küsib discord parooli, see on normaalne. Nüüd kopeeri token (see on see pikk numbrite, tähtede ning sümbolite jada).  
![Boti tokeni leidmine](images/9.png "Tokeni kopeerimine") 

Nüüd mine oma projekti alla ning aseta see token **KUSKILE**  
**<span style="color:cyan">Boti token:</span>** _MTMzMTkxNjMzMTk5NzcyNDY3Mg.GrqBgo.arZGbXr03qzGS_G9-oE7amyL7rUkSnc7cU4ODw_

Keri veel natuke allapoole ning lülita sisse _MESSAGE CONTENT INTENT_  
![Message contern intent sisse lülitamine](images/31.png "Message contern intent sisse lülitamine")  
Kindlasti salvesta ka muudatused.  
<details>

  <summary><b>Mis on intent?</b></summary>

  Intent on discordis eraldi viis kuidas botiga suhelda. Näiteks kui bot on kuskil kanalis, saab bot ainult sulle saata sõnumi, nii et teised seda sõnumit ei näe. Kuna uno mängus teised ei tohi su kaarte näha, siis on see väga hea viis enda kaartide nägemiseks.
  ![Discordi intent sõnum](images/32.png "Discordi intent sõnum")

</details>

Nüüd on bot valmis ning töökorras, kuid selleks et temast asja oleks, tuleb ta kutsuda serverisse.



## Boti kutsumine serverisse
Mine enda boti lehele [https://discord.com/developers/applications](https://discord.com/developers/applications).  

See järel mine OAuth2 alla ning OAtuh2 URL Generator alt vali "bot".
![Botile õiguste andmine](images/14.png "Botile õiguste andmine")

Õiguste alt ei pea valima midagi, vaid keri alla ning kopeeri link kopeeri genereeritud URL.
<!-- ![Boti Administraatoriks tegemine](images/15.png "Boti administraatoriks tegemine") -->
![URLi kopeerimine](images/16.png "URLi kopeerimine")  
**<span style="color:cyan"> Boti link:</span>** https://discord.com/oauth2/authorize?client_id=1331916331997724672&permissions=8&integration_type=0&scope=bot

Nüüd mine kopeeritud linigle ning vali, millisesse serverisse sa boti kutsuda tahad, seejärel vajuta _Continue_ ning _Authorize_.
![Boti serverisse lisamine](images/17.png "Boti serverisse lisamine")

Seejärel on bot sinu serverisse lisatud, kuid ta on offline.  
![Bot on lisatud serverisse](images/18.png "Bot on lisatud serverisse")

## Boti ellu äratamine ehk koodi jooksutamine
Selleks, et koodi käivitada, peab kõigepealt üles leidma faili, mida me käivitada tahame. Antud prjektis on selle faili nimi `game.py`.
![Faili käivitamine PyCharmis](images/33.png "Faili käivitamine PyCharmis")
Seejärel vajuta üleval paremas servas olevat rohelist noolekest (kolmunrk, mis on rohelisest putukast vasakul pool).
