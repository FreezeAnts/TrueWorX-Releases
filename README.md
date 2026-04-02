# TrueWorX (SolidWorks Add-in)
## TrueWorX — automation that just works

This is a SolidWorks add-in

## What it does
- **Create Drawing** (parts): writes custom properties, creates/overwrites a `.SLDDRW` using templates, adds standard views and a flat pattern sheet.
- **Assembly Process** (assemblies): exports sheet metal flat patterns to DXF/DWG and models to STEP into a job folder, and can generate/overwrite missing `.SLDDRW` files next to models (no PDFs).
- **Export PDFs**: exports PDFs from existing `.SLDDRW` files into a `PDF\\` subfolder.
- **Print DWGs**: batch-converts `.SLDDRW` files in a chosen folder to `DWG\\*.DWG`.


## Build
- Visual Studio: open `TrueWorX.sln` and build `Release|x64`.
- CLI: `dotnet build src\TrueWorXAddin\TrueWorXAddin.csproj -c Release`

Notes:
- The build automatically copies the add-in DLL to `Release\TrueWorX.dll` (used by the installer).

## Install
### Inno Setup (recommended)
1) Run the installer **as Administrator**:
   - `installer\TrueWorXSetup_<version>.exe`
3) Restart SolidWorks.
4) In SolidWorks: `Tools → Add-Ins` and enable **TrueWorX**.

To unregister: run `C:\TrueWorX\Release\unregister.bat` as Administrator.

## UI behavior
- **Assembly Process** runs the export work on a background STA thread and minimizes its window while running, so SolidWorks stays usable (no screen-locking modal dialog).



