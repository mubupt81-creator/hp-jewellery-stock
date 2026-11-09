# Hyatt Palace Jewellery Stock Manager

A mobile-first stock counting and reconciliation web app for iPhone and desktop browsers.

## Features
- Import WinGold stock exports in Excel or CSV format.
- Create a unique barcode for every physical piece when an imported row has no barcode (existing row barcode is retained for the first piece).
- Count stock by camera scan or manual barcode entry.
- Track expected and counted quantity and weight.
- Filter and search stock by category and item type.
- Export reconciliation reports to Excel or CSV and print reports.
- Download a complete JSON backup and restore it on another device.
- Install as a PWA; the app shell is cached for offline reopening after the first successful online visit.

## Important data notes
- Stock data is stored locally in the browser on each device. There is no cloud sync.
- Use Backup / Restore to transfer data between devices and keep regular backups.
- During Excel import, choose whether the source Weight column is total row weight or weight per piece. The app divides total row weight by quantity when that option is selected.
- Camera scanning and Excel import use external libraries loaded from CDNs; those features may require an internet connection if the libraries are not already cached by the browser.
- Barcode values already present in the source file are preserved for the first piece of each row; additional pieces receive generated unique IDs. Review duplicate source barcodes before a live stocktake.

## Publish
GitHub Pages can serve this repository. In repository Settings, open Pages, select the main branch and root folder, then open the published Pages URL over HTTPS.
