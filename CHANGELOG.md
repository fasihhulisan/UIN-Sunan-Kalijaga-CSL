# Changelog

All notable changes to this project will be documented in this file.

The format is inspired by Keep a Changelog.

---

## [1.0.0] - 2026-07-26

### Added

- Initial public release of the UIN Sunan Kalijaga Citation Style Language (CSL).
- Footnote citation style based on the official UIN Sunan Kalijaga thesis guidelines.
- Bibliography formatting according to UIN Sunan Kalijaga standards.
- Support for common CSL reference types, including:
  - Books
  - Book Chapters
  - Journal Articles
  - Conference Papers
  - Theses and Dissertations
  - Reports
  - Web Pages
  - Newspapers
  - Magazines
  - Legal Materials
  - Other CSL-supported item types
- Project documentation (README).
- Project license (CC BY-SA 3.0).
- Documentation of the Mendeley Cite page locator limitation.

### Changed

- Customized from the upstream Chicago Notes and Bibliography (CMOS 18th) CSL style to comply with UIN Sunan Kalijaga citation guidelines.
- Adjusted bibliography and footnote formatting.
- Customized author name formatting.
- Customized Indonesian localization.
- Adjusted editor formatting from **"ed. oleh John Doe"** to **"John Doe (ed.)"** to match UIN Sunan Kalijaga citation guidelines.
- Preserved translator formatting using the existing Chicago Notes & Bibliography convention.
- Began final audit of Book Section, Encyclopedia Article, and Edited Collection citation formats against the official UIN thesis manual.
- Removed the default "in" preposition before monographic container titles to match UIN Sunan Kalijaga citation guidelines.

### Fixed

- Correct implementation of:
  - Ibid.
  - Ibid., page.
  - Shortened citations after intervening references.
- Fixed CSL validator errors.
- Fixed archive locator handling.
- Fixed page locator labeling.
- Improved compatibility with Mendeley Reference Manager.

### Known Limitation

Mendeley Cite currently does not correctly parse page ranges entered as:

```
339-340
```

Use:

```
339
```

or

```
339, 340
```

instead.

This limitation originates from Mendeley Cite rather than this CSL.