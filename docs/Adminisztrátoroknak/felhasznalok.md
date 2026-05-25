# Felhasználók kezelése

A Felhasználók oldal (`/dashboard/users`) az összes munkatársi fiókot jeleníti meg, és innen kezelhető a teljes személyzet.

---

## Az oldal tartalma

### Összesítő statisztikák

Az oldal tetején kártyák mutatják az összes fiók, online/offline arány, adminok száma és más kulcsmutatók összesítését.

### Lista és keresés

A lista táblázatos és kártyás nézetben is megtekinthető. A keresőmezővel szűrhetsz:

- Név (kereszt- vagy vezetéknév)
- Felhasználónév
- E-mail cím
- Hozzárendelt állomás neve

---

## Szerepkörök

| Kód | Megnevezés | Jogosultságok |
|---|---|---|
| `0` | Állomáskezelő | Kezdőlap, saját állomás |
| `1` | Regisztrátor | Kezdőlap, Játékosok |
| `99` | Admin | Teljes hozzáférés |

---

## Új felhasználó létrehozása

Az **Új felhasználó** gombbal megnyíló felületen add meg az adatokat:

**Kötelező mezők:**

- Keresztnév, vezetéknév
- Felhasználónév (egyedi, csak kisbetű és szám ajánlott)
- E-mail cím
- Telefonszám
- Jelszó
- Szerepkör

**Opcionális:**

- Állomáshoz rendelés (melyik állomást kezeli)
- Egyedi belépési kód
- Profilkép URL

!!! tip
    Az állomáshoz rendelés nélküli felhasználó is be tud lépni, de az állomás kezelőfelületéhez nem férhet hozzá.

---

## Felhasználó szerkesztése

A listában minden sornál elérhető a szerkesztés gomb. A szerkesztési oldalon módosítható:

- Személyes adatok (név, e-mail, telefon)
- Jelszó (ha szükséges visszaállítás)
- Szerepkör
- Hozzárendelt állomás
- Profilkép URL

---

## Felhasználó törlése

A szerkesztési oldalon elérhető a törlés gomb. Törlés előtt a rendszer megerősítést kér.

!!! warning
    A törlés visszafordíthatatlan. A felhasználó összes munkamenet-adata elvész, de a rögzített pontbejegyzések és naplók megmaradnak (a fiók-hivatkozás nélkül).
