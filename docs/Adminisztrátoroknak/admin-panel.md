# Admin Panel

Az Admin Panel (`/dashboard/panel`) egy tabulált vezérlőpult, amely a rendszer egészének valós idejű áttekintését és gyors beavatkozási lehetőségeket nyújt.

---

## Fullscreen mód

A panel jobb felső sarkában lévő **Fullscreen panel** gombbal az egész képernyőt lefoglalhatja a vezérlőpult. Kilépés ugyanott, az **Kilépés fullscreenből** gombbal.

---

## Általános tab

Az Általános tab **másodpercenként automatikusan frissül**.

### Összesítő kártyák

| Kártya | Mit mutat |
|---|---|
| Online felhasználók | Jelenleg aktív munkamenetek száma |
| Játékosok | Összes regisztrált játékos |
| Állomások | Összes konfigurált állomás |
| Panel státusz | Utolsó frissítés időpontja |

### Legutóbbi rendszerlogs

Az utolsó 5 rendszerbejegyzés (auth, tranzakció, audit) forrással, eseménnyel, érintettel és időponttal.

### Top állomások

A legjobb success rate-tel rendelkező állomások (átlagos pont / maximum pont arány alapján rangsorolva).

### Top 5 játékos

A pontszám szerinti élmezőny, osztállyal és sorszámmal.

### Üzenetküldés { #uzenetkuldes }

Online felhasználóknak azonnal küldhető admin értesítés, amely egy felugró ablakban jelenik meg a címzetteknél.

**Lépések:**

1. A jobb oldali panelben jelöld be a kívánt online felhasználókat, vagy kattints az **Összes online kijelölése** gombra
2. Írd be az üzenetet a szövegmezőbe
3. Kattints az **Üzenet küldése** gombra

!!! note "Megjegyzés"
    Csak az aktuálisan online felhasználók választhatók ki. Offline felhasználók nem kapják meg az üzenetet.

---

## Játékosok tab { #jatekosok-tab }

### Top 10 ranglistaósa

A pontszám szerinti első tíz játékos.

### Kereshető játékoslista

Az összes játékos kereshető névre, sorszámra és osztályra. A találatok számát az oldal jelzi.

### Sorszámcsere

Egy játékos sorszámát gyorsan módosíthatod megerősítő ablakból:

1. Keresd meg a játékost
2. Kattints a **Sorszám csere** gombra
3. Add meg az új sorszámot (pozitív egész szám)
4. Kattints a **Módosítás mentése** gombra

Az esemény automatikusan bekerül az audit naplóba.

---

## Állomások tab { #allomasok-tab }

**Másodpercenként automatikusan frissül.**

### Összesítő kártyák

Összes állomás, nyitott állomások száma, későállomások száma, bejelentkezett operátorral rendelkező állomások száma.

### Állomásfigyelő

Minden állomás egy kártyán jelenik meg. A kártyán látható:

- Állomás neve és sorszáma
- Nyitva/Zárva állapot (zöld/piros jelzőfény)
- Bejelentkezett operátor neve (ha van)
- Jelzett késés percben
- Utolsó jelenlét ideje

!!! tip
    Sárga keret jelzi azokat az állomásokat, ahol késés van beállítva – így egy pillantással látható, hol van probléma.

**Jelzőfény-jelmagyarázat:**

| Szín | Jelentés |
|---|---|
| 🟢 Zöld | Nyitva |
| 🔴 Piros | Zárva |
| 🟡 Sárga keret | Késés van jelezve |

---

## Felhasználók tab

**3 másodpercenként automatikusan frissül.**

### Összesítő kártyák

Összes felhasználó, online, állomáshoz rendelt és adminok száma.

### Felhasználói figyelő

Minden felhasználó egy kártyán jelenik meg. A kártyán látható:

- Profilkép, teljes név, felhasználónév
- Online/Offline státusz
- Szerepkör
- Hozzárendelt állomás (ha van)
- E-mail és telefonszám
- Utolsó naplózott aktivitás és időpontja
- Utolsó jelenlét (relatív idő, pl. „2 perc")

**Elérhető műveletek:**

- **Üzenet** gomb – csak online felhasználóknál aktív; egyéni admin üzenetet küldhetssz
- **Szerkesztés** gomb (ceruza ikon) – közvetlen link a fiók szerkesztési oldalára

---

## Logok tab

Az összes naplóforrásból (auth, tranzakció, audit) betöltött, kereshető összesítő.

**Szűrési lehetőségek:**

- Keresőmező: esemény, érintett, részlet vagy azonosító alapján
- Forrás legördülő: Auth / Tranzakció / Audit / Minden forrás

**Bejegyzés részletei:**

A **Megnézés** gombbal minden bejegyzésnél megnyílik egy részletes ablak: időpont, érintett, leírás és log azonosító.
