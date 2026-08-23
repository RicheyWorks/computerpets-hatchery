# Hatchery design

Implement against this file, not folklore.

## Identity

- Product: **Hatchery**
- Repo: `computerpets-hatchery`
- Idea: Pet Evolution Lab
- Genre: Simulation
- Engine: React / Canvas
- Surface: `8080`

## Loop

Kennel is the calculator. Hatchery is the toy: drag two pets, watch the whelp table animate, lock a legal variant, send to Minter. Panda × fish is a red X, not a new species.

## Play beats

- Drop two owned pets onto the bench.
- See allele dice in real time.
- Illegal pair explains why.
- Commit whelp → mint request, not an overlay clone.

## Neighbors

- computerpets-kennel
- computerpets-lore
- computerpets-atelier
- computerpets-minter
- computerpets-studio

## Failure doctrine

Illegal pair never writes a token. Canvas fail → table still shows odds. Partial mint → Hatchery keeps the draft.

## Hard rules

1. Minigames cannot mint or burn NFTs by themselves (Minter is the write path).
2. Stats come from lived overlay care + Dojo caps, not cash shop.
3. Species kits stay inside Lore. Illegal hybrids never spawn.
4. Fail soft: the desktop overlay process is not this process.
