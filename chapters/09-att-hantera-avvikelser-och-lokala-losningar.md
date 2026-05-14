# Kapitel 9: Att hantera avvikelser och lokala lösningar

## Varför detta kapitel finns

I en decentraliserad organisation kommer avvikelser att uppstå. Operativa utvecklingsområden möter konkreta verksamhetsbehov, tidspress, tekniska begränsningar och ibland krav som inte passar perfekt med gemensamma principer, riktlinjer eller målarkitektur. Det är inte i sig ett misslyckande. Problemet uppstår när avvikelser blir osynliga, omotiverade eller permanenta utan att någon har förstått konsekvenserna.

Detta kapitel handlar om hur arkitekten kan hantera avvikelser och lokala lösningar på ett sätt som bevarar både handlingskraft och helhet. Syftet är inte att stoppa alla avsteg. Syftet är att göra avsteg medvetna, proportionerliga och möjliga att följa upp.

En mogen arkitekturorganisation behöver kunna säga både ja, nej och ja, men. Det viktiga är att svaret grundas i risk, konsekvens, livslängd och påverkan på andra.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- skilja mellan en rimlig lokal anpassning och en riskabel avvikelse
- förklara varför avvikelser behöver motiveras, riskbedömas och följas upp
- använda riskacceptans som ett medvetet beslut, inte som en tyst konsekvens
- identifiera när kompensatoriska åtgärder behövs
- avgöra när kvalitetssäkring och samordning bör initieras vid lokala lösningar

## Innan vi börjar

Tidigare kapitel har visat hur arkitekturprinciper, arkitekturbeslut, spårbarhet och samverkan mellan operativa och stödjande utvecklingsområden bidrar till helhet och kvalitet. I detta kapitel används dessa delar när ett team vill göra något som inte fullt ut följer gemensam riktning.

En avvikelse är nära kopplad till ett arkitekturbeslut. Skillnaden är att beslutet innebär ett medvetet vägval, medan avvikelsen innebär att vägvalet går utanför en etablerad princip, riktlinje, målarkitektur eller gemensam lösning.

## Huvudförklaring

### Alla lokala lösningar är inte problem

En lokal lösning kan vara helt rimlig. Ett operativt utvecklingsområde kan behöva en anpassning för att möta ett specifikt verksamhetsflöde, en lokal användargrupp eller ett särskilt regelkrav. Lokal anpassning är ofta en styrka i en decentraliserad organisation.

Problemet uppstår när en lokal lösning får konsekvenser som inte längre är lokala. Det kan handla om att lösningen använder information på ett annat sätt än andra områden, skapar nya integrationer, bygger upp ett parallellt tekniskt mönster, försvårar framtida förvaltning eller gör att en gemensam tjänst inte längre används.

Arkitektens första fråga bör därför inte vara: Följer detta modellen? En bättre första fråga är: Vilka konsekvenser får detta, och för vem?

### Avvikelse som medvetet vägval

En avvikelse bör beskrivas som ett medvetet avsteg från en gemensam riktning. Det betyder att avvikelsen behöver ha en tydlig motivering. Motiveringen bör inte bara säga att teamet har bråttom eller att den gemensamma lösningen inte passar. Den bör förklara vad som behöver uppnås, vilka alternativ som har övervägts och varför avsteget bedöms vara rimligt.

En avvikelse behöver också ha en bedömning av risk. Risk betyder här inte bara säkerhetsrisk. Det kan även handla om förvaltningsrisk, kostnadsrisk, informationsrisk, integrationsrisk, kompetensrisk eller risk för att lösningen kopieras av andra utan att förutsättningarna är desamma.

Avvikelsen bör dessutom ha en livslängd. Är den tillfällig tills en gemensam tjänst är förbättrad? Är den en lokal anpassning som ska få leva länge? Är den ett experiment som ska utvärderas? Utan livslängd blir tillfälliga lösningar lätt permanenta.

### Riskacceptans är ett beslut

I många organisationer sker riskacceptans utan att någon säger det. Teamet går vidare, arkitekten hinner inte granska, ett forum informeras sent och lösningen hamnar i produktion. Då har organisationen i praktiken accepterat risken, men utan att dokumentera vem som tog ställning, på vilka grunder eller hur risken ska följas upp.

Det är svagt arkitekturarbete.

Riskacceptans bör vara ett tydligt beslut. Någon med rätt mandat behöver förstå konsekvensen och acceptera den. Arkitektens roll är inte alltid att äga beslutet, men arkitekten bör hjälpa beslutsfattare att förstå vad de accepterar.

