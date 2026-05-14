# Kapitel 4: Samordning som praktiskt arkitekturarbete

## Varför detta kapitel finns

I en decentraliserad organisation kan mycket utveckling ske nära verksamhetens behov. Det är en styrka. Samtidigt ökar risken att flera utvecklingsområden löser liknande problem var för sig, använder samma information på olika sätt eller bygger beroenden som upptäcks för sent.

Samordning är därför inte ett sidospår från arkitekturarbetet. Det är en av arkitektens viktigaste praktiska uppgifter. Genom samordning hjälper arkitekten organisationen att se samband, undvika onödigt dubbelarbete och fatta beslut som fungerar över tid.

Kapitlet handlar om hur samordning sker i vardagen: vilka signaler arkitekten bör reagera på, vilka aktörer som behöver kopplas ihop och när samordning bör ske utan att skapa onödig administration.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara varför samordning är centralt i en decentraliserad arkitekturorganisation
- känna igen beroenden som kräver dialog med andra utvecklingsområden
- identifiera samordningsytor mellan initiativ, system, information och gemensamma förutsättningar
- avgöra när samordning bör ske tidigt, lättviktigt eller mer formellt
- använda samordning för att skapa bättre kvalitet utan att ta över teamens ansvar

## Innan vi börjar

Tidigare kapitel har etablerat tre viktiga utgångspunkter:

- Arkitekturarbete handlar om riktning, sammanhang och kvalitet.
- Decentraliserad styrning kräver balans mellan lokal handlingskraft och gemensamma ramar.
- Styrning i agil utveckling bör vara möjliggörande, proportionerlig och ske tidigt.

Samordning är den praktiska fortsättningen på detta. Riktning och guardrails hjälper team att förstå ramarna, men samordning behövs när flera initiativ, lösningar eller utvecklingsområden påverkar varandra i praktiken.

## Huvudförklaring

### Samordning börjar med att upptäcka samband

En arkitekt samordnar inte genom att vara med i alla möten eller granska alla detaljer. Samordning börjar med att upptäcka samband som andra kanske inte ser.

Det kan handla om att två team:

- behöver samma typ av integration
- använder samma verksamhetsinformation
- planerar liknande funktionalitet
- påverkar samma användarresa
- är beroende av samma plattform eller gemensamma tjänst
- gör teknikval som får konsekvenser för drift, säkerhet eller förvaltning
- tolkar en gemensam princip på olika sätt

Det viktiga är inte att alla samband automatiskt leder till ett gemensamt beslut. Det viktiga är att de blir synliga i tid.

När samband upptäcks sent blir samordning ofta upplevd som ett hinder. När samband upptäcks tidigt kan samordning i stället bli ett sätt att spara tid, minska risk och skapa bättre lösningar.

### Beroenden behöver göras begripliga

Ett beroende är en koppling som påverkar om en lösning kan genomföras hållbart. Beroenden kan vara tekniska, organisatoriska, informationsmässiga eller tidsmässiga.

Ett vanligt misstag är att bara betrakta beroenden som tekniska integrationer. I en större myndighet är många beroenden bredare än så. Ett team kan till exempel vara beroende av:

- att en informationsdefinition är gemensamt förstådd
- att ett stödjande utvecklingsområde kan leverera en plattformsförmåga
- att ett annat operativt område fattar ett kompletterande beslut
- att säkerhetskrav tolkas på samma sätt i flera lösningar
- att en gemensam tjänst har kapacitet, finansiering och förvaltningsansvar
- att arkitekturbeslut dokumenteras så att andra kan bygga vidare

Arkitektens uppgift är att formulera beroendet så konkret att det går att agera på. “Vi har ett beroende till plattformen” är ofta för vagt. En mer användbar formulering är: “Den digitala tjänsten behöver en autentiseringslösning som stödjer både interna handläggare och externa användare, och valet påverkar både säkerhetsarkitektur, användarresa och förvaltningsansvar.”

När beroenden blir konkreta blir det också tydligare vilka som behöver samordnas.

### Samordningsytor visar var dialog behövs

En samordningsyta är en plats där flera initiativ, lösningar eller ansvar möts. Det kan vara en faktisk mötesform, men oftare är det ett sakområde där dialog behövs.

