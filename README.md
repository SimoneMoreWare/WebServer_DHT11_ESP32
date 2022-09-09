# WebServer_DHT11_ESP32

Nell’articolo di oggi vedremo come utilizzare i PIN GPIO. Creeremo un web server con l’utilizzo del sensore di temperatura DHT11 per visualizzare via broswer dati relativi alla temperatura e umidità.

# Componenti
* esp32
* dht11

![alt text](https://i0.wp.com/www.moreware.org/wp/wp-content/uploads/2022/08/qa.png?w=670&ssl=1)

# Collegamenti

In seguito schema e diagramma di collegamento. Per costruire un circuito ricordati di tenere la scheda spenta.

![alt text](https://i0.wp.com/www.moreware.org/wp/wp-content/uploads/2022/08/qa-1.png?w=492&ssl=1)

# Codice
Se questo è il tuo primo articolo ti invito di leggere prima questo per l’installazione dei driver della scheda. Ecco qui un piccolo riepilogo prima di compilare e caricare il codice.

![alt text](https://i0.wp.com/www.moreware.org/wp/wp-content/uploads/2022/08/ltc-2.png?w=599&ssl=1)
![alt text](https://i0.wp.com/www.moreware.org/wp/wp-content/uploads/2022/08/ltc-3.png?w=557&ssl=1)

Dobbiamo installare la libreria dht.h, dobbiamo andare su Sketch->Include library-> Manage libraries e cercare nell’apposito menù la libreria dht.h.

![alt text](https://i0.wp.com/www.moreware.org/wp/wp-content/uploads/2023/01/adafruit_dht_library.png?w=750&ssl=1)

Installare la libreria ESPAsyncWebServer

* Installa la seguente libreria ESPAsyncWebServer
* Estrai la cartella
* Rinomina la cartella in ESPAsyncWebServer
* Spostala nella cartella di Arduino, in seguito spostala nella cartella “libraries”
* Entra nella cartella, vi sarà un’altra cartella denominata “ESPAsyncWebServer-master”, una volta entrati copiate e incollate tutte le cartelle presente al suo interno al di fuori della cartella “ESPAsyncWebServer-master”. In seguito andate nella cartella “src” copiate e incollate il contenuto al di fuori della cartella “src”.

Installare la libreria Async TCP

* Installa la seguente libreria AsyncTCP
* Estrai la cartella
* Rinomina la cartella in AsyncTCP
* Spostala nella cartella di Arduino, in seguito spostala nella cartella “libraries”
* Entra nella cartella, vi sarà un’altra cartella denominata “AsyncTCP-master”, una volta entrati copiate e incollate tutte le cartelle presente al suo interno al di fuori della cartella “AsyncTCP-master”. In seguito andate nella cartella “src” copiate e incollate il contenuto al di fuori della cartella “src”.

# conclusione
Compila e carica il codice sull’ESP32, ed ecco qui che potremo visualizzare l’indirizzo IP che utilizzeremo per accedere via broswer dal monitor seriale.
![alt text](https://i0.wp.com/www.moreware.org/wp/wp-content/uploads/2022/09/awswasxfa-1.png?w=1019&ssl=1)

Accesso server web
Per accedere al server web, apri il browser, incolla l’indirizzo IP di ESP32 e vedrai la pagina seguente. 
![alt text](https://i0.wp.com/www.moreware.org/wp/wp-content/uploads/2022/09/awswasxfa.png?resize=1024%2C479&ssl=1)

Ora puoi visualizzare i dati relativi alla temperatura e umidità nella rete locale, nel prossimo articolo vedremo come visualizzarlo anche al di fuori della rete locale.




