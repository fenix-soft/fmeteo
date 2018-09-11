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
    
    

**note:** some names of cities are made up of the aggregation of several names or terms, for some openweatermap recognizes them simply by writing them "all attacked" for others instead you have to write them separating them with the "space". In the terminal space is used to indicate the passage of further commands or options, so it is advisable to use the "% 20" character as space and enclose the name in quotation marks.

#### Some examples:

for example we want to recover the weather data  of a city called "**Tempio Pausania**" (IT) or "**New York**"(USA) that openwatermap has indexed  written with the space.

fmeteo "Tempio%20Pausania,IT"

fmeteo "New%20York,US"

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


**nota bene:** alcuni nomi di città sono costituiti dall'aggregazione di più nomi o termini, per alcuni openweatermap li riconosce semplicemente scrivendoli "tutti attacati" per altri invece bisogna scriverli separandoli con lo "spazio". Nel terminale lo spazio serve ad indicare il passaggio di ulteriori comandi o opzioni quindi è cosigliabile utilizzare il carattere "%20" come spazio e racchiudere il nome tra virgolette.

#### Alcuni esempi:

ad esempio vogliamo recuperare il tempo di una citta chiamata "**Tempio Pausania**"(IT), oppure  "**New York**"(USA) che openwatermap ha indicizzato scritta con lo spazio.

    fmeteo "Tempio%20Pausania,IT"

    fmeteo "New%20York,US"

