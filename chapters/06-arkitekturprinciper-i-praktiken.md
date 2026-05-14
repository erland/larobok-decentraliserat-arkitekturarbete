# Kapitel 6: Arkitekturprinciper i praktiken

## Varför detta kapitel finns

Arkitekturprinciper finns ofta i organisationer som redan arbetar med arkitekturstyrning. De kan vara formulerade i styrande dokument, målarkitektur, riktlinjer eller interna modeller. Ändå används de inte alltid i vardagen. Ibland upplevs de som abstrakta, självklara eller svåra att omsätta i konkreta beslut.

I en decentraliserad myndighet är principer särskilt viktiga. De hjälper många utvecklingsområden att fatta beslut som fungerar tillsammans, även när besluten fattas nära team och verksamhet. Men principer gör nytta först när de används som praktiskt beslutsstöd.

Det här kapitlet handlar om hur arkitekten kan använda arkitekturprinciper i dialog med team, produktledning, verksamhet och stödjande utvecklingsområden. Fokus ligger på hur principer hjälper till att tydliggöra avvägningar, kvalitetssäkra vägval och hantera avsteg utan att skapa onödig tröghet.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara varför arkitekturprinciper behövs i en decentraliserad organisation
- använda principer som stöd för dialog och beslut, inte bara som regler
- känna igen situationer där principer bör prövas tidigt
- göra principavvägningar när flera principer pekar åt olika håll
- hantera avsteg på ett medvetet, motiverat och uppföljningsbart sätt

## Innan vi börjar

Tidigare kapitel har beskrivit arkitekturarbete som arbete med riktning, sammanhang och kvalitet. Vi har också etablerat att styrning bör vara möjliggörande, att samordning synliggör beroenden och att kvalitetssäkring bör ske tidigt och stegvis.

Arkitekturprinciper binder ihop dessa delar. De ger riktning, gör kvalitet mer konkret och skapar ett gemensamt språk för samordning. När principer används väl hjälper de team att fatta bättre beslut själva. När de används dåligt blir de antingen hyllvärmare eller stoppregler.

## Huvudförklaring

### En princip är ett beslutsstöd

En arkitekturprincip beskriver en önskad riktning för återkommande beslut. Den säger inte alltid exakt vilken lösning som ska väljas, men den hjälper organisationen att resonera konsekvent.

En bra princip svarar ofta på tre frågor:

- Vad vill vi uppnå?
- Varför är det viktigt?
- Hur påverkar det våra beslut?

Exempel på principer kan vara:

- använd gemensamma förutsättningar där det är rimligt
- bygg lösningar som är möjliga att förvalta och vidareutveckla
- undvik onödig dubblering av information
- gör integrationer tydliga och ansvarssatta
- skydda information utifrån klassning och användningssituation
- välj lösningar som minskar långsiktig komplexitet

Det viktiga är inte den exakta formuleringen. Det viktiga är att principen hjälper människor att fatta beslut i praktiken.

Om en princip bara säger “vi ska ha hög kvalitet” är den för svag. Om den säger “alla lösningar måste alltid använda en viss komponent” kan den bli för rigid. En användbar princip ligger ofta mellan dessa ytterligheter: den ger tydlig riktning, men tillåter professionell bedömning.

### Principer skapar gemensam riktning utan detaljstyrning

I en centraliserad organisation kan många beslut styras genom gemensamma beslutsvägar. I en decentraliserad organisation behöver team och utvecklingsområden kunna fatta många beslut själva. Då behövs andra mekanismer för att hålla ihop helheten.

Arkitekturprinciper är en sådan mekanism. De gör det möjligt att decentralisera beslut utan att varje område utvecklar sin egen riktning.

Det betyder inte att principer ersätter dialog. Tvärtom. Principer ger ett gemensamt språk för dialogen. När ett team vill välja en lokal lösning kan arkitekten fråga:

