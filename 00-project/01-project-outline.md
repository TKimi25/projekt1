---
name: Jane Doe
neptun: ABC123
id: 2026-LG-02
github: https://github.com/example/sokoban-web-game
github_project: https://github.com/users/username/projects/1
---
# Sokoban webjáték

A Sokoban egy rácsalapú logikai játék, amelyben a játékos ládákat tol célmezőkre. A projekt a Sokoban webalkalmazásként történő megvalósítása reszponzív 2D-megjelenítéssel, játszható pályákkal és tartósan tárolt teljesítési haladással. A játékkliens PixiJS-t használ, a SvelteKit backend route-okat biztosít, a Prisma pedig az adatbázis elérését kezeli. A projekt végére a játékos pályát választhat, a böngészőben megoldhatja azt, majd visszatérhet a teljesített pályák tartósan eltárolt listájához.

## Célok

- **Elsődleges cél:** Teljes, reszponzív, böngészőben futó Sokoban játék elkészítése.
- **Célfelhasználók / érintettek:** Logikai játékok játékosai és pályakészítők.
- **Mérhető sikerkritériumok:** A játékos kiválaszthat és teljesíthet egy pályát; a teljesített állapot újratöltés után is tárolva és megjelenítve marad.
- **Korlátok:** TypeScript; PixiJS játékkliens; SvelteKit backend; Prisma adatbázis-elérés; hitelesítő adatok nem kerülhetnek a repóba.

## Hatókör

### Benne van a hatókörben

- Sokoban pályák kiválasztása és játszása a böngészőben.
- Billentyűzetes játékosmozgás és ládatolás.
- Győzelmi feltétel felismerése és pályateljesítési visszajelzés.
- Tartós pályaadatok és teljesített pályák haladása.
- Reszponzív, PixiJS-szel megjelenített játéktábla.

### Nincs benne a hatókörben

- Többjátékos játékmenet.
- Pályaszerkesztő az első verzióban.
- Online ranglisták vagy közösségi funkciók.

## Jegyzetek

Az első prototípus kis, kézzel készített pályakészletet használ. Pályaszerkesztő és további játékmódok csak akkor merülhetnek fel, ha az alap játékkör és a perzisztencia már megbízható.
