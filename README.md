# Hatchery

**Pet Evolution Lab** — Fusion and genetic breeding game to spawn new variants inside the 210-kind canon.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) universe. Map: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. Gameplay contract is frozen. Engine choice is the one in the brief. Implementation comes next.

## Loop

Kennel is the calculator. Hatchery is the toy: drag two pets, watch the whelp table animate, lock a legal variant, send to Minter. Panda × fish is a red X, not a new species.

## Genre & engine

- Genre: **Simulation**
- Engine: **React / Canvas**
- Stack: TypeScript · React 19 · Canvas 2D · Kennel genetics API · Atelier preview
- Default surface: `8080`

## How you play

1. Drop two owned pets onto the bench.
2. See allele dice in real time.
3. Illegal pair explains why.
4. Commit whelp → mint request, not an overlay clone.

## Talks to

- computerpets-kennel
- computerpets-lore
- computerpets-atelier
- computerpets-minter
- computerpets-studio

## Failure doctrine

Illegal pair never writes a token. Canvas fail → table still shows odds. Partial mint → Hatchery keeps the draft.

Canon rules that never yield:

- 210 living kinds. No illegal hybrids.
- Overlay pets can get tired, sick, or hide. Tokens are not burned by a minigame.
- Desktop walk stays the main quest. Closing Hatchery must leave Rui walking.

## Layout

```
computerpets-hatchery/
  README.md
  LICENSE
  docs/DESIGN.md
  src/                implementation lands here
```

## Run (Windows)

```powershell
cd app; npm install; npm run dev
```

Meet Rui first via the [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md). This game is optional.

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*
