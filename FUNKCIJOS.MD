## 🎬 25 funkcijos
 
 
### 👤 Domantas Lopatevas – Klientų ir filmų peržiūra
1.	Peržiūrėti filmų sąrašą
2.	Ieškoti filmo pagal pavadinimą
3.	Filtruoti filmus pagal žanrą, kalbą ir amžiaus cenzą
4.	Peržiūrėti išsamią filmo informaciją:
    *	Pagrindiniai duomenys gaunami iš sistemos DB
    *	Aprašymas, plakatas, aktoriai ir anonsas gaunami iš TMDB API
    *	Tinkamas TMDB filmas parenkamas pagal pavadinimą ir išleidimo metus
    *	Nepasiekiant TMDB API, rodoma sistemos DB saugoma informacija
5.	Peržiūrėti filmo atsiliepimus
6.	Parašyti filmo atsiliepimą ir skirti 1–5 balų įvertinimą
    *	Atsiliepimą gali rašyti tik prisijungęs klientas
    *	Vienas klientas vienam filmui gali pateikti tik vieną įvertinimą
    *	Klientas gali redaguoti tik savo atsiliepimą
    *	Klientas gali pašalinti tik savo atsiliepimą
7.	Apskaičiuoti filmo įvertinimo vidurkį pagal klientų įvertinimus
    *	Naudojami visi klientų skirti įvertinimai
    *	Pakeitus įvertinimą, vidurkis perskaičiuojamas
    *	Pašalinus įvertinimą, vidurkis perskaičiuojamas
    *	Rezultatas pateikiamas vieno skaičiaus po kablelio tikslumu, pvz. 4,2 iš 5

---
 
 ### 🎬 Gustavas Bliuva – Filmų valdymas
 
 6. Pridėti filmą
7. Redaguoti filmo informaciją
8. Pašalinti filmą
9. Priskirti filmui žanrą
10. **Automatiškai nustatyti, ar filmas šiuo metu rodomas, pagal rodymo pradžios ir pabaigos datas**
 
 > Pvz. jei šiandien yra tarp pradžios ir pabaigos datos → `RODOMAS`, kitu atveju → `NERODOMAS`.
 
---
 
 ### 🕐 Nojus Žeimys – Seansų valdymas
 
 11. Sukurti seansą
12. Redaguoti seansą
13. Atšaukti seansą
14. Peržiūrėti dienos seansų tvarkaraštį
15. **Patikrinti, ar naujas seansas nesikerta su kitu tos pačios salės seansu**
 
 Čia jau labai gera **advanced funkcija**.
 
 Pvz.:
 
```
Sala 1
 
18:00 ───── 20:00  Avatar
19:30 ───── 21:30  Minecraft
```
 
 Sistema turi neleisti sukurti antro seanso, nes laikai persidengia.
 
---
 
 ### 🎟️ Arminas Balčius – Bilietai ir rezervacijos
 
 16. Peržiūrėti laisvas ir užimtas vietas
17. Pasirinkti konkrečią vietą
18. Rezervuoti bilietą
19. Atšaukti rezervaciją
20. **Apskaičiuoti galutinę bilieto kainą pagal bilieto tipą, vietą ir nuolaidą**
 
 Pvz.:
 
```
Standartinis bilietas       8 €
VIP vieta                  +3 €
Studento nuolaida         -20 %
 
Galutinė kaina = 8.80 €
```
 
 Čia jau tikrai galima parodyti skaičiavimą per gynimą.
 
---
 
 ### 🏢 Laurynas Barzdenys – Administravimas ir statistika
 
 21. Pridėti ir redaguoti kino salę
22. Valdyti salės sėdimų vietų išdėstymą
23. **Apskaičiuoti konkretaus seanso užimtumo procentą**
24. **Apskaičiuoti kino teatro pajamas už pasirinktą laikotarpį**
25. **Nustatyti populiariausią filmą pagal parduotų bilietų skaičių**
 
 Pvz.:
 
```
Seansas: Avatar
Salės talpa: 100
Parduota: 73
 
Užimtumas = 73 / 100 × 100 = 73 %
```
 
 O pajamoms:
 
```
01-09-2026 → 07-09-2026
 
Parduota bilietų: 428
Bendra pajamų suma: 3 624 €
```
 
---
 
 # 🔥 Kurios funkcijos jau yra „advanced“?
 
 - **Filmo įvertinimo vidurkio skaičiavimas**
- **Filmo rodymo statuso nustatymas pagal datas**
- **Seansų laiko susikirtimo tikrinimas**
- **Bilieto galutinės kainos skaičiavimas**
- **Seanso užimtumo procento skaičiavimas**
- **Pajamų skaičiavimas**
- **Populiariausio filmo nustatymas**
 
 ### Dar vieną advanced funkciją galima pridėti vietoj paprasto „žanro priskyrimo“:
 
 **„Rekomenduoti klientui filmus pagal jo žiūrėtų filmų žanrus ir įvertinimus.“**
 
 Pvz. klientas daugiausiai žiūri `Action` ir `Sci-Fi`, todėl sistema jam parodo aukščiausiai įvertintus šių žanrų filmus.