Exempel på samordningsytor är:

- gemensam information, till exempel kund, ärende, beslut eller behörighet
- integrationer mellan system och tjänster
- gemensamma plattformar och tekniska förmågor
- användarresor som går över flera organisatoriska gränser
- säkerhet, behörighet och informationsklassning
- förvaltning, drift och support
- arkitekturprinciper och guardrails
- målarkitektur eller gemensam riktning

Arkitekten bör inte försöka skapa samordning överallt. Det skulle snabbt bli tungt. I stället bör arkitekten identifiera de samordningsytor där brist på dialog kan leda till dubbelarbete, kvalitetsbrister eller långsiktiga låsningar.

### Gemensamma förmågor är ofta viktigare än gemensamma lösningar

När flera områden har liknande behov är det lätt att fråga: “Kan vi bygga en gemensam lösning?” Det är ibland rätt fråga, men inte alltid.

En mer arkitekturell fråga är: “Finns det en gemensam förmåga som organisationen behöver utveckla?”

En gemensam förmåga kan vara teknisk, informationsmässig eller organisatorisk. Den kan bestå av en tjänst, en plattform, ett arbetssätt, en riktlinje, en modell eller en kombination av flera delar.

Skillnaden är viktig. Om arkitekten för snabbt driver mot en gemensam lösning kan det skapa motstånd, särskilt om lösningen inte passar de operativa behoven. Om arkitekten i stället börjar med den gemensamma förmågan blir samtalet bredare:

- Vilka behov är faktiskt gemensamma?
- Vilka delar bör lösas enhetligt?
- Vilka delar behöver kunna variera?
- Vem ska äga, finansiera och förvalta förmågan?
- Vilka operativa områden påverkas?
- Vilka stödjande områden behöver bidra?

Samordning handlar alltså inte alltid om att standardisera allt. Ofta handlar det om att förstå vad som bör vara gemensamt och vad som kan vara lokalt.

### Samordning behöver ske på rätt nivå

All samordning behöver inte ske i ett arkitekturråd eller ett formellt forum. I många fall räcker det med ett kort samtal mellan berörda arkitekter. I andra fall behövs en gemensam genomgång, ett dokumenterat beslut eller en eskalering till rätt beslutsforum.

En praktisk tumregel är att samordning bör vara lättviktig tills konsekvenserna kräver mer form.

Exempel:

- Ett team vill veta om en gemensam komponent redan finns. Det kan ofta hanteras genom direkt dialog.
- Två utvecklingsområden planerar liknande funktioner. Det kan kräva en gemensam analys av behov och ansvar.
- Ett initiativ vill avvika från en gemensam princip. Det behöver troligen dokumenteras och kvalitetssäkras.
- Flera lösningar påverkar samma informationsmodell. Det kan kräva samordning i ett etablerat forum och tydligt beslut om ägarskap.
- En lokal lösning riskerar att bli de facto-standard. Det bör lyftas tidigt, eftersom konsekvenserna kan bli breda.

Samordningens form bör alltså följa påverkan, risk och behov av gemensamt åtagande.

## Scenario: Flera områden planerar liknande funktioner

Det operativa utvecklingsområdet i bokens återkommande scenario arbetar med en ny digital tjänst. Teamet planerar en funktion där användare ska kunna följa status i sitt ärende.

Under en arkitekturdialog nämner en arkitekt från ett annat operativt område att de håller på att ta fram något liknande. Ett tredje område har redan byggt en enklare statusvy för en annan ärendetyp. Samtidigt arbetar ett stödjande utvecklingsområde med en gemensam komponent för meddelanden och notifieringar.

Till en början ser varje initiativ ut att vara lokalt. Varje område har egna krav, egen tidplan och egen finansiering. Men arkitekten ser flera samordningsytor:

- alla initiativ använder ärendeinformation
- användaren förväntar sig liknande beteende oavsett ärendetyp
- notifieringar bör inte byggas på tre olika sätt
- säkerhets- och behörighetskrav behöver tolkas konsekvent
- förvaltningen riskerar att få flera likartade lösningar med olika teknisk grund

