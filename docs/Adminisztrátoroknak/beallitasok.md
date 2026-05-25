# Beállítások

A Beállítások oldal (`/dashboard/settings`) két fő funkciót tartalmaz: a játékos osztálylista kezelését és az alkalmazásrészek zárolását.

---

## Játékos osztálylista

Az osztályok határozzák meg, hogy a játékosok milyen csoportokba sorolhatók (pl. „9.A", „10.B", „Felnőtt").

### Új osztály hozzáadása

1. Az **Új osztály** mezőbe írd be az osztály nevét
2. Kattints a **Hozzáadás** gombra

### Aktiválás és inaktiválás

Minden osztálynál megjelenik az aktuális státusza (**Aktív** / **Inaktív**), és az **Aktiválás** / **Inaktiválás** gombbal váltható.

| Státusz | Mit jelent |
|---|---|
| Aktív | Az osztály megjelenik a játékos-felvételi és szerkesztési felületeken |
| Inaktív | Az osztály nem választható új játékosnál, de a már hozzárendelt játékosoknál megmarad |

### Osztály törlése

A kuka ikon csak akkor aktív, ha az osztályhoz **egyetlen játékos sincs rendelve**. Ha van játékos az osztályban, a gomb szürke és inaktív.

!!! tip
    Ha törölni szeretnél egy osztályt, előbb mozgasd át vagy töröld az összes hozzá tartozó játékost.

---

## Alkalmazásrészek zárolása

Az egyes rendszerterületek adminisztrátori döntéssel zárolhatók. Zárolás után az érintett felhasználók egy tájékoztató oldalra kerülnek, és nem érhetik el az adott funkciót.

### Zárolható szegmensek

| Szegmens | Mit érint |
|---|---|
| Kezdőlap | A dashboard főoldal |
| Játékosok | A játékoslista oldal |
| Állomások | Az állomáslista oldal |
| Statisztika | A statisztikák oldal |
| Napló | A napló aloldalak |
| Állomás | Az állomás-kezelő felületek |
| Teljes alkalmazás | Minden oldal egyszerre |

### Zárolás és feloldás

Minden szegmens kártyáján egy gomb látható:

- **Zárolás** – zölddel jelzett (elérhető), piros gombbal zárható
- **Feloldás** – pirossal jelzett (zárolt), zöld gombbal feloldható

A lakat ikon és a keret színe azonnal jelzi az aktuális állapotot.

!!! danger "Teljes alkalmazás zárolása"
    Ha a **Teljes alkalmazás** szegmenst zárolod, **minden nem-admin felhasználó** kizáródik a rendszerből – az összes oldal a „zárolt" tájékoztatót fogja mutatni nekik. Adminok tovább hozzáférnek.

    Zárolás előtt győződj meg arról, hogy a többi felhasználó értesítve van, vagy le van jelentkezve.
