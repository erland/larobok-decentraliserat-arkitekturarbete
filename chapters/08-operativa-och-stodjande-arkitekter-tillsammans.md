# Kapitel 8: Operativa och stödjande arkitekter tillsammans

## Varför detta kapitel finns

I en decentraliserad organisation uppstår arkitekturarbete i mötet mellan lokala behov och gemensamma förutsättningar. De operativa utvecklingsområdena behöver kunna agera snabbt på verksamhetens behov. De stödjande och förutsättningsskapande utvecklingsområdena behöver samtidigt skapa lösningar, riktlinjer och tekniska förmågor som kan användas av flera.

Detta kapitel handlar om hur operativa och stödjande arkitekter kan arbeta tillsammans utan att fastna i två vanliga ytterligheter: att varje operativt område bygger egna lokala lösningar, eller att gemensamma förutsättningar blir så styrande att de upplevs som hinder. Båda ytterligheterna leder till sämre arkitektur. Den första skapar dubbelarbete, fragmentering och teknisk skuld. Den andra riskerar att minska ansvarstagande, tempo och verksamhetsnytta.

Arkitektens praktiska uppgift är att bidra till en bättre balans.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara varför operativa och stödjande arkitekter behöver samverka tidigt och konkret
- känna igen när ett lokalt behov kan vara ett tecken på en gemensam förmåga
- skilja mellan lokal anpassning, återanvändbar lösning och gemensam tjänst
- använda kvalitetssäkring för att pröva om en gemensam förutsättning faktiskt stödjer operativa behov
- använda samordning för att undvika både suboptimering och onödig centralisering

## Innan vi börjar

Tidigare kapitel har introducerat styrning, samordning, kvalitetssäkring, principer och arkitekturbeslut. I detta kapitel används de begreppen i en konkret samverkanssituation.

En viktig utgångspunkt är att decentralisering inte betyder att varje område ska lösa allt själv. Det betyder inte heller att stödjande områden ska fatta alla viktiga beslut. Decentralisering kräver ett fungerande samspel mellan lokal beslutskraft och gemensamma förutsättningar.

## Huvudförklaring

### Två perspektiv som båda är nödvändiga

Den operativa arkitekten står nära verksamhetens behov. Det innebär ofta bättre förståelse för användare, processer, prioriteringar, tidplaner och praktiska begränsningar. Den operativa arkitekten ser vad som måste fungera i tjänsten här och nu.

Den stödjande arkitekten står närmare organisationens gemensamma förutsättningar. Det kan handla om plattformar, integrationsmönster, säkerhetslösningar, gemensamma informationsmodeller, tekniska riktlinjer eller återanvändbara tjänster. Den stödjande arkitekten ser ofta mönster över flera initiativ.

Båda perspektiven är begränsade var för sig. Den operativa arkitekten riskerar att underskatta långsiktiga konsekvenser utanför det egna området. Den stödjande arkitekten riskerar att underskatta variationen i verkliga verksamhetsbehov. När perspektiven möts tidigt kan organisationen fatta bättre beslut.

### Förutsättningsskapande arbete är inte bara leverans av komponenter

Ett vanligt missförstånd är att stödjande utvecklingsområden främst levererar komponenter som andra ska använda. I praktiken är förutsättningsskapande arbete bredare än så. Det kan bestå av:

- tydliga guardrails
- gemensamma mönster
- återanvändbara tjänster
- rådgivning och arkitekturdialog
- mallar för beslut och granskning
- tekniska plattformar
- exempel och referenslösningar
- förvaltade principer och riktlinjer

Det stödjande området skapar värde när det gör det enklare för operativa områden att fatta bra beslut och leverera hållbara lösningar. En gemensam komponent är bara värdefull om den faktiskt går att använda i operativ utveckling.

### Lokala behov kan visa gemensamma mönster

När ett operativt område uttrycker ett behov bör arkitekten inte bara fråga: “Hur löser vi detta här?” Minst lika viktigt är att fråga: “Är detta ett behov som fler kommer att ha?”

Det betyder inte att varje behov ska göras gemensamt. Det betyder att arkitekten behöver upptäcka mönster. Ett lokalt behov kan vara:

- helt lokalt och bäst löst nära verksamheten
- lokalt just nu, men troligen återkommande i flera områden
- ett uttryck för en redan känd gemensam förmåga
- ett tecken på att en befintlig gemensam förutsättning inte räcker
- en avvikelse som behöver motiveras och följas upp

Arkitektens värde ligger ofta i att se vilken typ av behov det faktiskt är.

### Gemensamt får inte betyda stelt

Gemensamma förutsättningar behövs för effektivitet, kvalitet och samordning. Men gemensamma lösningar behöver vara användbara i verkliga sammanhang. Om en gemensam tjänst inte möter rimliga operativa behov kommer organisationen ändå att få lokala lösningar, ofta utan tydlig styrning eller spårbarhet.

