# Naplók

A naplóoldalak a navigáció **Napló** almenüjéből érhetők el. Három különálló nézet elérhető, mindegyik más forrásra fókuszál.

!!! info "Jogosultság"
    Minden naplóoldal kizárólag **Admin** szerepkörű felhasználóknak érhető el.

---

## Azonosítási logok

**URL:** `/dashboard/logs/authentication`

Minden belépési kísérlet rögzítve van itt – sikeres és sikertelen egyaránt.

### Összesítő kártyák

| Kártya | Leírás |
|---|---|
| Összes esemény | Az utolsó 100 azonosítási esemény száma |
| Sikeres | Sikeresen hitelesített belépések |
| Sikertelen | Hibás felhasználónév vagy jelszó miatti elutasítások |
| Egyedi felhasználók | Hány különböző felhasználónév szerepel a naplóban |

### Szűrés

- **Státusz**: Összes / Sikeres / Sikertelen
- **Keresés**: felhasználónév, e-mail vagy esemény szövege alapján

### Mikor hasznos?

- Gyanús belépési kísérleteket kell ellenőrizni
- Meg kell tudni, mikor lépett be egy adott felhasználó

---

## Tranzakciós logok

**URL:** `/dashboard/logs/transactions`

Az összes pontregisztrációs esemény listája.

### Minden bejegyzésnél látható

- Játékos neve és sorszáma
- Állomás neve és sorszáma
- Rögzített pontszám
- Időpont
- Leírás (a rendszer automatikusan generálja)

### Szerkesztés

Egyes bejegyzéseknél elérhető szerkesztési lehetőség – hibás pontbejegyzés esetén itt korrigálható.

### Mikor hasznos?

- Egy játékos pontjait kell ellenőrizni vagy visszakeresni
- Hibásan rögzített pontot kell javítani

---

## Összes log

**URL:** `/dashboard/logs/all`

Kombinált, időrendi nézet: azonosítási, tranzakciós és audit (rendszerszintű módosítások) bejegyzések együtt.

### Összesítő kártyák

| Kártya | Leírás |
|---|---|
| Összes bejegyzés | A három forrásból összefűzött legfrissebb bejegyzések száma |
| Auth logok | Belépési események |
| Tranzakciók | Pontregisztrációs események |
| Audit események | Felhasználó-, játékos- és állomásműveletek |

### Szűrési lehetőségek

| Szűrő | Lehetséges értékek |
|---|---|
| Forrás | Minden forrás / Auth / Tranzakció / Audit |
| Művelet | CREATE, UPDATE, DELETE, REGISTER_POINTS, UPDATE_DELAY, UPDATE_STATUS |
| Entitás | USER, PLAYER, STATION, POINTS |
| Keresés | Esemény, érintett, részlet vagy log azonosító |

### Bejegyzés részletes nézete

A **Megnézés** gombra kattintva egy felugró ablak jelenik meg a teljes bejegyzéssel: időpont, forrás, érintett, részletes leírás és a log egyedi azonosítója.

### Mikor hasznos?

- Egy adott esemény teljes nyomvonalát kell visszakeresni
- Auditáláshoz vagy ellenőrzéshez szükséges az összes forrás egyszerre
