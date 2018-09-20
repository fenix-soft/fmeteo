# fmeteo

## English: Read Me  version

**fmeteo** is a simple shell script that allows you to receive weather data from the [OpenWeatherMap](https://openweathermap.org/) service and to return the processed data to the terminal (bash).

The script is thus provided with a custom apikey for immediate use. It is possible to use a personal api-key just substitute it in the variable that is included in the script.

### dependencies:

curl

bc

[jq](https://stedolan.github.io/jq/)

cat

### use:

    fmeteo [city-name] [option]
    
#### option:
    -f              print "foorecast 5 days"
    -a              "all": print weather now and forecast 5 day  
    -j              get weather information in json format
    "no option"     print weather now

**note:** some names of cities are made up of the aggregation of several names or terms, for some openweatermap recognizes them simply by writing them "all attacked" for others instead you have to write them separating them with the "space". In the terminal space is used to indicate the passage of further commands or options, so it is advisable to use the "% 20" character as space and enclose the name in quotation marks.

#### Some examples:

for example we want to recover the "now weather data"  of a city called "**Tempio Pausania**" (IT) or "**New York**"(USA) that openwatermap has indexed  written with the space.

fmeteo "Tempio%20Pausania,IT"

fmeteo "New%20York,US"

#### example n2:

For example I want to know the current weather and the forecast of the next 5 days of "** New York **" (USA):


     fmeteo "New%20York,US" -a
    
or if we are a terminal that does not support xserver we can use a pager to display the data page by page:

      fmeteo "New%20York,US" -a | less
     
use space or the arrow to go forward or back, "q" to exit


***



## Italian: Read Me  version


**fmeteo** è un semplice script di shell che consente di ricevere dati meteo dal servizio [OpenWeatherMap](https://openweathermap.org/) e di restituire nel terminale (bash) i dati processati.

Lo script così  è fornito di una custom apikey per un immediata utilizzazione. E' possibile utilizzare un api-key personale basta sostituirla nella variabile approrpiata nello script.


### dipendenze:

curl

bc

[jq](https://stedolan.github.io/jq/)

cat

### uso:

    fmeteo [city-name] [option]

#### opzioni:
    -f                    stampa a video la previsione dei 5 giorni
    -a                    stampa il meteo corrente + la previsione dei 5 giorni
    -j                    scarica le informazioni meteo in formato json
    "nessuna opzione"     stampa il meteo corrente
    


**nota bene:** alcuni nomi di città sono costituiti dall'aggregazione di più nomi o termini, per alcuni openweatermap li riconosce semplicemente scrivendoli "tutti attacati" per altri invece bisogna scriverli separandoli con lo "spazio". Nel terminale lo spazio serve ad indicare il passaggio di ulteriori comandi o opzioni quindi è cosigliabile utilizzare il carattere "%20" come spazio e racchiudere il nome tra virgolette.

### Alcuni esempi:

ad esempio vogliamo recuperare il meteo corrente di una citta chiamata "**Tempio Pausania**"(IT), oppure  "**New York**"(USA) che openwatermap ha indicizzato scritta con lo spazio.

    fmeteo "Tempio%20Pausania,IT"

    fmeteo "New%20York,US"



#### esempio n2:

Ad esempio voglio sapere il meteo corrente e le previsioni dei prossimi 5 giorni di "**New York**"(USA):


    fmeteo "New%20York,US" -a
    
oppure se siamo in un terminale che non supporta xserver possiamo usare un paginatore per visualizzare i dati pagina per pagina:

     fmeteo "New%20York,US" -a | less
     
usa spazio o le freccia per andare avanti o indietro, "q" per uscire