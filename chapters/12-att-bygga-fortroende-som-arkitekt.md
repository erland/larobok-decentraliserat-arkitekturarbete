# Kapitel 12: Att bygga förtroende som arkitekt

## Varför detta kapitel finns

Arkitektens möjlighet att bidra avgörs inte bara av kompetens, mandat eller formella styrmodeller. Den avgörs också av förtroende. I en decentraliserad organisation, där mycket ansvar ligger nära operativa utvecklingsområden och agila team, behöver arkitekten ofta påverka utan att kunna beordra. Då blir relationer, tydlighet och förmågan att göra nytta i rätt ögonblick avgörande.

Det här kapitlet handlar om hur arkitekten bygger förtroende i vardagen. Fokus ligger på hur man kommunicerar arkitektoniska konsekvenser, gör kvalitetssäkring begriplig och visar varför samordning hjälper snarare än hindrar utveckling.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara varför förtroende är en praktisk förutsättning för fungerande arkitekturarbete
- skilja mellan att kontrollera, stödja och påverka
- kommunicera arkitekturella risker och konsekvenser på ett sätt som hjälper team och beslutsfattare
- identifiera situationer där kvalitetssäkring och samordning bör ske genom dialog snarare än formell granskning
- använda enkla arbetssätt för att bygga långsiktigt förtroende mellan operativa och stödjande utvecklingsområden

## Innan vi börjar

Tidigare kapitel har beskrivit arkitekturarbete som ett praktiskt arbete med riktning, sammanhang, kvalitet och konsekvenser. Vi har också sett hur styrning, samordning, kvalitetssäkring, principer, arkitekturbeslut, avvikelser, teknisk skuld och teamens flöde hänger ihop.

Detta kapitel bygger vidare på samma idé: arkitekten skapar värde när rätt frågor blir synliga i tid och när organisationen får bättre förutsättningar att fatta hållbara beslut. Skillnaden är att fokus nu ligger på hur arkitekten får gehör för detta i en vardag där många roller har olika mål, tidspress och perspektiv.

## Huvudförklaring

### Förtroende är inte ett sidospår

Det är lätt att tänka på förtroende som något mjukt vid sidan av det egentliga arkitekturarbetet. I praktiken är det tvärtom. Utan förtroende kommer arkitekten ofta in sent, får ofullständig information eller uppfattas som någon som säger nej. Med förtroende blir arkitekten inbjuden tidigare, får tillgång till verkliga problem och kan hjälpa team att hitta bättre vägval innan besluten har låst sig.

Förtroende betyder inte att arkitekten alltid håller med. Det betyder att andra upplever att arkitekten försöker förstå situationen, respekterar teamets uppdrag och bidrar med relevanta perspektiv. En arkitekt som bara pekar på brister skapar lätt försvar. En arkitekt som hjälper teamet att förstå konsekvenser och alternativ skapar handlingsutrymme.

### Från granskningsroll till medskapande roll

I en decentraliserad myndighet kan arkitekten behöva kvalitetssäkra utan att bli en separat kontrollinstans. Det kräver ett skifte från frågan “är lösningen godkänd?” till frågan “vad behöver vi förstå för att lösningen ska bli hållbar?”.

Det betyder inte att formell granskning saknar värde. Vissa beslut behöver dokumenteras, prövas och förankras tydligt. Men om all kvalitetssäkring sker sent och formellt blir den lätt dyr, konfliktfylld och svår att omsätta. Förtroende byggs när arkitekten deltar tidigare, ställer frågor som hjälper teamet och gör bedömningar proportionerliga.

En medskapande arkitekt:

- utgår från verksamhetsbehovet och teamets mål
- synliggör konsekvenser utan att överdramatisera
- skiljer mellan krav, rekommendationer och öppna avvägningar
- hjälper teamet hitta en framkomlig väg
- dokumenterar viktiga beslut utan att skapa onödig administration

### Kommunikation av konsekvenser

Arkitekter ser ofta beroenden, risker och långsiktiga effekter som andra roller inte ser lika tydligt. Utmaningen är att översätta detta till begriplig nytta. Ett vanligt misstag är att beskriva arkitekturproblem med interna arkitekturbegrepp när mottagaren egentligen behöver förstå påverkan på verksamhet, leverans, säkerhet, kostnad eller framtida förändringsförmåga.

En användbar struktur är:

1. Vad är vägvalet?
2. Vilka alternativ finns?
3. Vad vinner vi på det föreslagna valet?
4. Vilka konsekvenser skapar det på kort och lång sikt?
5. Vilka andra utvecklingsområden, tjänster eller informationsflöden påverkas?
6. Vad behöver följas upp?

