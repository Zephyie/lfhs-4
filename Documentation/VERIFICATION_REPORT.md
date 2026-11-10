# LFHS Classes 8–10 Academic Repository — Deep Forensic Verification & Audit Report (2025–2026)

## 1. Executive Summary
- **Total Unique Verified English-Medium PDFs**: **362 PDFs** (+ **5 Documentation & Manifest Files** = **367 Total Files** inside `LFHS_Classes_8-10_English_PDF_Collection.zip`)
- **Total Verified Page Count**: **9,100 Pages**
- **Total Uncompressed PDF Payload**: **1.75 GB (1,882,455,922 bytes)**
- **Syllabus Alignment**: **100% SCERT Kerala Revised Syllabus (2024–2026 / 2025–2026)**
- **Language Medium**: **100% English Medium** (Forensically audited across body pages; all Malayalam-medium files and 1-page Malayalam teacher Scheme-of-Work files removed)
- **Deduplication Status**: **Zero SHA-256 Duplicates & Zero Content Near-Duplicates** (All 5 redundant merged Master Compendium PDFs and 10 content near-duplicates removed so every verified resource appears once and only once)
- **GitHub 100 MB Per-File Compliance**: **100% Compliant** — 0 files exceed 100 MB (largest single PDF is `Class8_ActivityBook_Art_Education_2024.pdf` at **60.46 MB**)

---

## 2. Independent Forensic Audit Findings & Resolutions
1. **Redundant Master Compendium PDFs Removed (5 Files)**:
   - Inspection confirmed that the 5 merged Master Compendium PDFs were concatenated copies of the individual non-textbook PDFs already stored in `Class_{8,9,10}/`, and 4 of them exceeded GitHub's 100 MB per-file limit (ranging from 134 MB to 391 MB). All 5 merged compendium copies were removed so every resource is stored once and only once.
2. **16 Truncated SCERT Textbooks Re-Downloaded & Restored**:
   - Deep `pypdf` page-tree inspection detected 16 textbooks that had been truncated mid-stream (`Stream has ended unexpectedly` / missing `%%EOF`), which had also caused the total archive size to drop earlier. All 16 textbooks were re-downloaded from their official SCERT Kerala Google Drive file IDs and verified for complete page trees and `%%EOF` markers. All 22 textbooks over 28 MB are also backed up in 20 MB slices in `.tb_chunks/`.
3. **16 Malayalam-Medium & Non-English Teacher Scheme Files Removed**:
   - Multi-page Unicode character ratio scanning (`\u0D00-\u0D7F` vs ASCII) across pages 1–10 distinguished genuine English-medium booklets that merely had a 1–2 page Malayalam District Panchayat greeting (such as the DIET Kannur SMILE 2026 modules and Malappuram Vijayabheri 2026 English-medium question pools, which are 100% English from page 3/4 onward) from 16 genuinely Malayalam-medium files (14 1-page Malayalam Scheme-of-Work tables and 2 Malayalam Class 9 Chemistry/Physics papers), which were removed.
4. **10 Content Near-Duplicates Removed**:
   - Normalized alphanumeric text comparison caught 10 pairs of third-party notes/worksheets/keys that had been saved under two slightly different filenames or in both `Model_Examination_Papers` and `Previous_Year_Papers`. All 10 redundant copies were removed.
5. **Edition & Subject Taxonomy Normalized**:
   - Fixed the `2026–2026` edition string bug across all entries to canonical `SCERT Kerala Revised Syllabus (2025–2026)` and `SCERT Kerala Revised Syllabus (2024–2026)`.
   - Standardized all subject labels into 10 canonical SCERT subjects (`English`, `Mathematics`, `Basic Science`, `Physics`, `Chemistry`, `Biology`, `Social Science`, `Information & Communication Technology (ICT)`, `Art, Health & Work Education`, `Career Guidance`) with zero `All Subjects` or `General` placeholders.

---

## 3. Exact Mathematical Breakdown by Class & Category

| Class Level | Textbooks | Model Examination Papers | Chapter-Wise Notes | Previous Year Papers | Worksheets | Question Banks | **Class Total PDFs** | **Total Pages** | **Total Size** |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Class 8** | 13 | 31 | 17 | 13 | 6 | 6 | **86** | 1,920 | 541.87 MB |
| **Class 9** | 19 | 42 | 30 | 23 | 6 | 8 | **128** | 2,392 | 483.62 MB |
| **Class 10 (SSLC)** | 19 | 43 | 48 | 22 | 3 | 13 | **148** | 4,788 | 769.75 MB |
| **Total (Classes 8–10)** | **51** | **116** | **95** | **58** | **15** | **27** | **362** | **9,100** | **1.75 GB** |

---

## 4. Breakdown by Canonical Subject Across Classes 8–10

| Canonical SCERT Subject | Verified PDF Count | Total Pages | Total Size |
| :--- | :---: | :---: | :---: |
| **Art, Health & Work Education** | 24 | 906 | 258.76 MB |
| **Basic Science** | 21 | 398 | 140.06 MB |
| **Biology** | 38 | 884 | 174.97 MB |
| **Career Guidance** | 1 | 80 | 15.28 MB |
| **Chemistry** | 33 | 715 | 78.79 MB |
| **English** | 63 | 1,298 | 215.46 MB |
| **Information & Communication Technology (ICT)** | 10 | 615 | 135.10 MB |
| **Mathematics** | 52 | 1,286 | 205.80 MB |
| **Physics** | 39 | 705 | 125.88 MB |
| **Social Science** | 81 | 2,213 | 445.15 MB |
| **Total** | **362** | **9,100** | **1.75 GB** |
