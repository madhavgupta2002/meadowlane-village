# v1 vs v2 feature comparison

Both share: instanced chunk streaming (96 m chunks, seeded), cottages/farms/park with fountain, trees, fences, lamps, benches, cars,
gradient sky shader + sun disc + clouds + birds, ACES tone mapping, PCF soft shadows, touch joystick.

## Only in v2 (kept)
- Third-person animated character with collision-aware orbit camera; first-person toggle (V)
- Flight mode (F, Space/E up, Q/Ctrl down), unlimited speeds, wheel / +/- speed change
- Settings panel (speeds, boost multiplier, camera distance, look sensitivity, reset, return home)
- Full-screen detailed map: pan/zoom, district labels, waypoints with distance HUD, scale bar, plan-based (works beyond loaded chunks)
- Deterministic per-chunk plans shared by 3D and map; swept-box collision; altitude-aware fog and shadows
- Larger draw distance (camera far 3500, sky 2500), toasts, pause/resume menu system, blur/visibility pause

## Only in v1 (ported)
- "Welcome to Meadowlane" canvas-textured village sign near the start
- Telephone pole insulators on the cross arm
- Weather/time pill in the HUD ("Late afternoon, 23 deg")
- FOV widening while running and subtle camera roll sway in first person
- Softer shadow radius setting
- Fog-free warmer horizon falloff is equivalent; mailbox placement at the kerb, bush/flowers equivalent (not ported)

## v1 weaker / not ported
- Minimap only draws loaded chunks (v2 uses plans); no flight, no settings, no third person
- Substepped circle collision (v2 swept OBB collision is stronger)