När arkitekten kommunicerar på detta sätt blir kvalitetssäkring inte ett omdöme utifrån, utan en gemensam analys av konsekvenser.

### Att påverka utan att ta över

Arkitekten ska inte ta över teamets ansvar. Om arkitekten blir den som löser alla svåra frågor riskerar teamet att sluta utveckla egen förmåga. Om arkitekten däremot håller sig för långt bort kan viktiga arkitekturella frågor missas.

Balansen ligger i att hjälpa teamet att fatta bättre beslut, inte att fatta alla beslut åt teamet. Det kan innebära att arkitekten föreslår principer, visar konsekvenser, kopplar ihop team med stödjande förmågor eller hjälper till att formulera ett arkitekturbeslut. Men teamet behöver fortfarande förstå varför beslutet är rimligt och hur det påverkar deras arbete.

### Förtroende mellan operativa och stödjande arkitekter

Operativa arkitekter och stödjande/förutsättningsskapande arkitekter kan ibland uppleva olika verkligheter. Den operativa arkitekten står nära verksamhetens behov, leveranstryck och lokala kompromisser. Den stödjande arkitekten ser återkommande mönster, gemensamma lösningar och risker med fragmentering.

Förtroende byggs när båda perspektiven behandlas som legitima. Det operativa perspektivet behövs för att arkitekturen ska vara relevant. Det stödjande perspektivet behövs för att undvika att varje område bygger sin egen variant av samma förmåga. Konflikter uppstår ofta när någon av sidorna upplever att den andra inte förstår deras ansvar.

En praktisk regel är att börja med att formulera den andra sidans problem så väl att den känner igen sig. Först därefter blir det meningsfullt att föreslå lösningar, gemensamma principer eller samordningsåtgärder.

## Exempel: När arkitekten uppfattas som broms

I det återkommande scenariot arbetar ett operativt utvecklingsområde med en ny digital tjänst. Teamet har valt en lokal lösning för hantering av meddelanden till användare. Lösningen verkar snabb att bygga och passar det omedelbara behovet.

Den stödjande arkitekten ser att flera andra utvecklingsområden har liknande behov och att myndigheten redan diskuterar en gemensam meddelandeförmåga. Om varje område bygger sin egen lösning kan det leda till dubbelarbete, olika användarupplevelser, svårare informationsstyrning och högre förvaltningskostnad.

Ett kontrollorienterat agerande skulle kunna vara:

> “Ni får inte bygga den här lösningen. Den följer inte den gemensamma riktningen.”

Det kan vara sakligt motiverat, men riskerar att skapa motstånd om teamet inte förstår sammanhanget.

Ett förtroendebyggande agerande kan vara:

> “Jag förstår varför ni vill lösa detta snabbt. Samtidigt ser vi samma behov i flera områden. Låt oss titta på om ni kan komma vidare med en begränsad första lösning, samtidigt som vi tydliggör vad som behöver kunna ersättas eller återanvändas när den gemensamma förmågan är klar.”

Skillnaden är inte att arkitekten undviker styrning. Skillnaden är att styrningen kopplas till verksamhetsnytta, samordning och konsekvenser. Teamet får hjälp att komma vidare, men utan att dölja den långsiktiga arkitekturella frågan.

## Stöd: När kvalitetssäkring bör ske

Kvalitetssäkring bör ske när ett vägval kan påverka mer än den närmaste leveransen. Följande signaler tyder på att arkitekten bör initiera kvalitetssäkring genom dialog, granskning eller beslutsstöd:

- Lösningen introducerar en ny teknisk plattform, integrationsväg eller informationsmodell.
- Teamet gör ett vägval som blir svårt eller dyrt att ändra senare.
- Flera utvecklingsområden har liknande behov.
- Lösningen påverkar säkerhet, informationshantering, regelefterlevnad eller användarupplevelse.
- Det finns risk att lokal optimering skapar gemensam kostnad.
- Ett avsteg från princip, riktlinje eller tidigare arkitekturbeslut övervägs.
- Teamet saknar tydlig ägare för en långsiktig förvaltningskonsekvens.

Kvalitetssäkring behöver inte alltid vara ett möte eller ett dokument. I tidiga skeden kan den vara en kort dialog, en gemensam genomgång av alternativ eller ett stöd för att formulera ett beslut. Ju större påverkan, desto mer strukturerad bör kvalitetssäkringen vara.

