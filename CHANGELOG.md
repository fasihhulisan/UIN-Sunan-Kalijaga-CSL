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