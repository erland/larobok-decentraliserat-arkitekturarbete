# Kapitel 3: Varför styrning behövs även i agil utveckling

## Varför detta kapitel finns

När en organisation ställer om till agil utveckling kan ordet styrning uppfattas som något som hör till det gamla arbetssättet. Det kan associeras med långa beslutsvägar, omfattande dokumentation, sena granskningar och styrgrupper långt från teamens vardag. Om styrning förstås på det sättet är det naturligt att många vill undvika den.

Men arkitekturstyrning behöver inte betyda detaljkontroll. Rätt använd är styrning ett sätt att göra det enklare för team att fatta bra beslut i rätt tid. Den skapar gemensam riktning, tydliga ramar och stöd i de frågor där ett lokalt beslut kan påverka andra delar av organisationen.

I en decentraliserad myndighet blir detta särskilt viktigt. Många utvecklingsområden arbetar parallellt, ofta med egna mål, prioriteringar och tidplaner. Utan någon form av gemensam styrning riskerar organisationen att få lösningar som var för sig verkar rimliga men som tillsammans blir svåra att förvalta, samordna och vidareutveckla.

Det här kapitlet beskriver varför styrning behövs även i agil utveckling, hur arkitekten kan bidra till möjliggörande styrning och när styrning bör kopplas till kvalitetssäkring och samordning.

## Lärandemål

Efter kapitlet ska läsaren kunna:

- förklara skillnaden mellan möjliggörande styrning och detaljkontroll
- beskriva varför agil utveckling fortfarande behöver gemensamma ramar
- identifiera beslut som bör styras, kvalitetssäkras eller samordnas tidigt
- använda guardrails som praktiskt stöd för teamens beslut
- agera som arkitekt på ett sätt som stärker både tempo och långsiktig hållbarhet

## Innan vi börjar

I kapitel 1 beskrevs arkitekturarbete som praktiskt arbete med riktning, sammanhang och kvalitet. I kapitel 2 fördjupades bilden av den decentraliserade arkitektens vardag, där lokalt ansvar behöver balanseras mot gemensamma förutsättningar.

Det här kapitlet bygger vidare på samma spänningsfält. Frågan är inte om team ska få fatta beslut. Frågan är vilka beslut som bör fattas lokalt, vilka beslut som behöver gemensamma ramar och vilka beslut som behöver samordnas eftersom konsekvenserna når utanför det egna utvecklingsområdet.

Tre begrepp är centrala:

- **Möjliggörande styrning**: styrning som hjälper team att fatta bra beslut genom riktning, ramar, stöd och tidig återkoppling.
- **Arkitekturell riktning**: den gemensamma kurs som hjälper organisationen att utveckla lösningar som passar ihop över tid.
- **Guardrails**: tydliga ramar eller spelregler som anger vad team kan göra fritt, vad som kräver dialog och vad som kräver gemensamt beslut.

## Huvudförklaring

### Agilt arbetssätt tar inte bort behovet av styrning

Agil utveckling betonar snabb återkoppling, lärande, tät kontakt med verksamheten och förmågan att anpassa sig när ny kunskap uppstår. Det är värdefullt i en myndighet där behov, regelverk, teknik och förväntningar kan förändras över tid.

Men agilitet betyder inte att varje team bör optimera sin lösning helt isolerat. Ett team kan göra ett snabbt och rimligt val utifrån sitt uppdrag, men samma val kan skapa problem för integrationer, informationshantering, säkerhet, förvaltning eller andra utvecklingsområden.

Därför behövs arkitekturstyrning också i agil utveckling. Inte för att ersätta teamens ansvar, utan för att hjälpa teamen att förstå vilka ramar som redan finns, vilka konsekvenser olika val får och när fler behöver involveras.

### Problemet är inte styrning, utan fel sorts styrning

Många negativa erfarenheter av styrning kommer från situationer där styrningen sker för sent, är för generell eller saknar koppling till teamens verkliga beslut.

Fel sorts styrning kännetecknas ofta av att den:

- kommer in när lösningen redan är byggd
- fokuserar mer på formalia än på verkliga risker
- ger besked utan dialog
- kräver omfattande underlag innan osäkerheten är rimligt utredd
- behandlar alla beslut som lika viktiga
- gör arkitekten till granskare i stället för medskapare

Möjliggörande styrning fungerar annorlunda. Den försöker komma in tidigt, när vägval fortfarande är möjliga att påverka. Den hjälper teamet att förstå vad som är fritt, vad som behöver kvalitetssäkras och vad som behöver samordnas med andra.

### Styrning bör vara proportionerlig

Alla beslut behöver inte samma nivå av styrning. En viktig del av arkitektens vardag är att bedöma proportioner.

