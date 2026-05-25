# Statisztikák

!!! info "Jogosultság"
    Ez az oldal kizárólag **Admin** szerepkörű felhasználóknak érhető el.

A Statisztikák oldal (`/dashboard/statistics`) átfogó képet ad a verseny vagy esemény aktuális állapotáról: játékosok, állomások és személyzet összesítve, diagramokkal és mutatókkal.

---

## Összesítő kártyák

Az oldal tetején négy fő mutató jelenik meg:

| Kártya | Mit mutat |
|---|---|
| **Játékosok** | Összes regisztrált játékos száma és az osztályok száma |
| **Személyzet** | Felhasználók száma, bontva szerepkörönként (operátor / regisztrátor / admin) |
| **Állomások** | Összes állomás, azon belül aktív és késő állomások száma |
| **Készenléti szint** | Az aktív állomások aránya, százalékban |

---

## Diagramok

### Játékosok osztály szerinti megoszlása

Vizuális bontás: melyik osztályból hány játékos vesz részt. Hasznos a csoportok arányának áttekintéséhez.

### Felhasználói szerepkörök

A rendszer személyzetének összetétele: állomáskezelők, regisztrátorok és adminok száma.

---

## Operatív mutatók

A bal oldali kártyán négy számított mutató látható:

| Mutató | Leírás |
|---|---|
| **Csúcspontszám** | A toplista első helyezettjének pontszáma |
| **Top 5 pontösszeg** | Az első öt játékos összesített pontszáma |
| **Átlagos késés** | Csak a ténylegesen késő állomások átlagos csúszása (percben) |
| **Átlagos max pont** | Az összes állomás maximális pontszámának átlaga |

### Állomás-egészség

A jobb oldali kártyán az állomások fizikai állapotát láthatod:

- **Legtöbbet késő állomás**: melyiken a legnagyobb a jelzett csúszás
- **Aktív állomások aránya**: vizuális sávval megjelenítve (aktív / összes)

---

## Toplista

Az oldal alján a legjobb játékosok rangsora látható, pontlogok alapján számítva.

### Szűrés állomásra

A toplista felett egy legördülő menüvel kiválasztható egy adott állomás – ekkor a rangsor csak az ott szerzett pontokat veszi figyelembe. Ha nincs állomás kiválasztva, az összes bejegyzést összesíti.

Minden játékosnál látható:

- Helyezés és neve
- Osztálya
- Összesített pontszáma
- Hány pontbejegyzés (látogatás) alapján számolódik
