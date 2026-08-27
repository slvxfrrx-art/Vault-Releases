# Vault v1.8.0

Vault is a local-first desktop app for organizing protected operational connection data.

## Download

- Vault_1.8.0_x64-setup.exe

## Automatic updates

This release is available through signed automatic updates.

Updater metadata:

- latest.json
- release-summary.json
- Vault_1.8.0_x64-setup.exe.sig

## What is new in v1.8.0

- Personal remains the legacy Vault app with the existing updater channel and classic Windows installer names.
- Vault Business has a separate application identity, storage profile, and updater endpoint.
- Business Owner activation uses the licensing contract v2 foundation with root/child owner metadata.
- Business Member provisioning includes stable device identity, signed device proof, signed accept/reject, and secure token exchange.
- Personal and Business release routing are separated through p-vX.Y.Z, b-vX.Y.Z, and pb-vX.Y.Z source tags.
- Business Sync, Vault Platform Backup, hierarchy editing, permissions, Change Requests, and key rotation UI are not included in this release.

## Changes included from v1.5.9 to v1.8.0

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

### v1.8.0

- Personal legacy compatibility preserved.
- Licensing contract v2 and edition separation foundation.
- Vault Business app identity and release channel foundation.
- Business Owner root/child activation metadata.
- Business Member stable Device ID, Ed25519 device proof, signed accept/reject, and secure token exchange.
- Personal and Business updater channel separation.

## Manual installation

1. Download `Vault_1.8.0_x64-setup.exe`.
2. Run the installer.
3. Existing user data is preserved.

## Notes

Older releases remain available from GitHub Releases.
