# Pedagogisk canon

## Språk
Svenska. Engelska begrepp får användas där de är etablerade eller där en svensk översättning blir missvisande.

## Svårighetsgrad
Erfaren. Läsaren har praktisk IT-erfarenhet men behöver fördjupad förståelse för arkitektens roll i styrning, kvalitetssäkring och samordning.

## Målgrupp
IT-arkitekter i en decentraliserad myndighetsorganisation.

## Ton
Professionell, konkret, pedagogisk och reflekterande.

## Pedagogiskt grepp
Boken utgår från arkitektens vardag och använder ett återkommande scenario. Fokus ligger på vad arkitekten bör tänka på, varför det spelar roll och hur arkitekten kan agera.

## Kapitelkomponenter
Varje kapitel bör innehålla:
- Kapitelrubrik
- Varför kapitlet finns
- Lärandemål
- Koppling till tidigare kapitel
- Huvudförklaring
- Scenario
- Vad arkitekten bör tänka på
- När kvalitetssäkring bör ske
- När samordning bör ske
- Vanliga fallgropar
- Snabb sammanfattning
- Reflektionsfrågor
- Nästa steg

## Regel
Introducera inte centrala begrepp före de förklaras. Uppdatera `terminologi.md` när ett nytt begrepp etableras.


## Etablerat efter kapitel 1

### Centrala definitioner
- Arkitekturarbete definieras som praktiskt arbete med riktning, sammanhang och kvalitet.
- Riktning är inte detaljstyrning, utan ramar, principer och dialog som hjälper team att hålla kursen.
- Sammanhang innebär att förstå hur en lösning påverkar andra system, informationsflöden, ansvar och utvecklingsområden.
- Kvalitetssäkring ska framställas som tidig och stegvis återkoppling, inte som en sen kontrollpunkt.
- Samordning ska framställas som hantering av beroenden, risker och gemensamma möjligheter, inte som byråkrati.

### Progressionsnotering
Kapitel 2 ska bygga vidare på att arkitekten verkar i ett spänningsfält mellan lokal handlingsfrihet och gemensam riktning. Begreppen operativt utvecklingsområde och stödjande/förutsättningsskapande utvecklingsområde kan användas, men bör fördjupas i kapitel 2.


## Etablerat efter kapitel 2

### Centrala definitioner
- Decentraliserad styrning innebär att beslut flyttas nära verksamhet och team, men att gemensamma ramar fortfarande behövs för beslut som påverkar helheten.
- Operativa utvecklingsområden äger verksamhetsnära utveckling och behöver kunna fatta många lokala beslut.
- Stödjande/förutsättningsskapande utvecklingsområden skapar gemensamma förutsättningar som ska göra det enklare för operativa områden att utveckla effektivt och hållbart.
- Mandat ska beskrivas praktiskt: vilka beslut kan teamet fatta själv, vilka bör kvalitetssäkras och vilka behöver samordnas.
- Kvalitetssäkring och samordning ska ske proportionerligt: inte allt ska lyftas, men beslut med beroenden, gemensam påverkan eller långsiktiga konsekvenser ska hanteras tidigt.

### Progressionsnotering
Kapitel 3 ska bygga vidare på spänningen mellan lokal handlingskraft och gemensam riktning. Begreppet styrning är introducerat sedan tidigare, men bör i kapitel 3 fördjupas som möjliggörande styrning snarare än kontroll.


## Etablerat efter kapitel 3

### Centrala definitioner
- Möjliggörande styrning definieras som styrning som hjälper team att fatta bra beslut genom riktning, ramar, stöd och tidig återkoppling.
- Arkitekturell riktning är den gemensamma kurs som gör att lokala lösningar kan passa ihop över tid.
- Guardrails används som praktiska spelregler för vad team kan göra själva, vad som kräver dialog och vad som kräver gemensamt beslut.
- Proportionerlig styrning innebär att styrningens omfattning anpassas efter beslutets påverkan, risk och reversibilitet.

### Progressionsnotering
Kapitel 4 ska bygga vidare på att styrning inte är tillräcklig utan praktisk samordning. Fokus bör flyttas från ramar och riktning till hur arkitekten upptäcker beroenden, kopplar ihop berörda aktörer och minskar dubbelarbete mellan utvecklingsområden.

### Etablerad hållning
Boken ska konsekvent beskriva styrning i agil utveckling som något som bör ske tidigt, begripligt och proportionerligt. Styrning ska inte framställas som motsats till agilitet, utan som ett stöd för hållbara beslut i en decentraliserad miljö.


## Etablerat efter kapitel 4

