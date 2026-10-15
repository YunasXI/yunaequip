# YunaEquip

Your equipment on screen for **CatsEyeXI** (Ashita v4 and VanaCore), in the same look as [YunaGearOpt](https://github.com/YunasXI/yunagearopt).

- **A wheel of gear** round an animated figure of your job. Every job has its own picture; melee jobs draw their weapon when you engage and put it away when you disengage, and the energy round the figure glows when you engage or cast.
- **HP and MP on the bezel**: the ring's left half is your HP (red), the right half your MP (blue), filling from the bottom up, with a soft light gliding along them. TP sits above the wheel and pulses gold once you can weapon skill.
- **What your gear is set for**, under the wheel: TP when engaged, WEAPON SKILL, PRECAST, CURE, ENHANCING, ENFEEBLING, NUKE, SONG BUFF / DEBUFF (Bard), PDT, MDT, RESTING or IDLE. It follows your LegacyAC / LuAshitacast profile and the spell you're casting, and never shows long raw set names like TP_Hybrid_DT.
- **Sharp icons** at any size, a white ring on HQ / +1 items, and a dark Shadow effect in a slot when its piece changes.
- **Two looks** for the wheel: Sumi-e (ink brush ring) and Neon (glowing ring). Or the classic grid card instead of the wheel.

## Install

1. Download `yunaequip-x.y.z.zip` from [Releases](https://github.com/YunasXI/yunaequip/releases).
2. Unzip it into `Ashita\addons\` (VanaCore: `Vanacore\addons\ashita\`), so you have `addons\yunaequip\yunaequip.lua`.
3. In game: `/addon load yunaequip`

## Commands

`/yequip` or `/ye`

| Command | What it does |
| --- | --- |
| `/ye` | Show or hide YunaEquip |
| `/ye config` | The settings panel (or right-click it) |
| `/ye style [orbit \| card]` | The wheel round your job, or the classic grid |
| `/ye theme [sumi \| neon]` | The look of the wheel |
| `/ye pulse` | The HP / MP ring animation on or off |
| `/ye statsize <0.6-2>` | HP / MP / TP text size |
| `/ye setname` | The gear set name under the wheel on or off |
| `/ye blm` | Black Mage picture: wizard or warlock |
| `/ye art <10-100>` | Artwork opacity: how see-through the figure in the middle is |
| `/ye middle [art \| icon]` | The middle of the wheel: your job's artwork or its job icon |
| `/ye ring` | The HP / MP ring on or off (off: the gear floats on its own) |
| `/ye still` | The middle's animation on or off (off: a still icon / artwork, lighter) |
| `/ye test` | Play the Shadow swap effect on every slot |
| `/ye lock` / `unlock` | Stop or allow dragging |
| `/ye mini` | Mini mode (16 px icons) |
| `/ye icons <16-48>` | Icon size in px |
| `/ye layout [4x4 \| 8x2 \| 2x8 \| 16x1 \| 1x16]` | Card style: how the slots are arranged |
| `/ye reset` | Everything back to default |
| `/ye help` | List the commands |

## Good to know

- The set name comes from your gear-swap profile: `config\legacyac\<Name>_<JOB>.xml`, or else `config\addons\luashitacast\<Name>_<id>\<JOB>.lua`. YunaEquip shows the biggest set you're fully wearing; when no set is fully on it shows the closest one with a `~` in front. With no profile for your job it says *no gear profile*.
- Samurai uses the Yuna samurai; every other job has its own picture.
- The Shojumaru font in `fonts\` is under the SIL Open Font License (`fonts\OFL-shojumaru.txt`).
