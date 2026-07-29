# UIN Sunan Kalijaga CSL

A Citation Style Language (CSL) file for **UIN Sunan Kalijaga Yogyakarta**, designed for use with Zotero, Mendeley, and other CSL-compatible reference managers.

This CSL is based on the official citation and bibliography of the thesis guidelines of UIN Sunan Kalijaga and aims to provide consistent formatting for academic writing.

---

## Latest Release

Current stable release:

**v1.0.1**

- Repository-validator compliant
- Ready for CSL Repository submission

## Features

- Footnote-based citation style.
- Bibliography formatted according to UIN Sunan Kalijaga thesis guidelines.
- Supports books, journal articles, conference papers, theses, reports, websites, and other common reference types.
- Compatible with Zotero, Mendeley Reference Manager, and other CSL processors.
- Open source and freely available.

---

## Installation

1. Download the latest `UIN Sunan Kalijaga.csl` file.
2. Open your reference manager.
3. Import or install the CSL file.
4. Select **UIN Sunan Kalijaga** as your citation style.

---

## Compatibility

This CSL has been tested with:

-  Zotero
-  Mendeley Reference Manager
-  Mendeley Cite for Microsoft Word

---

## Supported Reference Types

This CSL supports common reference types including:

- Book
- Book Chapter
- Journal Article
- Conference Paper
- Thesis / Dissertation
- Report
- Web Page
- Newspaper Article
- Magazine Article
- Encyclopedia Entry
- Dictionary Entry
- Government Document
- Legal Material
- And other CSL standard item types

---

## Known Limitation

### Mendeley Cite Page Range Input

A limitation has been identified in **Mendeley Cite**, not in this CSL.

When inserting citations with page numbers:

✔ Works

```
339.
```

```
339, 340.
```

```
339, 340, 341.
```

✘ Does not work correctly

```
339-340.
```

The page range entered using a hyphen (`-`) is not parsed correctly by Mendeley Cite and therefore is not rendered in the generated citation.

As a workaround, enter individual page numbers separated by commas.

More details are available in:

```
docs/Mendeley Cite-Page Range Limitation.docx
```

---

## Documentation

Additional documentation is available in the `docs` directory.

---

## Contributing

Bug reports, suggestions, and pull requests are welcome.

If you encounter compatibility issues with specific reference managers, please open an Issue.

---

## License

This project is licensed under the **Creative Commons Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0)** License.

See the LICENSE file for details.

---

## Author

**Fasih Hulisan**

---

## Acknowledgements

- UIN Sunan Kalijaga Yogyakarta
- Citation Style Language (CSL) Project
- Zotero Community
- Mendeley Reference Manager

## Status

- GitHub Release
- ORCID Research Tool
- Preparing submission to the official Citation Style Language (CSL) Repository