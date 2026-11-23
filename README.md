# E.ON Szerelő – Gyors hibajelentés

Az 1. csapat megoldása az **E.ON × Corvinus UX/UI Design Day** szerelői app kihívására.

A terepi szerelő (Péter) a helyszínen talált hibát kb. egy perc alatt, gépelés nélkül jelzi a megfelelő csapatnak, és élőben látja, ki látta és ki jön.

## Mi van a repóban

| Útvonal | Tartalom |
|---|---|
| `index.html` | A működő app-demó: szerelő és kolléga nézet, fotó, azonosítás, súlyosság igen/nem kérdésekből, küldés, élő státusz, offline sor |
| `prototipus/` | A kattintható prototípus (forgatókönyv szerint végigkattintható) |
| `PRODUCT.md` | Termékleírás: felhasználók, cél, korlátok, elvek |

## Futtatás

Egyetlen önálló HTML-fájl, nincs build. Megnyitható közvetlenül böngészőben, vagy a GitHub Pages oldalon.

## Két futási mód

Az app a Claude artifact környezetében kapja a közös, élő adatbázist, a képfelismerést és a diktálást. **GitHub Pages-en ezek nem érhetők el**, ott az app egy eszközön működik:

- a bejelentések az adott böngészőben maradnak (helyi sor),
- a hibatípust kézzel kell kiválasztani (nincs automatikus javaslat),
- diktálás helyett a telefon billentyűzetének mikrofonja használható.

A két telefonos, élőben szinkronizált bemutatóhoz a Claude artifact verziót érdemes használni.

## Megjegyzés

Minden cím, munkalapszám és név fiktív, bemutatási célra.
