# Kapitel 13: Gemensam arkitekturmognad

## Varför detta kapitel finns

Arkitekturarbete blir starkare när det inte enbart vilar på enskilda arkitekters erfarenhet, personliga nätverk eller lokala arbetssätt. I en decentraliserad myndighet behövs gemensam arkitekturmognad: en förmåga att förstå, diskutera, kvalitetssäkra och samordna arkitektur på ett tillräckligt likartat sätt över utvecklingsområden.

Det här kapitlet handlar om hur arkitekter kan bidra till att organisationen lär sig över tid. Fokus ligger inte på att införa en stor mognadsmodell, utan på vardagliga arbetssätt som gör arkitekturarbetet mer begripligt, mer konsekvent och mer användbart för både operativa och stödjande utvecklingsområden.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara vad gemensam arkitekturmognad innebär i en decentraliserad organisation
- identifiera tecken på låg respektive ökande arkitekturmognad
- bidra till lärande mellan operativa och stödjande utvecklingsområden
- använda kvalitetssäkring som ett sätt att bygga gemensam förståelse, inte bara kontrollera enskilda lösningar
- se när samordning bör användas för att skapa organisatoriskt lärande och minska återkommande problem

## Innan vi börjar

Tidigare kapitel har beskrivit hur arkitekten skapar värde genom riktning, samordning, kvalitetssäkring, principer, spårbara beslut, hantering av avvikelser, synliggörande av teknisk skuld, kontinuerligt arbete i teamens flöde och förtroendefull påverkan.

Detta kapitel lyfter blicken från det enskilda initiativet till organisationens samlade förmåga. Frågan är inte bara hur en arkitekt agerar klokt i ett ärende, utan hur många arkitekter tillsammans kan göra organisationen bättre på att fatta hållbara arkitekturbeslut.

## Huvudförklaring

### Arkitekturmognad är förmågan att agera klokt, inte bara att ha modeller

En organisation kan ha mallar, principer, råd, forum och beslutsprocesser utan att vara särskilt mogen i sitt arkitekturarbete. Mognad visar sig i hur organisationen faktiskt agerar när det uppstår tidspress, otydliga krav, lokala behov, beroenden och svåra avvägningar.

Gemensam arkitekturmognad handlar därför om praktisk förmåga. Det märks när arkitekter ställer liknande typer av frågor, när team förstår varför vissa vägval behöver samordnas, när beslut dokumenteras så att andra kan lära av dem och när kvalitetssäkring sker tidigt nog för att påverka lösningen.

Mognad betyder inte att alla gör exakt likadant. I en decentraliserad organisation behöver det finnas utrymme för lokala behov och anpassningar. Men variationen behöver vara begriplig. När olika utvecklingsområden gör olika val bör det finnas tydliga skäl, dokumenterade konsekvenser och en gemensam förståelse för vad som är lokalt, vad som är gemensamt och vad som behöver eskaleras.

### Från individuellt kunnande till organisatorisk förmåga

Många myndigheter har erfarna arkitekter som löser svåra frågor genom erfarenhet, relationer och gott omdöme. Det är värdefullt, men sårbart. Om arbetssättet inte blir synligt och delbart stannar kunskapen hos enskilda personer.

Gemensam arkitekturmognad växer när arkitekter gör sitt tänkande mer explicit. Det kan handla om att beskriva varför en viss fråga behöver samordnas, vilka kvalitetskriterier som användes i en granskning eller varför ett avsteg accepterades. När resonemangen blir synliga kan andra återanvända dem, ifrågasätta dem och förbättra dem.

Arkitektens uppgift blir då inte bara att lösa det egna ärendet, utan också att bidra till organisationens minne. Det betyder att viktiga insikter från ett initiativ behöver kunna påverka principer, vägledningar, gemensamma tjänster, beslutspraxis och framtida granskningar.

### Mognad byggs i återkommande situationer

Arkitekturmognad utvecklas sällan genom enstaka utbildningar. Den byggs i återkommande situationer där organisationen tränar på att se konsekvenser, göra avvägningar och lära av resultat.

Exempel på sådana situationer är:

- tidiga arkitekturdialoger inför större initiativ
- kvalitetssäkring av lösningsförslag
- samordning kring gemensamma förmågor
- uppföljning av avvikelser
- gemensam genomgång av arkitekturbeslut
- retrospektiv kring teknisk skuld och långsiktig hållbarhet
- erfarenhetsutbyte mellan operativa och stödjande arkitekter

Det viktiga är inte att skapa fler möten. Det viktiga är att använda befintliga möten och forum bättre. Varje återkommande situation bör hjälpa organisationen att besvara tre frågor: Vad lärde vi oss? Behöver något ändras i våra gemensamma förutsättningar? Behöver andra utvecklingsområden känna till detta?

### Tecken på låg arkitekturmognad

