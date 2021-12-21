# ZoneCovidItalia
Visualizzazione grafica delle restrizioni regionali per covid ("colori") in vigore da novembre 2020

![image](https://user-images.githubusercontent.com/1620953/146897772-df97e7b3-64e4-48e4-9303-76b4aebaa4e3.png)

Il DPCM del 3 novembre 2020 ha istituito la suddivisione dell'Italia in "zone colorate" a seconda della gravità della situazione-covid, secondo questo schema:

- Zona bianca: art. 1, comma 11
- Zona gialla: art. 1
- Zona arancione: art. 2
- Zona rossa: art. 3

La [Protezione Civile](https://github.com/pcm-dpc/COVID-19) mette a disposizione [un file .json](https://github.com/pcm-dpc/COVID-19/tree/master/aree/geojson) contenente i dati relativi alle colorazioni, ma si tratta di un file di dimensioni enormi (30 MB zippato, 180 MB decompresso), perchè contiene anche informazioni grafiche sui confini di regione, che però ovviamente sono costanti, cosa che rende del tutto inutile scaricarli ogni volta; nonostante le richieste pervenute da più parti, non è stato possibile convincere il proprietario del repository a fornire un file più sello contenente solo i dati sui colori, quindi alcune persone hanno fatto da sè, mettendo a disposizione il loro lavoro su github:

- [covid19italia](https://github.com/ondata/covid19italia/blob/master/webservices/COVID-19Aree/processing/) (file [areeStorico.csv](https://raw.githubusercontent.com/ondata/covid19italia/master/webservices/COVID-19Aree/processing/areeStorico.csv)) - Estratto del file della protezione civile, coi soli colori
- [CloudItaly](https://github.com/CloudItaly/Indice-RT/) (file [colori.json](https://raw.githubusercontent.com/CloudItaly/Indice-RT/main/colori.json)) - File json ragguppato per ordinanze, parte da gennaio 2021
- [imcatta](https://github.com/imcatta/restrizioni_regionali_covid/) (file [dataset.csv](https://raw.githubusercontent.com/imcatta/restrizioni_regionali_covid/main/dataset.csv)) - file CSV ordinato per regione, parte dall'inizio (nov 2020)

Al momento il grafico è basato sui [dati](https://github.com/imcatta/restrizioni_regionali_covid/blob/main/dataset.json) presi da [repository imcatta/restrizioni_regionali_covid](https://github.com/imcatta/restrizioni_regionali_covid/) (--> [dati grezzi JSON](https://raw.githubusercontent.com/imcatta/restrizioni_regionali_covid/main/dataset.json)), l'unico costantemente aggiornato; versioni precedenti si basavano su altri repository:

- https://win98.altervista.org/coronavirus/grafico-colori-regioni-covid-zone-210.html ([dati](https://github.com/ondata/covid19italia/tree/master/webservices/COVID-19Aree/processing) di [onData](https://github.com/ondata/))
- https://win98.altervista.org/coronavirus/grafico-colori-regioni-covid-zone.html ([dati](https://raw.githubusercontent.com/CloudItaly/Indice-RT/main/colori.json) di [CloudItaly](https://raw.githubusercontent.com/CloudItaly/))


Riferimenti normativi:

[Elenco provvedimenti COVID-19 (Openpolis.it)](https://www.openpolis.it/coronavirus-lelenco-completo-degli-atti/)


