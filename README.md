# amandas
DT173G Moment 2, nodejs and gulp

## Automatisering
Syftet med automatiseringsprocessen är att förenkla utvecklingsarbetet. Man kan bland annat att sammanslå filer, komprimera innehållet, kopiera filer och konvertera innehållet i filerna.


## Paket och verktyg
* Visual Studio Code med Live reload.
* NodeJS
* Gulp

För att sammanslå och minifiera JavaScript
* Gulp-uglify
* Gulp-concat

För att sammanslå och minifiera CSS
* Gulp-concat-css
* Gulp-clean-css

För att minifiera bilderna
* Gulp-imagemin

För att kontrollera ändringar som gör i filsystemet
* Gulp-watch

De paket jag har valt är dels de som Mattias visade i föreläsningen. Utöver dessa har jag sökt på lämliga paket och gått efter om de uppdaterats nyligen samt hur många nedladdningar som gjorts för de olika paketen.


Jag har skapat en mapp som heter pub och en som heter src. I src arbetar jag med filerna. Sen har jag i min gulpfile funktioner för att flytta, minifiera och sammanslå de olika filerna som ska publiceras. Dessa hamnar i pub-mappen. Det är den mappens filer jag sedan använder om jag ska ladda upp arbetet någonstans. 

Starta terminalfönstret
Navigera till rätt katalog
npm init -> package.json-filen skapas i katalogen
npm install gulp --save-dev -> Gulp och alla dependencies laddas ner
En git init görs för att jag kommer att ladda upp det på github senare. 
Jag skapar .gitignore-filen och lägger in de filer som kan ignoreras där i. 
Sedan skapas gulpfile.js och alla andra filer så som index.php, css osv. 



De tasks som ingår är:
* copyhtml  -> Kopierar över html-filerna från src-mappen till pub-mappen.
* concminjs -> Sammanslår, minifierar och kopierar js-filerna.
* copyimg   -> Minifierar och flyttar bilderna.
* watcher   -> Kontrollerar ändringar som görs i filsystemet.