## Stöd: När samordning bör ske

Samordning bör ske när ett initiativ inte längre är enbart lokalt. Följande signaler visar att samordning behövs:

- Flera team påverkar samma informationsflöde, tjänst eller användarresa.
- Ett operativt behov liknar behov i andra utvecklingsområden.
- En lokal lösning kan bli en gemensam förmåga.
- En gemensam tjänst behöver anpassas för att fungera i praktiken.
- Beslut i ett område skapar beroenden för ett annat område.
- Det finns otydlighet om ansvar, mandat eller ägarskap.
- Samma diskussion återkommer i flera forum utan att leda till beslut.

Samordning är särskilt viktig när utvecklingen sker agilt och parallellt. Då kan många små beslut snabbt skapa en riktning som ingen formellt har valt. Arkitektens roll är att fånga dessa mönster tidigt och skapa forum där rätt personer kan fatta medvetna beslut.

## Vanliga misstag

- **Misstag: Att försöka vinna genom expertis**

- **Misstag: Att beskriva styrning som krav utan sammanhang**

- **Misstag: Att komma in för sent och sedan kräva stora ändringar**

- **Misstag: Att undvika svåra besked för att bevara relationen**

## Praktiska arbetssätt

### 1. Börja med uppdraget

Inled arkitekturdialoger med att förstå vad teamet försöker åstadkomma. Fråga vilket problem som ska lösas, vilka begränsningar som finns och vilka beslut som redan är tagna. Det skapar bättre underlag och visar respekt för teamets situation.

###
2. Gör konsekvenser synliga

Använd enkla formuleringar:

- “Det här påverkar främst förvaltning och ägarskap.”
- “Det här är sannolikt lätt att ändra senare.”
- “Det här valet kan skapa beroenden till flera andra områden.”
- “Det här behöver samordnas eftersom behovet återkommer på flera håll.”

Sådana formuleringar hjälper mottagaren att förstå varför arkitekturfrågan är relevant.

###
3. Skilj på måste, bör och kan

Allt är inte lika viktigt. Arkitekten bör vara tydlig med skillnaden mellan:

- **Måste:** krav, lag, säkerhet, beslutade ramar eller nödvändiga gemensamma vägval.
- **Bör:** stark rekommendation baserad på principer, erfarenhet eller långsiktig konsekvens.
- **Kan:** möjliga alternativ där teamet har större frihet att välja.

Denna uppdelning gör styrningen mer begriplig och minskar risken att allt uppfattas som förbud.

###
4. Erbjud nästa steg

Avsluta inte med endast en risk. Erbjud ett nästa steg: en kort samordning, ett beslutsunderlag, kontakt med ett stödjande område, en principavvägning eller en avstegsbedömning. Förtroende ökar när arkitekten hjälper arbetet framåt.

###
5. Följ upp det som sagts

Förtroende stärks när arkitekten återkommer till tidigare dialoger, ser om beslut fungerade och justerar stöd vid behov. Uppföljning visar att arkitektur inte är en engångsgranskning utan ett ansvar över tid.

## Reflektionsfrågor

1. I vilka situationer uppfattas arkitekter i din organisation som stöd, och i vilka situationer uppfattas de som kontroll?
2. Vilka arkitekturfrågor kommer ofta in för sent i utvecklingsflödet?
3. Hur kan du som arkitekt göra kvalitetssäkring mer begriplig för team och beslutsfattare?
4. Vilka återkommande samordningsbehov borde fångas tidigare?
5. Vad kan du göra nästa vecka för att bygga mer förtroende med ett operativt eller stödjande utvecklingsområde?

## Snabb sammanfattning

- Förtroende är en praktisk förutsättning för att arkitekten ska kunna påverka tidigt.
- Arkitekten bygger förtroende genom att förstå teamets uppdrag, synliggöra konsekvenser och hjälpa arbetet framåt.
- Kvalitetssäkring fungerar bäst när den sker proportionerligt och i tid.
- Samordning behövs när lokala vägval påverkar andra utvecklingsområden, gemensamma förmågor eller långsiktig hållbarhet.
- Arkitekten behöver kunna vara både stödjande och tydlig.
- Förtroende betyder inte att undvika styrning, utan att göra styrningen relevant, begriplig och användbar.

## Nästa steg

Nästa kapitel handlar om gemensam arkitekturmognad. Där flyttas fokus från den enskilda arkitektens förtroendeskapande vardag till hur organisationen som helhet kan lära, förbättra sina arbetssätt och successivt höja kvaliteten i arkitekturarbetet.
