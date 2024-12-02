# MedicineStorage
Sovelluksessa käytetään:
- C++
- Python, flask
- CSS
- SQL
- PythonAnywhere
- Gmail

Projektin toimintaa ja ulkoasua voidaan tarkastella [tästä](https://laaketilat.eu.pythonanywhere.com/kirjaudu). (Haku-ominaisuus on keskeneräinen ja sovelluksen ulkoasua sekä ominaisuuksia tullaan päivittämään).
- Käyttäjätunnus: testaaja
- Salasana: salasana
  
Projektissa tehtiin järjestelmä, jonka avulla lääkehuoneen tilan olosuhteita voidaan valvoa. Huoneeseen sijoitettiin neljä ESP32-alustaa (4 solmua), joista yksi keräsi kaikilta solmuilta saadut tiedot ja
lähetti ne eteenpäin tietyin aikavälein PythonAnywheressä olleelle web-palvelimelle. Sensoreista kerätty data tallennettiin PythonAnywheressä sijaitsevaan tietokantaan. Projektissa tehtiin käyttöliittymä, jossa
käyttäjältä vaadittiin salasana ja käyttäjätunnus lääkehuoneen eri tilojen olosuhteiden tarkastelemiseksi. Käyttäjä pystyi tarkastelemaan lääkehuoneen eri alueiden olosuhteita ja hän sai reaaliaikaisesti tiedon poikkeavista arvoista käyttöliittymään, jolloin käyttäjän tuli kuitata poikkeava-arvo. Poikkeavien arvojen kuittaus tallennettiin tietokantaan. Hälytys poikkeavasta arvosta lähetettiin myös käyttäjän sähköpostiin.\
Koska mittaukset ja kuittaukset tallennettiin tietokantaan käyttäjä pystyi myös tarkastelemaan aikaisempien päivien mittauksia hakutoiminnon avulla ja käyttäjän sähköpostiin voitiin lähettää
joka päivä klo 7.00 kooste edellisen päivän mittausarvoista ja poikkeavista arvoista. Projekti perustuu [sulautettujen  järjestelmien -loppuprojektiin](https://github.com/Okkimonkiainen/Studies/tree/main/EmbeddedSystems/fridge-project-main), jonka toimintaa korjataan ja päivitetään tässä projektissa. 
