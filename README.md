# volleyball-championship-database

**MySQL/MariaDB baza podataka** je namenjena za evidenciju i praćenju odbojkaškog prvenstva. Projekat demonstrira veštine u dizajnu baza podataka, radu sa tabelama, SQL upitima, pogledima, uskladištenim procedurama, okidačima i transakcijama.

## Struktura baze

Baza se sastoji od šest povezanih tabela:  
- **Reprezentacija** – čuva podatke o državama koje učestvuju  
- **Igrac** – sadrži informacije o igračima, njihovim performansama i reprezentacijama  
- **Igra** – evidentira statističke podatke o igračima u pojedinačnim utakmicama  
- **Utakmica** – beleži podatke o odigranim mečevima, fazama takmičenja i rezultatima  
- **Dvorana** – sadrži informacije o dvoranama u kojima se utakmice održavaju  
- **Sudija** – čuva podatke o sudijama i utakmicama koje sude  

---

## Funkcionalnosti baze

Baza omogućava niz operacija i analiza nad podacima:  

- **Filtriranje i izdvajanje podataka:**  
  - Pregled statistike igrača po parametrima, kao što su broj aseva, blok poena, grešaka pri servisu i autova, sa mogućnošću sortiranja i filtriranja po uslovima.  

- **Pogledi:**  
  - Kreirani pogledi omogućavaju jednostavno praćenje informacija, npr. koji sudija je sudio koje utakmice, sa prikazom imena, prezimena, datuma, vremena i faze takmičenja.  

- **Uskladištene procedure:**  
  - Automatski izvode složene upite, poput pronalaženja igrača sa najmanjim brojem poena u odnosu na izabranog igrača, uz korišćenje parametara.  

- **Okidači:**  
  - Proveravaju i ograničavaju unos podataka u tabelu `Utakmica`, osiguravajući validnost vrednosti setova.  

- **Transakcije:**  
  - Omogućavaju sigurno unošenje novih igrača, uz proveru da li je reprezentacija već unesena, automatsko određivanje primarnog ključa i kontrolu grešaka.  

---

## Korišćena tehnologija

Baza je kreirana i administrirana pomoću **phpMyAdmin**, alata koji omogućava jednostavno upravljanje MySQL/MariaDB bazama podataka preko web interfejsa.  
Karakteristike uključuju:  

- Kreiranje, modifikaciju i brisanje baza, tabela i kolona  
- Upravljanje korisničkim privilegijama i pristupom  
- Izvršavanje i uređivanje SQL upita  
- Rad sa uskladištenim procedurama, pogledima i okidačima  
- Export i import podataka u različitim formatima  
- Prikaz grafičke strukture baze i administracija više servera  

---

## Preuzimanje baze

Bazu možete preuzeti kao **ZIP fajl**:  
- `odbojkasko_prvenstvo.sql` – sadrži strukturu i podatke tabela  
- `radbaze.txt` – pokazuje rad sa podacima, uključujući upite, poglede, procedure, okidače i transakcije  
