
# NIEM 5.1 Beta 1

This is the beta 1 draft of the NIEM 5.1 minor release.

In a minor release, content may be updated in domains and code tables.  Core, namespaces imported by Core, and the architecture, which is defined by the NIEM Naming and Design Rules (NDR), will remain locked until the next major release.

## Feedback

Please submit feedback by Wednesday, August 18, 2021. Feedback can be posted directly to the NIEM Releases [issue tracker](https://github.com/NIEM/NIEM-Releases/issues) (see [help](https://github.com/NIEM/NIEM-Releases/wiki/Issues)) or emailed to [niem-comments@lists.gatech.edu](niem-comments@lists.gatech.edu).

## Key changes

The following is a summary of the key changes made in this release.  More details are available from the [5.1 issues](https://github.com/NIEM/NIEM-Releases/issues?page=1&q=is%3Aissue+label%3A5.1) in the NIEM Releases issue tracker, and the change log spreadsheet in the release package.

- **Biometrics domain**
  - Added additional DNA-related content ([#152](https://github.com/NIEM/NIEM-Releases/issues/152))

- **Cyber domain** (new)
  - Added content supporting Federal Incident Reporting Requirements (FIRR) ([#209](https://github.com/NIEM/NIEM-Releases/issues/209))
  - Added content supporting State, Local, Tribal, and Territorial (SLTT) Agency Cyber Incident Reporting Requirements (CIRR) ([#215](https://github.com/NIEM/NIEM-Releases/issues/215))

- **Emergency Management domain**
  - Added flood damage claim content from OpenFEMA ([#208](https://github.com/NIEM/NIEM-Releases/issues/208))

- **Justice domain**
  - Moved Justice elements with a NCIC data type to the NCIC namespace ([#214](https://github.com/NIEM/NIEM-Releases/issues/214))

- **Military Operations domain**
  - Added content from the Joint Non-Kinetic Effectiveness (JNKE) IEPD ([#210](https://github.com/NIEM/NIEM-Releases/issues/210))

- **NCIC codes**
  - Re-added 4.2 code sets that were removed from the 5.0 release due to harmonization efforts across the FBI and Justice code sets for legacy support. ([#211](https://github.com/NIEM/NIEM-Releases/issues/211))

## Code updates

- Updated CUI codes ([#212](https://github.com/NIEM/NIEM-Releases/issues/212))

## Minor fixes

- Updated the definition of hs:Visitation ([#213](https://github.com/NIEM/NIEM-Releases/issues/213))
