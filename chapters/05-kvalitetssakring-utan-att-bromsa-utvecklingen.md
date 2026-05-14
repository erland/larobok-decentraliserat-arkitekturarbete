# Kapitel 5: Kvalitetssäkring utan att bromsa utvecklingen

## Varför detta kapitel finns

Kvalitetssäkring uppfattas lätt som något som sker sent: en granskning, ett godkännande eller en kontroll innan en lösning får gå vidare. I en agil och decentraliserad organisation blir det ofta problematiskt. När återkoppling kommer sent har teamet redan hunnit göra många antaganden, bygga lösningsdelar och planera leveranser. Då kan kvalitetssäkring upplevas som ett stopp, även när återkopplingen är relevant.

För arkitekten är en viktig uppgift därför att flytta kvalitetssäkringen tidigare och göra den mer stegvis. Kvalitetssäkring ska hjälpa team och utvecklingsområden att fatta bättre beslut medan besluten fortfarande är möjliga att påverka.

Det här kapitlet handlar om hur kvalitetssäkring kan bli en naturlig del av arkitektens vardag: genom frågor, dialog, kriterier, riskbedömning och tidig återkoppling snarare än sen kontroll.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara varför kvalitetssäkring behöver ske tidigt och stegvis
- skilja mellan kvalitetssäkring som kontroll och kvalitetssäkring som stöd
- identifiera när ett lösningsförslag behöver arkitekturgranskning
- använda kvalitetskriterier för att föra en saklig dialog om lösningsval
- ge återkoppling på ett sätt som stärker teamets handlingsförmåga

## Innan vi börjar

Tidigare kapitel har etablerat att arkitekturarbete handlar om riktning, sammanhang och kvalitet. Vi har också beskrivit hur decentraliserad styrning kräver balans mellan lokal handlingskraft och gemensamma ramar, och hur samordning hjälper organisationen att upptäcka beroenden i tid.

Kvalitetssäkring är nästa steg. När beroenden, risker och viktiga vägval har blivit synliga behöver arkitekten hjälpa organisationen att bedöma om lösningen håller tillräcklig kvalitet. Det handlar inte om att hitta fel i efterhand, utan om att skapa bättre förutsättningar innan vägvalen låser sig.

## Huvudförklaring

### Kvalitetssäkring är inte samma sak som godkännande

I många organisationer blandas kvalitetssäkring ihop med godkännande. Det gör att arkitekturgranskning lätt blir en sen passagepunkt: teamet presenterar en lösning, någon bedömer den och utfallet blir godkänt, godkänt med villkor eller inte godkänt.

Den typen av beslut kan ibland behövas, särskilt när en lösning påverkar säkerhet, gemensamma plattformar, informationsansvar eller långsiktiga kostnader. Men om kvalitetssäkring bara sker som godkännande kommer den ofta för sent.

Kvalitetssäkring bör i stället ses som en kedja av återkopplingstillfällen. Arkitekten hjälper teamet att pröva antaganden, se konsekvenser och förstå vilka kvaliteter som är viktiga i sammanhanget. Ibland leder det till ett formellt beslut. Ofta leder det till bättre frågor, tydligare avvägningar och ett mer genomtänkt lösningsförslag.

### Kvalitet måste vara konkret

Alla vill ha hög kvalitet, men ordet kvalitet betyder olika saker beroende på sammanhang. För ett team kan kvalitet handla om snabb leverans och fungerande kod. För ett stödjande utvecklingsområde kan kvalitet handla om återanvändbarhet, säkerhet, driftbarhet och följsamhet till gemensamma förutsättningar. För verksamheten kan kvalitet handla om nytta, enkelhet och tillförlitlighet.

Arkitektens uppgift är inte att ersätta dessa perspektiv, utan att göra dem begripliga tillsammans. Det kräver kvalitetskriterier.

Ett kvalitetskriterium är en konkret fråga eller bedömningspunkt som hjälper organisationen att avgöra om lösningen är tillräckligt genomtänkt. Exempel:

