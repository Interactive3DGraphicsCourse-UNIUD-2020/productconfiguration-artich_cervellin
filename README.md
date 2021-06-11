# **Product Configuration Project**

di Eleonora Artich e Caterina Cervellin

 

## **Descrizione**

La nota azienda ACME richiede la realizzazione di un configuratore Web per la vendita di un prodotto attraverso un sito di e-commerce. Per lo svolgimento del progetto è stata scelta come prodotto una sedia, essendo un oggetto semplice e facile da fornire in diverse varianti.

![prodotto_finale](images\prodotto_finale.jpeg)

## **Obiettivi**

Creazione di un’applicazione Web (pagine HTML) che visualizzi il prodotto in 3D (utilizzando three.js) e che consenta all’utente un’ispezione interattiva del prodotto e la scelta di alcune sue varianti.

Lista dei passaggi:

* Creazione (o download) di un modello 3D (limite di 100.000 vertici);

* Illuminazione e *environment map*;

* Inserimento dei materiali (almeno 3 alternative);

* Tone mapping;

* BRDF;

* Interfaccia utente.

  

## **Oggetto**

Si è optato per il download di un modello 3D open source così da poter soddisfare tutti gli obiettivi richiesti dalla consegna. Come già anticipato è stato scaricato un modello 3D di una sedia e il sito scelto è *TurboSquid* (https://www.turbosquid.com/it/3d-models/3d-leather-chair-black-model-1551213). Dopo un colloquio sulla scelta delle varie tecniche da utilizzare e i vari step da eseguire è iniziata la fase di progettazione.



![modello](images\modello.png)



## File usati

Il progetto `productconfiguration-artich_cervellin ` è composto da:

- `index.html  `: file *.html* della scena;
- `journal.md`: documento di testo che riporta gli aggiornamenti del progetto;
- `readme.md`: questo documento di testo riassuntivo del progetto;
- `images`: cartella che contiene le immagini usate in journal.md e readme.md;
- `lib`: cartella che contiene le librerie di *Three.js*;
- `modules`: cartella che il modello 3D della sedia;
- `textures`: cartella che contiene le textures e le cubemaps utilizzate.



## Processo

Dopo una prima fase preparatoria di progettazione, svolta attraverso lo studio delle configurazioni di siti di e-commerce esistenti e delle loro interfacce utente, è stato impostato il codice di partenza impostando la scena, la camera, e il modello del file OBJ. Successivamente, è stata definita l'illuminazione più ottimale per la resa della scena, utilizzando una *point light*. La scena è stato fornita, inoltre, di un'*environment map*, in questo caso una *cubemap*, raffigurante un'ambiente di interni di una casa. 

![map](images\map.png)



Le texture dell'oggetto, in questo caso le *normal maps*, *roughness* e *color maps*, erano già presenti all'interno del modello scaricato, e sono state modificate attraverso Photoshop solamente per l'aggiunta delle varianti colore. L'interazione dell'utente consente quindi la scelta del colore della sedia tra le alternative nero, grigio e bianco, impostate tramite un radio button creato attraverso il sito *Bootstrap* (https://getbootstrap.com/) e il foglio di stile.



![texture](images\texture.png)



La scelta degli shader è ricaduta su quelli visti a lezione, dal momento che la scena richiedeva degli shader capaci di applicare le texture in nostro possesso alla scena.

Infine, è stato applicata un'operazione di *Tone Mapping* alla scena.



## **Risultato finale**

La configurazione finale rispetta quella ipotizzata inizialmente. L'utilizzo di un modello open source ha semplificato e velocizzato molto la parte iniziale del progetto, e la scelta di una sedia ha facilitato l'utilizzo di materiali e texture, nella possibilità di offrire delle varianti colore. Questo percoso ha reso possibile concentrare gli sforzi sulla comprensione delle varie fasi del progetto e sul rispetto di tutte le caratteristiche richieste. Lo svolgimento del progetto è stato reso possibile grazie anche agli esempi del corso *Interactive 3D graphics* (https://github.com/Interactive3DGraphicsCourse-UNIUD-2021/example-code) e alla guide online di *three.js* (https://threejs.org/), da cui sono stati presi vari spunti. Il risultato finale, nella sua semplicità ed essenzialità, mira a soddisfare tutti gli obiettivi richiesti, presentando quanto più possibile un risultato funzionante in tutte le sue parti e un layout dall'aspetto gradevole e quanto più convincente.



## Tools

**TurboSquid**: download modello e texture open source;

**Esercizi corso *Interactive 3D graphics***: spunti per il progetto, utilizzo vertex e fragment shader;

**three.js**: spunti per il progetto;

**Bootstrap**: definizione layout sito;

**Photoshop**: rielaborazione texture ed immagini per i file di testo.

