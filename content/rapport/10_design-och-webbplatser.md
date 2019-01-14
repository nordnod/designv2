# Kmom10 Uppdrag 2
## Analys valfri

Uppgiften går ut på att välja ut ett par webbplatser och analysera dessa.
Eftersom det är fri tolkning, inom ramen för kursen, av vad som ska analyseras väljer jag att laddningstid och hur väl mobilanpassade de är.

## Urval
Jag har valt att analysera ett par olika nyhetssiter.

[Expressen](https://www.expressen.se/)

[Aftonbladet](https://www.aftonbladet.se/)

[DN](https://www.dn.se/)

## Metod
Metoden för att analysera sidorna består i att mäta dem med “PageSpeed Insights” samt Firefox Devtools (nätverksfliken, cache avstängd).
Utöver det återger jag min personliga uppfattning om hur väl sidorna fungerar i mobilt läge.
Det mobila läget testas dels genom simulering i Firefox (profil: iPhone 6/7/8) samt med en iPhone 8 Plus med Safari.

# Resultat
#### [Expressen](https://www.expressen.se/)
[FIGURE src=image/expressen.png?w=500 class="left"]
När jag analyserar sidan med PageSpeed Insights uppnås ett gott resultat för desktop-versionen och ett medelbra resultat för mobila enheter.
I desktopläge får sidan 97 poäng och i mobilt läge 54 poäng.

Firefox Devtools rapporterar om en laddningstid på kring 20 sekunder, vilket är väldigt lång tid. Låter man sidan sen "stå", så fortsätter innehåll laddas och förfrågningarna blir fler och fler.
Efter någon minut har förfrågningarna passerat 180st och tiden för slutförd laddning passerat minuten.
Totalt laddas 9.91MB i desktopläge och 2.5MB i mobilt läge.
Sidan upplevs inte långsam vid normalt användande, däremot är det flera externa förfrågningar som tar lång tid. Bland annat externa script och CDN för annonser med mera.

I mobilt läge ser sidan helt OK ut. Tyvärr innhehåller de flesta nyhetssidor väldigt mycket reklam. Rent designmässigt stör jag mig lite på att en del artiklar/bilder endast kommer med till hälften.
Dock tror jag att det är avsett att vara så för att man ska förstå att dessa sektioner är scrollbara horisontellt.
Navbaren i ovankant går att scrolla och det finns även en hamburgermeny. Innehållet i dessa är inte exakt samma utan hamburgermenyn innehåller betydligt fler länkar. Detta gäller både i desktop- och mobilt läge.


#### [Aftonbladet](https://www.aftonbladet.se/)
[FIGURE src=image/aftonbladet.png?w=500 class="center"]
Analysen med PageSpeed Insights visar på ett riktigt bra resultat i desktopläge där sidan får 97 poäng. I mobilt läge däremot är resultatet mediokert med endast 30 poäng.
Rapportens huvudsakliga föreslag till åtgärd är att ta bort resurser som blockerar renderingen av sidan.
I Firefox Devtools får jag ett resultat som visar på 89 förfrågningar och totalt laddas 8.66MB. Laddningstiden är 6.34 sekunder.
I mobilt läge laddas 5.26MB

Mobilt läge påminner om föregående sida, här finns däremot ingen hamburgermeny utan istället en väldigt lång navbar som scrollar sidledes.
Det finns (vid användande på iPhone 8 och Safari) inget som upplyser användaren om att denna meny är scrollbar, utan det får man upptäcka själv.
I övrigt känner man igen sig jämfört med desktopversionen.

#### [DN](https://www.dn.se/)
[FIGURE src=image/dn.png?w=500 class="right"]
DN.se får ett gott resultat i PageSpeed Insights analysen. 95 poäng i desktopläge och 61 poäng i mobilt läge.
Ett förslag till åtgärd för förbättrad prestanda uppges vara att skjuta upp CSS som inte används, samt att skjuta upp inläsning av bilder som inte visas på skärmen.
Firefox Devtools rapporterar om 36 förfrågningar och en inläsningstid på 1.09 sekunder. Totalt laddas 1.14MB i desktopläge och 1.12MB i mobilt läge.

Det mobila läget får en extra meny alla längst upp som inte finns i desktopläge. Under denna är normalmenyn scrollbar i sidled vilket man får en hint om genom att ett menyalternativ är halvt suddigt
så man ska förstå att det går att scrolla.

# Analys
En sak jag noterat med Firefox Devtools igång är att det laddas in content efterhand man scrollar på sidan. Detta är naturligtvis smart på så sätt att inte mer data än nödvändigt laddas.
Sidorna i analysen upplevs inte särskilt långsamma, trots att de får ett ganska dåligt resultat åtminstone i mobilt läge.
De innehåller däremot väldigt mycket reklam så de hade troligtvis kunna vara betydligt alertare än vad de är.
Jag har dessutom gjort testerna på 500Mbit Wi-Fi, sannolikt hade det varit stor skillnad att testa över mobilt bredband.

I två av fallen laddas väldigt många resurser och kring 8-9MB för en sidladdning är väldigt mycket. Dock minskas sidladdningen i MB räknat till cirka en tredjedel i mobilt läge.
I ena fallet verkar dock ungefär samma mängd laddas, men den är också avsevärt mindre från början.

# Referenser
[PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/?hl=sv)

# Övrigt
Rapporten är utförd av David N på egen hand.
