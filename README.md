# TrueWorX (SolidWorks Add-in)
## TrueWorX — automation that just works

This repo hosts **downloads (installer)**, **templates**, and **end-user docs** for the TrueWorX SolidWorks add-in.

Source code:
- https://github.com/FreezeAnts/TrueWorX.git

## What it does
- **Create Drawing** (parts): writes custom properties, creates/overwrites a `.SLDDRW` using templates, adds standard views and a flat pattern sheet.
- **Assembly Process** (assemblies): exports sheet metal flat patterns to DXF/DWG and models to STEP into a job folder, and can generate/overwrite missing `.SLDDRW` files next to models (no PDFs).
- **Export PDFs**: exports PDFs from existing `.SLDDRW` files into a `PDF\\` subfolder.
- **Print DWGs**: batch-converts `.SLDDRW` files in a chosen folder to `DWG\\*.DWG`.


## Download & Install
1) Download the newest installer from `installer/` (highest version number):
   - `installer\TrueWorXSetup_<version>.exe`
2) Run the installer **as Administrator**.
3) Restart SolidWorks.
4) In SolidWorks: `Tools → Add-Ins` → enable **TrueWorX**.

To unregister: run `C:\TrueWorX\Release\unregister.bat` as Administrator.

## Updates
- Install the new version by running the newer installer (same steps as install).
- Settings are stored in `%APPDATA%\\TrueWorX\\settings.json` and typically survive updates.

## Templates
- `templates/` contains downloadable templates used by the add-in (example: `templates\\CutlistTemplate.xlsx`).
- In SolidWorks, open the TrueWorX settings dialog and point the template paths at the files you want to use.

## Notes
- **Assembly Process** runs in the background so SolidWorks stays usable while processing.