- Vilka principer stödjer lösningen?
- Vilka principer utmanas?
- Vad är konsekvensen för andra utvecklingsområden?
- Är valet lätt att ändra senare?
- Behöver vi samordna med någon innan beslutet tas?

På så sätt blir principen inte ett argument från arkitekten mot teamet. Den blir ett gemensamt verktyg för att förstå beslutet.

### Principer behöver tolkas i sitt sammanhang

En vanlig fallgrop är att behandla principer som absoluta regler. Det kan skapa onödig friktion, särskilt i en agil omställning där team behöver kunna agera på ny information.

En annan fallgrop är motsatsen: att principer blir så flexibla att de inte betyder något. Då kan varje avsteg motiveras med att situationen är speciell.

Arkitektens uppgift är att hjälpa organisationen att tolka principer i sitt sammanhang. Det innebär att se både principens syfte och den konkreta situationens behov.

Anta att en princip säger att gemensamma förutsättningar ska återanvändas där det är rimligt. Det betyder inte att varje team alltid måste använda varje gemensam komponent. Men det betyder att teamet behöver kunna svara på varför en lokal lösning är bättre i just detta fall, vilka konsekvenser det får och hur beslutet ska följas upp.

Frågan är alltså inte bara: “Följer lösningen principen?” Frågan är snarare: “Hur har principen påverkat beslutet, och är avvägningen rimlig?”

### Principavvägningar är en del av arkitektens hantverk

I praktiken pekar principer ibland åt olika håll. En princip kan betona återanvändning, medan en annan betonar enkelhet och snabb leverans. En princip kan betona standardisering, medan en annan betonar verksamhetsnära anpassning. En princip kan betona säkerhet, medan en annan betonar användbarhet.

Det är här arkitektens hantverk blir viktigt. Principer ska inte användas mekaniskt. De ska vägas mot varandra.

En principavvägning innebär att arkitekten synliggör:

- vilka principer som är relevanta
- vilka mål eller kvaliteter som står i spänning
- vilka konsekvenser olika alternativ får
- vilka risker som accepteras
- vilka beslut som behöver dokumenteras
- vilka uppföljningar som behövs

En användbar principavvägning behöver inte vara lång. För många beslut räcker det med några tydliga meningar i ett arkitekturbeslut, en beslutslogg eller ett underlag inför granskning. Det viktiga är att avvägningen går att förstå i efterhand.

### Principer ska hjälpa team att agera tidigare

Principer gör störst nytta när de används tidigt. Om principerna först tas fram vid en sen granskning kan de upplevas som efterhandskritik. Teamet kan då känna att spelreglerna ändrades efter att arbetet redan var gjort.

Arkitekten bör därför lyfta relevanta principer redan när behov, lösningsinriktning eller större vägval diskuteras. Det kan ske genom enkla frågor:

- Finns det en gemensam förutsättning vi bör börja med?
- Berör vi information som används av andra?
- Skapar vi något som fler utvecklingsområden kan behöva?
- Tar vi ett beslut som blir dyrt att ändra senare?
- Finns det en princip som bör vara styrande för detta vägval?
- Finns det en princip vi riskerar att avvika från?

När principer kommer in tidigt kan de påverka lösningen utan att stoppa arbetet. De blir en del av teamets tänkande, inte en extern kontroll.

### Avsteg är inte alltid fel

Ett avsteg från en princip är inte automatiskt ett misslyckande. Ibland finns goda skäl att avvika. Det kan handla om ett tillfälligt behov, en stark verksamhetsnytta, en teknisk begränsning, en pågående migration eller att den gemensamma förutsättningen ännu inte är mogen.

Problemet uppstår när avsteg sker omedvetet, upprepas utan lärande eller blir permanenta utan beslut.

Ett professionellt hanterat avsteg bör därför vara:

- medvetet
- motiverat
- riskbedömt
- tidsatt eller omprövningsbart
- dokumenterat
- samordnat med berörda parter
- kopplat till en plan för uppföljning

