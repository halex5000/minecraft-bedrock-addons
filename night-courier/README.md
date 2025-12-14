# Night Courier Add-On (Bedrock)

A lightweight Bedrock pack that drops in a mysterious nighttime messenger: new mob, loot, and behavior without touching the rest of your world. Use it as-is or as a starting point for your own encounter.

## What you get
| Folder | Purpose |
| --- | --- |
| `behavior_pack/` | AI, spawn rules, loot tables, items, events |
| `resource_pack/` | Models, textures, localization, client entity |

## Install it (Windows Bedrock)
1. Drop the behavior pack into `%LOCALAPPDATA%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\behavior_packs`.
2. Drop the resource pack into `%LOCALAPPDATA%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs`.
3. During active development you can also target `development_behavior_packs` and `development_resource_packs` in the same directory tree.

## Use it in a world
- Create or edit a world, enable “Night Courier - Resource Pack” and then “Night Courier - Behavior Pack”.
- Entity `td:night_courier` spawns on the Overworld surface at light level 7 or below.
- Killing one drops a Courier Token (`td:courier_token`).
- Courier Tokens are edible (nutrition 0) and grant Speed I for roughly five seconds.

## Package and share
- Zip `behavior_pack` and `resource_pack` separately, then distribute the zips.
- Recipients unpack them into the same `com.mojang` folders listed above.
- UUIDs in the manifests are placeholders—if you regenerate them, update the behavior-pack dependency so the pair stays linked.

## Refresh the placeholders
- `resource_pack/textures/items/courier_token.png` — supply your own 16×16-ish item art.
- `resource_pack/textures/entity/night_courier.png` — swap in a proper skin.

## Identifier quick reference
- Namespace: `td`
- Entity: `td:night_courier`
- Item: `td:courier_token`

## Next three upgrades
1. Add a low-health “dash away” behavior (event + goal set swap).
2. Introduce unique ambient/hurt sounds and glowing-eye accents.
3. Replace the placeholder model with a custom Blockbench build and UV map.
