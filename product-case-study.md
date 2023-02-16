# Product case study 

Marthe Bull Pettersen 

12.02.2023



## Introduksjon

Jeg har ikke laget et faktisk prosjekt til denne oppgaven, men vil gå dypere inn i og forklare MySQL og gi et eksempel på bruksområde til dette. 

### Hva er MySQL?
MySQL er et open-source relasjonelt databasesystem (RDBMS) som lar brukere lagre, administrere og manipulere data. Det er designet for å være effektiv, rask og enkel å bruke. Det er et klient-server-system, noe som betyr at en klient kobler seg til MySQL-serveren for å få tilgang til og manipulere data. MySQL støtter en rekke programmeringsspråk, inkludert PHP, Java, Python og C ++, som gjør det enkelt for utviklere å integrere det i applikasjonene sine.


## Bakgrunn

MySQL ble utviklet for å gi et pålitelig, robust og effektivt databasesystem for å håndtere store mengder data på en enkel og skalerbar måte. Det ble utviklet av en svensk programvareutvikler, Michael Widenius, og hans team på midten av 1990-tallet.

MySQL ble utviklet som en reaksjon på behovet for et pålitelig, rimelig og enkelt databasesystem for å håndtere store mengder data, spesielt på webapplikasjoner. MySQL var et av de første open source-relasjonsdatabasesystemene og var basert på SQL-språket som gjorde det enkelt for utviklere å lære og bruke.

Siden MySQL ble lansert har det blitt brukt av mange store organisasjoner og nettsteder, inkludert Facebook, Twitter, Google og Wikipedia. I 2008 ble MySQL kjøpt av Sun Microsystems, og i 2010 ble Sun kjøpt av Oracle Corporation, som nå utvikler og vedlikeholder MySQL.

I dag fortsetter MySQL å være en av de mest populære open source-databasesystemene og brukes til å lagre og hente data i mange forskjellige sammenhenger, inkludert webapplikasjoner, analyse og finansapplikasjoner.


## MySQL i praksis

### Egenskaper 

* Relasjonsdatabase: MySQL er en relasjonsdatabase som støtter relasjonell datahåndtering.

* SQL-språk: MySQL bruker SQL-språket for å administrere databasen, som er en standardisert språk for å administrere relasjonsdatabaser.

* Skalerbarhet: MySQL er en svært skalerbar database som kan håndtere store datamengder og tunge arbeidsbelastninger.

* Høy ytelse: MySQL er kjent for sin høye ytelse og raske svar på spørringer.

* Sikkerhet: MySQL har mange sikkerhetsfunksjoner, inkludert støtte for autentisering og autorisasjon, kryptering og beskyttelse mot SQL-injeksjonsangrep.

* Transaksjonsstøtte: MySQL støtter transaksjoner, som er grupper av databehandlingsoperasjoner som må utføres som en helhet.

* Indeksering: MySQL støtter indeksering, som gjør at databasen kan utføre spørringer raskere ved å organisere dataene på en optimal måte.

* Replicasjon: MySQL støtter replikering, som lar deg lage flere kopier av databasen for å distribuere arbeidsbelastningen og sikkerhetskopiere data.

* Lagring av store datamengder: MySQL kan håndtere store datamengder, noe som gjør det egnet for store applikasjoner og store datasett.

* Open source: MySQL er en open source-database, som betyr at det er gratis å bruke, og kildekoden er tilgjengelig for å tilpasse og videreutvikle databasen.

### Bruksområder 

Hvis applikasjonen krever et pålitelig og allsidig databasesystem for å lagre og hente data, kan MySQL være et godt valg. MySQL kan brukes til å lagre og hente data i mange forskjellige sammenhenger. Under finner du noen eksempler på applikasjoner som passer godt til MySQL-databaser:

* Webapplikasjoner: MySQL er mye brukt til å lage webapplikasjoner som blogger, nettbutikker og sosiale nettverk. Det er en populær database for å lagre brukerdata og innhold som kommentarer og bilder.

* Finansapplikasjoner: MySQL er også populær i finanssektoren, spesielt for applikasjoner som håndterer transaksjoner og kundeinformasjon. Det brukes ofte i banker, forsikringsselskaper og aksjehandelssystemer.

* Analytiske applikasjoner: MySQL kan også brukes i analytiske applikasjoner som krever komplekse spørringer og aggregatfunksjoner. Det er populært for å lage dashbord og rapporter som gir innsikt i store datamengder.

* E-handelsapplikasjoner: MySQL er også en populær database for e-handelsapplikasjoner som håndterer produktdata, bestillinger og kundeinformasjon. Det er enkelt å integrere med nettbutikkplattformer som WooCommerce og Magento.

* Content management systems: MySQL brukes også ofte i innholdsadministrasjons-systemer (CMS), som WordPress og Drupal, for å lagre innhold og brukerdata.

### Eksempel på prosjekt med burk av MySQL

Jeg hadde en ide om å lage en applikasjon som gir deg oversikt over klærne dine. Kanskje denne også kan ha flere brukere og gjøre det lettere å for eksempel organisere deling og bytting av klær, da man har oversikt over sine egne klær og kan søke opp andre brukere. 

Her vil det være relevant å kunne lagre data som type plagg, farge, størrelse, tilstand, beskrivelse og kjøpsdato, noe som MySQL lar deg gjøre. Ved å bruke et for eksempel PHP kan man lage en frontend som lar brukere opprette en konto hvor de kan legge til, endre, og slette klesplagg.  Med dette vil det også bli mulig søke og filtrere på det overnevnte. 