- Är ansvar för information tydligt?
- Bygger lösningen på befintliga gemensamma förutsättningar där det är rimligt?
- Finns beroenden till andra utvecklingsområden identifierade?
- Är säkerhets- och behörighetsfrågor hanterade på rätt nivå?
- Är lösningen möjlig att förvalta och vidareutveckla?
- Är avvikelser från gemensamma principer motiverade?
- Går beslutet att ändra senare, eller låser det organisationen under lång tid?

Kriterierna ska inte användas som en mekanisk checklista där allt måste vara perfekt. De ska hjälpa arkitekten och teamet att prata om rätt saker vid rätt tidpunkt.

### Tidig återkoppling minskar friktion

När arkitekten ger återkoppling tidigt är det oftast lättare för teamet att ta emot den. Ett förslag som ännu är under formning kan ändras utan stor kostnad. Ett färdigbyggt förslag är däremot förknippat med investerad tid, planering, prestige och beroenden.

Tidig återkoppling kan ske på flera nivåer:

- vid idé eller behovsformulering
- när teamet börjar se möjliga lösningsvägar
- när ett mer konkret lösningsförslag växer fram
- inför beslut som påverkar andra utvecklingsområden
- inför avsteg från principer eller gemensamma förutsättningar
- inför större investeringar, upphandlingar eller teknikval

Det viktiga är att återkopplingen kommer medan frågan fortfarande är öppen. Arkitekten bör därför söka sig till de tidiga samtalen, inte bara vänta på färdiga underlag.

### Arkitekturgranskning bör vara proportionerlig

Allt behöver inte granskas lika mycket. Om varje liten fråga kräver samma formella hantering kommer kvalitetssäkring att uppfattas som administration. Om stora vägval däremot inte granskas alls ökar risken för lokala lösningar, teknisk skuld och otydliga beroenden.

En proportionerlig arkitekturgranskning anpassas efter påverkan, risk och reversibilitet.

En lätt granskning kan räcka när:

- frågan är lokal
- beslutet är enkelt att ändra senare
- lösningen följer etablerade principer
- inga större beroenden finns
- påverkan på information, säkerhet och gemensamma förutsättningar är låg

En mer strukturerad granskning behövs ofta när:

- lösningen påverkar flera utvecklingsområden
- samma förmåga kan behövas av fler
- informationsansvar eller informationsflöden förändras
- säkerhet, behörighet eller spårbarhet påverkas
- lösningen innebär avsteg från gemensam riktning
- beslutet är dyrt eller svårt att ändra
- en lokal lösning riskerar att bli permanent standard

Arkitektens uppgift är att göra nivån på granskningen begriplig. Teamet bör förstå varför en fråga behöver mer dialog, inte bara att den behöver det.

### Återkoppling ska vara användbar

Kvalitetssäkring får störst effekt när återkopplingen går att agera på. Kommentarer som ”lösningen bör bli mer robust” eller ”det här verkar inte följa målbilden” kan vara korrekta men ändå svåra att använda.

Bra arkitekturell återkoppling bör vara:

- konkret: vad behöver förändras eller undersökas?
- motiverad: varför spelar det roll?
- prioriterad: vad är viktigast nu?
- proportionerlig: hur mycket behöver hanteras i detta skede?
- handlingsbar: vad är ett rimligt nästa steg?
- kopplad till konsekvens: vad händer om frågan lämnas olöst?

En arkitekt bör därför inte bara säga vad som är fel. Arkitekten bör hjälpa teamet att förstå vilken risk eller konsekvens som ligger bakom återkopplingen och vilka handlingsalternativ som finns.

## Scenario

Det operativa utvecklingsområdet arbetar vidare med den nya digitala tjänsten. Teamet har tagit fram ett lösningsförslag och vill få det arkitekturgranskat inför nästa planeringsperiod. Förslaget innehåller en ny integration, ett lokalt sätt att lagra viss verksamhetsinformation och en lösning för behörighetsstyrning som teamet bedömer som snabb att införa.

Arkitekten ser flera frågor:

- Integrationen liknar en lösning som ett annat utvecklingsområde redan arbetar med.
- Informationen som ska lagras används även i andra ärenden.
- Behörighetslösningen fungerar för den första versionen men kan bli svår att förvalta när fler användargrupper tillkommer.
- Teamet har inte beskrivit vilka delar som är tillfälliga och vilka som är tänkta som långsiktiga.