Det betyder inte att varje liten avvikelse ska skapa en tung process. Även här gäller proportionerlighet. Ett litet lokalt avsteg kan hanteras i en kort dialog. Ett avsteg som påverkar gemensam information, säkerhet, plattformar eller flera utvecklingsområden behöver hanteras mer strukturerat.

### Principer behöver vara levande

Om principer aldrig prövas, diskuteras eller uppdateras tappar de kraft. En princip som ofta kräver avsteg kan vara fel formulerad, för långt från verkligheten eller kopplad till en gemensam förutsättning som inte fungerar tillräckligt bra.

Arkitekter bör därför se principer som levande styrning. Det innebär att erfarenheter från operativa utvecklingsområden behöver återföras till den gemensamma modellen.

Exempel:

- Om flera team avviker från samma princip kan principen behöva förtydligas.
- Om en gemensam komponent ofta väljs bort kan dess förmåga eller användbarhet behöva förbättras.
- Om principer kolliderar ofta kan organisationen behöva tydligare prioriteringsregler.
- Om principer inte används kan de behöva göras mer konkreta och kopplas till vardagliga beslut.

På så sätt blir principerna inte bara krav från mitten av organisationen. De blir ett sätt att lära av praktiken och utveckla gemensam arkitekturmognad.

## Scenario

Det operativa utvecklingsområdet arbetar med den nya digitala tjänsten. Teamet vill bygga en lokal funktion för att hantera behörigheter eftersom det verkar gå snabbare än att använda en gemensam förutsättning.

Den operativa arkitekten ser att beslutet berör flera principer. Återanvändning av gemensamma förutsättningar talar för den gemensamma behörighetstjänsten. Snabb leverans och enkelhet talar för den lokala lösningen. Säkerhet och förvaltningsbarhet talar för att inte skapa en parallell behörighetsmodell utan tydligt ansvar.

Arkitekten väljer därför inte att börja med ett nej. I stället samlar arkitekten teamet, representant från det stödjande utvecklingsområdet och produktansvarig för att pröva frågan.

Dialogen landar i att den gemensamma förutsättningen ska användas för den långsiktiga lösningen, men att teamet får göra en begränsad tillfällig lösning för en intern pilot. Avsteget dokumenteras, tidsätts och kopplas till en uppföljning. Det stödjande området tar samtidigt med sig att den gemensamma tjänsten behöver bättre införandestöd.

Resultatet blir inte att principen “vann” över teamet. Resultatet blir att principen gjorde beslutet mer medvetet, samordnat och uppföljningsbart.

## Vad arkitekten bör tänka på

Arkitekten bör använda principer som samtalsstöd snarare än som färdiga svar. Det innebär att principen behöver kopplas till den aktuella situationen och till de konsekvenser som valet kan få.

Några praktiska frågor att använda i vardagen:

- Vilka principer är relevanta för detta vägval?
- Förstår teamet varför principen finns?
- Är principen tillräckligt konkret för att påverka beslutet?
- Finns det flera principer som behöver vägas mot varandra?
- Påverkar beslutet andra utvecklingsområden?
- Är ett eventuellt avsteg medvetet och motiverat?
- Behöver beslutet dokumenteras så att andra kan förstå det senare?
- Ger situationen återkoppling om att en princip eller gemensam förutsättning behöver förbättras?

Arkitekten bör också vara uppmärksam på ton och tajming. En princip som lyfts tidigt kan uppfattas som hjälp. Samma princip som lyfts sent kan uppfattas som kritik.

## När kvalitetssäkring bör ske

Kvalitetssäkring med hjälp av principer bör ske när ett vägval:

- påverkar gemensamma förutsättningar, plattformar eller tjänster
- kan skapa parallella lösningar eller dubbelarbete
- berör information, säkerhet, behörighet eller integrationer
- skapar långsiktig förvaltningspåverkan
- innebär ett möjligt avsteg från gemensam riktning
- är svårt eller dyrt att ändra senare
- riskerar att bli ett prejudikat för andra utvecklingsområden