### Centrala definitioner
- Samordning beskrivs som praktiskt arkitekturarbete där arkitekten upptäcker samband, formulerar beroenden och kopplar ihop rätt aktörer.
- Beroenden kan vara tekniska, informationsmässiga, organisatoriska, tidsmässiga eller ansvarsmässiga.
- Samordningsyta definieras som ett sakområde där flera initiativ, lösningar eller ansvar möts och där dialog behövs.
- Gemensam förmåga används för att skilja mellan det som organisationen behöver kunna gemensamt och den konkreta lösning som kan realisera förmågan.
- Samordning ska framställas som proportionerlig: lättviktig när påverkan är liten och mer strukturerad när konsekvenserna är stora.

### Progressionsnotering
Kapitel 5 ska bygga vidare på kapitel 4 genom att fördjupa kvalitetssäkring som tidig återkoppling. Fokus bör flyttas från att upptäcka och samordna beroenden till hur arkitekten bedömer lösningsval, risker, principer och kvalitet utan att skapa sena hinder.

### Etablerad hållning
Boken ska beskriva samordning som ett sätt att skapa handlingskraft och kvalitet i en decentraliserad organisation. Samordning får inte framställas som central kontroll eller mötesadministration, utan som ett praktiskt sätt att göra beroenden, gemensamma förmågor och konsekvenser synliga i tid.


## Etablerat efter kapitel 5

### Centrala definitioner
- Kvalitetssäkring definieras nu tydligare som tidig, stegvis och proportionerlig återkoppling som hjälper team att fatta bättre beslut.
- Arkitekturgranskning ska framställas som en bedömning av lösningsval, risker och konsekvenser, inte enbart som ett godkännande.
- Kvalitetskriterier används för att göra kvalitet konkret och skapa saklig dialog om lösningsförslag.
- Tidig återkoppling innebär att arkitekten engagerar sig medan vägval fortfarande är öppna.
- Handlingsbar återkoppling ska vara konkret, motiverad, prioriterad och kopplad till möjliga nästa steg.

### Progressionsnotering
Kapitel 6 ska bygga vidare på kvalitetssäkring genom att visa hur arkitekturprinciper används som beslutsstöd. Principer bör introduceras som praktiska hjälpmedel för avvägningar, inte som abstrakta regler eller efterhandsargument.

### Etablerad hållning
Boken ska beskriva kvalitetssäkring som ett sätt att skapa tempo och hållbarhet samtidigt. Den får inte framställas som en sen kontrollpunkt eller som arkitektens möjlighet att stoppa team, utan som ett professionellt stöd för bättre beslut i en decentraliserad och agil organisation.


## Etablerat efter kapitel 6

### Centrala definitioner
- Arkitekturprinciper definieras som praktiska beslutsstöd som uttrycker önskad riktning för återkommande vägval.
- Principer ska framställas som stöd för dialog, kvalitetssäkring och samordning, inte som sena stoppregler.
- Principavvägning innebär att flera principer, kvaliteter eller mål vägs mot varandra och att konsekvenserna görs begripliga.
- Avsteg från principer kan vara rimliga, men ska vara medvetna, motiverade, riskbedömda, dokumenterade och uppföljningsbara.
- Levande principer utvecklas genom praktisk användning och återkoppling från operativa och stödjande utvecklingsområden.

### Progressionsnotering
Kapitel 7 ska bygga vidare på principavvägningar genom att visa hur arkitekturbeslut formuleras, motiveras och dokumenteras så att andra kan förstå beslutet i efterhand. Fokus bör flyttas från principer som stöd för beslut till spårbarhet kring själva beslutet.

### Etablerad hållning
Boken ska beskriva arkitekturprinciper som något som skapar handlingsförmåga när de används tidigt och konkret. Principer ska inte framställas som abstrakta regler eller som argument för central kontroll, utan som gemensamma stöd för bättre lokala beslut i en decentraliserad organisation.

## Uppdatering efter kapitel 7

### Nya introducerade begrepp
- Arkitekturbeslut: ett vägval som påverkar lösningens struktur, kvalitet, ansvar eller framtida handlingsutrymme.
- Spårbarhet: sambandet mellan behov, alternativ, beslut, motivering, konsekvens och uppföljning.
- Beslutslogg: en samlad plats där viktiga arkitekturbeslut kan hittas, förstås och följas upp.

### Kontinuitetsnotering
Kapitel 7 knyter samman tidigare begrepp om styrning, samordning, kvalitetssäkring och arkitekturprinciper genom att visa hur konkreta vägval kan göras begripliga och möjliga att ompröva. Beslut ska dokumenteras på rätt nivå och användas som stöd för lärande, inte som administrativ belastning.

