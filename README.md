Market

Planned feature:
* Käyttäjä pystyy luomaan tunnuksen ja kirjautumaan sisään sovellukseen.
* Käyttäjä pystyy lisäämään sovellukseen ilmoituksia. 
* Lisäksi käyttäjä pystyy muokkaamaan ja poistamaan lisäämiään ilmoituksia.
* Käyttäjä näkee sovellukseen lisätyt ilmoitukset. 
* Käyttäjä pystyy etsimään ilmoituksia hakusanalla tai muulla perusteella. 
* Sovelluksessa on henkilökohtaiset käyttäjäsivut, jossa käyttäjä voi hallita profiiliaan ja ilmoituksiaan.
* Käyttäjä pystyy valitsemaan ilmoitukseen useamman luokittelun. Mahdolliset luokat ovat tietokannassa.
* Käyttäjä voi tarkastella toisen käyttäjän profiilia ja ilmoituksia.
* Käyttäjä voi lähettää viestin toiselle käyttäjälle.

Feature list 31.3

Käynnistysohjeet:
1. Kloonaa repo.
2. Asenna ekaksi virtuaaliympäristo komennolla: source venv/bin/activate
3. Asenna riippuvuudet: pip install -r requirements.txt
4. Käynnistä ohjelma: flask run
5. Avaa ohjelma omaan selaimeen napauttamalla hiirellä osoitetta http://127.0.0.1:5000
6. Tee käyttäjätunnus ja kirjaudu sisälle.

Ominaisuudet:
* Käyttäjä pystyy luomaan tunnuksen ja kirjautumaan sisään sovellukseen.
* Vain kirjautunut käyttäjä pystyy katselemaan ilmoituksia ja pääsemään kauppaan sisälle.
* Käyttäjä pystyy lisäämään, sekä muokkaamaan ja poistamaan omia ilmoituksia.
* Käyttäjä näkee sovellukseen lisätyt ilmoitukset.
* Käyttäjä pystyy etsimään ilmoituksia hakusanalla tai muulla perusteella.
* Estetty pääsy muokkaamaan tai poistamaan toisen käyttäjän ilmoituksia, eli lisätty oikeuksien tarkitukset.

Feature list 16.4
* Käyttäjä pystyy luomaan tunnuksen ja kirjautumaan sisään sovellukseen.
* Vain kirjautunut käyttäjä pystyy katselemaan ilmoituksia ja pääsemään kauppaan sisälle.
* Käyttäjä pystyy lisäämään, muokkaamaan ja poistamaan omia ilmoituksia.
* Käyttäjä pystyy myös lisäämään ilmotukselle kuvan (kuva tiedostossa), kappalemäärän, tavaraluokan ja kuntoluokan.
* Käyttäjä näkee sovellukseen lisätyt ilmoitukset.
* Käyttäjä pystyy etsimään ilmoituksia hakusanalla.
* Käyttäjä pystyy tekemään ostoksia ja ostokset menevät ostoskoriin.
* Käyttäjä pystyy muokkaamaan ostoskoria (poistamaan tai päivittämään ostettavien tuotteiden kpl määriä).
* Ostoskorissa ei pysty lisäämään tuotteita enempää kuin mitä myyjä on asettanut varastosaldoksi.
* Käyttäjä pystyy lähettämään muille käyttäjälle viestejä ja viestit tulevat näkymään Messages -sivulle.
* Viestit päivittyvät näkymään viestiketjuissa Messages -sivulle.
* Käyttäjä pystyy poistamaan viestiketjun.
* Lisätty Fernet salaus viestien tallentamiseen.
* Lisätty CSRF-suoja, lokitus ja rate limitteri.
* Lisätty yksinkertainen CAPTCHA 
* Lisätty profiilikuvan lisäysmahdollisuus (kuva taulussa BLOB)
* Lisätty sivutus
* Lisätty seed.py ja testattu seuraavilla arvoilla ilman huomattua hitautta:
user_count = 100000
item_count = 1000000
message_count = 100000
purchase_count = 100000
* Lisätty indeksointi items tauluun
* Lisätty tauluihin validointeja
* Lisätty melkein valmis CSS
* Lisätty label kentät
* Poistettu ulkopuoliset kirjastot
* Poistettu CAPTCHA
* Vaihdettu myös tuotteiden kuvat käyttämään tietokantaa (BLOB)
* Tuotteille lisätty kommentointi ja arvostelu
* (Tuotteilla on myös valittavana kaksi eri kategoriaa)
* Merkkijonoissa käytetty "
* Käyttökokemukseen kiinnitetty huomiota, mutta tarkoitus on kuitenkin, että kauppaan pitää kirjautua ennen kuin
tuotteita pääsee katsomaan
* Virheilmoitukset päivitetty
* Pitkät viestit laitettu rivittymään



TODO:
- seed.py toimimaan
- näyttää että tuotetta ei saatavilla jos varastosaldo mennyt nollaan.
- Checkout (selvitä palveluntarjoajien API:t).
- Profiilin sivu jonne käyttäjä syöttää tietonsa
- Lisää alasivuja, jossa tietoa Supermarketista
...
