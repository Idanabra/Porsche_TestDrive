# טופס נסיעת מבחן – בדיקת רכב

Test-drive form (Hebrew, RTL) for Porsche Israel, styled with SAP Horizon for embedding as a mashup in SAP Sales & Service Cloud V2.

## Steps
1. פרטי לקוח – ID scan (camera / upload) + customer details
2. פרטי נסיעה – car model, license plate, km, delivery/return dates
3. חתימה ואישור – summary document, customer signature, PDF export

## Run
Static site — serve the folder with any web server (opening via `file://` may block script loading):

```
npx serve .
# or
python3 -m http.server 8080
```

Then open `http://localhost:8080/index.html`.

## Notes
- ID OCR is simulated (fills sample data). Connect a real OCR service in `startScan()` inside `index.html`.
- Car models / plates are sample data in the `CARS` constant.
- Fonts: SAP "72" (bundled) + Assistant from Google Fonts for Hebrew glyphs.
