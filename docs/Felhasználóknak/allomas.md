# Állomás kezelése

Az állomás kezelőfelülete (`/dashboard/station/<azonosító>`) a pontregisztráció központja. Ide a Kezdőlapról, vagy az állomás kártyájára kattintva juthatsz.

---

## Az oldal elrendezése

Az oldal három fő részre oszlik:

```
[ Állapot vezérlő ] [ Pontbeviteli felület ] [ Késés vezérlő ]
     (bal oldal)          (középen)              (jobb oldal)
```

A bal alsó sarokban a **Sztornó** gomb, mellette a **Számológép** gomb található.

---

## Állapot vezérlő (Nyitva / Zárva)

Az állomás csak **Nyitva** állapotban fogad pontbevitelt. Zárva állapotban a billentyűzet inaktív.

Az állapotot egy gombnyomással válthatod:

- **Nyitva** → a billentyűzet aktív, kezdhető a pontregisztráció
- **Zárva** → a bevitel letiltva

!!! note "Megjegyzés"
    Az állapotváltás azonnal megjelenik az Admin Panelen – az adminisztrátorok valós időben látják, melyik állomás aktív.

---

## Pontregisztráció

### 1. lépés – Játékos azonosítása

A képernyő közepén lévő numerikus billentyűzettel add meg a játékos **sorszámát**.

- A **DEL** gomb törli az utolsó bevitt számjegyet
- Az **OK** gomb indítja a keresést

**Lehetséges eredmények:**

| Visszajelzés | Jelentés |
|---|---|
| Játékos neve és adatai megjelennek | Sikeres azonosítás, folytatható a pontbevitel |
| *„A játékos nem található"* | A sorszám nem létezik a rendszerben |
| *„A játékos már járt ezen az állomáson"* | Ismételt regisztráció nem lehetséges – ez a játékos az adott állomáson már kapott pontot |

### 2. lépés – Pontszám megadása

Sikeres azonosítás után a bal felső sarokban megjelenik a játékos neve, aktuális pontszáma és osztálya. A billentyűzet átáll **pontbeviteli módba**.

Add meg az elért pontszámot, majd nyomd meg az **OK** gombot.

!!! warning "Maximum pontszám"
    A megadott pontszám nem haladhatja meg az állomás beállított maximumát. Ha mégis megpróbálod, a rendszer hibaüzenetet jelenít meg és nem menti a pontot.

### 3. lépés – Mentés és visszaállás

Sikeres mentés után a rendszer visszajelzést ad, majd automatikusan visszaáll az 1. lépésre – készen a következő játékosra.

---

## Sztornó

Ha félbeszakadt a folyamat, hibás sorszámot adtál meg, vagy más okból vissza kell lépni:

1. Kattints a bal alsó sarokban lévő piros **Sztornó** gombra
2. A megjelenő megerősítő ablakban kattints a **Sztornózás** gombra

!!! info
    A Sztornó csak az **aktuális, még el nem mentett folyamatot** törli. A már sikeresen rögzített pontokat nem módosítja.

---

## Számológép

A Sztornó gomb melletti kalkulátor ikon megnyitja az állomáshoz tartozó **képletalapú számológépet**. Hasznos, ha a pontszámot valamilyen számítás (pl. idő × szorzó) alapján kell meghatározni. A képletet az adminisztrátor állítja be az állomás konfigurációjában.

---

## Késés jelzése

Ha az állomáson várakozás keletkezik (pl. technikai probléma, lassabb folyamat), jelezd a rendszerben is:

- **Jobb oldalt** találod a Késés vezérlőt
- Az adott gomb megnyomásával a rajta található késési idő állítható be.

A jelzett késés azonnal megjelenik az Admin Panelen és a Statisztikák oldalon, így az adminisztrátorok az összes állomás terhelési helyzetét átláthatják.

!!! tip
    Ha a forgalom rendeződött, állítsd vissza a késést nullára, hogy a monitor naprakész maradjon.