Om granskningen sker först nu, nära planering, finns risk att återkopplingen upplevs som ett stopp. Arkitekten väljer därför att dela upp kvalitetssäkringen i tre steg:

1. En snabb dialog med teamet om lösningens viktigaste antaganden.
2. En samordning med det stödjande utvecklingsområdet som ansvarar för gemensamma integrationsmönster och behörighetsförutsättningar.
3. En kort arkitekturbedömning som tydliggör vad som kan gå vidare nu, vad som behöver justeras och vad som behöver följas upp.

På så sätt blir kvalitetssäkringen inte bara ett ja eller nej. Den hjälper teamet att behålla tempo, samtidigt som risker och beroenden hanteras innan lösningen blir för låst.

## Vad arkitekten bör tänka på

### Börja med beslutet, inte dokumentet

Fråga först: vilket beslut är teamet på väg att fatta? Därefter: vilket underlag behövs för att beslutet ska bli tillräckligt bra?

Det är lätt att börja i mallar, dokument och granskningsformat. Men kvalitetssäkring blir mer relevant när den utgår från beslutets betydelse. Ett litet reversibelt beslut kräver inte samma underlag som ett vägval som påverkar flera utvecklingsområden under flera år.

### Bedöm konsekvens, inte bara följsamhet

Det är viktigt att lösningar följer principer, riktlinjer och gemensamma förutsättningar. Men arkitekten bör inte stanna vid frågan om följsamhet. Den viktigare frågan är vilken konsekvens ett vägval får.

En lösning kan följa en princip men ändå vara olämplig i ett visst sammanhang. En annan lösning kan avvika från en princip men vara rimlig som medvetet, tidsbegränsat avsteg. Därför behöver kvalitetssäkring handla om avvägningar, risker och konsekvenser.

### Skilj på blockerande frågor och förbättringsförslag

All återkoppling är inte lika viktig. Vissa frågor behöver lösas innan teamet går vidare. Andra kan hanteras senare, följas upp eller noteras som förbättringar.

Arkitekten bör vara tydlig med skillnaden:

- Vad måste hanteras nu?
- Vad bör hanteras innan nästa större beslut?
- Vad kan följas upp senare?
- Vad är bara ett möjligt förbättringsförslag?

Den tydligheten minskar friktion och gör kvalitetssäkringen mer användbar.

### Gör kvalitetssäkring lärande

Varje granskning är också ett tillfälle att höja organisationens arkitekturmognad. Om samma frågor återkommer i flera team kan det vara ett tecken på att stöd, principer eller gemensamma förutsättningar behöver förbättras.

Arkitekten bör därför inte bara fråga vad som är fel i lösningen, utan också vad organisationen kan lära av återkopplingen.

## När kvalitetssäkring bör ske

Kvalitetssäkring bör ske när ett beslut kan få arkitekturella konsekvenser. Den behöver inte alltid vara formell, men den bör vara medveten.

### Tidigt i behovs- och idéfasen

Kvalitetssäkra tidigt när initiativet kan påverka flera system, informationsflöden eller utvecklingsområden. I detta skede räcker det ofta med frågor:

- Vilka förmågor påverkas?
- Finns liknande behov någon annanstans?
- Vilken information berörs?
- Finns gemensamma förutsättningar som bör användas?
- Vilka beslut riskerar att bli svåra att ändra senare?

### Vid lösningsinriktning

När teamet börjar välja lösningsväg bör arkitekten hjälpa till att pröva alternativen. Fokus bör ligga på konsekvenser, beroenden och risker, inte på detaljer.

Här passar lättviktig arkitekturgranskning, till exempel ett strukturerat samtal eller en kort bedömning av lösningsalternativ.

### Inför större eller svårändrade beslut

Mer strukturerad kvalitetssäkring behövs när beslutet påverkar säkerhet, information, integrationer, plattformar, kostnad, förvaltning eller gemensam riktning.

Det gäller särskilt beslut som:

