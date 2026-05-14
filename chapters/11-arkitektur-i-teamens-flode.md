# Kapitel 11: Arkitektur i teamens flöde

## Varför detta kapitel finns

Arkitekturfrågor skapar störst nytta när de kommer in tidigt i teamens ordinarie arbete. När de i stället dyker upp sent, till exempel inför en leverans, en granskning eller ett produktionssättningsbeslut, uppfattas arkitekturen lätt som ett hinder. Då blir arkitektens återkoppling svårare att ta emot, även när den är sakligt viktig.

I en agil omställning är detta en central utmaning. Teamen förväntas kunna leverera löpande, lära sig snabbt och fatta beslut nära verksamhetens behov. Samtidigt påverkar många beslut integrationer, informationsflöden, säkerhet, förvaltning, gemensamma tjänster och teknisk skuld. Arkitektens arbete behöver därför finnas i teamets flöde, inte vid sidan av det.

Detta kapitel handlar om hur arkitekturarbete kan kopplas till backlogg, refinement, planering, leverans och uppföljning. Fokus ligger på vad arkitekten bör tänka på i vardagen för att arkitektur ska bli en del av arbetet, snarare än en separat kontrollpunkt.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara varför arkitekturfrågor bör hanteras i teamets ordinarie flöde
- beskriva vad kontinuerlig arkitektur innebär i praktiken
- identifiera arkitekturfrågor som behöver synliggöras i backloggen
- använda refinement och planering för tidig kvalitetssäkring och samordning
- avgöra när en fråga bör hanteras av teamet, samordnas med andra eller lyftas till ett gemensamt forum

## Innan vi börjar

Tidigare kapitel har visat att arkitekturbeslut, avvikelser och teknisk skuld behöver bli synliga, motiverade och möjliga att följa upp. Detta kapitel tar nästa steg: hur får arkitekten in dessa frågor i det dagliga utvecklingsarbetet?

Utgångspunkten är att arkitektur inte ska vara ett parallellt spår som teamet besöker ibland. Arkitektur är en del av hur lösningen formas. Därför behöver arkitekturella frågor finnas där arbetet redan planeras, prioriteras och genomförs.

## Huvudförklaring

### Kontinuerlig arkitektur

Kontinuerlig arkitektur innebär att arkitekturella frågor hanteras löpande, i takt med att lösningen växer fram. Det betyder inte att alla beslut ska fattas i förväg. Det betyder heller inte att arkitekten ska delta i varje detalj. Det betyder att frågor med arkitekturell konsekvens fångas upp tillräckligt tidigt för att teamet ska kunna agera utan onödiga omtag.

I praktiken handlar det om att arkitekten hjälper teamet att se vilka vägval som är små och reverserbara, och vilka som skapar långsiktiga konsekvenser. En lokal ändring i användargränssnittet kan ofta hanteras inom teamet. Ett nytt informationsflöde, en ny integration, ett avsteg från en gemensam tjänst eller ett beslut som påverkar säkerhet och förvaltning behöver däremot ofta kvalitetssäkras eller samordnas.

Kontinuerlig arkitektur kräver närvaro i arbetets rytm. Arkitekten behöver förstå var beslut uppstår: i idéfasen, i backloggen, vid refinement, vid planering, under implementation, vid test, vid driftsättning och vid uppföljning. Varje steg har olika möjligheter att påverka.

### Backloggen som arkitekturens synlighetsyta

Backloggen är inte bara en lista över funktioner. Den är också en plats där risker, beroenden, tekniska förutsättningar och arkitekturella behov kan göras synliga. Om arkitekturfrågor inte syns i backloggen riskerar de att bli osynligt arbete, personberoende diskussioner eller sena hinder.

En arkitekturell backlogg behöver inte vara en separat backlogg. Ofta är det bättre att arkitekturella frågor kopplas till teamets befintliga backlogg. Det kan handla om att skapa uppgifter för att utreda ett vägval, dokumentera ett arkitekturbeslut, verifiera en integrationsprincip, minska teknisk skuld eller samordna med ett stödjande utvecklingsområde.

Det viktiga är att arkitekturarbete blir planeringsbart. Om teamet behöver ta fram en lösningsskiss, jämföra två alternativ eller säkra att en gemensam tjänst kan användas, bör detta vara synligt som arbete. Annars behandlas arkitektur som något som ska ske vid sidan av leveransen, vilket ofta leder till stress, genvägar och svagare beslut.

### Refinement som tidig kvalitetssäkring

Refinement är ett av de viktigaste tillfällena för arkitekten att bidra. Det är där behov bryts ned, osäkerheter blir synliga och teamet börjar förstå vad som faktiskt krävs. Om arkitekturfrågor fångas här kan de hanteras innan lösningen är låst.

Arkitekten bör särskilt lyssna efter formuleringar som tyder på dolda vägval:

- ”Vi behöver bara koppla på ett nytt system.”
- ”Vi kan nog lösa det lokalt så länge.”
- ”Det här borde inte påverka någon annan.”
- ”Vi använder samma data, men på ett lite annat sätt.”
- ”Det stödjande området hinner nog inte hjälpa oss.”
- ”Vi dokumenterar beslutet senare.”