Därför behöver stödjande arkitekter vara nyfikna på varför operativa områden upplever en gemensam lösning som begränsande. Det kan bero på missförstånd, bristande kommunikation eller låg kännedom. Men det kan också bero på att den gemensamma lösningen faktiskt saknar nödvändig funktionalitet, har för hög tröskel eller bygger på antaganden som inte längre stämmer.

Kvalitetssäkring bör därför riktas åt båda håll. Den operativa lösningen behöver kvalitetssäkras mot gemensamma principer. Den gemensamma förutsättningen behöver kvalitetssäkras mot operativa behov.

### Samarbete kräver tydliga samverkanspunkter

Operativa och stödjande arkitekter behöver inte samordna allt. Men vissa situationer bör nästan alltid skapa dialog:

- när ett operativt område behöver göra ett avsteg från en gemensam lösning
- när flera områden efterfrågar liknande funktionalitet
- när en gemensam tjänst behöver anpassas för ett konkret verksamhetsflöde
- när det råder oklarhet om ansvar för information, integration eller förvaltning
- när en lokal lösning kan bli återanvändbar
- när ett stödjande område planerar förändringar som påverkar flera operativa områden
- när en operativ leverans är beroende av en gemensam förutsättning som inte är färdig

Poängen är inte att skapa fler forum. Poängen är att skapa rätt samtal i rätt tid.

## Scenario

Det operativa utvecklingsområdet arbetar vidare med den nya digitala tjänsten. Teamet behöver en funktion för notifieringar till användare. Det finns en gemensam notifieringstjänst som det stödjande utvecklingsområdet ansvarar för, men teamet upplever att tjänsten inte stödjer alla krav i det aktuella flödet.

Teamet överväger därför att bygga en egen notifieringslösning. Den operativa arkitekten ser att detta skulle ge snabbare framdrift. Samtidigt finns risker: dubbla lösningar, otydlig förvaltning, inkonsekvent användarupplevelse och svårare uppföljning av utskick.

Den stödjande arkitekten ser en annan risk. Om varje område gör egna undantag urholkas den gemensamma notifieringsförmågan. Men den stödjande arkitekten behöver också förstå om den gemensamma tjänsten faktiskt saknar nödvändigt stöd.

Ett konstruktivt arbetssätt blir att arkitekterna tillsammans formulerar frågan som ett arkitekturbeslut:

- Vilka behov i den digitala tjänsten täcks av den gemensamma notifieringstjänsten?
- Vilka behov täcks inte?
- Är de saknade behoven specifika för detta område eller troligen generella?
- Kan den gemensamma tjänsten kompletteras inom rimlig tid?
- Behövs en tillfällig lokal lösning?
- Hur ska ansvar och uppföljning hanteras om en lokal lösning används?
- När ska beslutet omprövas?

På detta sätt blir frågan inte en konflikt mellan “lokalt” och “centralt”. Den blir en gemensam arkitekturbedömning.

## Vad arkitekten bör tänka på

### Börja med behovet, inte lösningsägaren

Det är lätt att samtalet börjar med frågan om vem som äger lösningen. Den frågan är viktig, men den bör inte komma först. Börja istället med behovet:

- Vilket problem ska lösas?
- För vem?
- Hur ofta uppstår behovet?
- Finns liknande behov i andra områden?
- Vilka kvaliteter är viktiga: säkerhet, robusthet, användbarhet, spårbarhet, kostnad, förändringsbarhet?
- Vilka konsekvenser får en lokal respektive gemensam lösning?

När behovet är tydligt blir ansvarsdialogen mer saklig.

### Synliggör skillnaden mellan återanvändning och tvång

Återanvändning fungerar bäst när den skapar nytta för den som återanvänder. Om en gemensam lösning bara uppfattas som ett krav ökar risken för motstånd och informella omvägar.

Arkitekten bör därför kunna förklara varför återanvändning är viktig. Det kan handla om lägre förvaltningskostnad, bättre säkerhet, konsekvent användarupplevelse, snabbare framtida utveckling eller minskad teknisk skuld. Men arkitekten behöver också vara beredd att lyssna när återanvändning inte fungerar i praktiken.

### Gör gemensamma förutsättningar begripliga

En gemensam tjänst eller princip behöver vara begriplig för operativa områden. Det räcker inte att den finns. Operativa arkitekter och team behöver förstå:

- när den ska användas
- vilka behov den stödjer
- vilka begränsningar den har
- hur man ansluter till den
- vem man kontaktar vid frågor
- hur avvikelser hanteras
- hur förbättringsbehov fångas upp

Om detta saknas kommer den gemensamma förutsättningen att vara svår att använda även om den tekniskt sett är bra.

### Behandla friktion som information

Friktion mellan operativa och stödjande perspektiv är inte alltid ett problem. Den kan vara en viktig signal. Friktion kan visa att ett behov är otydligt, att en princip är svår att tolka, att en gemensam tjänst saknar funktionalitet eller att ansvarsfördelningen är oklar.

