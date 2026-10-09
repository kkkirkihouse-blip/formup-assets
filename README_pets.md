# FormUp AI — Pets pack (everything for the pet)

## Folders
- cat/, dog/ — 6 ages × 5 states, original coat. Name: {cat|dog}_{N_age}_{state}.png
  - ages: 1_baby, 2_little, 3_teen, 4_youngathlete, 5_champion, 6_legend
  - states: happy, asking, hungry, weak, lastchance
- coats/{cat|dog}_{coat}/ — same 30 images per coat. Name: {cat|dog}_{coat}_{N_age}_{state}.png
  - Cat coats: original (grey tabby), ginger, calico, chocolate, silver, lilac
  - Dog coats: original (ginger), chocolate, merle, blacktan, dalmatian, cream
- wear/{cat|dog}/ — pet ALREADY WEARING each accessory (drawn, not overlaid). 6 ages × 8 items per animal = 96 images. Name: {cat|dog}_{N_age}_{item}.png, item = collar, cap, headband, medal, legendary, scarf, bow, sunglasses
- wear_cat_overview.png, wear_dog_overview.png — preview of all worn images
- accessories/ — store icons acc_*.png for the Accessories grid (icons only)
- rooms/ — room_home, room_gym, room_park (backgrounds, 1024×1536)
- *_overview.png — previews

## Pet age thresholds (treats fed in total)
Baby 0 · Little 10 · Teen 25 · Young athlete 50 · Champion 100 · Legend 300

## States
happy (normal) · asking (wants food) · hungry · weak · lastchance.
Dead = show the lastchance image with a memorial overlay (wings, halo, cloud, flowers) — no new art needed.

## Accessories
Level rewards (unlocked automatically when the pet reaches the age):
- Little → Collar
- Teen → Cap
- Young athlete → Headband
- Champion → Medal (new)
- Legend → Legendary outfit = Crown + Royal mantle
Outfits (unlocked by streaks, wearable any time after):
- 7-day streak → Scarf
- 14-day streak → Bow
- 30-day streak → Sunglasses (new)

One accessory at a time: the user picks ONE equipped item; the happy image is replaced by wear/{animal}/{animal}_{age}_{item}.png. Nothing equipped → normal happy image.
Accessories are visible ONLY in the happy state (hidden in asking/hungry/weak/lastchance).
No overlay/positioning code is needed. Store icons in the Accessories grid = the acc_*.png files.
Worn images exist for the original coat only; with another coat equipped, show the coat's happy image without accessory (or regenerate worn images per coat later).

## Display in the pet card
Images are square, transparent, figure bottom-aligned. In the pet card (about 3:2) show the image with aspect-fit, height ≈ 85% of the card, bottom-aligned with ~4% bottom margin, horizontally centred; leave headroom for hats. Profile avatar: crop the top ~55% of the image, centred.
