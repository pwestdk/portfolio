## 1.2. Development process

### Git branching
For at mindske merge konflikter implementerede vi nedenstående branching struktur:



![alt text](INDSÆT LINK "Branching")    

Her en kort beskrivelse af de forskellige led i strukturen:

- **Master**
Live branch (produktion). Hele applikation er testet igennem og alt *burde* virke. 

- **Developer**
Udviklings branch. Kode som **umiddelbart** virker. Denne branch merges ind i Master når alt er testet gennem og man klar til at det skal i produktion.

- **User Stories**
Story branches. På baggrund af vores *Github Issues / User Stories* oprettes her en ny branch hver gang en ny påbegyndes. Merges op i Developer når story er testet igennem. 

- **Tasks**
Opgaver branches. Ud fra vores *Github Issues / User Stories* er oprettet en række *tasks*. En task branches ud fra en story branch. Merges op i story branch når task er løst og testet igennem. 

I teorien vil strukturen ovenfor være tæt på *“Bullet-Proof”* hvis fulgt nøje. Alle var dog overbevist om, at trods god struktur er vi blot mennesker og derfor vil det være uundgåeligt at der ikke vil opstå konflikter. I praksis gik det hurtigt op for os at *Task* branching i nogle tilfælde ikke gav meget mening. Hvis en story kun var tildelt en person, var det kun ekstra arbejde at branche yderligere ud i tasks. Derfor blev vi enige om, at hvis man var ene om en story, var det ikke nødvendigt at branche yderligere ud. Ydermere oplevede vi merge konflikter i stor set alle led af strukturen. *Best Practice* er: *Inden der merges op i en branch, merges den branch først ned i ens egen, for på den måde at sikre at de to branches kan snakke sammen inden det endelig merge sker.* Hvis vi gjorde dette hver gang ville størstedelen af vores merge-konflikter kunne have været forhindret. 
