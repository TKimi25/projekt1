---
name: Tóth Joakim
neptun: NV8CXW
id: 2026-SD-02
github: https://github.com/TKimi25/projekt1
github_project: https://github.com/users/TKimi25/projects/2
---
# Társasjáték-szabálymagyarázó alkalmazás forráshivatkozásokkal

Társasjáték közben egy konkrét helyzet megítéléséhez több szabályrész együttes értelmezésére lehet szükség. A projekt célja egy olyan, mobilon is használható webalkalmazás, amely a kiválasztott játék szabálykönyvéből keres vissza, és helyzetfüggő kérdésekre válaszolva az állításait pontos forráshelyekkel támasztja alá az LLM segítségével. A projekt végére a felhasználó képes lesz szabálykönyveket feltölteni, kérdéseket feltenni, szükség esetén pontosítani a helyzetet, majd megtekinteni a választ és az eredeti szövegkörnyezetet a forrásrészletekben.

## Célok

- **Elsődleges cél:** Reszponzív webalkalmazás és LLM-alapú (RAG) dokumentumfeldolgozó és lekérdezési folyamat elkészítése társasjátékok szabályainak magyarázatához.
- **Célfelhasználók / érintettek:** Társasjátékosok, akik játék közben megbízható és pontos forrásokon alapuló válaszokat keresnek a szabálykérdésekre.
- **Mérhető sikerkritériumok:** A felhasználó feltölthet legalább szöveges PDF vagy Markdown alapú szabálykönyvet, feltehet egy kérdést, és a rendszer releváns, forrásrészletekkel alátámasztott választ ad; a dokumentumok, kérdések és saját megjegyzések tartósan tárolva maradnak.
- **Korlátok:** Az alkalmazás, az adattárolás és az MI-integráció logikája különüljön el; a dokumentum tartalma nem írhatja felül az alkalmazás utasításait; a szolgáltatáskulcsok és titkos adatok nem kerülhetnek a Git repóba.

## Hatókör

### Benne van a hatókörben

- Szabálykönyvek, oldalszámok, szakaszazonosítók, kiadások, kiegészítők és házi szabályok kezelése, elkülönítése.
- Visszakeresés kulcsszavas és szemantikus jelöltek egyesítésével, valamint indokolt szabállyal történő újrarangsorolással.
- Helyzetfüggő kérdések megválaszolása és visszakérdezés hiányzó helyzetadat esetén.
- Eredeti szövegkörnyezet megjelenítése a hivatkozás megnyitásakor.
- Kérdések, megjegyzések mentése, és a hibás MI-válaszok felhasználói jelölése (a használt dokumentumverzió rögzítésével).

### Nincs benne a hatókörben

- Teljes játékmotor megvalósítása.
- Gépi ellenfél készítése.
- Automatikus játéklevezetés.

## Jegyzetek

A fejlesztés mellett kötelező kutatási és mérési feladat a kulcsszavas és szemantikus visszakeresés (valamint a darabolási stratégiák) összehasonlítása egy kézzel ellenőrzött kérdés–válasz–forrás készleten. Lehetséges, de nem kötelező bővítési irányok a többnyelvű kérdezés, a táblázatok értelmezése vagy egy közös játékalkalom kérdésgyűjteményének megvalósítása.