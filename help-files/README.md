# Praktisk Web Blog Site

For at komme godt i gang efter en forhåbentlig herligt god sommerferie, starter vi op med en forholdvis afgrænset opgave der gerne skulle opfriske hukommelsen på alt det vi har arbejdet med før sommerferien.

Opgaven går ud på at få konstrueret et enkelt blog web site, som er drevet fra en mysql database.

Det er din opgave at udtænke database strukturen, og bygge både serverside og clientside delen af websitet med routes og templates efter behov.

Sitet skal være baseret på routes/views konceptet som det vi benyttede ved nyhedssitet før ferien.

Der er nogle enkle krav til løsningen:

* Forsiden af bloggen skal vise den nyeste indsatte blogpost baseret på dato.

* På alle sider skal der være en dynamisk navigation hvor man kan vælge fra hvilken kategori man vil se blogposter. Posterne vises efter nyeste øverst princippet.

* Også synligt på alle sider, er et søge felt hvor man kan søge i blogposter titel og indholdstekst.

* En blog skal som minimum indeholde: en id, en titel, noget tekst, en dato og være knyttet til en kategori.

* En kategori skal som minimum indeholde: en id og en titel.

* Der skal være et grundlæggende administrations område, hvor man kan oprette, rette og slette blogposter. 

Blogside
Menu
Blogpost: ID, Titel, Tekst, Dato, Kategori
Søgefelt
Kategori-navigation: ID og Titel

Derudover er der en samling funktioner der kan være interesante at udvide med, hvis man har mod på det:

* Et login system der forhindrer adgang til administrationen med mindre man er logget på.
* Tilknytning af nøgleord til blogposterne som kan benyttes til at vise relaterede blogposter på tværs af kategorierne.
* Billede upload, med skalereing hvis man har lyst til at prøve kræfter med det.
* Bruger administration, så flere brugere kan poste blogs.
* Dynamisk udskiftning af clientside delens design, en form for temaer (f.eks. udskiftning af stylesheet via en menu)
* WYSIWYG editor ved oprettelse af nye poster (f.eks. ck-editor)


Der er ikke noget fast design, her er der frihed til at være lidt kreativ.

--- 

Der er sat 1 arbejdsuge af til opgaven, dvs fredag d. 9 august kl 13.30 er det sidste push til github. 

---

Lige et par tekniske pointer som er værd at have med:

Kør `npm init -y` for at initialisere projektet

brug `npm install express --save` til at installere `express` modulet, der er en samling andre moduler som også er nødvendige, kig f.eks. under *dependencies* i `package.json` filen fra *the awesome newspage*. Det er nok meget de samme moduler vi har brug for her på blog sitet.

Kopier de filer / funktioner der er brugbare fra *the awesome newspage* eller *views and templates* projekterne. Især `server.js` og `mysql.js` kan være et godt sted at starte.

Husk at lave en sql dump af din database og push den til github.

