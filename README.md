
# NIEM 5.1

This is the NIEM 5.1 minor release.

In a minor release, content may be updated in domains and code tables.  Core, namespaces imported by Core, and the architecture, which is defined by the NIEM Naming and Design Rules (NDR), will remain locked until the next major release.

## Key changes

The following is a summary of the key changes made in this release.  More details are available from the [5.1 issues](https://github.com/NIEM/NIEM-Releases/issues?page=1&q=is%3Aissue+label%3A5.1) in the NIEM Releases issue tracker, and the change log spreadsheet in the release package.

- **Biometrics domain**
  - Added additional DNA-related content ([#152](https://github.com/NIEM/NIEM-Releases/issues/152))
  - Updated pedigree content ([#224](https://github.com/NIEM/NIEM-Releases/issues/224))
  - Restored DNAPedigree components from the 4.1 release for backward compatibility ([#227](https://github.com/NIEM/NIEM-Releases/issues/227))

- **CUI**
  - Split the single Limited Dissemination Control (LDC) code set into separate document marking and portion marking LDC code sets ([#233](https://github.com/NIEM/NIEM-Releases/issues/223))

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
  - Removed ncic:BOATCodeType as it is no longer being used ([#218](https://github.com/NIEM/NIEM-Releases/issues/218))
  - Updated codes for NIEM 5.1, with changes to the MAK, VMA, and VMO code sets ([#219](https://github.com/NIEM/NIEM-Releases/issues/219))

## Code updates

- Updated CUI codes ([#212](https://github.com/NIEM/NIEM-Releases/issues/212) and [#225](https://github.com/NIEM/NIEM-Releases/issues/225))

- Updated ISO 639-3 language codes *(2012-02-18 update)* ([#222](https://github.com/NIEM/NIEM-Releases/issues/222))

- Updated ucr:IncidentBiasMotivationCodeSimpleType code value and definition ([#229](https://github.com/NIEM/NIEM-Releases/issues/229))

## Minor fixes

- Updated the definition of hs:Visitation ([#213](https://github.com/NIEM/NIEM-Releases/issues/213))

- Updated the definition of the Geospatial adapter namespace (geo) to reflect that GML is now included with NIEM as a subset ([#220](https://github.com/NIEM/NIEM-Releases/issues/220))