Låg arkitekturmognad märks ofta genom återkommande friktion. Samma frågor behöver lösas om och om igen. Liknande lösningar byggs parallellt. Arkitekturbeslut blir personberoende. Kvalitetssäkring sker sent och uppfattas som ett hinder. Samordning sker först när ett beroende redan har blivit ett problem.

Andra tecken är att principer används som hänvisningar utan förklaring, att avvikelser accepteras utan uppföljning eller att teknisk skuld diskuteras först när den redan blockerar utveckling. I en sådan miljö kan arkitekter arbeta hårt utan att organisationen egentligen blir bättre på arkitektur.

En viktig signal är när varje initiativ upplever sig vara ett specialfall. Vissa initiativ är verkligen speciella, men om allt behandlas som unikt blir det svårt att bygga gemensamma lösningar, gemensamt språk och gemensam kvalitet.

### Tecken på ökande arkitekturmognad

Ökande arkitekturmognad syns när arkitekturfrågor kommer upp tidigare och hanteras mer proportionerligt. Team vet när de kan fatta beslut själva och när de bör söka dialog. Operativa arkitekter och stödjande arkitekter använder gemensamma begrepp. Beslut och avvägningar dokumenteras tillräckligt för att andra ska förstå dem.

Ett annat tecken är att kvalitetssäkring förändras från sen granskning till löpande lärande. Granskningar ger inte bara besked om en lösning, utan fångar också återkommande mönster: otydliga principer, saknade förutsättningar, svaga informationsmodeller, återkommande integrationsproblem eller behov av bättre stöd till teamen.

Mognad syns också när organisationen vågar förbättra sina egna arbetssätt. Om samma avvikelse återkommer flera gånger kanske problemet inte ligger hos teamen, utan i en princip som är otydlig, en gemensam tjänst som inte möter behoven eller ett stödjande område som behöver ändra sitt erbjudande.

## Scenario: Den digitala tjänsten blir ett lärande exempel

Det operativa utvecklingsområdet som arbetar med den nya digitala tjänsten har under resans gång behövt hantera integrationsfrågor, informationsansvar, säkerhet, avvikelser, arkitekturbeslut och beroenden till stödjande utvecklingsområden. Flera frågor har liknat sådant som andra områden också mött.

I början sågs arbetet som ett lokalt initiativ. Efter hand blir det tydligt att erfarenheterna har bredare värde. Teamet har till exempel upptäckt att flera digitala tjänster behöver liknande stöd för informationsutbyte, behörighetsstyrning och spårbarhet. Det finns också återkommande osäkerhet kring när stödjande arkitekter bör involveras.

En mogen arkitekturpraktik stannar inte vid att lösa detta projekt. Arkitekterna samlar lärdomarna: vilka frågor kom upp för sent, vilka beslut behövde samordnas, vilka principer var hjälpsamma, vilka förutsättningar saknades och vad bör nästa initiativ kunna återanvända?

Resultatet kan bli en förbättrad vägledning, en tydligare samordningspunkt, ett återanvändbart lösningsmönster eller en justerad kvalitetscheck. Det viktiga är att erfarenheten omvandlas till gemensam förmåga.

## Vad arkitekten bör tänka på

### Gör lärandet konkret

Det räcker inte att säga att organisationen behöver bli bättre på arkitektur. Arkitekten behöver konkretisera vad som ska förbättras. Är problemet att team inte vet när de ska samordna? Att principer är svåra att använda? Att kvalitetssäkring sker för sent? Att avvikelser inte följs upp? Att samma tekniska skuld återkommer?

När förbättringsområdet blir konkret går det också att göra små förändringar. En ny fråga i en checklista, en tydligare definition, ett kort exempel på ett bra arkitekturbeslut eller en återkommande genomgång av avvikelser kan göra större nytta än en omfattande modell som ingen använder.

### Skilj mellan variation och oönskad spretighet

Decentralisering innebär att olika utvecklingsområden behöver kunna arbeta olika. Det är inte i sig ett problem. Problemet uppstår när skillnaderna inte är medvetna, inte går att förklara eller skapar onödig komplexitet för helheten.

Arkitekten bör därför inte reflexmässigt försöka standardisera allt. Frågan bör vara: vilken variation är motiverad, och vilken variation gör organisationen långsamt sämre? Motiverad variation kan dokumenteras och accepteras. Oönskad spretighet behöver synliggöras, samordnas och ibland styras om.

### Använd återkommande problem som förbättringsdata

När samma problem återkommer är det lätt att bli frustrerad över att teamen inte följer riktningen. Men återkommande problem är också data. De visar var organisationens förutsättningar inte fungerar.