### Scenario
Den digitala tjänsten behöver välja integrationsmönster. Beslutet används för att visa hur alternativ, motivering, beroenden, konsekvenser och uppföljning kan dokumenteras utan att skapa tung dokumentation.


## Uppdatering efter kapitel 8

### Nya introducerade begrepp
- Förutsättningsskapande arbete: arbete som skapar gemensamma förutsättningar för operativa utvecklingsområden.
- Gemensam tjänst: en tjänst eller komponent som flera utvecklingsområden kan använda för återkommande behov.
- Återanvändbar lösning: en lösning, komponent eller ett mönster som kan användas i flera sammanhang.
- Lokal anpassning: en anpassning för ett specifikt operativt behov som behöver bedömas mot gemensamma konsekvenser.

### Kontinuitetsnotering
Kapitel 8 fördjupar relationen mellan operativa och stödjande/förutsättningsskapande arkitekter. Boken ska fortsätta beskriva detta som ett ömsesidigt samspel, inte som en konflikt mellan lokalt självbestämmande och central kontroll. Gemensamma förutsättningar ska framställas som värdefulla när de är begripliga, användbara och möjliga att förbättra utifrån operativa erfarenheter.

### Scenario
Den digitala tjänsten behöver notifieringsfunktionalitet. Kapitlet använder detta för att visa hur operativa och stödjande arkitekter kan pröva om en gemensam tjänst räcker, behöver förbättras eller tillfälligt behöver kompletteras med en lokal lösning.

### Progressionsnotering
Kapitel 9 ska bygga vidare på detta genom att fördjupa avvikelser och lokala lösningar. Fokus bör vara när avsteg är rimliga, hur de dokumenteras och hur de hindras från att bli omedveten teknisk skuld.


## Etablerat efter kapitel 9

### Centrala definitioner
- En lokal lösning är inte automatiskt ett problem; den blir arkitekturellt viktig när den påverkar andra, skapar ny förvaltning eller avviker från gemensam riktning.
- En avvikelse ska beskrivas som ett medvetet avsteg från princip, riktlinje, målarkitektur eller gemensam lösning.
- Riskacceptans ska vara ett tydligt beslut med motivering, mandat och uppföljningspunkt.
- Kompensatoriska åtgärder används för att minska risken med en avvikelse utan att avvikelsen nödvändigtvis tas bort.
- Återkommande avvikelser kan vara en signal om att gemensamma principer, riktlinjer eller tjänster behöver förbättras.

### Progressionsnotering
Kapitel 10 ska bygga vidare på att lokala lösningar och avvikelser kan skapa långsiktiga konsekvenser om de inte följs upp. Fokus bör flyttas från enskilda avsteg till hur teknisk och arkitekturell skuld uppstår, synliggörs och hanteras över tid.


## Etablerat efter kapitel 10

### Centrala definitioner
- Teknisk skuld beskrivs som framtida friktion som uppstår genom vägval över tid.
- Skuld kan vara medveten, omedveten eller ackumulerad.
- Medveten skuld kan vara rimlig när den är dokumenterad, motiverad, tidsatt, ägarsatt och accepterad på rätt nivå.
- Långsiktig hållbarhet handlar om begriplighet, förvaltningsbarhet, säkerhet, förändringsbarhet och rimligt ansvar under lösningens avsedda livslängd.
- Skuld ska beskrivas genom konkreta konsekvenser, inte användas som abstrakt kritik.

### Kontinuitetsnotering
Kapitel 10 kopplar ihop avvikelser, lokala lösningar och teknisk skuld. Boken ska fortsätta behandla skuld som en naturlig konsekvens av vägval, inte som ett moraliskt fel. Arkitekten ska framställas som den som gör skuld begriplig, prioriterbar och hanterbar.

### Scenario
Den lokala notifieringslösningen från kapitel 9 börjar användas av fler och skapar risk för parallella mönster, otydligt ansvar och högre förvaltningskostnad. Kapitlet visar hur operativa och stödjande arkitekter kan göra skulden synlig och koppla den till förbättring av den gemensamma notifieringstjänsten.

### Progressionsnotering
Kapitel 11 ska bygga vidare på hur skuld, beslut, kvalitetssäkring och samordning kan integreras i teamens vardag. Fokus bör flyttas från vad arkitekten bör uppmärksamma till när och hur arkitekturarbetet sker i backlogg, planering, refinement och leveransflöde.


## Etablerat efter kapitel 11

