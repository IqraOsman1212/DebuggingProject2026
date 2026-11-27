# Opgave 1 – Debugging i IntelliJ

## 1. Horisontal og vertikal placering
Fejlen skyldtes, at `getRandomInteger(1)` altid returnerede 0. Jeg ændrede argumentet til 2, så både 0 og 1 kan vælges, og skibet kan placeres både horisontalt og vertikalt.

## 2. Ship sunk!
I metoden `isSunk()` blev operatoren `>` brugt i stedet for `>=`. Jeg ændrede operatoren, så beskeden vises efter tre registrerede træffere.

## 3. ArrayIndexOutOfBoundsException
Skibets slutposition lå nogle gange uden for spillepladen. Jeg tilføjede en do-while-løkke, som vælger en ny placering, hvis slutpositionen overskrider spillepladens grænser.

## Test
Jeg kørte programmet flere gange og observerede både horisontale og vertikale skibe. Beskeden `Ship sunk!` blev vist efter tre registrerede træffere, og programmet kunne afsluttes med exit code 0. Testene dækkede ikke alle mulige placeringer.