Ett lokalt val som bara påverkar en intern komponent kan ofta hanteras inom teamet. Ett val som påverkar informationsmodell, integrationer, gemensam plattform, säkerhet, åtkomst, förvaltning eller användning av gemensamma tjänster kräver däremot ofta mer samordning och kvalitetssäkring.

En praktisk tumregel är att ställa tre frågor:

1. Påverkar beslutet fler än det egna teamet eller utvecklingsområdet?
2. Är beslutet svårt, dyrt eller riskabelt att ändra senare?
3. Påverkar beslutet gemensamma principer, information, säkerhet eller tekniska förutsättningar?

Om svaret är ja på någon av frågorna bör arkitekten överväga tidig styrning, kvalitetssäkring eller samordning.

### Guardrails gör styrning begriplig

Guardrails är ett praktiskt sätt att göra styrning användbar i vardagen. De fungerar som tydliga spelregler snarare än detaljerade instruktioner för varje situation.

Ett bra guardrail kan till exempel säga:

- vilka typer av lösningar som bör återanvända gemensamma förmågor
- när en integration ska diskuteras med ett stödjande utvecklingsområde
- vilka säkerhets- eller informationskrav som alltid måste beaktas
- vilka teknikval som är rekommenderade, accepterade eller kräver särskilt beslut
- när en avvikelse behöver dokumenteras och följas upp

Guardrails bör inte vara så breda att de blir självklara men oanvändbara. De bör inte heller vara så detaljerade att de hindrar teamet från att lösa sitt uppdrag. Värdet ligger i att de hjälper teamet att se när ett beslut är lokalt och när det berör helheten.

### Arkitekten som översättare mellan riktning och vardag

I en agil och decentraliserad organisation behöver arkitekten ofta översätta mellan olika perspektiv.

För teamet behöver arkitekten kunna förklara varför en gemensam princip eller ram är relevant i just deras situation. För stödjande eller styrande forum behöver arkitekten kunna förklara vilka behov, osäkerheter och praktiska begränsningar teamet faktiskt har.

Det gör arkitektens roll mindre som kontrollant och mer som möjliggörare. Arkitekten hjälper organisationen att fatta beslut som är tillräckligt bra nu, men inte skapar onödiga problem senare.

## Scenario: Snabba teknikval i den nya digitala tjänsten

Det operativa utvecklingsområdet som arbetar med den nya digitala tjänsten behöver snabbt välja teknisk lösning för en central del av tjänsten. Teamet har hittat ett alternativ som verkar passa väl för den första leveransen. Det är enkelt att komma igång, utvecklarna kan tekniken och lösningen skulle minska tiden till första resultat.

Arkitekten ser samtidigt att valet kan få konsekvenser utanför teamet. Lösningen behöver hantera information som även används av andra utvecklingsområden. Den behöver integrera med befintliga tjänster. Den kan också påverka hur säkerhet, åtkomst och förvaltning ska fungera över tid.

I ett detaljstyrt arbetssätt skulle arkitekten kanske stoppa valet och kräva en fullständig utredning innan teamet får gå vidare. I ett helt ostyrt arbetssätt skulle teamet kanske bygga vidare och hantera problemen senare.

Ett möjliggörande arbetssätt är att arkitekten hjälper teamet att snabbt sortera beslutet:

- Vad behöver vara klart nu för att teamet ska kunna fortsätta?
- Vilka delar av beslutet är reversibla och kan justeras senare?
- Vilka delar kan påverka andra utvecklingsområden?
- Vilka gemensamma guardrails gäller för information, integration och säkerhet?
- Behöver ett stödjande utvecklingsområde involveras innan lösningen låses?

Resultatet blir inte nödvändigtvis ett nej. Det kan bli ett ja med villkor, ett tillfälligt vägval, en avvikelse med uppföljning eller en justerad lösning som bättre passar både teamets behov och organisationens helhet.

## Vad arkitekten bör tänka på

Arkitekten bör särskilt vara uppmärksam på beslut som verkar små i teamets vardag men som kan bli stora i organisationens helhet. Det gäller till exempel val av integrationsmönster, informationsägarskap, säkerhetslösningar, datalagring, beroenden till gemensamma plattformar och återanvändning av befintliga förmågor.

Arkitekten bör också skilja mellan osäkerhet och risk. Allt som är oklart behöver inte stoppas. Men sådant som är oklart och samtidigt kan få stora konsekvenser behöver hanteras aktivt. Det kan ske genom en kort analys, en dialog med berörda arkitekter, en tidsbegränsad avvikelse eller ett beslut med tydliga antaganden.

En annan viktig sak är att styrning behöver vara begriplig för teamet. Om arkitekten säger att något måste kvalitetssäkras bör det vara tydligt varför. Är det för att beslutet påverkar säkerhet? För att det skapar beroenden? För att det avviker från en gemensam riktning? För att det kan bli dyrt att ändra senare?

