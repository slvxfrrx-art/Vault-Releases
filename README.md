# Vault v1.5.13

Vault is a local-first desktop app for organizing protected operational connection data.

## Download

- Vault_1.5.13_x64-setup.exe

## Automatic updates

This release is available through signed automatic updates.

Updater metadata:

- latest.json
- Vault_1.5.13_x64-setup.exe.sig

## What is new in v1.5.13

- SAP GUI Landscape import from SAPUILandscape.xml.
- SAP connections are grouped under the related Client.
- Import preview before writing data.
- Imported data is placed under Importati -> SAP GUI.
- No SAP passwords, users or VPNs are imported.

## Changes included from v1.5.9 to v1.5.13

### v1.5.9

- Tutorial UX cleanup and Tutorial Center improvements.
- Guided creation of folder, subfolder and Client.
- Client terminology replaced child/figlio in user-facing text.
- Licensing architecture documented for future implementation.
- Team excluded from tutorial scope.

### v1.5.10

- Team / Collaboration UI removed from the product experience.
- Vault refocused on local-first workflow.
- Existing local Vault data is preserved.
- Team-related database structures remain in place for safety.
- Team planned for future redesign.

### v1.5.11

- Client export to .vault.
- Copy VPN, connections and users in readable title-value format.
- Passwords excluded by default from export/copy.
- Tree state restored after auto-lock.
- Layout fixes for maximized and narrow windows.
- Side tree pinned, collapsed and auto-hide modes.
- Settings updater flicker fix.

### v1.5.12

- .vault import from Dashboard.
- Import preview with tree structure.
- Imported data placed under Importati.
- Drag and drop tree node movement.
- Dashboard dropdown readability fix.
- Foundation for future SAP tree import.

### v1.5.13

- Import source selector.
- SAP GUI Landscape import from SAPUILandscape.xml.
- SAP tree preview before import.
- SAP data imported under Importati -> SAP GUI.
- SAP folders converted into Clients.
- SAP services under the same SAP node imported as Connections of the same Client.
- SAP import does not create VPNs, users, credentials or passwords.

## Manual installation

1. Download `Vault_1.5.13_x64-setup.exe`.
2. Run the installer.
3. Existing user data is preserved.

## Notes

Older releases remain available from GitHub Releases.
