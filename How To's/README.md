# How To’s (TrueWorX)

## Install

1) Download and run the installer **as Administrator**:
   - `installer\TrueWorXSetup_Latest.exe`
2) Restart SolidWorks.
3) In SolidWorks: `Tools → Add-Ins` → enable **TrueWorX**.

To uninstall/unregister: run `C:\TrueWorX\Release\unregister.bat` as Administrator (then uninstall from Apps & Features if needed).

## Configure templates

1) Download templates from `templates\` (example: `templates\CutlistTemplate.xlsx`).
2) In SolidWorks: `TrueWorX → Settings` and point the template paths at the files you want to use.

## Licensing / trial

- TrueWorX includes a **30‑day trial** that starts automatically on first run.
- Optional: in SolidWorks open `TrueWorX → License…` and register your email for licensing help/updates.
- To purchase a license, start at: https://www.freezeants.com/

Offline environments:
- If the machine cannot reach the internet, contact support for an **offline activation token** (you’ll need the machine id shown in the license dialog).

## Troubleshooting

**TrueWorX doesn’t show in Add‑Ins**
- Close SolidWorks and re-run the installer as Administrator.
- Restart SolidWorks, then check `Tools → Add‑Ins` again.

**Licensing/trial looks wrong**
- In SolidWorks: `TrueWorX → Settings`
- Confirm **License API base URL** is set to:
  - `https://licensing.freezeants.com`
- Then open `TrueWorX → License…` and try again.

**Need help**
- Start at https://www.freezeants.com/
- Or email: support@freezeants.com
