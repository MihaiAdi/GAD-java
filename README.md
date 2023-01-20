# GAD-java
1. Acest cod implementează Builder Design Pattern.

Clasa "builderDesignPattern" conține câmpurile:"nrStrada", "strada", "oras", "judet", "codPostal", "nrTelefon".

Clasa "Builder" are metode setter pentru fiecare câmp care returnează obiectul Builder.

În clasa Main, sunt create trei instanțe de clasa, fiecare cu valori diferite transmise clasei builder. 
Primele două instanțe au toate câmpurile setate, în timp ce a treia are nrTelefon setat la null. 
Ultima instanță este de asemenea afișată și este afișat un mesaj că numărul de telefon lipsește.

Builder permite construirea unor obiecte complexe într-un mod pas cu pas și oferă o modalitate de a crea obiecte care sunt imutabile (câmpurile sunt finale).

2. Acest cod utilizează Decorator Design Pattern pentru a crea diferite tipuri de cafea și să afișeze costurile pentru acestea.

Există o clasă abstractă numită "coffee" care are un câmp "price" protejat și o metodă abstractă "getPrice". 

Există o clasă "cafeaSimpla" care extinde clasa "coffee" și implementează metoda "getPrice" și setează prețul pentru cafea simpla ca fiind 10.

Există o clasă abstractă "coffeeDecorator" care extinde clasa "coffee" și are un câmp "decoratedCoffee" protejat care conține o referință la o instanță a clasei "coffee". 
Aceasta clasă are o metodă "getPrice" care delegă apelul către metoda "getPrice" pe obiectul "decoratedCoffee".

Există trei clase concrete "cafeaLapte", "cafeaFrisca" și "cafeaOreo" care extind clasa "coffeeDecorator" și suprascriu metoda "getPrice" 
pentru a adăuga un preț suplimentar pentru fiecare adaos de ingredient.

În clasa Main, se creează diferite tipuri de cafea prin adăugarea adaosurilor în ordinea dorită, și se afișează prețul final pentru fiecare tip de cafea.
