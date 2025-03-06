# Discord boti loomine

| Sisukord | |
-----------|--------------
| [Discordi konto loomine](#discordi-konto-loomine-kui-sul-pole-veel-seda) | Kui sul on juba discordi konto, siis võid selle vahele jätta (peaasi et parooli tead või mingil muul moel saad sisse) |
| [Boti loomine](#Boti-loomine) |  
| [Boti kutsumine serverisse](#boti-kutsumine-serverisse) |



## Discordi konto loomine (kui pole veel seda)
Selleks, et boti luua, peab olema discordi konto, selle tegemiseks mine lehele [https://discord.com/register](https://discord.com/register).  
Konto kasutajanimeks võid kasutada ükskõik mida (ei pea olema sinu päris nimi).
![Discordi konto loomine](images/5.png "Discordi konto loomine")



## Boti loomine
Mine lehele [https://discord.com/developers/applications](https://discord.com/developers/applications) ning loo uus rakendus <kbd>New Application</kbd>.  
![Discordi rakenduse loomine](images/6.png "Discordi rakenduse loomine")
Anna enda botile mingi nimi.  
![Botile nime andmine](images/7.png "Botile nime andmine")

Selleks, et boti kasutada saaks, tuleb temale juurdepääs saada. Selleks on vaja boti tokenit. Seega mine <kbd>Bot</kbd> alla ning vajuta <kbd>Reset Token</kbd>.
![Boti tokeni leidmine](images/8.png "Boti tokeni leidmine")  

Token-i resettimise käigus ilmselt küsib discord parooli, see on normaalne. Nüüd kopeeri token (see on see pikk numbrite, tähtede ning sümbolite jada).  
![Boti tokeni leidmine](images/9.png "Tokeni kopeerimine") 

Aseta token näiteks notepadi, selleks et see ära ei kaoks. Juhul kui peaks ära kaduma, siis selle saab uuesti genereerida.  
Näiteks võib token välja näha nagu midagi sellist: _MTMzMTkxNjMzMTk5NzcyNDY3Mg.GrqBgo.arZGbXr03qzGS_G9-oE7amyL7rUkSnc7cU4ODw_

Keri veel natuke allapoole ning lülita sisse _MESSAGE CONTENT INTENT_  
![Message content intent sisse lülitamine](images/31.png "Message content intent sisse lülitamine")  
Kindlasti salvesta ka muudatused.  
<details>

  <summary><b>Mis on intent?</b></summary>

  Intent on discordis eraldi viis kuidas botiga suhelda. Näiteks kui bot on kuskil kanalis, saab bot ainult sulle saata sõnumi, nii et teised seda sõnumit ei näe. Kuna uno mängus teised ei tohi su kaarte näha, siis on see väga hea viis enda kaartide nägemiseks.
  ![Discordi intent sõnum](images/32.png "Discordi intent sõnum")

</details>

Nüüd on bot valmis ning töökorras, kuid selleks et temast asja oleks, tuleb ta kutsuda serverisse.



## Boti kutsumine serverisse
Mine enda boti lehele [https://discord.com/developers/applications](https://discord.com/developers/applications).  

See järel mine OAuth2 alla ning OAuth2 URL Generator alt vali <kbd>bot</kbd>.
![Botile õiguste andmine](images/14.png "Botile õiguste andmine")

Õiguste alt ei pea valima midagi, vaid keri alla ning kopeeri link kopeeri genereeritud URL.
<!-- ![Boti Administraatoriks tegemine](images/15.png "Boti administraatoriks tegemine") -->
![URLi kopeerimine](images/16.png "URLi kopeerimine")  


Nüüd mine kopeeritud lingile ning vali, millisesse serverisse sa boti kutsuda tahad, seejärel vajuta <kbd>Continue</kbd> ning <kbd>Authorize</kbd>.
![Boti serverisse lisamine](images/17.png "Boti serverisse lisamine")

Seejärel on bot sinu serverisse lisatud, kuid ta on offline.  
![Bot on lisatud serverisse](images/18.png "Bot on lisatud serverisse")


## Edasised sammud
Järgmine samm on katsetada seda et token ning bot töötavad, selle jaoks liigu siia ning lae alla: https://livettu-my.sharepoint.com/:u:/g/personal/anmeno_taltech_ee/EWpn1ydGryJNoM7vOjGJp5IBX4VWH7dnYeYer3NJcCgk3Q?e=ig4KkC

