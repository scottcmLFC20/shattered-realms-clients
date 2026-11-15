# Shattered Realms client add-ons

Health and mana bars, your enemy's health, and (Mudlet only) an automatic map
for **Shattered Realms** (178.128.230.115, port 4000).

These use the game's GMCP feature, which Mudlet and MUSHclient both support.

## Mudlet

**Quick install:** connect to the game, then paste this into Mudlet's input line and press Enter:

```
lua installPackage("https://raw.githubusercontent.com/scottcmLFC20/shattered-realms-clients/main/mudlet/ShatteredRealms.xml")
```

**Or by hand:** download [`mudlet/ShatteredRealms.xml`](mudlet/ShatteredRealms.xml)
(click the file, then the download button), then Toolbox -> Package Manager -> Install,
and pick the file.

Install it once in **each Mudlet profile** you play. Each character's profile needs its own copy.

What you get:
- HP (red) and Mana (blue) bars along the bottom of the window.
- An Enemy bar that appears while you are fighting.
- An automatic map that fills in as you walk. Click Mudlet's **Map** button to open it.

## MUSHclient

1. Download [`mushclient/ShatteredRealms_GMCP.xml`](mushclient/ShatteredRealms_GMCP.xml)
   (click the file, then the download button).
2. In MUSHclient: File -> Plugins -> Add, and pick the file.
3. Disconnect and reconnect. MUSHclient only switches the bars on when it connects.

What you get: a small window with HP, Mana and Enemy bars. Drag its title strip to move it.

## Bars missing or stuck?

- Type `request char` in the game to resend your health and mana (`request all` also resends the map).
- Mudlet: Settings -> General -> make sure **Enable GMCP** is ticked, then reconnect.
- In game, `help gmcp` has the same instructions.
