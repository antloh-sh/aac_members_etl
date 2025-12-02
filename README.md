# AAC Members ETL (CSV Cleaner)

A small browser-based tool to clean and transform AAC member CSV exports.  
The app runs entirely in the browser and can be hosted on GitHub Pages.

## Features

- Load a CSV export directly from your computer (no upload to any server).
- Extract only the required columns:
  - `CurrentMembershipStatus`
  - `JoinedDate`
  - `RegistrationDocumentNumber`
  - `FullNameNative`
  - `ToAddressAs`
  - `DateOfBirth`
  - `Gender`
  - `Race`
  - `Phone`
  - `ResidesWithinServiceBoundaryStr`
  - `NricAddress_PostalCode`
  - `FullAddress`
  - `SpokenLanguage`
- Convert `JoinedDate` and `DateOfBirth` from `DD-MMM-YYYY` (for example `11-Sep-2025`) to `YYYY-MM-DD`.
- Export a cleaned CSV with lower‑case headers:
  - `currentmembershipstatus`
  - `joineddate`
  - `registrationdocumentnumber`
  - `fullnamenative`
  - `toaddressas`
  - `dateofbirth`
  - `gender`
  - `race`
  - `phone`
  - `resideswithinserviceboundarystr`
  - `nricaddress_postalcode`
  - `fulladdress`
  - `spokenlanguage`

## Tech stack

- **HTML + JavaScript** only (no backend).
- **PapaParse** for reliable CSV parsing in the browser.
- **Tailwind CSS (CDN)** for a simple, modern UI.

## How to use

1. Open the app in your browser (via GitHub Pages once enabled).
2. Click the upload area and select the original CSV export.
3. Click **“Process & Download CSV”**.
4. A new file named `aac_members_transformed.csv` will be downloaded to your computer.

## Local development

If you want to test locally before pushing:

1. Clone this repository.
2. Open `index.html` directly in your browser (no build step needed).
3. Use the app as described above.

## Deploying with GitHub Pages

1. Commit `index.html` and this `README.md` to the `main` branch.
2. In the repository **Settings → Pages**, choose:
   - **Source**: “Deploy from a branch”
   - **Branch**: `main` and folder `/root`.
3. Save. After a short while your app will be available at:

`https://<your-username>.github.io/aac_members_etl/`

