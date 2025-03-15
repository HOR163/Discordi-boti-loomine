# Discord boti loomine

## Discordi konto loomine (kui pole veel seda)
Selleks, et boti luua, peab olema discordi konto, selle tegemiseks mine lehele [https://discord.com/register](https://discord.com/register).  
Konto kasutajanimeks võid kasutada ükskõik mida (ei pea olema sinu päris nimi).  
<img src="images/create_discord_account.png" width=75%/>  


## Boti loomine ja kutsumine serverisse
Ühine Boti töötoa serveriga: [https://discord.gg/azW56CWK](https://discord.gg/azW56CWK)

Loo servrisse UnoBot sektsiooni alla uus kanal, kuhu paned ka emoji või sümboli millega boti välja kutsuma hakkad (siis ei hakka teiste botid teile vastama)  
<img src="images/channel_creation.png" width=33% />
<img src="images/channel_name.png" width=33% />

Mine lehele [https://discord.com/developers/applications](https://discord.com/developers/applications) ning loo uus rakendus <kbd>New Application</kbd>.  
<img src="images/new_discord_application.png" width=75%/>  
<img src="images/naming_the_bot.png" width=50%/>  

Liigu **OAuth2** menüüsse ning **OAuth2 URL Generator** alt vali <kbd>bot</kbd>.  
<img src="images/url_generator_settings.png" width=75%/>

Õiguste alt ei pea valima midagi, vaid keri alla ning kopeeri loodud link.  
<img src="images/copy_bot_invite_link.png" width=75%/>

Nüüd mine sellele lingile ning vali, millisesse serverisse sa boti kutsuda tahad, seejärel vajuta <kbd>Continue</kbd> ning <kbd>Authorize</kbd>.
<img src="images/invite_bot_to_server.png" width=75%/>

Seejärel on bot serverisse lisatud ning ta on offline (peabki olema).  
<img src="images/bot_in_the_server.png" width=75%/>


## Õiguste andmine botile

Liigu vasakul menüüs <kbd>Bot</kbd> alla, keri natuke allapoole ning lülita sisse **PRESENCE INTENT**, **SERVER MEMBERS INTENT**, **MESSAGE CONTENT INTENT** ning vajuta <kbd>Save Changes</kbd>  
<img src="images/adding_intents.png" width=75%/>  


## Tokeni loomine botile

Selleks, et boti kasutada saaks, tuleb kuidagi temaga suhelda. Token on nagu emaili aadress: kui sa tead boti tokenit, siis saad talle korraldusi saata. Seega mine <kbd>Bot</kbd> alla ning vajuta <kbd>Reset Token</kbd>.
<img src="images/resetting_bot_token.png" width=75%/>  

Token-i resettimise käigus küsib discord parooli (või mingit muud autentimisviisi), see on normaalne.  
<img src="images/reset_bot_token_popup.png" width=33%>
<img src="images/password_for_resetting_the_token.png" width=33%>

Kopeeri token (see on see pikk numbrite, tähtede ning sümbolite jada) ning aseta see kuskile turvalisse kohta (näiteks notepadi), sest seda läheb hiljem tarvis.  
<img src="images/copying_bot_token.png" width=75%/>  

## Edasised sammud
Järgmine samm on katsetada seda et token ning bot töötavad, selle jaoks liigu järgnevale lingile ning järgi juhiseid: https://github.com/anpeep/uno-pygame  
Peale seda unobotiga mängimist saab luua endale lihtsat chatboti: https://github.com/taltech-coding/discord-bot

