# Validation results — 2026-09-16

- Asset and syntax check: passed; 64 unique products, 10 categories, 64 WebP files, 3.23 MB total.
- Domain/API tests: 19 passed.
- Desktop + mobile browser tests: 10 passed (8 full flow checks + 2 static-host fallback checks).
- npm audit --omit=dev --audit-level=high: 0 vulnerabilities reported.
- git diff --check: passed.
- Visual inspection: desktop/mobile menu, product contact sheet, order board. Two unsuitable generated images regenerated (hot chocolate + espresso, espresso freddo).
- Original vs migrated product IDs, category membership and prices compared independently before committing.
- SQLite backup opened and verified; orders/settings/loyalty ledger persist after restart.
- Chrome tested at 1440×1050 and 390×844. Docker build and public production hosting not run.
- Test data uses separate disposable databases / .runtime/ui-tests, never the real preview database.

Files: preview-desktop.png, preview-products.png, preview-mobile-products.png, preview-owner.png, products-contact-sheet.png.
