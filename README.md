# 📂 Membership ETL Tool

A lightweight, browser-based utility to transform membership data exports into a standardized ETL format. This tool runs entirely in your browser via GitHub Pages, ensuring your data never leaves your local machine.

## 🚀 Live Link
[**Click here to open the Web App**](https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/)
*(Note: Replace the link above with your actual GitHub Pages URL)*

---

## 🛠 Functionality
This tool automates the cleaning and reformatting of membership CSV files.

### 1. Data Mapping
It maps the original source columns to the required system headers:
| Source Column (DataListing) | Target Header (ETL) |
| :--- | :--- |
| `RegistrationDocumentNumber` | `registrationdocumentnumber` |
| `FullNameNative` | `fullnamenative` |
| `ToAddressAs` | `toaddressas` |
| `DateOfBirth` | `dateofbirth` |
| `Gender` | `gender` |
| `Phone` | `phone` |
| `ResidesWithinServiceBoundaryStr` | `resideswithinserviceboundarystr` |
| `FullAddress` | `fulladdress` |

### 2. Automated Transformations
* **Date Formatting:** Converts dates (e.g., `01-Oct-1942`) to ISO format (`1942-10-01`).
* **Boolean Mapping:** Converts `Yes/No` values to `true/false` for system compatibility.
* **Case Normalization:** Ensures all headers are converted to lowercase.

---

## 📖 How to Use
1.  **Export** your membership data as a CSV (default: `DataListing-AACMemberDetails.csv`).
2.  **Open** this Web App link.
3.  **Upload** the CSV file using the file picker.
4.  **Click "Process File"**.
5.  **Download** the resulting `ETL-AACMemberDetails.csv` and save it to your local drive.

---

## 🔒 Privacy & Security
* **Zero Server Uploads:** This app uses `PapaParse.js` to process data locally in your browser's memory.
* **Privacy:** No membership data is sent to GitHub or any external server. 

---

## 🏗 Setup for Developers
If you want to host this yourself:
1. Clone this repository.
2. Ensure `index.html` is in the root directory.
3. Enable **GitHub Pages** in the repository settings under the `main` branch.
