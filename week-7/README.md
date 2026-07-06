# Nädal 7: Python ja pandas — RFM-kliendisegmenteerimine

## Minu roll

Roll D: visualiseerimine ja leidude esitamine. Kasutasin Roll C loodud RFM-tabelit, et koostada Plotly diagrammid kliendisegmentide jaotuse, profiili ning kümne suurima VIP-kliendi kohta. Lisaks sõnastasin tulemuste ärilise tähenduse ja soovitused Markole.

## Meetod

RFM-analüüs hindab iga kliendi puhul kolme näitajat:

- **Recency:** kui hiljuti klient viimati ostis;
- **Frequency:** kui sageli klient ostab;
- **Monetary:** kui palju klient kokku kulutab.

Nende põhjal jagati kliendid segmentidesse `VIP Champions`, `Loyal`, `Potential`, `At Risk` ja `Lost`.

## Peamised leiud

- Analüüs hõlmas 2454 klienti ja ligikaudu 2,49 miljoni euro väärtuses oste.
- 422 `VIP Champions` klienti moodustasid vaid 17,2% kliendibaasist, kuid genereerisid 41,7% käibest ehk ligikaudu 1,04 miljonit eurot.
- `Potential` oli suurim segment: 713 klienti ehk 29,1% kliendibaasist. Neid saab lojaalsusprogrammi ja sihitud pakkumistega kasvatada väärtuslikumateks klientideks.
- `Loyal` segmenti kuulus 697 klienti, kes andsid 31,2% käibest. Koos VIP-klientidega genereerisid nad 72,8% kogukäibest.
- `At Risk` ja `Lost` segmentides oli kokku 622 klienti. Nende keskmisest viimasest ostust oli möödunud vastavalt ligikaudu 297 ja 487 päeva, mistõttu vajavad nad kiiret tagasivõitmise kampaaniat.
- RFM-segmendid põhinevad tegelikul ostukäitumisel. Neid tasub võrrelda olemasoleva `loyalty_tier` väljaga, et leida vastuolud ametliku staatuse ja kliendi päris käitumise vahel.

## Ärilised soovitused

- Hoida `VIP Champions` kliente varajase ligipääsu, tasuta saatmise ja personaalse teenindusega.
- Suunata `Potential` klientidele kordusostu soodustavad pakkumised, sest nad moodustavad suurima kasvupotentsiaaliga rühma.
- Käivitada `At Risk` klientidele ajaliselt piiratud tagasivõitmise kampaania ning käsitleda `Lost` segmenti eraldi madalama kuluga automatiseeritud kampaanias.

## Väljundid

- [Minu Roll D notebook](individual/week7_rfm_D.ipynb)
- [RFM-segmentide CSV](individual/rfm_segments.csv)
- [Meeskonna terviklik notebook](team/week7_rfm_complete.ipynb)

Individuaalne notebook sisaldab Roll D osa ja eeldab sisendina Roll C loodud `rfm_viz` DataFrame'i. Terviklik töövoog on meeskonna notebook'is.

## AI kasutamine

Kasutasin AI-d Plotly visualiseeringute paigutuse ja värvikasutuse parandamiseks ning äriliste soovituste selgemaks sõnastamiseks. Kontrollisin tulemused RFM-andmete ja diagrammide põhjal ise üle.