Arkitektens första åtgärd är inte att stoppa arbetet. I stället formulerar arkitekten ett antal frågor:

- Vilka behov är gemensamma och vilka är specifika?
- Finns en gemensam förmåga kring ärendestatus som bör etableras?
- Kan ett stödjande område bidra med komponenter eller riktlinjer?
- Vilka beslut behöver vara gemensamma redan nu?
- Vilka delar kan varje operativt område fortsätta utveckla själv?

Genom att samla berörda arkitekter tidigt blir det möjligt att skilja mellan lokalt handlingsutrymme och gemensamma vägval. Teamen kan fortsätta arbeta, men med bättre förståelse för vilka delar som bör samordnas.

## Vad arkitekten bör tänka på

### Börja med behovet, inte forumet

Det är lätt att tänka att samordning betyder att ett ärende ska till ett visst möte. Men arkitektens första fråga bör vara: vad behöver samordnas och varför?

Forumet kommer senare. Ibland behövs inget formellt forum alls. Ibland behövs en etablerad beslutsväg. Det avgörande är att samordningen utgår från ett konkret behov.

Frågor att ställa:

- Vad riskerar att gå fel om vi inte samordnar?
- Vilka påverkas av beslutet?
- Är påverkan teknisk, informationsmässig, organisatorisk eller ekonomisk?
- Finns det en gemensam förmåga eller princip som berörs?
- Behöver beslutet dokumenteras för framtida spårbarhet?

### Gör samordning användbar för teamen

Samordning får inte bara skapa mer arbete. Den behöver ge något tillbaka. För teamen kan värdet vara:

- snabbare svar på vägval
- återanvändning av befintliga lösningar
- minskad risk för omtag
- tydligare ansvar
- bättre beslutsunderlag
- färre sena invändningar
- stöd från rätt kompetenser

När team upplever att samordning hjälper dem att komma framåt ökar viljan att involvera arkitekter tidigt.

### Var tydlig med vad som är gemensamt och vad som är lokalt

En av arkitektens viktigaste samordningsuppgifter är att skilja mellan gemensamma och lokala beslut.

Allt behöver inte vara gemensamt. Om för mycket lyfts till gemensam nivå tappar organisationen tempo och ansvar. Men om för lite samordnas skapas lokala lösningar som senare blir svåra att förändra.

Arkitekten behöver därför kunna säga:

- “Det här kan teamet besluta själv.”
- “Det här behöver ni stämma av med berört stödjande område.”
- “Det här påverkar flera utvecklingsområden och bör samordnas.”
- “Det här är ett gemensamt vägval som behöver dokumenteras.”
- “Det här är ett möjligt avsteg och bör hanteras enligt etablerad beslutsväg.”

Den tydligheten gör samordning mer begriplig och mindre personberoende.

## När kvalitetssäkring bör ske

I detta kapitel handlar kvalitetssäkring främst om att pröva om samordningen har fångat rätt beroenden och konsekvenser.

Kvalitetssäkring bör ske när:

- ett initiativ påverkar flera utvecklingsområden
- samma information används eller förändras i flera lösningar
- flera team bygger liknande funktioner
- ett lokalt teknikval kan påverka gemensam drift, säkerhet eller förvaltning
- en lösning använder eller förändrar en gemensam förutsättning
- ansvar för ägarskap, finansiering eller förvaltning är otydligt
- en lösning riskerar att bli återanvänd av andra utan att vara byggd för det
- beslutet är svårt eller dyrt att ändra senare

Kvalitetssäkringen behöver inte alltid vara omfattande. I tidiga skeden kan den bestå av en strukturerad dialog:

- Har vi identifierat berörda utvecklingsområden?
- Har vi förstått informationspåverkan?
- Har vi stämt av med rätt stödjande förmågor?
- Har vi dokumenterat de viktigaste antagandena?
- Är det tydligt vilka delar som är gemensamma och vilka som är lokala?

Målet är inte att hitta alla detaljer. Målet är att undvika att viktiga beroenden och konsekvenser förblir osynliga.

## När samordning bör ske

Samordning bör ske tidigt när ett initiativ passerar en organisatorisk, teknisk eller informationsmässig gräns.

Särskilt viktigt är det att samordna när:

