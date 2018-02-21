# RseminarOppg2
Hjelp


getwd()
setwd("~/Documents/Rstudio")

## Frida - kvinne, 22, student, 12000 
## Per - mann, 25, murer, 30000
## Ole - mann, 35, konsulent, 50000
## Ida - kvinne, 27, sykepleier, 32000
## Nils - mann, 28, arbeidsledig, 10000

Frida <- c("kvinne", 22, "student", 12000)
Per <- c("mann", 25, "murer", 30000)
Ole <- c("mann", 35, "konsulent", 50000)
Ida <- c("kvinne", 27, "sykepleier", 32000)
Nils <- c("mann", 28, "arbeidsledig", 10000)
?t()
?rbind()
rbind(Frida, Ida, Nils, Ole, Per)
datasett <- data.frame( Frida, Ida, Nils, Ole, Per, stringsAsFactors = FALSE)


datasett

rownames(datasett) <- c("kjonn", "alder", "yrke", "lonn")
datasett

rownames(datasett)

## ok så basically, her er oppgaven:
## Vis hvordan du kan identifisere de enhetene som har månedslønn større
## eller lik 30000 i datasettet, ved hjelp av which() og en logisk test. 
##Bruk denne informasjonen til å indeksere følgende informasjon fra datasettet ditt:

## 1. Alle verdier på variabelen lønn som er større eller lik 30000
## 2. Alle verdier på variabelen kjønn, for de enhetene som har lønn større eller lik 30000
## 3. Alle verdier på variablene alder og yrke, for dem som har lønn under 15000. 

## Her jeg sliter, aner ikke hvordan jeg skal bruke which til å bare sjekke <= 30000 
## i raden "lonn". 


which(datasett <=30000)
which(datasett[lonn] <= 30000)
datasett

which(datasett <= 30000)

which(datasett <= 30000)
View(datasett)

datasett[which( row(4) <= 30000)]

datasett[3,4]
View(datasett)
datasett[ c(4,1), c(4,2), c(4,3), c(4,4), c(4,5) ]