### Centrala definitioner
- Kontinuerlig arkitektur innebär att arkitekturella frågor hanteras löpande i teamens ordinarie flöde, inte som separat slutkontroll.
- Arkitekturell backlogg ska förstås som synliggjort arkitekturellt arbete i eller kopplat till teamets befintliga backlogg.
- Refinement är etablerat som en central plats för tidig kvalitetssäkring, eftersom behov, osäkerheter och vägval blir synliga där.
- Arkitekturell signal är en praktisk indikation på att ett vägval kan behöva kvalitetssäkras eller samordnas.
- Kvalitetssäkring och samordning bör planeras som arbete, inte läggas ovanpå teamens flöde som osynliga sidouppgifter.

### Progressionsnotering
Kapitel 12 ska bygga vidare på att arkitekturfrågor behöver hanteras i teamens vardag. Fokus flyttas från arbetssätt till relation och påverkan: hur arkitekten skapar förtroende, förklarar konsekvenser och gör styrning begriplig utan att uppfattas som extern kontroll.


## Uppdatering efter kapitel 12

Kapitel 12 introducerar förtroende som en praktisk förutsättning för fungerande arkitekturarbete i en decentraliserad organisation. Arkitekten beskrivs inte som extern kontrollant utan som en medskapande aktör som hjälper team och beslutsfattare att förstå konsekvenser, samordningsbehov och kvalitetssäkringsbehov i tid.

### Nya eller förtydligade begrepp
- Förtroende: praktisk grund för att arkitekten ska få tillgång till tidiga frågor och kunna påverka konstruktivt.
- Medskapande arkitekt: arkitekt som stödjer vägval genom dialog, analys och nästa steg.
- Påverkan utan övertagande: att hjälpa team fatta bättre beslut utan att ta över deras ansvar.
- Måste, bör och kan: struktur för att tydliggöra skillnaden mellan krav, starka rekommendationer och valbara alternativ.

### Kontinuitetsregel
När kommande kapitel beskriver organisatoriskt lärande och arkitekturmognad ska de bygga vidare på att förtroende skapas genom konkret nytta, tydlig kommunikation och återkommande uppföljning.


## Etablerat efter kapitel 13

### Centrala definitioner
- Gemensam arkitekturmognad definieras som organisationens praktiska förmåga att förstå, diskutera, kvalitetssäkra och samordna arkitektur på ett tillräckligt konsekvent sätt.
- Mognad ska beskrivas som beteenden och organisatorisk förmåga, inte som enbart modeller, mallar eller forum.
- Kvalitetssäkring kan användas som lärandetillfälle när återkommande brister, avvikelser eller riskmönster synliggör behov av bättre gemensamma förutsättningar.
- Samordning på mognadsnivå handlar om att se mönster över tid och omvandla erfarenheter till gemensamma vägledningar, lösningsmönster eller tjänster.
- Motiverad variation skiljs från oönskad spretighet. Decentralisering ska tillåta lokala anpassningar men inte omedveten komplexitet.

### Progressionsnotering
Kapitel 14 ska knyta samman hela boken och visa hur arkitekturarbete kan gå från att uppfattas som kontroll till att fungera som möjliggörande arkitektur.


## Etablerat efter kapitel 14

### Centrala definitioner
- Möjliggörande arkitektur definieras som arkitekturarbete som hjälper team och utvecklingsområden att fatta bättre beslut tidigare, med tydlig riktning, proportionerlig kvalitetssäkring och träffsäker samordning.
- Balanserad styrning innebär att skilja mellan beslut som team kan fatta själva, beslut som kräver dialog eller kvalitetssäkring och beslut som behöver gemensam hantering.
- Gemensam riktning är den delade förståelse för mål, principer, guardrails och förmågor som gör att decentraliserade initiativ kan utvecklas lokalt utan att tappa helheten.

### Progressionsnotering
Kapitel 14 avslutar första kapitelutkastet genom att knyta ihop bokens återkommande teman: riktning, sammanhang, kvalitet, samordning, spårbarhet, förtroende och organisatoriskt lärande.

### Etablerad hållning
Boken ska konsekvent beskriva arkitekturstyrning som möjliggörande när den sker tidigt, tydligt, proportionerligt och lärande. Kvalitetssäkring och samordning ska framställas som praktiska stöd för bättre utveckling, inte som separata kontrollspår.

## Inledning
- Inledningen beskriver bokens syfte, målgrupp, användning och grundsyn.
- Inledningen ska placeras före kapitel 1 i export och läsordning.

## Metadata
- Författare: Erland Lindmark
