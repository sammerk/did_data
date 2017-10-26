# did_data = Didaktische Daten  
Dieses Repositorium enthält Datensätze, welche in der Lehre eingesetzt werden.  
Sie können direkt programmatisch in eine Session geladen werden:  

    Erstis <- read_delim("https://raw.githubusercontent.com/sammerk/did_data/master/Erstis.dat", delim = "\t", na = c("-9"))

## Liste der Datensätze
* __Erstis__. Datensatz aus Luhman (2015). _delimiter = "\t", missings = -9_
* __BigFive__. Datensatz aus Luhman (2015). _delimiter = ";", missings = ""_
* __KidIQ__. Datensatz aus Gelman & Hill (2006). _delimiter = ";", missings = ""_
* __STAR__. Datensatz des Tennessee's Student Teacher Achievement Ratio project (2006). _Delimiter = ";", Missings = ""; Codes = siehe gleichnamige .sav-Datei_
* __VertEig__. Simulierter Datensatz einer Selbstevaluation zur Untersuchung von Verteilungseigenschaften und -effekten. _Delimiter = ";", Missings = ""
