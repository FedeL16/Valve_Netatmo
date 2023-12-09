Se apprezzi questo progetto, sarei grato del tuo supporto tramite un semplice caffè, cosi io posso continuare a creare altri contenuti e tenere aggiornati quelli pubblicati.


[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/V7V1RWSFR)

GESTIONE VALVOLE NETATMO:

ho cercato di creare una card e vari sensori di appoggio, affinchè si possa controllare, tramite Home Assistant il funzionamento e le accensioni dei caloriferi, affinchè si possa mantenere una temperatura più confortevole possibile, tagliando il tempo di accensione dei caloriferi e radiatori.

Potete installare il tutto sia come package, sia inserendo i sensori nel vostro configuration.yaml/template.yaml a seconda se usate o no i package. Stessa cosa per le automazioni e gli script, potete installarli sia inserendoli in yaml nei rispettivi file, oppure inserirli singolarmente tramite "modifica in yaml" attraverso impostazioni -> dispositivi e servizi -> automazioni e scenari.

Massima flessibilità per chi non è troppo pratico.

Non ho inserito la parte grafica dei sensori che monitorano le accensioni quotidiane,mensili e annuali, in quanto ognuno può integrarli come meglio crede, graficamente (io uso mushroom scaricabile da HACS), restano comunque fuori dalla singola card di ogni valvola.

In ogni caso questo è il risultato finale:

![IMG_3151](https://github.com/FedeL16/Valve_Netatmo/assets/141550943/d90e9e12-5fe9-4bbc-8a54-457453b6305f)

INSTALLAZIONE:

- Inserire in package il file climate_sensors.yaml così come il file automation.yaml e script.yaml, oppure copiate ogni sensore nel vostro file dei sensori o in configuration.yaml, mentre create ogni automazione e  ogni script via yaml nel menù di riferimento, come sopra descritto.
RICORDARSI di variare le entità contenute nei file con le vostre corrette. (ogni sensore, automazione e script dovrà essere rinominato e associato alla vostra entità).

- Riavviate HA

- Scaricate le varie immagini e inseritele nella vostra configurazione. Per farlo consiglio di creare, all'interno della cartella www, la cartella chiamata "netatmo"  e al suo interno inserite ogni singola immagini .png. Rispettate il percorso e i nomi delle immagini così non dovrete cambiare nulla nella card.

- Andate nella vostra dashboard che preferite, aggiungete la card tramite card manuale e copiate il codice, ricordandovi anche qui di cambiare le vostre entità correttamente. Potete eliminare le parti che reputate di non inserire o di cui non disponete (vedi sensore apertura finestra)

- Infine i sensori che conteggiano i tempi di accensione potete inserirli fuori dalla card (mio consiglio) o anche all'interno, ma dovreste modificare il codice della card stessa. Io uso la grafica di mushroom (scaricabile da HACS) e ho inserito tutto esternamente.

Se avete più valvole dovrete rifare questa procedura per ciascuna, tranne l'upload delle immagini.

PS Capitolo Apertura Valvole: questo sensore non va creato, ma dovreste trovarlo come attributo nella pagina strumenti per sviluppatori->stati>ricerca entità>nomedellavostraentità e allora potrete inserirlo in card con la vostra dicitura corretta. 

La card funziona sia con integrazione ufficiale netatmo che con l'addon di sdomotica, nella card dovete solo aggiungere la riga: "heat: local/netatmo/netatmo_on.jpg" nella parte di codice riferita al pulsante on e off (modalita_auto_e_off_xxx).

Vi ringrazio qualora voleste contribuire al miglioramento del package.



Un Saluto
