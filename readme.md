# PVA2 - Programování a vývoj aplikací
## Cvičení 11: Datum a čas

### 1 

* Zobazte aktuální datum a čas
* Zobrazte aktuální datum
* Zobrazte aktuální čas

### 2
Vystavujete fakturu. Vypočítejte a zobrazte datum splatnosti 14 dní od data vystavení. Datum zdanitelného plnění je před pěti dny.


### 3
Zobrazte pro libovolné datum výstup ve tvaru:
Název dne, Číslo dne, Název měsíce, rok

`Pro 20.2.2023` očekávaný výstup: `Monday 20 February 2023`

### 4
* K aktuálnímu času přičtěte 6 dní a 3 hodin
* K specifickému datu přičtěte 12 dní a 6 hodin

### 5
Zobrazte aktuální čas v milisekundách

### 6
Vytvořte funkci calcDays. Funkce bude vracet počet dnů mezi dvěma daty. 

Obě data zadá uživatel

### 7
Prodej ubytování
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
