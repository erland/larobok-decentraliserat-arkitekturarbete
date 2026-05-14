# EPUB-exportunderlag

Detta dokument beskriver vad som behöver användas vid framtida EPUB-export.

## Metadata

- Titel: Arkitektens vardag i en decentraliserad myndighet
- Undertitel: Praktisk styrning, samordning och kvalitetssäkring av arkitektur
- Författare: Erland Lindmark
- Språk: sv
- Utgåva: 1
- Version: 0.15

Den primära metadatafilen är `docs/export-metadata.yaml`. Den ska användas som källa för kapitelordning, titel, författare, språk och exportinställningar.

## Kapitelordning

EPUB-exporten ska följa ordningen i `chapters`-listan i `docs/export-metadata.yaml`. Inledningen ligger före kapitel 1:

1. `chapters/00-inledning.md`
2. `chapters/01-vad-arkitekturarbete-egentligen-handlar-om.md`
3. `chapters/02-den-decentraliserade-arkitektens-vardag.md`
4. `chapters/03-varfor-styrning-behovs-aven-i-agil-utveckling.md`
5. `chapters/04-samordning-som-praktiskt-arkitekturarbete.md`
6. `chapters/05-kvalitetssakring-utan-att-bromsa-utvecklingen.md`
7. `chapters/06-arkitekturprinciper-i-praktiken.md`
8. `chapters/07-arkitekturbeslut-och-sparbarhet.md`
9. `chapters/08-operativa-och-stodjande-arkitekter-tillsammans.md`
10. `chapters/09-att-hantera-avvikelser-och-lokala-losningar.md`
11. `chapters/10-teknisk-skuld-och-langsiktig-hallbarhet.md`
12. `chapters/11-arkitektur-i-teamens-flode.md`
13. `chapters/12-att-bygga-fortroende-som-arkitekt.md`
14. `chapters/13-gemensam-arkitekturmognad.md`
15. `chapters/14-fran-kontroll-till-mojliggorande-arkitektur.md`

## Rekommenderad exportprincip

Vid export bör kapitel sammanfogas i metadataordning. Rubriker i Markdown ska behållas och användas för EPUB-navigering. Omslagsbild, ISBN eller publiceringsinformation kan kompletteras senare i `docs/export-metadata.yaml`.