**Eksempel** på kode som oppretter en tabell for en bruker, og med kolonner for id, produkttype, størrelse, pris og farge. Etter den er opprettet settes det inn tre klesplagg i databsen med disse verdiene: 

```
CREATE TABLE marthe_bull_pettersen (
  id INT NOT NULL AUTO_INCREMENT,
  product_type VARCHAR(50) NOT NULL,
  size VARCHAR(20),
  price DECIMAL(10, 2) NOT NULL,
  color VARCHAR(20),
  PRIMARY KEY (id)
);

INSERT INTO marthe_bull_pettersen (product_type, size, price, color)
VALUES
  ('T-skjorte', 'M', 299.00, 'Blå'),
  ('Genser', 'S', 599.00, 'Grønn'),
  ('Bukse', 'L', 899.00, 'Svart');
````

## Fordeler med MyQSL 

Det er flere grunner til hvorfor man vil velge en MySQL-database:

* Open source: MySQL er open-source-programvare, noe som betyr at det er gratis å bruke og kan tilpasses for å møte spesifikke behov. Dette gjør det til et kostnadseffektivt alternativ for enkeltpersoner og organisasjoner som trenger en database-løsning.

* Pålitelighet og ytelse: MySQL er kjent for sin pålitelighet og ytelse, noe som gjør det til et populært valg for kritiske applikasjoner. Den kan håndtere store mengder data og høy trafikkbelastning uten treighet eller krasj.

* Kompatibilitet: MySQL er kompatibel med et bredt spekter av operativsystemer, programmeringsspråk og plattformer, noe som gjør det til en allsidig database-løsning. Den kan integreres med annen programvare og applikasjoner enkelt.

* Sikkerhet: MySQL tilbyr flere sikkerhetsfunksjoner for å beskytte data mot uautorisert tilgang og angrep. Den støtter SSL-kryptering, tilgangskontroller og andre sikkerhetstiltak for å sikre at data holdes trygge.

* Fellesskap: MySQL har et stort og aktivt fellesskap av utviklere og brukere som gir støtte, deler kunnskap og bidrar til dens utvikling. Dette fellesskapet sikrer at MySQL forblir oppdatert og relevant.

Totalt sett er MySQL en pålitelig, fleksibel og kostnadseffektiv database-løsning som kan brukes i en rekke applikasjoner.

## Ulemper med MySQL 

Selv om MySQL er et populært og pålitelig databasesystem, er det noen tilfeller der det kanskje ikke er det beste valget:

* Komplekse datastrukturer: MySQL er ikke egnet for å administrere komplekse datastrukturer, som hierarkiske data eller grafdata. I slike tilfeller kan en NoSQL-database, som MongoDB eller Neo4j, være et bedre valg.

* Tung skrivebelastning: Hvis databasen forventes å ha høyt volum av skriveoperasjoner, som hyppige oppdateringer eller innsettinger, kan MySQL være et dårlig valg. I slike tilfeller kan en databasesystem som er designet for skriveintensive arbeidsmengder, som PostgreSQL eller Cassandra, være et bedre alternativ.

* Begrenset skalerbarhet: Mens MySQL kan håndtere høye datavolum, kan det ikke skalere godt i visse scenarioer, som når det er store antall samtidige brukere eller høy skrivebelastning. I slike tilfeller kan et distribuert databasesystem, som Apache Hadoop eller Amazon DynamoDB, være et bedre valg.

## Sammenlikning 

Relasjonelle og ikke-relasjonelle databaser er to forskjellige tilnærminger til lagring og organisering av data. 
Her er en kort sammenlikning:

Relasjonelle databaser (feks MySQL, Oracle, SQL Server):
* Relasjonelle databaser er basert på relasjoner mellom tabeller og data.
* De bruker SQL (Structured Query Language) til å behandle data og gjøre spørringer i databasen.
* Dataene organiseres i strukturerte tabeller med rader og kolonner, og det er en klar definert relasjon mellom tabellene.

Ikke-relasjonelle databaser (feks MongoDB, Cassandra, Redis):
* Ikke-relasjonelle databaser er basert på ikke-strukturerte eller semi-strukturerte data som kan variere i form og format.
* De bruker forskjellige typer query-språk og datamodeller til å håndtere data.
* Dataene organiseres på forskjellige måter som i dokumenter, nøkkelverdipar, grafer og andre strukturer.


## Sammendrag

MySQL er en av verdens mest populære relasjonelle databaser. Den er open source og gratis å bruke. MySQL støtter mange ulike operativsystemer og er en robust, sikker og skalerbar database som brukes av millioner av utviklere og bedrifter over hele verden.

Det tilbyr en rekke funksjoner, inkludert et kraftig query-språk (SQL), ACID-kompatibilitet (Atomicity, Consistency, Isolation, Durability), transaksjonsstøtte og indeksering for raskere søk. MySQL kan integreres med mange ulike programmerings- og scripting-språk, og støtter også ulike lagringsmotorer og tilleggsfunksjoner.

Databasesystemet kan brukes til en rekke ulike applikasjoner, fra små enkle nettsider til store komplekse forretningsapplikasjoner. Det er også en populær database for bruk innenfor skyteknologi og Big Data-løsninger. MySQL er kjent for å være en stabil og pålitelig database som kan håndtere store datamengder og samtidige brukere.

Det er viktig å huske at selv om MySQL har mange fordeler, er det ikke alltid det beste valget. For eksempel, hvis du jobber med store mengder ustrukturert data, kan en ikke-relasjonell database som MongoDB være mer passende. Her er det viktig å ta en vurdering basert på spesifikke behov og tenkt bruk.



