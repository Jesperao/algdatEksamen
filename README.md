# Mappeeksamen i Algoritmer og Datastrukturer Høst 2020

# Krav til innlevering

Se oblig-tekst for alle krav, og husk spesielt på følgende:

* Git er brukt til å dokumentere arbeid (minst 2 commits per oppgave, beskrivende commit-meldinger)	
* git bundle er levert inn
* Hovedklassen ligger i denne path'en i git: src/no/oslomet/cs/algdat/Eksamen/EksamenSBinTre.java
* Ingen debug-utskrifter
* Alle testene i test-programmet kjører og gir null feil (også spesialtilfeller)
* Readme-filen her er fyllt ut som beskrevet


# Beskrivelse av oppgaveløsning (4-8 linjer/setninger per oppgave)

Vi har brukt git til å dokumentere arbeidet vårt. Jeg har 16 commits totalt, og hver logg-melding beskriver det jeg har gjort av endringer.

* Oppgave 1: hentet program kode 5.2.3 a) fra kompendiet og gitt ut ifra det for å kode resten av oppgaven.
* Oppgave 2: deklarerer antall like vedier som int like = 0. cmp sammenligner innsatt verdi med p.verdi, hvis innsatt verdi er mindre enn p.verdi blir p til venstrebarnet. er innsatt verdi større enn p.verdi blir p til høyre barn og hvis innsatt verdi er lik p.verdi teller like og p blir til høyrebarnet.
* Oppgave 3: forstePostorden bruker en while løkke for å flytte pekeren nedover til venstre, hvis det ikke finnes en venstre node går den til høyre. dette er den forste noden i postorden.
nestePostorden sjekker om forelder til peker er null, hvis den er det så er peker på rotnoden og traverseringen av treet er ferdig. Ellers så bruker jeg kriteriene for postorden fra kompentiet for å lage if setninger som sjekker hvilken node som er neste.
* Oppgave 4: I metoden postorden bruker jeg førstePostorden metoden til å finne første node i postorden, derretter setter jeg opp en while løkke som kaller på nestepostorden så lenge p ikke er like null. PostordenRecursive traverserer også treet på postorden, men den kaller på seg selv får å bevege seg gjennom treet.
* Oppgave 5: Starter ved å oppette arraylisten som verdiene skal settes inn i og en kø, og rotnoden legges inn i køen. Deretter brukes en whileløkke for å legge til verdiene som er i køen inn i en arraylist, for å så traversere gjennom treet og legge til nye verdier i køen. whileløkken fjerner også de verdiene som blir tatt ut.
* Oppgave 6: For metoden public boolean fjern, ser jeg på programkode 5.2.8 d) som nevnt i oppgaven. jeg har lagt til en if setning som korrekt håndterer foreldre peker under fjerning.
For fjernAlle metoden har jeg fått hjelp fra løsningsforslag til oppgave 3 i avsnitt 5.2.8 i kompendiet.

# Warnings
Det er 5 warnings jeg ikke får gjort noe med som gjenstår.
* Linje 12 og 179 er det bruk av non-ASCII symbol.
* Linje 36 er antall instansiert men blir adri brukt.
* Linje 47 er public boolean inneholder aldri brukt.
* Linje 84 er det warning for at returverdien til public boolean leggInn ikke blir tatt i bruk, og kan ikke returnere void uten å forande på metoden.
