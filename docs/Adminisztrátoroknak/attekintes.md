# Admin leírás – Áttekintés

!!! warning "Csak adminoknak"
    Az ebben a szekcióban leírt funkciók kizárólag **Admin (rank 99)** szerepkörű fiókokkal érhetők el. Más jogosultságú felhasználók automatikusan a Kezdőlapra kerülnek, ha megpróbálják elérni ezeket az oldalakat.

---

## Az admin felületek térképe

| Oldal | URL | Funkció |
|---|---|---|
| Felhasználók | `/dashboard/users` | Fiókok kezelése, szerepkörök, állomáshoz rendelés |
| Állomások | `/dashboard/stations` | Állomás konfiguráció, képlet, max pont |
| Játékosok | `/dashboard/players` | Játékoslista, pontok, osztályok |
| Statisztikák | `/dashboard/statistics` | Átfogó operatív mutatók |
| Admin Panel | `/dashboard/panel` | Valós idejű felügyelet, üzenetküldés, sorszámcsere |
| Beállítások | `/dashboard/settings` | Osztálylista, zárolások |
| Naplók | `/dashboard/logs/*` | Auth, tranzakció és audit naplók |

---

## Részletes leírások

- [Felhasználók kezelése](felhasznalok.md)
- [Állomások kezelése](allomasok.md)
- [Játékosok kezelése](jatekosok.md)
- [Admin Panel](admin-panel.md)
- [Beállítások](beallitasok.md)
- [Naplók](naplok.md)

---

## Legjobb gyakorlatok

### Esemény megkezdése előtt

- [ ] Hozd létre az összes osztályt a [Beállítások](beallitasok.md) oldalon
- [ ] Rögzítsd az összes állomást a megfelelő konfigurációval
- [ ] Rendeld hozzá a felhasználókat az állomásokhoz
- [ ] Ellenőrizd, hogy minden szegmens feloldott (nem zárolva)

### Esemény közben

- Kövesd az online felhasználókat és az állomások állapotát az [Admin Panel → Általános](admin-panel.md#altalanos-tab) tabon
- Figyelj a késésekre az [Állomások](admin-panel.md#allomások-tab) tabon
- Operatív értesítést az [Üzenetküldés](admin-panel.md#uzenetkuldes) funkcióval küldhetsz

### Esemény után

- Tekintsd át a naplókat a [Naplók](naplok.md) oldalon
- A [Statisztikák](../felhasznaloi/statisztikak.md) oldalon ments el képernyőképet az eredményekről
- Szükség esetén zárold a szegmenseket a [Beállítások](beallitasok.md) oldalon
