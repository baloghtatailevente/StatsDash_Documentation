# Állomások kezelése

Az Állomások oldal (`/dashboard/stations`) az összes konfigurált állomást listázza, és innen kezelhető a teljes infrastruktúra.

---

## Az oldal tartalma

A keresőmezővel szűrhetsz névre, sorszámra, képletre vagy állapotra. Az adatok táblázatos és kártyás nézetben is megtekinthetők.

Minden állomásnál látható:

| Mező | Leírás |
|---|---|
| **Név** | Az állomás megjelenítési neve |
| **Sorszám** | Egyedi sorszám (pl. 1, 2, 3…) |
| **Maximum pont** | Az állomáson szerezhető legmagasabb pont |
| **Képlet** | Pontszámítási képlet (ha be van állítva) |
| **Állapot** | Nyitva / Zárva |
| **Késés** | Aktuálisan jelzett késési perc |

---

## Új állomás hozzáadása

Az **Új állomás** gombbal megnyíló felületen add meg az adatokat:

**Kötelező mezők:**

- Név
- Sorszám (egyedi egész szám)
- Maximum pont

**Opcionális:**

- Képlet – matematikai kifejezés, amely a pontszámítást segíti (pl. `x * 10 - y`). Ez jelenik meg az állomás számológépében.
- Kép URL – az állomás megjelenítési képe
- Állapot – alapértelmezetten **Zárva**

---

## Állomás szerkesztése

A listában minden sornál elérhető a szerkesztés link. Az összes fenti adat módosítható.

!!! note "Megjegyzés"
    Az állapot és a késés az állomás kezelőfelületéről (`/dashboard/station/<id>`) is módosítható valós időben – az operátor is tudja kezelni.

---

## Állomás törlése

A szerkesztési oldalon elérhető a törlés. Törlés előtt a rendszer megerősítést kér.

!!! warning
    Ha az állomáshoz felhasználó van rendelve, a törlés után azok a fiókok elveszítik az állomás-hozzárendelésüket. Az állomáshoz tartozó pontbejegyzések megmaradnak, de állomás-hivatkozás nélkül.