Arkitektens uppgift är inte att undvika all friktion. Uppgiften är att använda friktionen för att förstå vad som behöver förbättras.

## När kvalitetssäkring bör ske

Kvalitetssäkring bör ske när samarbetet mellan operativa och stödjande arkitekter påverkar lösningens långsiktiga hållbarhet. Särskilt viktigt är det vid följande tillfällen:

### När en gemensam förutsättning ska användas i ett nytt sammanhang

Kvalitetssäkra om den gemensamma lösningen verkligen stödjer behovet. Pröva inte bara teknisk anslutning, utan även ansvar, användbarhet, säkerhet, förvaltning och framtida förändringar.

### När ett operativt område vill bygga en lokal lösning

Kvalitetssäkra varför den lokala lösningen behövs. Är det ett legitimt specialbehov, en tillfällig lösning, en brist i den gemensamma förutsättningen eller ett tecken på låg kännedom om befintliga alternativ?

### När en gemensam lösning upplevs som hinder

Kvalitetssäkra både den operativa tolkningen och den gemensamma lösningens utformning. Ibland behöver teamet mer stöd. Ibland behöver den gemensamma lösningen förbättras.

### När ett tillfälligt avsteg accepteras

Kvalitetssäkra att avsteget har tydlig motivering, riskbedömning, ansvar, livslängd och uppföljningspunkt. Ett tillfälligt avsteg utan uppföljning blir ofta permanent teknisk skuld.

### När flera områden efterfrågar liknande funktionalitet

Kvalitetssäkra om organisationen bör etablera eller vidareutveckla en gemensam förmåga. Här bör fokus ligga på mönster, inte på ett enskilt teams behov.

## När samordning bör ske

Samordning bör ske när beslutet inte längre är enbart lokalt. Det gäller särskilt när flera utvecklingsområden påverkas direkt eller indirekt.

### Samordna när behov återkommer

Om flera operativa områden beskriver liknande behov bör arkitekter samordna analysen. Målet är inte automatiskt att skapa en gemensam tjänst, utan att förstå om en gemensam förmåga behövs.

### Samordna när ansvar är otydligt

Många arkitekturproblem uppstår i mellanrummen mellan organisationens delar. Samordning behövs när det är oklart vem som ansvarar för information, integrationer, förvaltning, support eller vidareutveckling.

### Samordna när en stödjande förändring påverkar operativa leveranser

Stödjande områden behöver samordna förändringar som påverkar flera operativa områden. Annars riskerar gemensamma förbättringar att skapa lokala störningar.

### Samordna när lokala lösningar kan påverka gemensamma mönster

Om ett operativt område gör ett vägval som kan bli prejudicerande bör det samordnas. Annars kan organisationen få flera olika lösningar på samma typ av problem utan att ha valt det medvetet.

### Samordna när beroenden påverkar tidplaner

Om en operativ leverans är beroende av en gemensam tjänst, plattform eller riktlinje behöver arkitekterna synliggöra beroendet tidigt. Annars riskerar frågan att upptäckas först när teamet redan är låst i sin planering.

## Vanliga fallgropar

- **Fallgrop: “Det stödjande området vet bäst”**

- **Fallgrop: “Det operativa området måste få bestämma själv”**

- **Fallgrop: “Gemensamt betyder en lösning för alla”**

- **Fallgrop: “Avsteg hanteras informellt”**

- **Fallgrop: “Dialogen sker för sent”**

## Snabb sammanfattning

- Operativa arkitekter bidrar med närhet till verksamhet, användare och leverans.
- Stödjande arkitekter bidrar med gemensamma förutsättningar, mönster och helhet över flera områden.
- Bra arkitekturarbete uppstår när dessa perspektiv möts tidigt.
- Lokala behov kan vara helt lokala, men kan också visa behov av gemensamma förmågor.
- Kvalitetssäkring bör pröva både lokala lösningar och gemensamma förutsättningar.
- Samordning behövs när behov, ansvar, beroenden eller konsekvenser går över områdesgränser.
- Gemensamma lösningar skapar värde först när de är begripliga, användbara och möjliga att förbättra.

## Reflektionsfrågor

1. Vilka gemensamma förutsättningar i din organisation upplevs som verkligt hjälpsamma av operativa team?
2. Var finns det återkommande lokala behov som kanske borde ses som gemensamma mönster?
3. Hur fångas förbättringsbehov från operativa områden upp av stödjande utvecklingsområden?
4. Vilka avsteg från gemensamma lösningar riskerar att bli permanenta utan uppföljning?
5. Finns det samverkanspunkter tidigt nog för att påverka viktiga vägval?

## Nästa steg

Nästa kapitel fördjupar hur arkitekten kan hantera avvikelser och lokala lösningar. Där flyttas fokus från samverkan mellan operativa och stödjande arkitekter till hur organisationen kan bedöma när avsteg är rimliga, när de är riskabla och hur de bör följas upp.
