# PVA2 - Programování a vývoj aplikací
## Cvičení 11: Datum a čas

## Obsah

### 1 Aktuální datum a čas

Zobrazte uživateli **aktuální** datum/čas dle vzoru:
* `Rok Měsíc. Den.` např. `2024 12. 24.`
* `YYYY-MM/DD` např. `2024-12/24`
* `Hodiny:Minuty:Sekundy` např. `14:20:15`
* `2024-12-24 14:03:15`
* dle české normy vzor:`14. 12. 2024 13:02`

### 2. Výpočet s časem
Vypočtěte a zobrazte uživateli:
* Aktuální datum
* Zítřejší datum
* První den následujícího měsíce
* Poslední den následujícího měsíce
* Včerejší datum
* Datum splatnosti 14 dní od data vystavení
* Datum zdanitelného plnění před třemi dny


### 3. Lokalizované datum
Zobrazte pro libovolné datum výstup ve tvaru: 

Název dne, Číslo dne, Název měsíce, rok

`Pro 20.2.2023` očekávaný výstup: `Monday 20 February 2023`

### 4 Délka trvání události
Vytvořte funkci, která přijímá dvě data a časy a vrací délku trvání mezi nimi ve formě přehledného textu, například `3 dny, 4 hodiny a 30 minut`.

### 5 Události v budoucnosti 
Vytvořte funkci, která vytvoří seznam následujících 5 událostí, které se budou konat každý měsíc ve stejný den a čas jako aktuální datum.

### 6 Relativní čas
Formátování relativního času: Vytvořte kód, který přijme časový údaj a vypíše ho ve formátu relativního času, například `před 5 minutami`, `před 2 dny`, atd.

### 7 Prodej ubytování
Vytvoř program na prodej ubytování v rámci malého hotelu. Ceny ubytování jsou v tabulce níže.

| Datum | Cena |
| ------------- |-------------:| 
| 3. 1. 2025 - 31. 5. 2025 | 2900 Kč | 
| 1. 6. 2025 - 31. 8. 2025 | 3500 Kč | 
| 1. 9. 2025 - 22. 12. 2025 | 2500 Kč |
| 23. 12. 2025 - 2. 1. 2026 | 4200 Kč |

Z důvodu rekonstrukce bude hotel v únoru a březnu uzavřen.

Tvůj program se nejprve zeptá uživatele na datum a počet osob, pro které uživatel chce ubytování koupit. Uživatel zadá datum ve středoevropském formátu. Převeď řetězec zadaný uživatelem na datum pomocí funkce `datetime.strptime()`.

Pokud by uživatel zadal příjezd mimo otevírací dobu, vypiš, že je hotel v této době uzavřen. Pokud je hotel v provozu, spočítej a vypiš cenu za ubytování.

Data lze porovnávat pomocí známých operátorů <, >, <=, >=, ==, !=. Tyto operátory můžeš použít v podmínce if. Níže vidíš příklad porovnání dvou dat. Program vypíše text `První datum je dřívější než druhé datum.`.
