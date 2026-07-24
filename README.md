# Vault v1.6.6

Vault is a local-first desktop app for organizing protected operational connection data.

## Download

- Vault_1.6.6_x64-setup.exe

## Automatic updates

This release is available through signed automatic updates.

Updater metadata:

- latest.json
- release-summary.json
- Vault_1.6.6_x64-setup.exe.sig

## What is new in v1.6.6

- GitHub release builds receive the Google Drive OAuth secrets needed for connection.
- Release validation blocks builds without Google Client ID or Client Secret configured.
- Google Drive shows a clearer message when OAuth configuration is missing in a build.
- Local and published build behavior are aligned.
- Backup registry and restore behavior from previous releases remain unchanged.

## Changes included from v1.5.9 to v1.6.6

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

### v1.6.6

- GitHub release builds receive the Google Drive OAuth secrets needed for connection.
- Release validation blocks builds without Google Client ID or Client Secret configured.
- Google Drive shows a clearer message when OAuth configuration is missing in a build.
- Local and published build behavior are aligned.
- Backup registry and restore behavior from previous releases remain unchanged.

## Manual installation

1. Download `Vault_1.6.6_x64-setup.exe`.
2. Run the installer.
3. Existing user data is preserved.

## Notes

Older releases remain available from GitHub Releases.
