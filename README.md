# NORTH-4 AGEING REPORT (GR103 / GR105)

Simple PHP Ageing Report System for SAP GR103 and GR105 transactions.

## ✅ FEATURES
- Upload Excel file
- Reads GR103 and GR105 sheets
- Matches using PO KEY
- Computes ageing (days)
- Shows Outstanding / Closed status

## ✅ REQUIREMENTS
- PHP 7.4+
- XAMPP / WAMP / Local server
- PhpSpreadsheet library

## ✅ INSTALLATION
1. Download PhpSpreadsheet:
   https://github.com/PHPOffice/PhpSpreadsheet

2. Extract the folder beside `ageing_report.php`

3. Do NOT upload PhpSpreadsheet to GitHub

## ✅ HOW TO RUN
1. Start Apache (XAMPP)
2. Place project inside `htdocs`
3. Open browser:
   http://localhost/ageing_report.php

## ✅ MATCHING LOGIC
| Transaction | Purpose |
|-----------|--------|
| GR103 | Start date |
| GR105 | Clearing |
| PO KEY | Matching |
| No GR105 | Outstanding |
| With GR105 | Closed |