En enkel formulering kan vara:

> Vi accepterar denna avvikelse under dessa förutsättningar, med dessa risker, fram till denna uppföljningspunkt.

Det gör beslutet synligt och möjligt att ompröva.

### Kompensatoriska åtgärder

Ibland är en avvikelse rimlig, men bara om något annat görs för att minska risken. Det kallas här kompensatorisk åtgärd. Det är en åtgärd som inte tar bort avvikelsen, men gör den mer kontrollerad.

Exempel på kompensatoriska åtgärder kan vara:

- extra uppföljning efter första leverans
- tydlig dokumentation av avvikelsen och dess livslängd
- begränsning av vilka användare eller flöden lösningen gäller för
- krav på att lösningen inte återanvänds av andra utan ny prövning
- plan för migrering till gemensam tjänst när den finns
- kompletterande säkerhets- eller informationsgranskning
- ansvarig person eller roll som följer upp avvikelsen

Kompensatoriska åtgärder gör störst nytta när de är konkreta. En formulering som “hanteras i förvaltning” är sällan tillräcklig. Det bör framgå vad som ska göras, av vem och när.

### När ett avsteg visar något viktigt

Återkommande avvikelser kan vara ett tecken på att den gemensamma riktningen är otydlig, för stel eller otillräckligt användbar. Om flera operativa utvecklingsområden gör liknande avsteg bör arkitekten inte bara försöka få dem att följa principen bättre. Arkitekten bör också fråga om principen, riktlinjen eller den gemensamma tjänsten behöver utvecklas.

På så sätt blir avvikelser en källa till lärande. De visar var den gemensamma modellen möter praktiska behov. De kan peka på luckor i förutsättningsskapande arbete, bristande kommunikation eller behov av nya gemensamma förmågor.

En avvikelse är därför inte bara ett undantag. Den kan också vara en signal.

## Scenario

Det operativa utvecklingsområdet arbetar med den nya digitala tjänsten. Teamet behöver lösa ett verksamhetskritiskt behov före nästa större leverans. Den rekommenderade gemensamma tjänsten för ärendeavisering stödjer inte ett specifikt flöde som verksamheten anser nödvändigt.

Teamet föreslår därför en lokal lösning. Den är snabbare att införa och passar det aktuella behovet, men den innebär att området bygger en parallell aviseringsfunktion.

Den operativa arkitekten ser nyttan, men också risken. Om lösningen permanentas kan den skapa dubbel funktionalitet, egen förvaltning och otydlighet om vilken aviseringstjänst andra områden bör använda. Den stödjande arkitekten ser samtidigt att behovet kanske inte är unikt. Fler områden kan komma att behöva liknande funktionalitet.

I stället för att direkt stoppa lösningen genomför arkitekterna en kort avvikelseprövning:

- Vilket behov måste lösas nu?
- Vilken gemensam princip eller riktlinje avviker lösningen från?
- Vilka alternativ finns?
- Är avvikelsen tillfällig eller långsiktig?
- Vilka risker uppstår?
- Vem accepterar risken?
- Vilka kompensatoriska åtgärder krävs?
- När ska beslutet följas upp?

Resultatet blir ett tidsbegränsat avsteg. Teamet får använda den lokala lösningen för ett avgränsat flöde. Samtidigt dokumenteras att lösningen inte får spridas vidare utan ny prövning. Det stödjande området tar med behovet i vidareutvecklingen av den gemensamma aviseringstjänsten. En uppföljningspunkt sätts efter första produktionssättningen.

Det viktiga är inte att avvikelsen försvinner direkt. Det viktiga är att den blir synlig, motiverad, avgränsad och möjlig att lära av.

## Vad arkitekten bör tänka på

### Börja med behovet

Avvikelsehantering blir lätt defensiv om samtalet börjar med regler. Börja i stället med behovet. Vad behöver verksamheten uppnå? Varför räcker inte den gemensamma lösningen? Vilken tidspress, risk eller begränsning finns?

När behovet är begripligt blir det lättare att bedöma avvikelsen sakligt.

### Skilj på avvikelse, förbättringsförslag och lokal variation

Allt som skiljer sig från ett standardmönster är inte en avvikelse. Ibland är det en legitim lokal variation. Ibland är det ett förbättringsförslag till en gemensam tjänst. Ibland är det en verklig avvikelse som behöver riskacceptans.