Sådana formuleringar betyder inte att teamet gör fel. De visar att det finns osäkerhet eller ett vägval som kan behöva förtydligas. Arkitektens roll är att hjälpa teamet ställa rätt frågor innan arbetet går för långt.

### Planering som samordningspunkt

Planering är ett naturligt tillfälle att bedöma om arbetet är tillräckligt moget för att starta. För arkitekten handlar det inte om att kräva fullständig design innan teamet får börja. Det handlar om att se till att teamet har hanterat de arkitekturella osäkerheter som kan skapa stora omtag.

En enkel planeringsfråga är: ”Vilka beslut i detta arbete kan påverka andra än oss själva?” Om svaret omfattar integrationer, information, gemensamma tjänster, säkerhetsmönster, plattformar, förvaltningsansvar eller avsteg från principer bör samordning planeras in.

Planering bör också synliggöra om ett arbete kräver stöd från ett annat utvecklingsområde. Om stödet kommer in först när teamet redan har byggt en lösning ökar risken för konflikt mellan lokal framdrift och gemensam kvalitet.

### Leverans är inte första arkitekturkontrollen

När arkitekturfrågor hanteras först inför leverans har organisationen ofta redan investerat tid, prestige och beroenden i en viss lösning. Då blir kvalitetssäkring lätt en fråga om att godkänna eller stoppa. Det är ett svagt läge för både teamet och arkitekten.

En bättre modell är att använda flera lätta avstämningar under arbetets gång. Det kan vara korta dialoger om lösningsinriktning, avstämning av arkitekturbeslut, genomgång av avvikelser eller kontroll av att beroenden är hanterade. Ju tidigare en fråga hanteras, desto mindre dramatisk behöver kvalitetssäkringen bli.

Målet är att teamet ska kunna leverera med större trygghet. Kvalitetssäkring blir då inte en extern grind, utan en del av hur teamet minskar risk.

## Scenario: Den sena arkitekturfrågan

Det operativa utvecklingsområdet arbetar vidare med den digitala tjänsten. Teamet har brutit ned arbetet i flera funktioner och planerar att leverera stegvis. I en user story står det att tjänsten ska hämta viss information från ett befintligt system.

Vid första anblicken ser det enkelt ut. Teamet bedömer att det bara behövs en ny integration. Arkitekten deltar inte i refinementet eftersom frågan uppfattas som teknisk implementation. Två sprintar senare visar det sig att informationen även används av ett annat operativt utvecklingsområde, att det finns oklarheter kring informationsansvar och att ett stödjande utvecklingsområde redan arbetar med en gemensam integrationslösning.

Teamet har nu byggt en lokal lösning som fungerar tekniskt, men som riskerar att bli svår att förvalta. Det stödjande området upplever att teamet gått före. Det andra operativa området är oroligt för att informationsflödet får dubbla tolkningar. Arkitekten får frågan sent och behöver hantera både sakfrågan och frustrationen.

En mer hållbar hantering hade varit att fånga integrationsfrågan i backloggen redan när behovet identifierades. Under refinement hade teamet kunnat markera frågan som arkitekturellt relevant. Planeringen hade då kunnat inkludera en kort samordning med informationsägare, det andra utvecklingsområdet och det stödjande området. Teamet hade fortfarande kunnat komma vidare, men med bättre förståelse för beroenden och gemensam riktning.

## Vad arkitekten bör tänka på

Arkitekten bör leta efter arkitekturella signaler i teamets ordinarie arbete. En signal är något som antyder att ett vägval kan påverka struktur, kvalitet, samordning eller långsiktig hållbarhet. Signalerna finns ofta i vardagliga formuleringar, inte i färdiga arkitekturdokument.

Särskilt viktiga signaler är när teamet:

- skapar eller ändrar integrationer
- använder information på ett nytt sätt
- avviker från en gemensam princip eller tjänst
- bygger något som kan behövas av flera utvecklingsområden
- väljer teknik med lång livslängd
- tar en genväg för att hinna leverera
- antar att ett beroende inte påverkar någon annan
- skjuter dokumentation eller beslut till senare

Arkitekten bör också vara noga med att inte göra allt till arkitekturfrågor. Om varje detalj lyfts till samordning tappar teamet tempo och förtroende. Den praktiska frågan är därför inte ”finns det någon arkitekturaspekt?”, utan ”är konsekvensen tillräckligt stor för att kräva särskild hantering?”.

## När kvalitetssäkring bör ske

Kvalitetssäkring bör ske i teamets flöde när ett arbete rör beslut som är svåra att ändra, påverkar flera parter eller kan skapa långsiktig skuld. Den bör helst ske i flera små steg:

1. När behovet identifieras: finns det arkitekturella konsekvenser?
2. Under refinement: är beroenden, ansvar och kvalitetskrav tillräckligt tydliga?
3. Vid lösningsinriktning: är valda mönster, principer och avsteg rimliga?
4. Under implementation: har nya insikter ändrat riskbilden?
5. Inför leverans: är beslut, avvikelser och kvarvarande skuld dokumenterade?
6. Efter leverans: vad behöver följas upp eller förbättras?

