# Kapitel 2: Den decentraliserade arkitektens vardag

## Varför detta kapitel finns

I en decentraliserad organisation sker mycket av utvecklingskraften nära verksamhetens behov. Det är en styrka. Operativa utvecklingsområden kan prioritera, utforska och leverera lösningar med bättre förståelse för de problem som ska lösas.

Samtidigt uppstår en särskild utmaning: när många områden arbetar självständigt kan arkitekturella beslut börja dra åt olika håll. Lösningar kan överlappa varandra, bygga på olika antaganden eller skapa beroenden som ingen har helhetsbild över. Arkitektens vardag handlar därför ofta om att hjälpa organisationen att behålla både lokal handlingskraft och gemensam riktning.

Det här kapitlet beskriver vad den decentraliserade arkitekten behöver vara uppmärksam på, hur samspel mellan operativa och stödjande utvecklingsområden kan fungera, och när kvalitetssäkring och samordning bör ske.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- beskriva skillnaden mellan operativa och stödjande/förutsättningsskapande utvecklingsområden
- förklara varför arkitektens roll förändras i en decentraliserad och agil organisation
- identifiera situationer där lokala beslut behöver samordnas med gemensamma förutsättningar
- avgöra när kvalitetssäkring bör ske i den decentraliserade vardagen
- agera praktiskt utan att ta över teamens ansvar eller skapa onödig kontroll

## Innan vi börjar

I kapitel 1 beskrevs arkitekturarbete som praktiskt arbete med riktning, sammanhang och kvalitet. Den bilden är viktig här. I en decentraliserad organisation räcker det inte att arkitekten har en bra lösningsbild för sitt eget område. Arkitekten behöver också förstå hur området samspelar med andra områden, gemensamma plattformar, informationsflöden, säkerhetskrav och långsiktig förvaltning.

Två begrepp används särskilt i detta kapitel:

- **Operativt utvecklingsområde**: ett område som utvecklar IT-stöd och digitala tjänster för att möta verksamhetens behov.
- **Stödjande/förutsättningsskapande utvecklingsområde**: ett område som skapar gemensamma förutsättningar, exempelvis plattformar, riktlinjer, gemensamma tjänster eller arkitekturstöd.

Båda typerna av områden behövs. Problemet uppstår när de arbetar som om de vore oberoende av varandra.

## Huvudförklaring

### Decentralisering ger fart, men kräver tydligare samspel

Decentralisering innebär att beslut flyttas närmare den plats där kunskap, behov och leveransansvar finns. För arkitekturarbetet innebär det att många frågor kan lösas snabbare än i en hårt centraliserad modell. Team och områden behöver inte vänta på att varje detalj ska godkännas långt från verksamheten.

Men decentralisering betyder inte att varje område bör optimera enbart för sig självt. En myndighet har ofta gemensamma informationsmängder, säkerhetskrav, tekniska plattformar, integrationsmönster och förvaltningsansvar. När ett område fattar beslut som påverkar dessa delar blir beslutet inte längre bara lokalt.

Arkitektens uppgift är därför inte att centralisera alla beslut igen. Uppgiften är att hjälpa organisationen att se vilka beslut som kan fattas lokalt och vilka som behöver samordnas.

En användbar tumregel är:

> Ju mer ett beslut påverkar andra områden, gemensamma förmågor eller långsiktig hållbarhet, desto tidigare bör arkitekten söka samordning och kvalitetssäkring.

### Operativa utvecklingsområden behöver ägarskap

Ett operativt utvecklingsområde behöver kunna ta ansvar för sin leverans. Det innebär att området behöver förstå användarbehov, prioritera förändringar, analysera lösningsalternativ och fatta många praktiska beslut.

För arkitekten i ett operativt område innebär vardagen ofta att vara nära teamens arbete. Arkitekten behöver förstå vad som faktiskt byggs, vilka avvägningar teamet gör och vilka begränsningar som finns. Arkitekten behöver också kunna översätta verksamhetens behov till arkitekturella frågor:

- Vilken information hanteras?
- Vilka andra system påverkas?
- Vilka integrationer behövs?
- Finns gemensamma komponenter eller tjänster som bör användas?
- Vilka säkerhets- eller förvaltningskrav följer med lösningen?
- Är lösningen hållbar över tid eller bara snabb för stunden?

Det operativa perspektivet är viktigt eftersom arkitektur annars riskerar att bli abstrakt. En arkitekt som inte förstår den lokala kontexten kan ge råd som är principiellt rimliga men svåra att använda.

### Stödjande områden behöver förstå den operativa verkligheten

