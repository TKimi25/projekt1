---
name: [Hallgató neve]
neptun: [NEPTUN kód]
id: 2026-SD-02
github: [GitHub repozitórium URL]
github_project: [GitHub projekt URL]
---
# Társasjáték-szabálymagyarázó alkalmazás forráshivatkozásokkal

Társasjáték közben egy konkrét helyzet megítéléséhez több szabályrész együttes értelmezésére lehet szükség[cite: 1]. A projekt célja egy olyan, mobilon is használható webalkalmazás, amely a kiválasztott játék szabálykönyvéből keres vissza, és helyzetfüggő kérdésekre válaszolva az állításait pontos forráshelyekkel támasztja alá az LLM segítségével[cite: 1]. A projekt végére a felhasználó képes lesz szabálykönyveket feltölteni, kérdéseket feltenni, szükség esetén pontosítani a helyzetet, majd megtekinteni a választ és az eredeti szövegkörnyezetet a forrásrészletekben[cite: 1].

## Célok

- **Elsődleges cél:** Reszponzív webalkalmazás és LLM-alapú (RAG) dokumentumfeldolgozó és lekérdezési folyamat elkészítése társasjátékok szabályainak magyarázatához[cite: 1].
- **Célfelhasználók / érintettek:** Társasjátékosok, akik játék közben megbízható és pontos forrásokon alapuló válaszokat keresnek a szabálykérdésekre.
- **Mérhető sikerkritériumok:** A felhasználó feltölthet legalább szöveges PDF vagy Markdown alapú szabálykönyvet, feltehet egy kérdést, és a rendszer releváns, forrásrészletekkel alátámasztott választ ad; a dokumentumok, kérdések és saját megjegyzések tartósan tárolva maradnak[cite: 1].
- **Korlátok:** Az alkalmazás, az adattárolás és az MI-integráció logikája különüljön el; a dokumentum tartalma nem írhatja felül az alkalmazás utasításait; a szolgáltatáskulcsok és titkos adatok nem kerülhetnek a Git repóba[cite: 1].

## Hatókör

### Benne van a hatókörben

- Szabálykönyvek, oldalszámok, szakaszazonosítók, kiadások, kiegészítők és házi szabályok kezelése, elkülönítése[cite: 1].
- Visszakeresés kulcsszavas és szemantikus jelöltek egyesítésével, valamint indokolt szabállyal történő újrarangsorolással[cite: 1].
- Helyzetfüggő kérdések megválaszolása és visszakérdezés hiányzó helyzetadat esetén[cite: 1].
- Eredeti szövegkörnyezet megjelenítése a hivatkozás megnyitásakor[cite: 1].
- Kérdések, megjegyzések mentése, és a hibás MI-válaszok felhasználói jelölése (a használt dokumentumverzió rögzítésével)[cite: 1].

### Nincs benne a hatókörben

- Teljes játékmotor megvalósítása[cite: 1].
- Gépi ellenfél készítése[cite: 1].
- Automatikus játéklevezetés[cite: 1].

## Jegyzetek

A fejlesztés mellett kötelező kutatási és mérési feladat a kulcsszavas és szemantikus visszakeresés (valamint a darabolási stratégiák) összehasonlítása egy kézzel ellenőrzött kérdés–válasz–forrás készleten[cite: 1]. Lehetséges, de nem kötelező bővítési irányok a többnyelvű kérdezés, a táblázatok értelmezése vagy egy közös játékalkalom kérdésgyűjteményének megvalósítása[cite: 1].