Arkitekten bör hjälpa organisationen att sortera frågan rätt. Fel sortering skapar antingen onödig byråkrati eller för svag kontroll.

### Titta på spridningsrisken

En lokal lösning kan vara hanterbar så länge den är just lokal. Risken ökar om den blir ett mönster andra kopierar, om den börjar användas som informell standard eller om den binder organisationen till ett nytt tekniskt spår.

Fråga därför: Vad händer om tre andra områden gör likadant?

### Gör avvikelsen tidsatt

Avvikelser utan slutpunkt tenderar att bli permanenta. Även om avvikelsen kan behöva leva länge bör det finnas en uppföljningspunkt. Uppföljning betyder inte automatiskt att lösningen ska avvecklas. Det betyder att organisationen aktivt tar ställning igen.

### Koppla tillbaka till gemensamt lärande

En avvikelse ska inte bara arkiveras. Den bör också kunna användas för att förbättra principer, riktlinjer, gemensamma tjänster eller arbetssätt. Annars riskerar organisationen att hantera samma typ av undantag om och om igen.

## När kvalitetssäkring bör ske

Kvalitetssäkring bör ske när en lokal lösning eller avvikelse:

- går emot en etablerad arkitekturprincip, riktlinje eller målarkitektur
- påverkar information, säkerhet, integrationer eller gemensamma tjänster
- riskerar att bli permanent trots att den beskrivs som tillfällig
- skapar ny teknisk eller organisatorisk förvaltning
- bygger på antaganden som ännu inte är verifierade
- kan påverka andra utvecklingsområdens lösningar eller vägval
- innebär att en gemensam tjänst väljs bort
- kräver att någon accepterar risk utanför teamets eget mandat

Kvalitetssäkringen bör vara proportionerlig. En mindre avvikelse kan räcka att hantera genom kort dokumentation och arkitekturdialog. En större avvikelse kan behöva strukturerad granskning, beslutslogg, riskacceptans och uppföljning i lämpligt forum.

## När samordning bör ske

Samordning bör ske när en avvikelse eller lokal lösning:

- berör ett stödjande eller förutsättningsskapande utvecklingsområde
- kan vara relevant för flera operativa utvecklingsområden
- påverkar gemensamma informationsflöden eller integrationsmönster
- skapar behov av förändring i en gemensam tjänst
- riskerar att leda till dubbelarbete
- kan bli ett informellt mönster som andra börjar följa
- kräver gemensam prioritering mellan lokal nytta och gemensam utveckling

Samordning behöver inte alltid betyda stort möte eller formellt forum. I tidiga skeden kan det räcka med en kort dialog mellan berörda arkitekter. Det viktiga är att rätt personer får möjlighet att förstå konsekvensen innan lösningen låses.

## Vanliga fallgropar

- **Fallgrop: Att behandla alla avvikelser som fel**

- **Fallgrop: Att acceptera avvikelser utan beslut**

- **Fallgrop: Att kalla permanenta lösningar tillfälliga**

- **Fallgrop: Att inte återföra lärdomar till gemensamma förutsättningar**

## Snabb sammanfattning

- Avvikelser är inte alltid fel, men de behöver vara medvetna.
- En lokal lösning blir arkitekturellt viktig när den påverkar andra, skapar ny förvaltning eller avviker från gemensam riktning.
- Riskacceptans bör vara ett tydligt beslut, inte en tyst konsekvens.
- Kompensatoriska åtgärder kan göra en avvikelse hanterbar.
- Avvikelser bör tidsättas, följas upp och användas som lärande.
- Kvalitetssäkring och samordning ska anpassas efter påverkan, risk och reversibilitet.

## Reflektionsfrågor

1. Vilka typer av avvikelser uppstår oftast i din organisation?
2. Hur synliggörs i dag vem som accepterar risk när ett avsteg görs?
3. Finns det avvikelser som återkommer så ofta att de egentligen pekar på brister i gemensamma förutsättningar?
4. Vilka avvikelser borde hanteras lättviktigt, och vilka borde få tydligare uppföljning?
5. Vad skulle göra det enklare för operativa och stödjande arkitekter att hantera avvikelser utan att skapa onödig friktion?

## Nästa steg

Nästa kapitel handlar om teknisk skuld och långsiktig hållbarhet. Där fördjupas frågan om vad som händer när kortsiktiga vägval, lokala lösningar och tillfälliga avsteg inte följs upp. Fokus flyttas från att hantera enskilda avvikelser till att förstå hur skuld byggs upp över tid och hur arkitekten kan göra den synlig.