Stödjande och förutsättningsskapande utvecklingsområden har en annan tyngdpunkt. De ska skapa förutsättningar som gör det lättare för de operativa områdena att utveckla IT effektivt och konsekvent. Det kan handla om gemensamma plattformar, standardiserade integrationsmönster, vägledningar, återanvändbara tjänster, säkerhetsstöd eller arkitekturprinciper.

Risken för stödjande områden är att de uppfattas som avlägsna från vardagen. Om deras riktlinjer, plattformar eller beslut inte svarar mot operativa behov kan de upplevas som hinder. Då kan operativa områden börja skapa egna lösningar vid sidan av de gemensamma, vilket ökar komplexitet och teknisk skuld.

Arkitekter i stödjande områden behöver därför arbeta nära de operativa. De behöver inte bara formulera vad som bör gälla, utan också förstå varför operativa områden ibland väljer andra vägar. En avvikelse kan bero på bristande följsamhet, men den kan också avslöja att den gemensamma förutsättningen inte är tillräckligt användbar.

### Arkitektens vardag är ofta ett gränsarbete

I en decentraliserad myndighet arbetar arkitekten ofta i gränsen mellan flera perspektiv:

- lokal leverans och gemensam riktning
- snabb utveckling och långsiktig hållbarhet
- verksamhetsbehov och tekniska förutsättningar
- teamets självständighet och myndighetens helhetsansvar
- principer och praktiska undantag

Detta gränsarbete kräver mer än teknisk kunskap. Arkitekten behöver kunna ställa rätt frågor, skapa förtroende, synliggöra konsekvenser och hjälpa olika parter att hitta beslut som fungerar. Ofta är det viktigaste arkitekturarbetet inte att presentera en färdig lösning, utan att göra ett otydligt problem möjligt att prata om.

### Mandat behöver vara tydligt men inte tungt

En vanlig svårighet i decentraliserade organisationer är otydligt mandat. Vem får besluta om vad? När är ett arkitekturbeslut lokalt? När behöver det lyftas? Vem äger en gemensam princip? Vem kan godkänna en avvikelse?

Om mandatet är otydligt kan två problem uppstå. Antingen fattas beslut lokalt utan tillräcklig samordning, eller så vågar ingen fatta beslut och arbetet tappar tempo. Båda problemen skadar arkitekturarbetet.

Arkitekten behöver därför bidra till att skapa praktisk tydlighet. Det betyder inte att alla beslut måste formaliseras tungt. Det betyder att det bör vara klart:

- vilka beslut teamet kan fatta själv
- vilka beslut som bör kvalitetssäkras inom området
- vilka beslut som behöver samordnas med andra områden
- vilka beslut som kräver gemensam arkitekturhantering eller särskilt forum
- hur avvikelser dokumenteras, motiveras och följs upp

När detta är tydligt blir styrning mindre personlig. Det handlar inte om att en viss arkitekt säger ja eller nej, utan om att organisationen har gemensamma spelregler för beslut som påverkar helheten.

## Scenario: Den nya digitala tjänsten möter den decentraliserade verkligheten

Det operativa utvecklingsområdet Kundmöte ska ta fram en ny digital tjänst för att medborgare enklare ska kunna följa status i ett ärende. Teamet har en tydlig verksamhetsnytta, en prioriterad backlogg och hög motivation. I ett tidigt lösningsmöte föreslår teamet att tjänsten ska lagra vissa statusuppgifter lokalt för att kunna visa information snabbt.

Den operativa arkitekten ser att detta kan fungera för den första versionen. Samtidigt väcker förslaget flera frågor:

- Är statusinformationen redan definierad i ett annat område?
- Finns det en gemensam informationsmodell?
- Vilket system är källa för informationen?
- Kan lokal lagring skapa avvikelser mellan olika tjänster?
- Finns en gemensam integrationslösning som bör användas?
- Behöver ett stödjande område involveras för plattforms- eller säkerhetsfrågor?

Arkitekten stoppar inte arbetet. I stället gör arkitekten två saker. Först hjälper hen teamet att formulera beslutet som ett arkitekturellt vägval: ska tjänsten läsa status direkt från källsystemet, via en gemensam tjänst eller via lokal lagring? Därefter kontaktar hen arkitekter i ett stödjande område som ansvarar för integrationsmönster och gemensamma informationsprinciper.

Resultatet blir inte ett långt granskningsärende. Det blir en kort samordningsdialog där teamet får veta att ett annat operativt område har ett liknande behov. Tillsammans kan områdena återanvända ett gemensamt integrationsmönster och undvika att två lokala lösningar skapas parallellt.

