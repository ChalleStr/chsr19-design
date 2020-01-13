Webbplatsers laddningstid
=============================

Skriv en eller två rader om vad uppgiften handlar om.

Urval
-----------------------

Jag har valt tre webbplatser att analysera:  
- Coop.se  
- Ica.se  
- Willys.se  

Jag är ett fan av att handla mat online och få det hemkört men många av deras webbplatser är långsamma och hakar upp sig hela tiden. Därför var jag intresserad av hur laddningstiden för de olika matkedjornas webbplatser ser ut.

Metod
-----------------------

Berätta kort om din "metod", hur du gör för att utföra undersökningen. Berätta om du använder något speciellt verktyg.

Resultat
-----------------------

Länk till kalkylark med mina mätningar: https://docs.google.com/spreadsheets/d/19ZYi0NU0BcuIRAKyFL3hP4X9YWGXKyaQadu3XQ_W5pI/edit?usp=sharing 

Mätningarna med devtools visade att Icas sidor tog längst tid att ladda och Willys gick snabbast. Pagespeed rankade dock Coops sidor högst och Willys lägst på desktop. Mobile var högre för båda.

####Coop  

[FIGURE src=image/coop.png?w=100%&h=900&crop-to-fit caption="Snapshot coop.se." class="center"]

[Coop.se](http://www.coop.se/)  
[Coop.se/recept](http://www.coop.se/recept)  
[Coop.se/handla](http://www.coop.se/handla)  

Pagespeed desktop rankade coop.se högst av sidorna med ett snitt på 71 över de undersidor jag testade medan mobile låg betydligt lägre på 19. Mina mätningar med devtools gav snitt på 6,15 sekunder i laddninstid, total storlek på 5,7 MB och antal resurser på 94. Överlag har sidorna många bilder vilket jag tror är största orsaken till att den laddar långsamt, särskilt på mobil.

####Ica  

[FIGURE src=image/ica.png?w=100%&h=900&crop-to-fit caption="Snapshot ica.se." class="center"]

[Ica.se](http://www.ica.se/)  
[Ica.se/recept](http://www.ica.se/recept)  
[Ica handla](http://handla.ica.se/?returnUrl=https%3A%2F%2Fwww.ica.se)  

Näst bäst enligt Pagespeed desktop var Ica med ett snitt på 58. Mobile låg på 15,25. Devtools snittade på laddninstid 15,7 sekunder, total storlek på 2,82 MB och antal resurser på 72. Även här är bilder en bov och Ica skulle kunna förbättra hastigheten på sin handlingsida.

####Willys

[FIGURE src=image/willys.png?w=100%&h=900&crop-to-fit caption="Snapshot willys.se." class="center"]

[willys.se](http://www.willys.se/)  
[Willys handla](https://www.willys.se/erbjudanden/ehandel)  
[Willys kundservice](https://www.willys.se/artikel/kundservice)  

Willys fick ett snitt på 39 av Pagespeed desktop och 20 för mobile. Mina mätningar med devtools gav snitt på 2,83 sekunders laddningstid, 64 resurser och en storlek på 3,96 MB.


Analys
-----------------------

Mätningarna med devtools skiljde sig en del från Pagespeeds rankning. Enligt snittet jag fick fram med mätningarna i devtools hade Willys den snabbaste laddningstiden samt minst antal resurser och flest MB i total storlek. Däremot fick Willys ett lågt snitt på Pagespeeds betyg. Det beror antagligen på att snittet blir lite missvisande då två av tre sidor faktiskt hade ok betyg medan en tredje hade sämre och drog ner snittet. Betyget för mobile är genomgående dålig för Willys däremot. Pagespeed föreslår ett antal förbättringsåtgärdet så som att undvika ett onödigt stort DOM-träff och att minska arbetsbelastningen på modertråden. Man rekommenderar också att minska körningstiden för Javascript och att skicka statistiska tillgångar med en effektiv cachelagringspolicy.

Coop fick bäst snittbetyg av Pagespeed desktop men enligt devtools mätningar var laddningtiden sämre än Willys. Antalet laddade resurser var högst av alla. Det var framför allt sidan för handla online som drog upp snittet där. Pagespeed rekommenderar att skjuta upp laddning av bilder som inte används på skärmen, använda bilder i ett modernare bildformat, ta bort oanvänd CSS samt minifiera CSS och minska bildstorlekarna

Icas sidor tog avsevärt mycket längre tid att ladda än konkurrenternas. Första laddningen av handla online-sidan tog över en minut men de påföljande laddningarna tog bara runt två sekunder. Jag vet inte vad som spelade in där. Pagespeed desktop gav ett högt betyg på just den sidan. Däremot var mobile genomgående lågt med till exempel 1 på en av undersidorna Rekommenderade förbättringar var att ta bort resurser som blockerar rendering, aktivera textkomprimering, ta bort oanvänd CSS och att undvika upprepade omdirigeringar.

Samtliga webbplatser i analysen fick låga betyg av Pagespeed för sin mobila version. Av egen erfarenhet vet jag att coop.se i mobilen är långsamt och oberäkneligt med betalningar som hakat upp sig och kundkorgar som helt plötsligt tömt sig själva så att man fått göra om hela handlingen. Deras mobilapp är dock mycket bättre. Kanske väljer man att inte optimera webbplatsen så väl för mobil som man skulle kunna göra för att man vet att folk väljer appen i första hand?
Gemensamt för alla tre är att ingen av sidorna får särskilt höga betyg av Pagespeed varken för desktop eller mobil.

Baserat på mina mätningar har jag rangordnat webbplatserna enligt följande:  
 1. Willys  
 2. Coop  
 3. Ica  

Jag har gjort valet med laddningshastigheten som främsta argument då det är den aspekten som märks tydligast hos användaren.

Efter lite testande har jag märkt att jag upplever sidor som laddar långsammare än tre sekunder som långsamma. Precis som många av artiklarna säger så beror det en del på vilken sorts webbplats man besöker. Men om jag väljer att handla mat online gör jag det för att det ska gå snabbare än att fysiskt åka till affären. Då vill man inte ha en massa trassel. Generellt verkar det finnas en smärtgräns för två sekunders laddningstid för e-handel. Bara ett fåtal av sidorna jag testade klarar den gränsen och då endast på en enstaka mätning. Jag upplever inte att sidorna laddar långsamt utan det är snarare när det påverkar funktionerna som det blir störande.



Referenser
-----------------------

Google Pagespeed

Övrigt
-----------------------

Charlotte Strand
