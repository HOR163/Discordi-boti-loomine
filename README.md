# Discord boti loomine

## Discordi konto loomine (kui pole veel seda)
Selleks, et boti luua, peab olema discordi konto, selle tegemiseks mine lehele [https://discord.com/register](https://discord.com/register).  
Konto kasutajanimeks võid kasutada ükskõik mida (ei pea olema sinu päris nimi).  
<img src="images/5.png" width=75%/>  


## Boti loomine ja kutsumine serverisse
Mine lehele [https://discord.com/developers/applications](https://discord.com/developers/applications) ning loo uus rakendus <kbd>New Application</kbd>.  
<img src="images/6.png" width=75%/>  
<img src="images/7.png" width=50%/>  

Liigu OAuth2 alla ning **OAuth2 URL Generator** alt vali <kbd>bot</kbd>.  
<img src="images/14.png" width=75%/>

Õiguste alt ei pea valima midagi, vaid keri alla ning kopeeri loodud link.  
<img src="images/16.png" width=75%/>

Nüüd mine sellele lingile ning vali, millisesse serverisse sa boti kutsuda tahad, seejärel vajuta <kbd>Continue</kbd> ning <kbd>Authorize</kbd>.
<img src="images/17.png" width=75%/>

Seejärel on bot serverisse lisatud ning ta on offline (peabki olema).  
<img src="images/18.png" width=75%/>


## Õiguste andmine botile

Liigu vasakul menüüs <kbd>Bot</kbd> alla, keri natuke allapoole ning lülita sisse **PRESENCE INTENT**, **SERVER MEMBERS INTENT**, **MESSAGE CONTENT INTENT** ning vajuta **Save Changes**  
<img src="images/31.png" width=75%/>  


## Tokeni loomine botile

Selleks, et boti kasutada saaks, tuleb kuidagi temaga suhelda. Token on nagu emaili aadress: kui sa tead boti tokenit, siis saad talle korraldusi saata. Seega mine <kbd>Bot</kbd> alla ning vajuta <kbd>Reset Token</kbd>.
<img src="images/8.png" width=75%/>  

Token-i resettimise käigus küsib discord parooli (või mingit muud autentimisviisi), see on normaalne.  
Kopeeri token (see on see pikk numbrite, tähtede ning sümbolite jada) ning aseta see kuskil turvalisse kohta (näiteks notepadi), sest seda läheb hiljem tarvis.  
<img src="images/9.png" width=75%/>  

## Edasised sammud
Järgmine samm on katsetada seda et token ning bot töötavad, selle jaoks liigu järgnevale lingile ning järgi juhiseid: https://github.com/anpeep/uno-pygame

