ENGLISH

If you appreciate this project, I would be grateful for your support through a simple coffee, so I can continue to create other content and keep those published up to date.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/V7V1RWSFR)

NETATMO VALVE MANAGEMENT:

I tried to create a card and various support sensors, so that you can control, through Home Assistant, the operation and ignition of the heaters, so that you can maintain a temperature that is as comfortable as possible, cutting the ignition time of the heaters and radiators.

You can install everything either as a package, or by inserting the sensors into your configuration.yaml/template.yaml depending on whether or not you use the packages. Same thing for automations and scripts, you can install them either by inserting them in yaml in their respective files, or inserting them individually via "edit in yaml" through settings -> devices and services -> automations and scenarios.

Maximum flexibility for those who are not too practical.

I did not insert the graphic part of the sensors that monitor the daily, monthly and annual stim-ups, as everyone can integrate them as they see fit, graphically (I use mushroom downloadable from HACS), they still remain outside the single card of each valve.

In any case, this is the end result:

![IMG_3151](https://github.com/FedeL16/Valve_Netatmo/assets/141550943/d90e9e12-5fe9-4bbc-8a54-457453b6305f)

INSTALLATION:

- Insert the climate_sensors.yaml file as well as the automation.yaml and script.yaml file into the package, or copy each sensor into your sensor file or configuration.yaml, while creating each automation and each script via yaml in the reference menu, as described above.

REMEMBER to vary the entities contained in the files with your correct ones. (each sensor, automation, and script will need to be renamed and associated with your entity).

- Restart HA

- Download the various images and insert them into your configuration. To do this I recommend creating, within the www folder, the folder called "netatmo" and inside it you insert every single .png image. Respect the path and the names of the images so you don't have to change anything in the card.

- Go to your preferred dashboard, add the card via manual card and copy the code, also reminding you here to change your entities correctly. You can delete parts that you think you don't fit or don't have (see window opening sensor)

- Finally, the sensors that count the power-on times you can insert them outside the card (my advice) or even inside, but you should change the code of the card itself. I use mushroom graphics (downloadable from HACS) and I have inserted everything externally.

If you have multiple valves you will have to redo this procedure for each one, except for uploading the images.

PS Chapter Opening Valves: This sensor should not be created, but you should find it as an attribute on the developer tools->states>search entity>name of your entity and then you can insert it into the card with your correct wording.

The card works both with official netatmo integration and with the sdomotica addon, in the card you just have to add the line: "heat: local/netatmo/netatmo_on.jpg" in the part of the code referring to the on and off button (auto_and_off_xxx mode).

Thank you if you would like to contribute to the improvement of the package.

A Greeting







###############################

ITALIANO

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