Kvalitetssäkringen bör börja med förståelse: vilken princip är relevant, vilket problem försöker teamet lösa och vilka alternativ finns? Därefter kan arkitekten hjälpa till att bedöma om lösningen följer principen, om en principavvägning behövs eller om ett avsteg bör hanteras.

## När samordning bör ske

Samordning bör ske när principfrågan inte bara är lokal. Det gäller särskilt när:

- flera utvecklingsområden tolkar samma princip olika
- en lokal lösning kan bli relevant för fler
- en gemensam förutsättning inte möter ett operativt behov
- ett avsteg påverkar plattform, information, säkerhet eller förvaltning
- beslutet kan skapa förväntningar på hur liknande frågor ska hanteras framöver
- stödjande och operativa utvecklingsområden behöver förstå varandras behov

Samordning handlar då inte om att alla ska tycka lika. Det handlar om att rätt personer får möjlighet att förstå konsekvenserna innan beslutet låser sig.

## Vanliga fallgropar

- **Fallgrop: Principer används som sena stoppregler**
  - **Varför det händer:** Principerna kommer in först vid granskning eller beslut.
  - **Hur man undviker det:** Lyft relevanta principer tidigt i behovs- och lösningsdialog.

- **Fallgrop: Principer blir för abstrakta**
  - **Varför det händer:** De uttrycker önskade värden men kopplas inte till konkreta beslut.
  - **Hur man undviker det:** Koppla varje princip till typiska frågor, exempel och beslutssituationer.

- **Fallgrop: Alla avsteg behandlas som fel**
  - **Varför det händer:** Organisationen vill skapa följsamhet men saknar ett moget sätt att hantera undantag.
  - **Hur man undviker det:** Hantera avsteg proportionerligt, med motivering, riskbedömning och uppföljning.

- **Fallgrop: Principer tolkas olika i olika utvecklingsområden**
  - **Varför det händer:** Decentraliserade team möter olika behov och har olika erfarenheter.
  - **Hur man undviker det:** Använd samordning för att jämföra tolkningar och skapa gemensamma exempel.

- **Fallgrop: Principer används för att vinna argument**
  - **Varför det händer:** Arkitekten eller teamet använder principen selektivt för att stödja en redan bestämd lösning.
  - **Hur man undviker det:** Synliggör flera relevanta principer och gör avvägningen explicit.

## Snabb sammanfattning

- Arkitekturprinciper är praktiska beslutsstöd, inte bara styrande texter.
- Principer hjälper decentraliserade utvecklingsområden att fatta lokala beslut i gemensam riktning.
- Principer behöver tolkas i sitt sammanhang och vägas mot varandra.
- Avsteg kan vara rimliga, men bör vara medvetna, motiverade, riskbedömda och uppföljningsbara.
- Principer gör störst nytta när de används tidigt i dialogen.
- Återkommande avsteg kan visa att en princip, gemensam förutsättning eller arbetssätt behöver utvecklas.

## Reflektionsfrågor

1. Vilka principer används ofta i din vardag, och vilka finns mest i dokument?
2. När blir en princip ett stöd för teamet, och när upplevs den som hinder?
3. Vilka typer av avsteg bör kunna hanteras lättviktigt i din organisation?
4. Hur kan operativa erfarenheter användas för att förbättra gemensamma principer?
5. Vilken princip skulle behöva förklaras bättre för att bli mer användbar i praktiken?

## Nästa steg

Nästa kapitel bygger vidare på principerna genom att behandla arkitekturbeslut och spårbarhet. När principer påverkar ett viktigt vägval behöver beslutet ofta formuleras så att andra kan förstå varför valet gjordes, vilka alternativ som övervägdes och vad som behöver följas upp.