Kvalitetssäkring bör inte vänta tills allt är färdigbyggt. Då blir återkopplingen dyrare och svårare att omsätta.

## När samordning bör ske

Samordning bör ske när teamets arbete berör andra utvecklingsområden, gemensamma förutsättningar eller beslut som kan återkomma i flera sammanhang. Det gäller särskilt när arbetet påverkar:

- gemensamma tjänster eller plattformar
- informationsflöden och informationsansvar
- integrationer mellan system
- säkerhet, behörighet eller spårbarhet
- förvaltningsansvar och livscykel
- gemensamma principer, riktlinjer eller målarkitektur
- lösningar som kan återanvändas av andra

Samordning bör planeras som arbete, inte behandlas som ett möte som läggs ovanpå allt annat. Om samordning krävs bör det synas i backloggen och i teamets planering.

## Vanliga fallgropar

- **Fallgrop: Arkitektur hanteras som en slutgranskning**
  - **Varför det händer:** Teamet vill hålla tempo och arkitekturfrågor uppfattas som något externt.
  - **Hur man undviker det:** Lägg in arkitekturfrågor i refinement, planering och löpande avstämningar.

- **Fallgrop: Arkitekturarbete blir osynligt**
  - **Varför det händer:** Utredningar, avvägningar och samordning sker informellt utan att planeras.
  - **Hur man undviker det:** Gör arkitekturellt arbete synligt i backloggen med tydliga syften och förväntade resultat.

- **Fallgrop: Arkitekten försöker vara med i allt**
  - **Varför det händer:** Rädslan för missade konsekvenser leder till överinvolvering.
  - **Hur man undviker det:** Använd tydliga signaler för när frågor kräver kvalitetssäkring eller samordning.

- **Fallgrop: Teamet startar implementation innan beroenden är förstådda**
  - **Varför det händer:** Behovet uppfattas som lokalt eller tekniskt enkelt.
  - **Hur man undviker det:** Ställ tidigt frågan vilka andra som påverkas av beslutet.

- **Fallgrop: Samordning sker utan beslut eller uppföljning**
  - **Varför det händer:** Möten hålls, men resultatet blir inte synligt i teamets arbete.
  - **Hur man undviker det:** Koppla samordning till beslut, backloggposter, ansvar och uppföljning.

## Praktiskt stöd: frågor att använda i teamets flöde

### Vid backlogggenomgång

- Finns det kommande arbete som påverkar integrationer, information eller gemensamma tjänster?
- Finns det teknisk skuld eller avvikelser som behöver synliggöras?
- Finns det arkitekturellt arbete som saknar egen backloggpost?
- Finns det beslut som behöver dokumenteras innan teamet går vidare?

### Vid refinement

- Vilka antaganden gör vi om andra system, team eller utvecklingsområden?
- Vilka kvalitetskrav påverkar lösningsvalet?
- Är vägvalet reverserbart, eller låser det oss långsiktigt?
- Behöver vi involvera ett stödjande utvecklingsområde tidigt?

### Vid planering

- Är de viktigaste beroendena identifierade?
- Finns det samordningsaktiviteter som behöver planeras in?
- Är eventuell kvalitetssäkring tillräckligt tidig?
- Är beslutsmandatet tydligt?

### Vid leverans

- Är viktiga arkitekturbeslut dokumenterade?
- Finns det kvarvarande avvikelser eller teknisk skuld?
- Har berörda parter fått möjlighet att förstå konsekvenserna?
- Behöver något följas upp efter driftsättning?

## Snabb sammanfattning

- Arkitektur skapar mest nytta när den finns i teamens ordinarie flöde.
- Kontinuerlig arkitektur innebär löpande hantering av frågor med arkitekturell konsekvens.
- Backloggen bör synliggöra arkitekturellt arbete, inte dölja det som informella sidouppgifter.
- Refinement är ett viktigt tillfälle för tidig kvalitetssäkring.
- Planering bör användas för att identifiera samordning, beroenden och beslutsmandat.
- Leverans bör inte vara första tillfället då arkitekturen granskas.
- Arkitekten behöver skilja mellan lokala detaljer och vägval som påverkar helheten.

## Reflektionsfrågor

1. Var i ert nuvarande flöde upptäcks arkitekturfrågor oftast: tidigt i planering eller sent inför leverans?
2. Vilka typer av arkitekturellt arbete är i dag osynliga i backloggen?
3. Vilka signaler bör få ett team att involvera arkitekt eller stödjande utvecklingsområde?
4. Hur kan kvalitetssäkring göras tidigare utan att skapa onödig administration?
5. Vilka samordningsfrågor återkommer ofta och borde få en tydligare plats i teamens arbetssätt?

## Nästa steg

När arkitektur blir en del av teamens flöde förändras också arkitektens sätt att påverka. Det räcker inte att ha rätt i sak. Arkitekten behöver skapa förståelse, förtroende och konstruktiv dialog. Nästa kapitel handlar därför om hur arkitekten bygger förtroende och påverkar utan att uppfattas som en extern kontrollfunktion.
