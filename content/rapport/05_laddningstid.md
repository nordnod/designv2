# Kmom05 Laddningstid

Uppgiften går ut på att välja ut tre webbplatser, efter eget tycke och smak, för att sedan analysera dessa sidors laddningstid.

## Urval
Mitt urval av sidor att analysera består dels av två sidor relaterade till World Of Warcraft, dels en nyhetssida för PC samt spelvärlden generellt.
Jag valde att använda samma sidor att analysera som jag hade i föregående uppgift.

[Raidbots](https://www.raidbots.com/)

[Icy Veins](https://www.icy-veins.com/)

[Sweclockers](https://www.sweclockers.com/)

## Metod

Metoden för att analysera sidorna består i att mäta dem med "PageSpeed Insights" samt Firefox Devtools (nätverksfliken, cache avstängd).

# Resultat
#### [Raidbots](https://www.raidbots.com/)
[FIGURE src=image/raidbots.png?w=300 class="right"]
Analysen med Pagespeed visar på ett väldigt gott resultat gällande desktop-versionen, men ett mindre bra resultat för mobila enheter.
Sidan fick i snitt 99 poäng i desktopläge och 33,7 poäng i mobilt läge när jag analyserade med PageSpeed.
Laddningstiden i Firefox Devtools blev i snitt 1.29s.
Antalet resurser som laddas är 12st och den totala storleken 2.58MB.
Det som tar mest tid att ladda är ett tungt Javascript (2.36MB).

Eftersom detta är en central del av sidan (scriptet som gör analysen av ens karaktär) är det troligtvis inte mycket man kan göra åt detta.
Provar jag att använda sidan mobilt kan jag inte påstå att den upplevs så långsam som testet gör gällande.

#### [Icy Veins](https://www.icy-veins.com/)
[FIGURE src=image/icy.png?w=300 class="left"]
Detta är en sida med dels nyheter om Blizzards (spelutvecklare) spel, men även med spelguider av olika slag.
Analysen med Pagespeed visar återigen på ett mycket gott resultat för desktop-versionen och ett medelbetyg för mobila enheter.
I desktopläge hamnar snittet på 99 poäng respektive 60 poäng för mobil.
Laddningstiden i Devtools blev i snitt 2.11s.
Antalet resurser som laddas är 88st och storleken 2.2MB.

Ändringar som föreslås för desktopläge är användning av modernare bildformat samt att ta bort/flytta Javascript-kod som blockerar renderingen.
Vad gäller mobilläge så är det dels återigen användning av modernare bildformat som föreslås men framförallt att skjuta upp inläsning av bilder som inte visas på skärmen.
Många bilder är onödigt stora, i synnerhet för mobilt läge.

#### [Sweclockers](https://www.sweclockers.com/)
[FIGURE src=image/swec.png?w=300 class="left"]
Även detta är en nyhetssida och därför lite svårare att analysera rent färgmässigt. Mycket består av bilder och förhandsvisningar av artikar.
Min analys med PageSpeed ger ett mycket bra resultat för desktopläge, medans resultatet inte är fullt lika bra i mobilt läge.
Det blir 100 poäng i desktopläge och i snitt 32.3 poäng i mobilt läge.
I Devtools är den genomsnittliga laddningstiden 788ms.
Antalet resurser är 59st och storleken 2.49MB.

PageSpeed föreslår för desktopläge användande av modernare bildformat samt att ta bort resurser som blockerar renderingen av sidan.
För mobilt läge föreslås att skjuta upp inläsning av bilder som inte visas på skärmen samt att läsa in viktiga resurser i förväg.
Även här skulle det vara fördelaktigt att använda modernare bildformat.

# Analys
[Analysdokument - Excel](kmom05_laddningstid.xlsx)

En laddningstid på kring två sekunder tycker jag upplevs snabbt.
Tar det upp emot fem sekunder är sidan för långsam.
Samtliga sidor i min analys känns snabba att använda både på datorn och på mobilen.

Jag utser Sweclockers till vinnare av min analys. Sidan är grymt snabb i desktopläge och upplevs snabb även i mobilt läge, även om den inte fick bäst betyg i PageSpeed Insights.
Vanligaste åtgärden för sidorna i min analys är att senarelägga inläsning av bilder som inte visas, samt att optimera bilderna till modernare format.
Testresultaten visare att Sweclockers har den snabbaste inläsningen både vad gäller desktopläge samt mobilt läge.
Raidbots är just något snabbare än Icy Veins i desktopläge, men desto långsammare i mobilt läge. Således hamnar Icy Veins på plats två.
Återstår gör då plats tre vilken går till Raidbots.

I takt med att bredbandsuppkopplingarna blir snabbare och snabbare blir kravet på snabbladdande sidor
större och större. Förr hade man mer tålamod med långsamma sidor och jag vill minnas att jag någonstans läst att genomsnittstiden man orkar vänta på att en app eller ett program
svarar på ens handlande är kring 3 sekunder.
Även om mobila uppkopplingar också blir snabbare finns det en poäng med att optimera sidorna för dessa enheter, inte minst som de flesta mobilabonnemang fortfarande
har en begränsad mängd data per månad.



# Referenser
[PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)

# Övrigt
Rapporten är utförd av David N på egen hand.
