# Changelog

All notable changes to this project will be documented in this file.

The format is inspired by Keep a Changelog.

---

## [1.0.0] - 2026-07-28

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
- Customized monographic note formatting for UIN Sunan Kalijaga guideline.
- Removed the automatic preposition "dalam" for edited monographic works (Book Section, Encyclopedia Article, and similar references).
- Added a dedicated `source-monographic-note-uin` macro to preserve Chicago behavior for other reference types.
- Applied the custom UIN formatting only to monographic references with editors, leaving all other citation types unchanged.
- Added a dedicated bibliography macro for edited monographic works.
- Removed the automatic "In" prefix in bibliography entries for edited books.
- Replaced the default Chicago "edited by" label with the UIN-preferred "(ed.)" notation.
- Applied the customization only to Book Section, Encyclopedia Article, and similar edited monographic references.
- Adjusted handling of multivolume books in footnotes.
- Suppressed duplicate volume output before publication information for `book` references with page locators.
- Prepared CSL behavior to match the UIN Sunan Kalijaga guideline format for multivolume books (`Title (Place: Publisher, Year), III:155`).
- Improved footnote formatting for multivolume books by separating volume handling from the standard monographic identifier.
- Added dedicated `book-volume-bib` macro to support bibliography formatting for multivolume books.
- Prepared independent volume handling to simplify future customization of UIN citation rules.
- Updated CSL metadata (`<rights>`) to comply with CitationStyles.org validator.
- Added license section to README.
### Fixed

- Correct implementation of:
  - Ibid.
  - Ibid., page.
  - Shortened citations after intervening references.
- Fixed CSL validator errors.
- Fixed archive locator handling.
- Fixed page locator labeling.
- Improved compatibility with Mendeley Reference Manager.
- Removed unnecessary "in" from footnotes and bibliography for edited monographic sources (book sections, encyclopedia entries, and anthology chapters) to match UIN Sunan Kalijaga citation guidelines.
- Changed edited monographic references to use `Editor (ed.)` instead of `edited by` in bibliography.
- Improved multivolume book handling by suppressing redundant volume labels in footnotes, preparing support for UIN-style volume-page formatting (e.g., `III:155`).
- Adjusted multivolume book footnote handling to correctly combine volume and page locator.
- Adjusted Working Paper (`report`) title formatting to comply with UIN Sunan Kalijaga citation guidelines.
- Changed Working Paper titles from italic to quoted style in both footnotes and bibliography.
- Preserved institutional document names (`collection-title`) as plain text following the title.
- Verified compatibility with Mendeley Reference Manager Working Paper item type.

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