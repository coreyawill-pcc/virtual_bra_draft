# The Virtual Sports Bra

An interactive 3D museum of The Sports Bra (Portland, OR): a photogrammetry scan of the bar with scanned memorabilia placed inside. Drag to look around; tap a pink marker to open an exhibit.

Built for GEO 254 Drone Modeling II by Corey Williams.

## How it was made
- Room: Insta360 360° capture → Agisoft Metashape (spherical cameras) → textured mesh
- Artifacts: individual photogrammetry scans
- Assembly: Blender → GLB
- Viewer: three.js (loaded from jsDelivr)

## Files
- `index.html`: the viewer, with exhibit labels in the `exhibit-data` block
- `models/interior.glb`: the room
- `models/artifacts.glb`: the placed artifacts (object names match each exhibit's `node`)
- `thumbs/`: placard photos

To update the scan, export new GLBs from Blender with the same object names and replace the files in `models/`.

Exhibit labels are drafts; confirm details with Sports Bra staff before sharing widely.