Det viktiga i scenariot är inte att arkitekten hittade ett perfekt svar direkt. Det viktiga är att arkitekten såg när ett lokalt beslut kunde få större konsekvenser och därför skapade samordning tidigt nog för att påverka lösningen.

## Vad arkitekten bör tänka på

### Börja i leveransens verklighet

Arkitektens råd blir bättre när de tar hänsyn till teamets mål, tidplan, beroenden och osäkerheter. En rekommendation som inte går att omsätta i teamets vardag riskerar att ignoreras, även om den är arkitekturellt korrekt.

Fråga därför först:

- Vad försöker teamet åstadkomma?
- Vilken nytta är viktigast?
- Vilka beslut är redan tagna?
- Vilka beslut är fortfarande öppna?
- Vad är osäkert?
- Vilka konsekvenser kan bli svåra att ändra senare?

### Skilj på lokala val och gemensamma vägval

Alla beslut behöver inte samordnas. Om arkitekten försöker lyfta för mycket skapas tröghet och irritation. Samordning bör fokusera på beslut som påverkar andra, riskerar dubbelarbete eller skapar långsiktiga bindningar.

Exempel på beslut som ofta kan vara lokala:

- mindre interna designval i en komponent
- val av arbetsfördelning inom teamet
- detaljer som enkelt kan ändras senare
- lösningar som inte påverkar gemensamma informationsflöden eller andra system

Exempel på beslut som ofta bör samordnas:

- nya integrationsmönster
- nya eller förändrade informationsägarskap
- användning av gemensamma plattformar
- avsteg från principer eller riktlinjer
- lösningar som flera områden kan behöva
- beslut som påverkar säkerhet, förvaltning eller långsiktig kostnad

### Gör beroenden synliga tidigt

Beroenden blir dyrare att hantera ju senare de upptäcks. Arkitekten bör därför aktivt leta efter beroenden redan när ett initiativ formas, inte först när lösningen är nästan färdig.

Ett beroende kan vara tekniskt, organisatoriskt eller informationsmässigt. Det kan handla om ett system, en plattform, ett API, en gemensam datadefinition, ett beslutande forum, en rättslig förutsättning eller ett annat utvecklingsområdes tidsplan.

När beroenden synliggörs tidigt kan de hanteras som en del av planeringen. När de upptäcks sent upplevs de ofta som hinder.

### Var tydlig med varför, inte bara vad

I organisationer där förståelsen för arkitekturarbete varierar behöver arkitekten ofta förklara varför en fråga är viktig. Det räcker sällan att säga att något “måste samordnas” eller “ska kvalitetssäkras”.

Förklara i stället konsekvensen:

- “Om vi lagrar den här informationen lokalt behöver vi säkerställa hur den hålls synkroniserad.”
- “Om vi skapar ett eget API här kan ett annat område behöva lösa samma problem igen.”
- “Om vi gör avsteg från det gemensamma mönstret behöver vi veta om det är ett tillfälligt undantag eller ett tecken på att mönstret behöver utvecklas.”
- “Om beslutet påverkar informationsansvar behöver rätt parter vara med innan lösningen låses.”

När arkitekten förklarar varför blir styrning lättare att acceptera.

## När kvalitetssäkring bör ske

Kvalitetssäkring i en decentraliserad organisation bör ske tidigt, stegvis och nära besluten. Den bör inte vänta tills teamet redan byggt lösningen.

Kvalitetssäkring bör särskilt ske när:

- ett initiativ går från idé till konkret lösningsinriktning
- teamet väljer integrationsmönster, informationshantering eller teknisk plattform
- lösningen påverkar andra utvecklingsområden
- en gemensam princip, riktlinje eller målbild berörs
- teamet föreslår en lokal lösning på ett problem som kan vara gemensamt
- en avvikelse övervägs
- ett beslut blir svårt eller dyrt att ändra senare
- lösningen påverkar säkerhet, robusthet, förvaltningsbarhet eller långsiktig kostnad

Praktiskt kan kvalitetssäkring ske genom korta arkitekturdialoger, granskning av vägval, gemensam genomgång av risker eller deltagande i refinement och planering. Formen är mindre viktig än att rätt frågor ställs i rätt tid.

## När samordning bör ske

Samordning bör ske när ett lokalt beslut har eller kan få betydelse utanför det egna teamet eller området.

Samordning bör särskilt initieras när:

- flera områden arbetar med liknande behov
- ett område behöver använda en gemensam plattform eller tjänst
- lösningen kräver integration med system som ägs av andra
- informationsdefinitioner, begrepp eller datakällor behöver vara gemensamma
- ett operativt behov visar att en stödjande förutsättning saknas eller inte fungerar
- det finns risk för dubbelarbete
- ett beslut kan påverka framtida arkitekturriktning
- olika områden tolkar en princip eller riktlinje på olika sätt

