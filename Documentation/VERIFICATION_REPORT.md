# LFHS PDF Collection Verification Report (Post-Cleanup & Audit Sync)

- **Total Catalogued PDFs**: 372 (362 legacy forensic-verification records + 10 new multilingual textbooks)
- **Corrupted / Invalid PDFs**: 0
- **Third-Party Blog Watermarks Remaining**: 0 (291 affected non-textbooks stripped lossless + 15 SMask logos + 8 Class 9 raster PDFs cleaned)
- **Total Page Count**: 9,847 pages
- **Total Size**: 2.06 GiB (2,214,942,048 bytes)
- **Files >= 100 MB**: 0 (largest is 60.46 MB)
- **Special Exceptions Documented**:
  - `LFHS-119` (`Class9_ModelPaper_Set2_2026_Physics_Key.pdf`): Handwritten Second Term 2025 Physics answer key in **Malayalam medium** (tagged `medium: "Malayalam"`).
  - `LFHS-359` (`Class10_QuestionBank_Vijayabheri2026_English.pdf`): Malappuram District Panchayat Vijayabheri **2021-22 Step-Up English Bridge Course (Classes 8–9)** archived in Class 10 Question Banks (tagged `cls: "8-10"`, `year: "2022"`).

## Class Breakdown

| Class | Files | Pages | Size |
|---|---:|---:|---:|
| Class 8 | 90 | 2,182 | 681.54 MB |
| Class 9 | 133 | 2,673 | 595.32 MB |
| Class 10 | 150 | 5,022 | 939.46 MB |
| **Total** | **372** | **9,847** | **2.06 GiB** |


## Multilingual Textbook Additions (LFHS-363–LFHS-372)

Ten additional SCERT textbooks are catalogued and hosted in `lfhs-4`: seven Malayalam-medium and three Hindi-medium PDFs across Classes 8–10. Their metadata is present in the central JSON manifest. These ten additions have not yet been added to the legacy CSV/XLSX forensic fingerprint exports, so the existing SHA-256 verification statements apply to the original 362-record audit set only.

Academic Hub: https://lfhs-site.vercel.app/
