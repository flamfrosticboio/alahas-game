# Elemental Fighters

This is a game about elemental fighters.

## Notation

It uses similar style for tekken

n - neutral
1 - left hand
2 - right hand
3 - left leg
4 - right leg
r - runic activation
x - grab1 (can be activated with 14)
y - grab2 (can be activated with 23)
z - grab12 (can be activated with 124)
u - up
d - down
b - back
f - forward

Information to notations:
H - Hits High
M - Hits Mid
L - Hits Low
LN - Linear
PC - power crush
HC - high crush
LC - low crush
MC - mid crush
T - throw
ST - stance
HOLD - hold
PR - Creates Projectile
R - Runic hit

> [!Example]
>
> - `b2ML` - back right-hand that hits mid and its linear
> - `2PML` - right hand with projectile, hits mid, and its linear

### Modding

It is possible to map these notations into different commands on mod support
(later 1.1 release)

## Roadmap

[0.1a]

- Basic Game Engine (walk, attack, idle, hit damage)
- Basic Character - Fighter
  - hp: 150
  - 1 H - left jab
  - 2 M - hook
  - 3 L - kick
  - r H R - special jab (activates rune)
- Runic Mechanic
  - 3 rune uses per match (not rounds)
- New Rune - Fire
  - 5% damage increase
  - on runic hit - 2 DOT for 3 seconds

[0.2a]

- New Character - Swordsman
  - hp: 125
  - 1 H - slash
  - 2 M - heavy slash
  - 3 L - kick
  - r H R - runic slash (non-projectile)
- New states
  - crouch (d HOLD) - blocks all high attacks, holdable
  - lean-forward (u) - blocks all high and mid linear attacks but slower
  - lean-backaward (d) - blocks all high attacks
  - block (b HOLD)
- New Rune - Ice
  - 10% block damage reduction increase
  - on runic hit - 20% movement speed decrease

[0.3a]

- New states (stance, throws)
- New mechanic: Limited Uses
- Projectile support
- New character (Archer) (max 10 arrows)
  - hp: 125
  - 1 H - weapon swing
  - 2 M - heavy weapon swing
  - b2 S-HOLD - draw bow
    - n H - shoot quick arrow (removes one arrow)
    - d MS - shoot mid arrow (removes one arrow)
    - db H - shoot special arrow
  - 3 L - low kick
  - r H R - runic swing
- New Rune - Plant
  - 5% additional health
  - on runic hit - 1 DOT for 5 seconds
- Add new stance for:
  - Fighter - Charge stance (d12 ST)
    - f2 mL - bash (goes back to normal stance)
    - 3m PC - power kick (goes back to normal stance)
    - x MT - knockdown (goes back to normal stance)
  - Swordsman - Draw stance (d12 ST)
    - 2 H - unsheathe slash (goes back to normal stance)
    - f2 M - unsheathe dash (goes back to normal stance)
    - b2 MS - runic slash (projectile) (goes back to normal stance)

[0.4a]

- New character (Mage)
  - hp: 100
  - 1 H - weapon swing
  - 2 MS PR - manaball
  - 3 L - low kick
  - r MS PR R - runic ball
  - df12 ST - forward staff stance
    - 1 M - poke
    - 3 L - low poke
    - 2 PR MS - manaball
    - r PR MS R - runic ball
    - b2 M - heavy weapon swing (goes back to normal stance)
    - b - normal stance
    - Note: Cannot Block / Escape
  - db12 S - backward staff stance
    - 1 M - poke
    - 3 L - low poke
    - 2 PC M - heavy poke
    - 34 PC L - heavy low poke
    - b - normal stance
    - Note: Cannot Block / Escape
- New Rune - Dark
  - 10% movement speed
  - on runic hit - 10% movement decrease
- local 2-player mode
- Game Match Settings
  - adjustable max rune activations
  - adjustable rounds

[1.0]

- Game menu
  - Settings
  - VS. CPU
  - Training
- Bot support

[1.1]:

- Multiplayer mode
- Modularity and Mods support
  - Uses "patches"
  - Custom loading of images and sounds using "patches"
  - Custom maps (not stored in "patches" but in a separate file)
