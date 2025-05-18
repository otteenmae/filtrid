# Gümnaasiumi uurimistöö "Tartu Ülikooli Tartu Observatooriumi 1.5-meetrise teleskoobi fotomeetri filtrite karakteriseerimine" elektroonilised lisad

Autor: Ott Eenmäe
Juhendajad: Tõnis Eenmäe ja Ruth Maal
Töö esitamise kuupäev: 2025-05-16

Selles GitHubi repositooriumis on kättesaadavaks tehtud uurimistöö viimane versioon koos kõigi andmefailidega.

# Repositooriumi kataloogipuu

Juurkataloogis on litsents, käesolev dokument ja uurimistöö täisteks PDF-formaadis. Alamkataloogid on järgnevad:

## Kataloog andmefailid
Siin on kõik originaalsed ja arvutatud andmefailid

Töös leitud värviülekande ja värvusindeksi ülekande võrrandite kordajad on TAB-iga eraldatud väljadega ASCII failides (vt. töö peatükk 3):
- varviulekande_kordajad_tabel3.dat
- varvusindeksi_ulekande_kordajad_tabel4.dat


### Kataloog filtrid
Selles kataloogis on originaalandmed Benthami monokromaatorist, selle alamkataloogid on erinevad filtrite nimelised kataloogid. Suurte tähtedega on Johnson-Cousins filtrid, väiketähtedega Sloani filtrid. Mitte-standardsete filtrite mõõtmised on kataloogides Halpha, Luminance ja exoBB.

Eraldi kataloogides on monokromaatori valgusallika stabiilsuse uurimise (lambi_stabiilsus_alguses) ja kiire ülevaatespektrite (fullscan_kiire) mõõtmiste kataloogid. Lisatud on kataloog Standard_filtrid, mis pärinevad [SVO filtrite profiilide teenusest](https://svo2.cab.inta-csic.es/theory/fps/).

Benthami monokromaatorist pärit failides on asjasse puutuvad andmetulbad esimene ja teine -- lainepikkus nanomeetrites ja mõõdetud signaal.

### Kataloog filtrid_detailne
Siin on kõigi mõõdetud filtrite tiheda sammu ja paljude kordustega mõõtmistulemused - selle töö otsene tulemus. Failid on 2-tulbalised ASCII failid, mille esimene tulp on lainepikkus ongströmides ja teine tulp on filtri läbilaskvus.

Nende arvutamiseks kasutati Jupyteri töölehte Filtrite_koverate_genereerimine.ipynb

### Kataloog filtrid_ulevaade
Siin on kõigi mõõdetud filtrite kiiresti mõõdetud mõõtmistulemused kogu mõõtevahemikus (300-1200 nm) - ka selle töö otsene tulemus. Failid on 2-tulbalised ASCII failid, mille esimene tulp on lainepikkus ongströmides ja teine tulp on filtri läbilaskvus.

Ka nende arvutamiseks kasutati Jupyteri töölehte Filtrite_koverate_genereerimine.ipynb


### Kataloog teleskoop_ja_ccd
Siia on kogutud fotomeetris kasutatava EMCCD-kaamera iXon Ultra 888 CCD-sensori kvantefektiivsuse kõver (ccd_efektiivsus.dat) ja selle kaamera sisendakna efektiivsuse kõver (ccd_akna_efektiivsus.dat). Need andmed on pärit [Andor Technologies kaamera akna valimise veebitööriistast](https://andor.oxinst.com/tools/camera-window-selector)

Teleskoobi läbilaskekõver pärineb Tartu Observatooriumis olemas olevast dokumentatsioonist teleskoobi pinnakatete kohta.


## Kataloog joonised
Siin kataloogis on toodud kõik töös kasutatud joonised PDF-formaadis failidena. Failide nimed on isedokumenteerivad.

Kataloogis on kõigi mõõdetud filtrite kiire ülevaate joonised: failid nimega filtri_ulevaade_<filtri_nimi>.pdf

Ülevaatejoonised tehti Jupyteri töölehega Filtrite_koverate_genereerimine.ipynb

### Kataloog filtrid_detailne_mittestandard
Siin on Halpha, Luminance ja exoBB filtrite detailsete läbilaskekõverate joonised.

Mittestandardsüsteemi filtrite joonised tehti Jupyteri töölehega Filtrite_koverate_genereerimine.ipynb

### Kataloog filtrid_detailne_standardiga
Siin on kõigi mõõdetud standardsete fotomeetriliste süsteemide filtrite kõverad võrrelduna nende filtrite standardsete läbilaskekõveratega.

Ülevaatejoonised tehti Jupyteri töölehega Filtrite_koverate_genereerimine.ipynb

### Kataloog regressioonid_varviulekanne
Töös leitud värviülekande võrrandite lahendamise tulemuste esitamise joonised regressioonisirgetega.

Ülevaatejoonised tehti Jupyteri töölehega Synteetiline_fotomeetria_ja_regressioonid.ipynb

### Kataloog regressioonid_varvusindeks
Töös leitud värvusindeksi ülekandevõrrandite lahendamise tulemuste esitamise joonised regressioonisirgetega.

Ülevaatejoonised tehti Jupyteri töölehega Synteetiline_fotomeetria_ja_regressioonid.ipynb

## Kataloog python
Siin asuvad töös loodud Jupyteri töölehed, millega tehti kogu analüüs. Need loodi kasutades Pythoni versiooni 3.12.7 ja Jupyterlab'i versiooni 4.3.4.

- Jupyteri tööleht Filtrite_koverate_genereerimine.ipynb filtrite läbilaskekõverate arvutamiseks
- Jupyteri tööleht Synteetiline_fotomeetria_ja_regressioonid.ipynb sünteetilise fotomeetria ja värviülekandevõrrandite lahendamiseks.

