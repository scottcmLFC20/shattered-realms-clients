# shattered-realms-clients
# Client files for Shattered Realms

These add health and mana bars, your enemy's health, and (Mudlet only) an
automatic map. They use the game's GMCP feature. Neither file shows a moves
bar: the server intentionally never sends moves.

## Mudlet

Install: Toolbox -> Package Manager -> Install, and pick `mudlet/ShatteredRealms.xml`.
Install it once in each Mudlet profile you play (each character's profile needs its own copy).
Open the map window (Map button) to see the map.

Shows:
- HP (red) and Mana (blue) bars along the bottom of the window.
- An Enemy bar that appears while you are fighting and shows its health percent.
- An automatic map, built as you walk. Rooms are placed one step from the
  last room in the direction you moved. If you arrive some other way
  (recall, portal), the room is placed beside the previous one and marked `?`.
  Rooms are grouped into areas by zone. Nothing is drawn while you are blind
  or asleep.

If the bars are missing or look stale, type `request char` (or `request all` for bars and map).

## MUSHclient

Install: File -> Plugins -> Add, and pick `mushclient/ShatteredRealms_GMCP.xml`.

Shows a small window with HP, Mana and Enemy bars and numbers. Drag it by
its title strip to move it. There is no map in this version.

## Published copy

Players download these from the public repo
https://github.com/scottcmLFC20/shattered-realms-clients (local clone ~/shattered-realms-clients).
After changing a file here, copy it there and push, or players keep the old version.