Om flera initiativ gör liknande avsteg kan det betyda att principen är svår att tillämpa, att den gemensamma lösningen är för krånglig, att beslutsgången är otydlig eller att det saknas stöd i teamens flöde. Arkitekturmognad handlar om att använda sådana signaler för att förbättra systemet, inte bara korrigera enskilda fall.

### Bygg gemensamt språk

Gemensam mognad kräver gemensamma ord. Om olika arkitekter menar olika saker med exempelvis samordning, kvalitetssäkring, avvikelse, teknisk skuld eller arkitekturbeslut blir det svårt att agera konsekvent.

Ett gemensamt språk behöver inte vara perfekt från början. Det kan växa fram genom terminologi, exempel, beslutsmallar och återkommande dialog. Det viktiga är att centrala begrepp används på ett sätt som team, arkitekter och beslutsfattare kan förstå och känna igen.

## När kvalitetssäkring bör ske

Kvalitetssäkring bör användas som ett lärandetillfälle när:

- samma typ av brist eller risk återkommer i flera initiativ
- ett beslut kan skapa ett mönster som andra kommer att följa
- en avvikelse kan tyda på att en princip, riktlinje eller gemensam tjänst behöver förbättras
- ett initiativ visar att organisationens gemensamma förutsättningar inte räcker till
- teknisk skuld riskerar att bli ett strukturellt problem, inte bara ett lokalt problem
- granskningen kan ge insikt som bör delas med fler än det aktuella teamet

I dessa lägen bör kvalitetssäkring inte bara besvara frågan om lösningen är tillräckligt bra. Den bör också besvara frågan vad organisationen bör lära sig av ärendet.

## När samordning bör ske

Samordning bör ske när:

- flera utvecklingsområden står inför liknande vägval
- ett lokalt beslut kan påverka gemensamma förmågor, plattformar, information eller säkerhet
- flera avvikelser pekar på samma bakomliggande problem
- operativa områden efterfrågar stöd som de stödjande områdena ännu inte erbjuder
- det finns risk för parallella lösningar på samma behov
- erfarenheter från ett initiativ bör omvandlas till gemensamt mönster, vägledning eller tjänst

Samordning på mognadsnivå handlar alltså inte bara om att lösa beroenden. Den handlar om att se mönster över tid och skapa bättre förutsättningar för nästa initiativ.

## Vanliga fallgropar

- **Fallgrop: Att likställa mognad med mer formalia**
  - **Varför det händer:** Det är lätt att tro att fler mallar och beslutspunkter automatiskt ger bättre arkitektur.
  - **Hur man undviker det:** Utgå från vilka beslut, risker och lärdomar som behöver bli tydligare. Lägg bara till formalia som hjälper arbetet.

- **Fallgrop: Att göra mognadsarbete för abstrakt**
  - **Varför det händer:** Begrepp som mognad, förmåga och styrning kan bli svåra att omsätta i vardagen.
  - **Hur man undviker det:** Koppla alltid förbättringar till konkreta situationer, exempel och återkommande problem.

- **Fallgrop: Att skylla låg mognad på enskilda team**
  - **Varför det händer:** Det är synligt när team gör olika val, men mindre synligt när gemensamma förutsättningar saknas.
  - **Hur man undviker det:** Fråga vad organisationen behöver göra enklare, tydligare eller mer användbart.

- **Fallgrop: Att försöka standardisera bort all variation**
  - **Varför det händer:** Spretighet kan skapa frustration och ge en önskan om full enhetlighet.
  - **Hur man undviker det:** Skilj mellan motiverad lokal anpassning och variation som skapar onödig komplexitet.

## Snabb sammanfattning

- Gemensam arkitekturmognad handlar om organisationens praktiska förmåga att fatta hållbara arkitekturbeslut.
- Mognad syns i beteenden, inte bara i modeller, mallar eller forum.
- Kvalitetssäkring kan användas för att skapa lärande och upptäcka återkommande mönster.
- Samordning bör inte bara hantera beroenden i enskilda initiativ, utan också förbättra gemensamma förutsättningar över tid.
- Arkitekten bidrar till mognad genom att göra resonemang, beslut, avvägningar och lärdomar synliga och delbara.

## Reflektionsfrågor

1. Vilka arkitekturfrågor återkommer ofta i din organisation?
2. Vad säger de återkommande frågorna om organisationens gemensamma förutsättningar?
3. Vilka lärdomar från ett lokalt initiativ borde fler utvecklingsområden få nytta av?
4. Var finns risken att ni har skapat mer formalia än faktisk hjälp?
5. Vilken liten förändring skulle göra arkitekturarbetet mer begripligt och återanvändbart?

## Nästa steg

Nästa kapitel sammanfattar bokens huvudlinje: hur arkitekturarbete kan gå från att uppfattas som kontroll till att fungera som möjliggörande arkitektur. Där knyts styrning, samordning, kvalitetssäkring, förtroende och mognad samman till en praktisk modell för arkitektens vardag.
