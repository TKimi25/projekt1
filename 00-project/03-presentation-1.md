# Társasjáték-szabálymagyarázó alkalmazás
## Projekt bemutató
* Szerző: Tóth Joakim
* Neptun: NV8CXW
* Témavezető: Sári Dávid
* Projektazonosító: 2026-SD-02
---
# A Probléma

* Társasjáték közben vitás helyzetek alakulhatnak ki.
* Egy konkrét helyzet megítéléséhez több szabályrész együttes értelmezésére lehet szükség.
* A szabálykönyvekben való keresés lassú és nehézkes.

---
# Célfelhasználók

* Társasjátékosok.
* Akik gyors, pontos és hivatkozásokkal alátámasztott válaszokat keresnek bonyolult játékhelyzetekben.

---
# Tervezett hatókör (Beletartozik)

* Mobilon is használható webalkalmazás.
* Szabálykönyvek feltöltése (szöveges PDF vagy Markdown).
* Oldalszámok, szakaszazonosítók, kiadások és kiegészítők kezelése.
* LLM (Nagy Nyelvi Modell) alapú válaszadás.
* Állítások alátámasztása pontos forráshelyekkel.

---
# Tervezett hatókör (Nem része)

* Teljes játékmotor.
* Gépi ellenfél.
* Automatikus játéklevezetés.

---
# Kezdeti felhasználói utak

1. Játék és szabályváltozat kiválasztása.
2. Helyzetfüggő kérdés feltevése.
3. Helyzet pontosítása, ha a rendszer visszakérdez.
4. Válasz és forrásrészletek megtekintése.
5. Eredeti szövegkörnyezet megnyitása a hivatkozáson keresztül.
6. Kérdések, megjegyzések mentése, hibás válaszok jelölése.

---
# Következő lépések (Fejlesztés)

* Önálló dokumentumfeldolgozó és lekérdezési folyamat kialakítása.
* Reszponzív webes felület és tartós adattárolás implementálása.
* Git-alapú repozitórium létrehozása futtatási útmutatóval.

---
# Következő lépések (Kutatás)

* Kulcsszavas vs. szemantikus visszakeresés összehasonlítása.
* Egyszerű darabolás vs. szakaszhierarchiát kezelő RAG-megoldás mérése.
* Találati arány, helyesség és késleltetés mérése ellenőrzött adatkészleten.