När orsaken är tydlig blir styrningen lättare att acceptera.

## När kvalitetssäkring bör ske

Kvalitetssäkring bör ske tidigt när ett beslut:

- påverkar säkerhet, informationshantering eller regelefterlevnad
- berör gemensamma plattformar, tjänster eller tekniska riktlinjer
- skapar nya integrationer eller förändrar befintliga informationsflöden
- innebär ett teknikval som kan bli svårt att byta senare
- avviker från kända principer, målarkitektur eller guardrails
- får konsekvenser för förvaltning, drift eller långsiktig utvecklingsbarhet
- bygger på antaganden som ännu inte är förankrade

Kvalitetssäkring bör inte vänta tills lösningen är färdig. Den bör göras när det fortfarande går att påverka vägvalet utan stora omarbetningar.

I praktiken kan kvalitetssäkring vara ett kort samtal, en arkitekturdialog, en genomgång av alternativ, en riskbedömning eller ett beslut om att följa upp en osäkerhet senare. Formen bör anpassas efter beslutets betydelse.

## När samordning bör ske

Samordning bör ske när ett beslut eller en lösning:

- påverkar fler än ett utvecklingsområde
- använder eller förändrar en gemensam förutsättning
- överlappar med initiativ i andra delar av organisationen
- kräver gemensam informationsförståelse
- skapar beroenden i tidplan, teknik, ansvar eller förvaltning
- kan leda till dubbelarbete om andra inte involveras
- behöver stöd från ett stödjande/förutsättningsskapande utvecklingsområde

Samordning bör inte bara ske när det redan finns en konflikt. Den bör användas för att upptäcka beroenden innan de blir problem.

Arkitektens uppgift är ofta att avgöra vilka som behöver prata med varandra, vad som behöver klargöras och vilken nivå av gemensamt beslut som krävs.

## Vanliga fallgropar

- **Fallgrop: Att likställa agilitet med frånvaro av styrning**
  - **Varför det händer:** Team vill undvika långsamma beslutsvägar och uppfattar styrning som motsats till tempo.
  - **Hur man undviker det:** Beskriv styrning som tidigt stöd, tydliga ramar och hjälp att fatta hållbara beslut.

- **Fallgrop: Att styra allt lika mycket**
  - **Varför det händer:** Organisationen vill minska risk men saknar tydliga kriterier för vad som är viktigt.
  - **Hur man undviker det:** Använd proportionerlig styrning. Lägg mest energi på beslut med stor påverkan eller låg reversibilitet.

- **Fallgrop: Att komma in för sent**
  - **Varför det händer:** Arkitekturfrågor lyfts först när teamet behöver ett formellt godkännande.
  - **Hur man undviker det:** Bygg in arkitekturdialog i tidig planering, refinement och större vägval.

- **Fallgrop: Att använda principer utan förklaring**
  - **Varför det händer:** Principerna är kända för arkitekter men inte översatta till teamets konkreta situation.
  - **Hur man undviker det:** Förklara vilken risk principen hanterar och hur den påverkar den aktuella lösningen.

- **Fallgrop: Att göra guardrails för vaga**
  - **Varför det händer:** Man vill skapa generella regler som passar många situationer.
  - **Hur man undviker det:** Formulera guardrails så att team förstår vad de kan göra själva, vad som kräver dialog och vad som kräver beslut.

## Snabb sammanfattning

- Agil utveckling minskar inte behovet av arkitekturstyrning.
- Styrning bör vara möjliggörande, inte detaljkontrollerande.
- Arkitekten hjälper team att förstå vilka beslut som är lokala och vilka som påverkar helheten.
- Guardrails gör styrning praktisk och begriplig.
- Kvalitetssäkring bör ske tidigt när beslut påverkar säkerhet, information, integrationer, gemensamma plattformar eller långsiktig hållbarhet.
- Samordning bör ske innan beroenden och överlapp blir problem.

## Reflektionsfrågor

1. Vilka beslut i ditt utvecklingsområde hanteras idag som lokala, men påverkar egentligen fler?
2. Var uppstår mest friktion mellan agil utveckling och arkitekturstyrning?
3. Vilka guardrails skulle hjälpa teamen att fatta bättre beslut utan att behöva fråga om allt?
4. Vilka kvalitetssäkringar sker för sent idag?
5. Hur kan arkitekter bli bättre på att förklara varför styrning behövs i konkreta situationer?

## Nästa steg

Nästa kapitel går djupare in i samordning som praktiskt arkitekturarbete. Där flyttas fokus från varför styrning behövs till hur arkitekten konkret kan upptäcka beroenden, minska dubbelarbete och skapa gemensam riktning mellan utvecklingsområden.
