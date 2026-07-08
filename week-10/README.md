# Nädal 10 – tervikportfoolio ja lõpuesitlus

## Lühikontekst

Nädala 10 meeskonnatöö eesmärk oli võtta kokku UrbanStyle'i kümne nädala andmetöö ning esitada juhatusele peamised leiud, äriline mõju ja AI kasutamise õppetunnid. Meeskonna ühine lõpuesitlus on [Google Slidesis](https://docs.google.com/presentation/d/1iBQHFeCvxdUea-CU_Zz2cQaKRO6UKCX90DvVh5Q3hh0/edit?usp=sharing).

## Minu panus

Minu vastutus oli esitluse Pythoni, RFM-analüüsi ja AI kasutamise osa. Koostasin ning esitlesin:

- [slaidi 5 – „Python – Sirja”](https://docs.google.com/presentation/d/1iBQHFeCvxdUea-CU_Zz2cQaKRO6UKCX90DvVh5Q3hh0/edit?slide=id.p5#slide=id.p5), kus tõin välja RFM-analüüsi põhitulemused ja automatiseeritud töövoo;
- [slaidi 7 – „AI kasutamine – õpetajast kaaspiloodiks – Sirja”](https://docs.google.com/presentation/d/1iBQHFeCvxdUea-CU_Zz2cQaKRO6UKCX90DvVh5Q3hh0/edit?slide=id.p7#slide=id.p7), kus kirjeldasin AI rolli õppimisel, analüüsis ja kommunikatsioonis ning inimese vastutust tulemuste eest.

### RFM-analüüsi põhitulemused

- **422 VIP-klienti** ehk 17% klientidest andsid **42% käibest** – neile sobib sihitud VIP-programm.
- **502 riskiklienti** moodustasid 20% klientidest – neid tuleks personaalse pakkumisega tagasi võita.
- **713 potentsiaalset lojaalset klienti** moodustasid 29% klientidest – nende kordusoste tuleks kasvatada.

Analüüsi aluseks ja tehniliseks väljundiks olid [minu RFM-notebook](../week-7/individual/week7_rfm_D.ipynb), [meeskonna terviknotebook](../week-7/team/week7_rfm_complete.ipynb) ning [segmenteeritud tulemused](../week-7/individual/rfm_segments.csv).

### Automatiseeritud Pythoni töövoog

Esitluses võtsin kokku töövoo:

`Supabase API → andmete puhastamine ja ühendamine → KPI-d → Plotly → CSV/HTML`

Töövoo eesmärk oli teha korduv aruandlus ühe käivitusega, vähendada käsitööd ja vigade ohtu ning anda korratav tulemus. Seotud artefaktid on [minu API andmelaadija](../week-8/individual/data_fetcher.py) ja [meeskonna pipeline'i demo](../week-8/team/week8_pipeline_demo.md).

## AI kasutamine

Kasutasin AI-d õppimise ja tehnilise toe kaaspiloodina:

- NotebookLM/RAG aitas õppematerjalidest vajalikku infot leida;
- AI aitas selgitada SQL-i ja Pythoni veateateid ning koodi siluda;
- AI aitas täiustada RFM-analüüsi ja dashboard'ide visuaalset selgust;
- AI aitas korrastada README-sid, annotatsioone ja ärisoovituste sõnastust.

AI väljundeid ei kasutanud ma kontrollimata. Käivitasin koodi ise, kontrollisin tulemusi pärisandmetega ning tegin lõplikud järeldused ja otsused ise. Minu peamine õppetund oli, et AI kiirendab tööd, kuid ei asenda analüütilist mõtlemist ega vastutust tulemuse eest.

## Tulemus ja õppetund

Suurim väärtus oli tehnilise analüüsi tõlkimine juhatusele arusaadavaks otsuseks: esmalt segmentida kliendid ning seejärel automatiseerida müügiaruandlus. RFM-analüüsi numbrid annavad selge aluse VIP-klientide hoidmiseks, riskiklientide tagasivõitmiseks ja potentsiaalsete lojaalsete klientide kasvatamiseks.

Minu peamine õppetund oli, et hea analüüs ei lõpe töötava koodiga. Tulemus peab olema kontrollitud, korratav ja sõnastatud nii, et selle põhjal saab teha konkreetse äriotsuse.