- är dyra att ändra
- skapar nya beroenden
- påverkar flera utvecklingsområden
- innebär ny teknik eller ny lösningsmodell
- riskerar att bli normbildande
- innebär avsteg från principer eller målarkitektur

### När återkommande mönster syns

Kvalitetssäkring bör också ske när arkitekten ser att flera team gör liknande val. Då handlar det inte bara om ett enskilt initiativ, utan om ett möjligt organisatoriskt mönster.

Frågan blir då: behöver organisationen en gemensam förutsättning, tydligare princip, bättre vägledning eller ett forum för samordning?

## När samordning bör ske

Kvalitetssäkring och samordning hänger ofta ihop. En granskning visar vad som behöver bedömas. Samordning visar vilka som behöver vara med i bedömningen.

Samordning bör ske när kvalitetssäkringen visar att:

- lösningen påverkar andra utvecklingsområden
- det finns gemensamma informationsmängder eller informationsansvar
- samma förmåga utvecklas på flera håll
- teamet behöver stöd från ett förutsättningsskapande område
- ett lokalt vägval kan påverka gemensamma plattformar eller tjänster
- ett avsteg kan bli prejudicerande
- beslutet kräver gemensam riktning snarare än lokal optimering

Arkitekten behöver inte samordna allt själv. Ibland räcker det att koppla ihop rätt personer, formulera frågan tydligt och säkerställa att beslutet dokumenteras eller följs upp.

## Vanliga fallgropar

- **Fallgrop: Kvalitetssäkring sker för sent**
  - **Varför det händer:** Teamet söker granskning först när lösningen är färdigformulerad.
  - **Hur man undviker det:** Skapa tidiga återkopplingstillfällen vid idé, inriktning och större vägval.

- **Fallgrop: Granskningen blir för omfattande för frågans storlek**
  - **Varför det händer:** Samma granskningsform används för både små och stora beslut.
  - **Hur man undviker det:** Anpassa formen efter påverkan, risk och reversibilitet.

- **Fallgrop: Återkopplingen blir abstrakt**
  - **Varför det händer:** Arkitekten beskriver principer men inte konsekvenser eller nästa steg.
  - **Hur man undviker det:** Koppla varje viktig synpunkt till risk, konsekvens och handlingsalternativ.

- **Fallgrop: Kvalitetssäkring blir personlig**
  - **Varför det händer:** Återkoppling ges som kritik av teamets lösning snarare än som stöd för beslutet.
  - **Hur man undviker det:** Fokusera på gemensamma kriterier, konsekvenser och vad organisationen behöver uppnå.

- **Fallgrop: All återkoppling behandlas som lika viktig**
  - **Varför det händer:** Granskningsresultat saknar prioritering.
  - **Hur man undviker det:** Skilj tydligt mellan måste, bör, kan vänta och förbättringsförslag.

## Snabb sammanfattning

- Kvalitetssäkring bör vara tidig, stegvis och proportionerlig.
- Syftet är att hjälpa team att fatta bättre beslut, inte att stoppa utveckling.
- Kvalitet behöver göras konkret genom kriterier, frågor och konsekvensbedömning.
- Arkitekturgranskning bör anpassas efter beslutets påverkan, risk och reversibilitet.
- Återkoppling ska vara tydlig, motiverad, prioriterad och handlingsbar.
- Kvalitetssäkring och samordning hänger ihop när en lösning påverkar fler än det egna teamet.

## Reflektionsfrågor

1. Vilka typer av beslut i din organisation granskas ofta för sent?
2. Vilka kvalitetskriterier skulle hjälpa dina team att få tidigare och bättre återkoppling?
3. När blir kvalitetssäkring ett stöd, och när riskerar den att uppfattas som kontroll?
4. Hur kan du skilja tydligare mellan blockerande frågor och förbättringsförslag?
5. Vilka återkommande granskningsfrågor visar att organisationen behöver bättre gemensamma förutsättningar?

## Nästa steg

Nästa kapitel handlar om arkitekturprinciper i praktiken. Där fördjupar vi hur principer kan användas som beslutsstöd i vardagen, hur de bör vägas mot varandra och hur arkitekten kan hantera avsteg utan att tappa gemensam riktning.
