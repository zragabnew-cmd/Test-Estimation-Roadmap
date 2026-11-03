# Test Estimation Roadmap

An interactive, single-file web app that helps testers estimate how long testing a user story will take.

## How it works
A road with six stops and a car that drives to the next stop as you go:

1. **Start**
2. **Business**: pick your system type (E-commerce, Banking, Healthcare, Telecom, and more). This sets a suggested contingency and best-fit techniques.
3. **Techniques**: nine estimation techniques with formulas, pros, cons and examples (Ratio-based, Extrapolation, Wideband Delphi, Planning Poker, Three-Point, WBS, Analogous, Function/Test Point, Expert judgment).
4. **Calculate**: Three-Point (PERT) calculator per test case with live maths, plus a small calculator for every other technique. A retesting percentage and a pinned **Total time** bar are included.
5. **Results**: total estimation, confidence ranges (68 / 95 / 99.7 %), person-days and a bell curve.
6. **Export**: CSV, JSON, an HTML report, or a copied summary.

## Three-Point formulas
- Expected: `E = (a + 4m + b) / 6`
- Standard deviation: `SD = (b - a) / 6`
- Total: `Σ E`, and total SD = `√(Σ SD²)`
- Total estimation = base × (1 + retesting %) × (1 + contingency %)

## Run it
No build step. Open `index.html` in a browser, or enable GitHub Pages for the `main` branch.
