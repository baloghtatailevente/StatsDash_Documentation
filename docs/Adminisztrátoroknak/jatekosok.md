# Játékosok kezelése

A Játékosok oldal adminisztrátori nézete megegyezik a regisztrátori nézettel, de kiegészül a szerkesztési és törlési funkciókkal.

Részletes leírás az oldalról: [Játékosok](../felhasznaloi/jatekosok.md)

---

## Új játékos hozzáadása

Az **Új játékos** gombra kattintva add meg az adatokat:

| Mező | Kötelező? | Leírás |
|---|---|---|
| Név | Igen | A játékos teljes neve |
| Sorszám | Igen | Egyedi azonosítószám (pozitív egész) |
| Osztály | Igen | A beállításokban létrehozott osztályok közül választható |
| Pontszám | Nem | Alapértelmezetten 0 |

!!! tip
    Az osztályok a [Beállítások](beallitasok.md) oldalon kezelhetők. Ha az osztály nem szerepel a listában, előbb ott kell létrehozni.

---

## Játékos szerkesztése

A listában minden sornál elérhető a szerkesztés. Módosítható: név, sorszám, osztály, pontszám.

---

## Játékos törlése

A szerkesztési oldalon elérhető a törlés. Az érintett pontbejegyzések megmaradnak, de játékos-hivatkozás nélkül.

---

## Sorszámcsere az Admin Panelből

Ha verseny közben kell sorszámot módosítani, azt az [Admin Panel → Játékosok tab](admin-panel.md#jatekosok-tab) felületről is elvégezheted – megerősítő ablakkal és automatikus audit naplóbejegyzéssel.
