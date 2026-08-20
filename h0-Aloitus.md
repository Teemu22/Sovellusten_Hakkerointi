# H0 Compile and Analyze

## Lähdekoodi
Tein Hello world harjoitukset C kielellä testi.c nimiseen tiedostoon. 
 
 <img width="340" height="199" alt="image" src="https://github.com/user-attachments/assets/d7ddd7c7-be06-4137-b79e-c8dae80c620d" /> 

*Kuva 1. Hello World -ohjelman lähdekoodi C-kielellä.*

## Kääntäminen
Tallennettuani tiedoston ajoin komennon ```g++ testi1.c -o H0```. Komento kääntää lähdekoodin suoritettavaksi ohjelmaksi nimeltä h0.

<img width="536" height="138" alt="image" src="https://github.com/user-attachments/assets/7683a48b-c1e8-48dc-81ea-8591035ede33" />

*Kuva 2. C-kielisen lähdekoodin kääntäminen suoritettavaksi ohjelmaksi ```g++```-komennolla.*

## Suorittaminen
Suoritin käännetyn ohjelman komennolla ```./h0```. Tämän jälkeen ohjelma tulosti terminaaliin tekstin "Hello world", joten ohjelma toimii oikein.

<img width="509" height="142" alt="image" src="https://github.com/user-attachments/assets/8cfc3602-f747-4eb6-a16a-e9cd5570e903" />

*Kuva 3. Käännetyn ohjelman suorittaminen ja "Hello world" -tuloste.*

## Binäärin analysointi

Tarkastelin käännetyn ohjelman binääriä ```objcopy```-komennolla. Muunsin ohjelman Intel HEX-muotoon komennolla ```objcopy -O ihex h0 main.hex```. Tämän jälkeen katsoin ```main.hex```-tiedostoa ```cat main.hex```-komennolla.

<img width="730" height="804" alt="image" src="https://github.com/user-attachments/assets/9682ded0-04d6-4b6b-9561-2358399604dd" />

*Kuva 4. Ohjelman muuntaminen Intel HEX -muotoon ```objcopy```-komennolla ja muodostetun ```main.hex```-tiedoston tarkastelu.*

Tulosteessa näkyy ohjelman sisältämä data Intel HEX -muodossa. Tämä havainnollistaa, miten C-kielisestä lähdekoodista käännetty ohjelma on muutettu koneen käsiteltävään muotoon. 

## Lähteet
Tero Karvinen - Sovellusten hakkerointi: https://terokarvinen.com/application-hacking/#kertauspaketti Luettu: 20.8.2026
Create a Web Page Using Github: https://terokarvinen.com/2023/create-a-web-page-using-github/ Luettu: 20.8.2026
Tekoälyä (ChatGPT) on käytetty tehtävien ymmärtämisessä ja komentojen selittämisessä. Kaikki tehtävät on kuitenkin tehty itse ja testattu käytännössä.
