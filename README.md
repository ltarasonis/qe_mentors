# QE Mentor Lookup

A static page where QE students enter their student number and see their mentor.

- `index.html` – the page
- `data.js` – student number → mentor and year (generated; no names or e-mails)
- `scripts/build_data.py` – regenerates `data.js` from the tutors spreadsheet

## Updating the list

```bash
pip install openpyxl
python scripts/build_data.py path/to/QE_Tutors.xlsx
```

Each sheet needs a header row with `Student No.` and `Tutor` columns.
Don't commit the spreadsheet itself.

## Publishing

Enable GitHub Pages (Settings → Pages → Deploy from a branch → `main`, `/ (root)`).