- flera initiativ berör samma användarresa
- flera lösningar använder samma centrala information
- ett operativt område behöver en gemensam tjänst eller plattform
- ett stödjande område planerar en förmåga som flera operativa områden behöver
- ett lokalt behov kan vara relevant för flera områden
- olika team tolkar samma princip eller riktlinje olika
- tidplaner eller prioriteringar skapar beroenden mellan områden
- det finns risk för dubbelarbete eller motstridiga lösningar

Samordning bör inte vänta tills lösningen är färdigritad. Då blir samtalet lätt en granskning av något som teamet redan investerat i. Det är bättre att samordna när det fortfarande finns handlingsutrymme.

En enkel modell är att samordna vid tre tillfällen:

1. **Vid idé eller behov:** Finns liknande initiativ, gemensam information eller berörda förmågor?
2. **Vid lösningsinriktning:** Vilka vägval påverkar andra områden eller gemensamma förutsättningar?
3. **Inför större beslut:** Behöver beslut dokumenteras, kvalitetssäkras eller förankras i ett gemensamt forum?

## Vanliga fallgropar

- **Fallgrop: Samordning sker för sent**

- **Fallgrop: Allt lyfts till gemensam nivå**

- **Fallgrop: Samordning saknar tydligt syfte**

- **Fallgrop: Tekniska beroenden syns men informationsberoenden missas**

- **Fallgrop: Stödjande områden involveras bara som leverantörer**

## Praktiskt stöd: Samordningsfrågor för arkitekten

När du som arkitekt möter ett initiativ kan följande frågor användas som snabb kontroll:

### 1. Påverkan

- Påverkar initiativet fler än det egna teamet?
- Påverkar det flera system, processer eller användargrupper?
- Kan beslutet bli svårt att ändra senare?

###
2. Information

- Vilken central information används eller förändras?
- Finns gemensamma definitioner?
- Vem äger informationen?
- Finns risk att samma information hanteras olika i olika lösningar?

###
3. Teknik och integration

- Finns befintliga tjänster, plattformar eller integrationer som bör användas?
- Bygger teamet något som redan finns?
- Skapas nya beroenden till drift, säkerhet eller förvaltning?

###
4. Ansvar

- Vem äger lösningen efter leverans?
- Vem ansvarar för gemensamma komponenter?
- Behöver finansiering eller förvaltningsansvar samordnas?

###
5. Gemensam riktning

- Stämmer lösningen med etablerade principer och guardrails?
- Finns ett avsteg som behöver hanteras?
- Kan behovet vara relevant för andra utvecklingsområden?

Frågorna ska inte användas som en tung checklista i varje ärende. De är ett stöd för att upptäcka när samordning behövs.

## Snabb sammanfattning

- Samordning är praktiskt arkitekturarbete, inte administrativt sidospår.
- Arkitekten samordnar genom att upptäcka samband, formulera beroenden och koppla ihop rätt aktörer.
- Beroenden kan vara tekniska, informationsmässiga, organisatoriska, tidsmässiga eller ansvarsmässiga.
- Samordningsytor visar var dialog behövs mellan initiativ, lösningar och utvecklingsområden.
- Gemensamma förmågor är ofta en bättre utgångspunkt än att direkt föreslå gemensamma lösningar.
- Samordning bör vara proportionerlig: lätt där påverkan är liten, mer strukturerad där konsekvenserna är stora.
- Kvalitetssäkring bör ske när bristande samordning kan leda till dubbelarbete, motstridiga lösningar eller långsiktiga låsningar.

## Reflektionsfrågor

1. Vilka samordningsytor är vanligast i din arkitekturvardag?
2. Vilka beroenden upptäcks ofta för sent i din organisation?
3. När fungerar samordning som stöd, och när upplevs den som hinder?
4. Vilka beslut bör team kunna fatta själva utan samordning?
5. Vilka signaler visar att ett lokalt initiativ egentligen berör en gemensam förmåga?

## Nästa steg

Nästa kapitel fördjupar kvalitetssäkring. Där flyttas fokus från att upptäcka och samordna beroenden till att ge tidig återkoppling på lösningsval, principer, risker och arkitekturell kvalitet utan att bromsa utvecklingen.
