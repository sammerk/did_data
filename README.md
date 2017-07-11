# did_data = Didaktische Daten  
Dieses Repositorium enthält Datensätze, welche in der Lehre eingesetzt werden:

## Liste der Datensätze
* __Erstis__. Datensatz aus Luhman (2013)



Reading a text (e.g., csv) file from github

On the getup website, navigate to the text file. E.g., here is the web page for the nutrients data set of the Beninca et al (2008) reproduction. Find the button that says "Raw" and click on it. Here is what you see for the nutrients data. Its a raw text file. It is the URL of this web page that we give to R as the location of the data. So copy this URL. Then we insert the URL into the following R code:

require(RCurl)

    nuts <-read.csv(text=getURL("https://raw.githubusercontent.com/opetchey/RREEBES/master/Beninca_etal_2008_Nature/data/nutrients_original.csv"), skip=7, header=T)

The first line loads the RCurl library (which you will need to have installed) so we can use the getURL() function. The next line uses the read.csv() function to read the data from the URL, with the URL dealt with by the getURL() function. Note that the skip and header function are specific to the nutrients dataset, and are not a part of reading the data from the online repository.
Reading a Rdata file from github

Again, navigate to the Rdata file on the github website repository, again locate the "Raw" button, but don't click on it. If you do click on it, you will likely get a copy of the file downloaded. Instead, right click and select "copy link". Then paste the link in to the following R code:

library(repmis)

    source_data("https://github.com/opetchey/RREEBES/raw/Beninca_development/Beninca_etal_2008_Nature/data/GLE_estimate.Rdata?raw=True")
