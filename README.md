# Vault v1.7.0

Vault is a local-first desktop app for organizing protected operational connection data.

## Download

- Vault_1.7.0_x64-setup.exe

## Automatic updates

This release is available through signed automatic updates.

Updater metadata:

- latest.json
- release-summary.json
- Vault_1.7.0_x64-setup.exe.sig

## What is new in v1.7.0

- Vault Desktop links to a Vault Platform account through the browser.
- License selection happens on Vault Platform, without manual license key entry in the desktop.
- Approved devices are associated securely and can be revoked from the site.
- Signed offline license tokens allow local validation for up to 7 days offline.
- Operational Vault functions require a valid license, while local data is never deleted by licensing.
- Vault uses a stable UUID v4 device ID instead of sensitive hardware fingerprinting.

## Changes included from v1.5.9 to v1.7.0

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

### v1.7.0

- Account-based licensing through Vault Platform.
- Browser-based desktop account linking.
- License selection through the Vault Platform Area Personale.
- Secure approved-device association and revocation.
- Signed offline token validation with a maximum offline period of 7 days.
- Local data is preserved when licensing is invalid.

## Manual installation

1. Download `Vault_1.7.0_x64-setup.exe`.
2. Run the installer.
3. Existing user data is preserved.

## Notes

Older releases remain available from GitHub Releases.
