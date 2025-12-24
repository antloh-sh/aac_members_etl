# 📂 AAC Membership & Family ETL Tool

A web-based tool hosted on GitHub Pages for processing membership and family listings.

## 🚀 Live Link
[**Open the Web App**](https://antloh-sh.github.io/aac_members_etl/)

---

## 🛠 Supported Conversions

### 1. Member Details
- **Source:** `DataListing-AACMemberDetails.csv`
- **Output:** `ETL-AACMemberDetails.csv`
- **Actions:** Maps 8 core columns, converts dates to `YYYY-MM-DD`, and changes "Yes/No" to "true/false".

### 2. Family Members Listing
- **Source:** `FamilyMembersListing.csv`
- **Output:** `ETL-FamilyMembersListing.csv`
- **Actions:** Maps patient NRIC, names, relationships, and phones. Automatically generates an `id` sequence.

---

## 📖 Instructions
1. Select the **File Type** from the dropdown menu.
2. Upload the corresponding **Source CSV** from your local drive.
3. Click **Run ETL Process**.
4. Click **Download Result** to save the formatted file back to your computer.

---

## 🔒 Security
All processing is done **client-side** in your browser. No data is ever uploaded to a server or stored on GitHub.