Samordning behöver inte alltid vara ett stort forum. Ofta räcker det med att rätt arkitekter pratar tidigt, dokumenterar slutsatsen och gör det tydligt vem som gör vad.

## Vanliga fallgropar

- **Fallgrop: Arkitekten väntar på att bli inbjuden**
  - **Varför det händer:** Arkitektens roll är otydlig eller teamet ser arkitektur som en sen granskning.
  - **Hur man undviker det:** Följ initiativ tidigt, delta i planering och erbjud konkreta frågor snarare än abstrakta krav.

- **Fallgrop: Allt behandlas som en samordningsfråga**
  - **Varför det händer:** Arkitekten vill undvika risker men skiljer inte på lokala och gemensamma beslut.
  - **Hur man undviker det:** Samordna främst beslut som påverkar andra, skapar beroenden eller får långsiktiga konsekvenser.

- **Fallgrop: Stödjande områden uppfattas som kontrollinstanser**
  - **Varför det händer:** Dialogen sker sent eller uttrycks som krav utan tydlig nytta.
  - **Hur man undviker det:** Förankra stödjande förutsättningar i operativa behov och var tydlig med vilket problem de hjälper till att lösa.

- **Fallgrop: Operativa områden skapar lokala lösningar för gemensamma problem**
  - **Varför det händer:** Gemensamma lösningar saknas, är svåra att använda eller är okända.
  - **Hur man undviker det:** Fånga återkommande behov, lyft dem till stödjande områden och dokumentera om avvikelsen är tillfällig eller visar ett större gap.

- **Fallgrop: Mandat blir personberoende**
  - **Varför det händer:** Det är oklart vilka beslut som hör hemma var.
  - **Hur man undviker det:** Etablera enkla beslutsregler och tydliggör när team, område, stödjande funktion eller gemensamt forum behöver involveras.

## Praktiskt arbetssätt för arkitekten

Ett enkelt arbetssätt i vardagen är att använda fem återkommande frågor:

1. **Vad är det lokala behovet?**  
   Förstå varför initiativet finns och vilken nytta det ska skapa.
2. **Vilka beslut är arkitekturellt betydelsefulla?**  
   Identifiera vägval som påverkar struktur, information, integrationer, säkerhet, förvaltning eller andra områden.
3. **Vem påverkas utanför teamet?**  
   Leta efter beroenden till andra operativa områden, stödjande områden eller gemensamma förmågor.
4. **Vad behöver kvalitetssäkras nu?**  
   Fokusera på de frågor som kan bli dyra att ändra senare.
5. **Vilken samordning är tillräcklig?**  
   Välj den lättaste form som ger rätt gemensam förståelse: kort dialog, dokumenterat beslut, gemensam genomgång eller formellt forum.

Det här arbetssättet hjälper arkitekten att vara både praktisk och proportionerlig. Målet är inte maximal kontroll, utan rätt nivå av gemensam styrning.

## Snabb sammanfattning

- Decentralisering ger närhet till verksamheten och högre handlingskraft, men kräver tydligt samspel.
- Operativa utvecklingsområden behöver ägarskap över sin leverans.
- Stödjande/förutsättningsskapande områden behöver skapa användbara gemensamma förutsättningar.
- Arkitektens vardag handlar ofta om att balansera lokal frihet med gemensam riktning.
- Kvalitetssäkring bör ske tidigt och stegvis, nära viktiga vägval.
- Samordning bör ske när beslut påverkar andra områden, gemensamma förmågor eller långsiktig hållbarhet.
- Arkitekten behöver förklara varför en fråga är viktig, inte bara att den ska hanteras.

## Reflektionsfrågor

1. Vilka typer av beslut i ditt utvecklingsområde kan fattas lokalt utan större samordning?
2. Vilka beslut brukar få konsekvenser för andra områden?
3. När upptäcks beroenden i dag: tidigt i planeringen eller sent i genomförandet?
4. Finns det situationer där stödjande områden uppfattas som kontrollinstanser snarare än möjliggörare?
5. Vilken enkel samordningsform skulle kunna förebygga mest dubbelarbete i din vardag?

## Nästa steg

Nästa kapitel går djupare in i varför styrning behövs även i agil utveckling. Där utvecklas skillnaden mellan möjliggörande styrning och detaljkontroll, och hur arkitekten kan bidra med ramar som hjälper teamen att fatta bättre beslut utan att ta ifrån dem ansvar.
