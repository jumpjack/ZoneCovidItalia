# ZoneCovidItalia
Visualizzazione grafica delle restrizioni regionali per covid ("colori") in vigore da novembre 2020

![image](https://user-images.githubusercontent.com/1620953/146897772-df97e7b3-64e4-48e4-9303-76b4aebaa4e3.png)

Il [DPCM del 3 novembre 2020](https://www.gazzettaufficiale.it/eli/id/2020/11/04/20A06109/sg) ha istituito la suddivisione dell'Italia in "zone colorate" a seconda della gravità della situazione-covid, secondo questo schema:

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

- [Elenco provvedimenti COVID-19 (Openpolis.it)](https://www.openpolis.it/coronavirus-lelenco-completo-degli-atti/)
- [Elenco provvedimenti normativi COVID-19 (ISTITUTO PROFESSIONALE DI STATO “ALFIO MONCADA” )](https://www.ipsmoncada.edu.it/pagine/covid-2019-normativa-gazzetta-ufficiale-e-link-ad-altri-organi)
- [DECRETO-LEGGE 25 marzo 2020, n. 19 (in G.U. 25/03/2020, n.79)](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2020-03-25;19)  (Successivamente modificato per introdurre i colori delle regioni nell'articolo 16)
- DPCM di istituzione delle zone a colori - 3 novembre 2020: [link](https://www.gazzettaufficiale.it/eli/id/2020/11/04/20A06109/sg)
- "Decreto di Natale", con norme sui colori delle regioni in vigore nel periodo di Natale 2020 (GU n.299 del 02-12-2020): [link]( https://www.normattiva.it/atto/caricaDettaglioAtto?atto.dataPubblicazioneGazzetta=2020-12-02&atto.codiceRedazionale=20G00184&tipoDettaglio=originario&qId=&tabID=0.48476910017483954&title=Atto%20originario&bloccoAggiornamentoBreadCrumb=true) - abogato dalla  [Legge 29 GENNAIO 2021, N. 6](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2021-01-29;6)
- Successive modifiche delle regole per la determinazione dei colori delle regioni - 1 agosto 2021: https://www.ticonsiglio.com/colori-regioni-regole-governo/

Sequenza:
- [decreto-legge 25 marzo 2020, n. 19](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2020-03-25;19)  -->  [legge 22 maggio  2020,  n.  35](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2020-05-22;35)
- [decreto-legge 16 maggio 2020, n. 33](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2020-05-16;33) --> [legge 14 luglio 2020, n. 74](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2020-07-14;74) (GU n.125 del 16-05-2020)  (**zone colorate nazionali**, art.1, comma 16-septies )
- [DPCM (Decreto Presidente Consiglio dei Ministri) 3/11/2020 (Gazzetta Ufficiale della Repubblica italiana 4  novembre 2020,n. 275)](https://www.gazzettaufficiale.it/eli/id/2020/11/04/20A06109/sg)  (**zone colorate regionali**)
- ["Decreto di Natale" 2020](https://www.normattiva.it/atto/caricaDettaglioAtto?atto.dataPubblicazioneGazzetta=2020-12-02&atto.codiceRedazionale=20G00184&tipoDettaglio=originario&qId=&tabID=0.48476910017483954&title=Atto%20originario&bloccoAggiornamentoBreadCrumb=true)
- [DECRETO-LEGGE 14 gennaio 2021, n. 2 (in G.U. 14/01/2021, n.10)](https://www.normattiva.it/atto/caricaDettaglioAtto?atto.dataPubblicazioneGazzetta=2021-01-14&atto.codiceRedazionale=21G00002&atto.articolo.numero=1&atto.articolo.sottoArticolo=1&atto.articolo.tipoArticolo=0) (**Cambio regole per le zone**, con introduzoine comma 16-septies all'articolo 1)
- [decreto-legge 1°  aprile  2021,  n.  44](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2021-04-01;44) --> [legge 28 maggio 2021,  n.  76](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2021-05-28;76)
- [decreto-legge 22  aprile  2021,  n.  52](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2021-04-22;52) --> [legge 17 giugno 2021,  n.  87](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2021-06-17;87)
- [decreto-legge 23 luglio  2021,  n.  105](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2021-07-23;105)  --> [legge 16 settembre 2021, n. 126](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2021-09-16;126)
- [decreto-legge 6  agosto  2021,  n.  111](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2021-08-06;111) --> [legge 24 settembre 2021, n. 133](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2021-09-24;133)
- [decreto-legge 21 settembre 2021, n. 127](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2021-09-21;127) --> [legge 19 novembre 2021, n. 165](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:2021-11-19;165)
- [decreto-legge  8   ottobre   2021,   n.   139](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legge:2021-10-08;139) --> (attendere prego...)

