
# NIEM 5.0

This is the NIEM 5.0 major release.

In a major release, content may be updated in any namespace, including Core.  Changes may also be made to the NIEM architecture, which may be reflected in the structure and layout of the NIEM schemas.

The following is a summary of the key changes made in this release.  More details are available from the [5.0 issues](https://github.com/NIEM/NIEM-Releases/issues?page=1&q=is%3Aissue+label%3A5.0) in the NIEM Releases issue tracker, and the change log spreadsheet in the release package.

- [NIEM specification updates](#niem-specification-updates)
  - [NIEM Naming and Design Rules (NDR) 5.0](#niem-naming-and-design-rules-ndr-50)
- [Auxiliary content](#auxiliary-content)
- [Core](#core)
  - [Additions](#additions)
  - [Harmonization](#harmonization)
  - [Merged Core Supplements](#merged-core-supplements)
- [Domain changes](#domain-changes)
  - [Cross-domain harmonization](#cross-domain-harmonization)
  - [Biometrics](#biometrics)
  - [CBRN](#cbrn)
  - [Emergency Management](#emergency-management)
  - [Immigration](#immigration)
  - [Intelligence](#intelligence)
  - [Justice](#justice)
  - [MilOps](#milops)
  - [Screening](#screening)
- [Codes](#codes)
  - [General changes](#general-changes)
  - [Version updates](#version-updates)
- [External Standards](#external-standards)
- [Release package updates](#release-package-updates)
- [Other updates](#other-updates)

## NIEM specification updates

This release reflects updates made to the NIEM specifications that define rules for NIEM reference schemas.

### NIEM Naming and Design Rules (NDR) 5.0

- Updated structures and appinfo utility schemas and added definitions [(#157)](https://github.com/NIEM/NIEM-Releases/issues/157)
- Reestablished structures:sequenceID attribute [(#154)](https://github.com/NIEM/NIEM-Releases/issues/154)

## Auxiliary content

NIEM 5.0 has introduced auxiliary schemas to the release package.  These are similar to the NIEM code schemas, which provide codes in a NIEM-conformant format from authoritative sources that may or may not participate in NIEM releases or governance processes.  The auxiliary schemas provide full NIEM-conformant content (properties and types, in addition to codes) from authoritative sources that are not NIEM domains and may or may not actively participate in NIEM releases and governance.

- Added Controlled Unclassified Information (CUI) marking metadata [(#156)](https://github.com/NIEM/NIEM-Releases/issues/156)
- Added Generic Statistical Information Model (GSIM) content [(#155)](https://github.com/NIEM/NIEM-Releases/issues/155)

## Core

### Additions

- Added ActivityLocation element to nc:ActivityType [(#71)](https://github.com/NIEM/NIEM-Releases/issues/71)
- Added AreaMeasureType [(#143)](https://github.com/NIEM/NIEM-Releases/issues/143)
- Added employment assignment and position components [(#105)](https://github.com/NIEM/NIEM-Releases/issues/105)
- Added MailingAddress and PhysicalAddress as more specific substitutions for nc:Address [(#72)](https://github.com/NIEM/NIEM-Releases/issues/72)
- Added metadata to represent the reason for empty values [(#76)](https://github.com/NIEM/NIEM-Releases/issues/76)
- Added MilitaryPersonIdentification element to nc:MilitarySummaryType [(#32)](https://github.com/NIEM/NIEM-Releases/issues/32)
- Added PercentType to clearly define the expected value range for percentage elements [(#7)](https://github.com/NIEM/NIEM-Releases/issues/7)
- Added PersonContactInformation element to represent generic contact information in nc:PersonType [(#29)](https://github.com/NIEM/NIEM-Releases/issues/29)
- Added street category codes and updated street directionals [(#80)](https://github.com/NIEM/NIEM-Releases/issues/80)
- Added street direction substitution groups for alternate code representations [(#65)](https://github.com/NIEM/NIEM-Releases/issues/65)
- Added substitution groups for easier inclusion of local code sets [(#82)](https://github.com/NIEM/NIEM-Releases/issues/82)

### Harmonization

- Harmonized activity components [(#147)](https://github.com/NIEM/NIEM-Releases/issues/147)
- Harmonized address components [(#111)](https://github.com/NIEM/NIEM-Releases/issues/111)
- Harmonized aircraft components [(#120)](https://github.com/NIEM/NIEM-Releases/issues/120)
- Harmonized assessment components [(#148)](https://github.com/NIEM/NIEM-Releases/issues/148)
- Harmonized building components [(#98)](https://github.com/NIEM/NIEM-Releases/issues/98)
- Harmonized capability components [(#149)](https://github.com/NIEM/NIEM-Releases/issues/149)
- Harmonized citizenship and nationality components [(#124)](https://github.com/NIEM/NIEM-Releases/issues/124)
- Harmonized citizenship and nationality country codes via the use of nc:CountryType [(#93)](https://github.com/NIEM/NIEM-Releases/issues/93)
- Harmonized conveyance components [(#119)](https://github.com/NIEM/NIEM-Releases/issues/119)
- Harmonized country and state class terms [(#67)](https://github.com/NIEM/NIEM-Releases/issues/67)
- Harmonized document components and added a new ReportType [(#129)](https://github.com/NIEM/NIEM-Releases/issues/129)
- Harmonized education components [(#113)](https://github.com/NIEM/NIEM-Releases/issues/113)
- Harmonized employment components [(#105)](https://github.com/NIEM/NIEM-Releases/issues/105)
- Harmonized item components [(#115)](https://github.com/NIEM/NIEM-Releases/issues/115)
- Harmonized jurisdiction components [(#141)](https://github.com/NIEM/NIEM-Releases/issues/141)
- Harmonized location elements [(#100)](https://github.com/NIEM/NIEM-Releases/issues/100)
- Harmonized location area elements and GML adapters [(#101)](https://github.com/NIEM/NIEM-Releases/issues/101)
- Harmonized metadata components [(#142)](https://github.com/NIEM/NIEM-Releases/issues/142)
- Harmonized military summary components [(#86)](https://github.com/NIEM/NIEM-Releases/issues/86)
- Harmonized orientation components [(#151)](https://github.com/NIEM/NIEM-Releases/issues/151)
- Harmonized organization components [(#150)](https://github.com/NIEM/NIEM-Releases/issues/150)
- Harmonized plan components [(#160)](https://github.com/NIEM/NIEM-Releases/issues/160)
- Harmonized software components [(#118)](https://github.com/NIEM/NIEM-Releases/issues/118)
- Harmonized task components [(#161)](https://github.com/NIEM/NIEM-Releases/issues/161)
- Harmonized vehicle components [(#122)](https://github.com/NIEM/NIEM-Releases/issues/122)

### Merged Core Supplements

NIEM 5.0 merges the changes made in the Core Supplements published since the last major release, NIEM 4.0.

- Merged Core Supplement 4.0.1. [(#127)](https://github.com/NIEM/NIEM-Releases/issues/127)
  - Replaced nc:PolygonCoordinate (nc:Location2DGeospatialCoordinateType) with new nc:PolygonNodeLocation (nc:LocationType) [(#9)](https://github.com/NIEM/NIEM-Releases/issues/9)
  - Changed the parent type of nc:LocationHeightMeasureType from nc:MeasureType to nc:LengthMeasureType [(#13)](https://github.com/NIEM/NIEM-Releases/issues/13).
- Merged Core Supplement 4.0.2 [(#127)](https://github.com/NIEM/NIEM-Releases/issues/127)
  - Updated Census county codes [(#45)](https://github.com/NIEM/NIEM-Releases/issues/45)
  - Updated Census / DOT commodity codes [(#48)](https://github.com/NIEM/NIEM-Releases/issues/48)
  - Updated DEA drug codes [(#49)](https://github.com/NIEM/NIEM-Releases/issues/49)
  - Updated Dept of Labor occupation codes [(#50)](https://github.com/NIEM/NIEM-Releases/issues/50)
  - Updated Census FIPS state codes [(#51)](https://github.com/NIEM/NIEM-Releases/issues/51)
  - Updated HazMat codes [(#53)](https://github.com/NIEM/NIEM-Releases/issues/53)
  - Updated HL7 religion codes [(#54)](https://github.com/NIEM/NIEM-Releases/issues/54)
  - Updated ISO 4217 currency codes [(#55)](https://github.com/NIEM/NIEM-Releases/issues/55)
  - Updated ISO 639-3 language codes [(#56)](https://github.com/NIEM/NIEM-Releases/issues/56)
  - Updated OmniClass facility codes [(#57)](https://github.com/NIEM/NIEM-Releases/issues/57)
  - Added GENC XML Schema enumerations [(#66)](https://github.com/NIEM/NIEM-Releases/issues/66)

## Domain changes

### Cross-domain harmonization

- Harmonized warrant components in Justice and Screening [(#62)](https://github.com/NIEM/NIEM-Releases/issues/62)

### Biometrics

- Harmonized biom:ImageType [(#99)](https://github.com/NIEM/NIEM-Releases/issues/99)

### CBRN

- Refactored schedule week information [(#164)](https://github.com/NIEM/NIEM-Releases/issues/164)

### Emergency Management

- Added additional content from the Public Health Emergency Operations Center (PHEOC) Minimum Data Set [(#138)](https://github.com/NIEM/NIEM-Releases/issues/138)
- Fixed base type of em:DamCategoryCodeType [(#188)](https://github.com/NIEM/NIEM-Releases/issues/188)

### Immigration

- Refactored CountryType as an augmentation for better reusability with nc:CountryType [(#112)](https://github.com/NIEM/NIEM-Releases/issues/112)

### Intelligence

- Refactored PersonAugmentationType [(#114)](https://github.com/NIEM/NIEM-Releases/issues/114)

### Justice

- Updated person sex codes [(#146)](https://github.com/NIEM/NIEM-Releases/issues/146)
- Moved j:ArresteeType elements to new j:ArrestSubjectAssociationType [(#70)](https://github.com/NIEM/NIEM-Releases/issues/70)
- Moved j:ChargeNCICText to substitution group [(#27)](https://github.com/NIEM/NIEM-Releases/issues/27)
- Moved j:MedicalTreatmentType elements into j:TreatmentAugmentationType [(#103)](https://github.com/NIEM/NIEM-Releases/issues/103)
- Moved nc:PleaCategoryCodeType to the Justice domain [(#24)](https://github.com/NIEM/NIEM-Releases/issues/24)
- Moved additional justice-specific types from Core to Justice [(#79)](https://github.com/NIEM/NIEM-Releases/issues/79)
- Renamed j:SupervisionFineAmount and j:CourtCostAmount elements in j:SentenceType [(#25)](https://github.com/NIEM/NIEM-Releases/issues/25)
- Removed person finger position elements from j:PersonAugmentationType [(#159)](https://github.com/NIEM/NIEM-Releases/issues/159)
- Removed nested element j:SupervisionRestriction from j:SupervisionRestrictionType [(#187)](https://github.com/NIEM/NIEM-Releases/issues/187)
- Updated the definition of deprecated aamva:DriverLicenseClassCodeSimpleType code "M" [(#108)](https://github.com/NIEM/NIEM-Releases/issues/108)
- Updated accident-related definitions in the Justice domain to add the term 'crash' for better search and discovery [(#107)](https://github.com/NIEM/NIEM-Releases/issues/107)
- Updated definition of j:PersonSignature [(#92)](https://github.com/NIEM/NIEM-Releases/issues/92)

### MilOps

- Added approval status codes to replace the corresponding set removed from NDEx [(#173)](https://github.com/NIEM/NIEM-Releases/issues/173)
- Updated TelephoneNumberCategoryCodeSimpleType from a token to a union of xCard and MilOps codes [(#172)](https://github.com/NIEM/NIEM-Releases/issues/172)

### Screening

- Refactored AddressAugmentationType [(#110)](https://github.com/NIEM/NIEM-Releases/issues/110)
- Refactored PersonNameAugmentation and PersonNameTextAugmentation [(#77)](https://github.com/NIEM/NIEM-Releases/issues/77)

## Codes

### General changes

- Moved Core code elements to code namespaces to enable easier code updates during minor releases [(#90)](https://github.com/NIEM/NIEM-Releases/issues/90)
- Simplified namespace definitions [(#139)](https://github.com/NIEM/NIEM-Releases/issues/139)
- Synchronized folders, file names, and target namespaces [(#58)](https://github.com/NIEM/NIEM-Releases/issues/58)
- Added GENC alpha-2 and numeric country codes [(#94)](https://github.com/NIEM/NIEM-Releases/issues/94)
- Added appinfo to GENC code types to meet requirements for codespace identifiers [(#163)](https://github.com/NIEM/NIEM-Releases/issues/163)
- Added FIPS unique 5-digit county code set [(#47)](https://github.com/NIEM/NIEM-Releases/issues/47)
- Harmonized FBI codes across NCIC, NDEx, UCR, and Justice (see individual changes below)
- Merged BLS and DOL namespaces into single BLS namespace [(#145)](C:\cdm\niem\releases\5.0\input\harmonization\145-bls)
- Merged FIPS 5-2 state codes and Census county codes into consolidated FIPS namespaces [(#52)](https://github.com/NIEM/NIEM-Releases/issues/52)
- Replaced non-breaking spaces in OmniClass facility codes [(#133)](https://github.com/NIEM/NIEM-Releases/issues/133)
- Replaced NCIC vehicle model (VMO) codes with unique values [(#47)](https://github.com/NIEM/NIEM-Releases/issues/47)

### Version updates

- Updated FIPS county codes to 2019 version [(#181)](https://github.com/NIEM/NIEM-Releases/issues/181)
- Updated GENC codes to version 3-11 [(#162)](https://github.com/NIEM/NIEM-Releases/issues/162)
- Updated Hazmat codes [(#175)](https://github.com/NIEM/NIEM-Releases/issues/175)
- Updated ISO 3166-1 country codes to ISO 3166-1:2020 [(#183)](https://github.com/NIEM/NIEM-Releases/issues/183)
- Updated ISO 639-3 language codes to 2020-01-30 update [(#185)](https://github.com/NIEM/NIEM-Releases/issues/185)
- Updated Justice domain codes [(#137)](https://github.com/NIEM/NIEM-Releases/issues/137)
- Updated NCIC codes [(#134)](https://github.com/NIEM/NIEM-Releases/issues/134)
- Updated NDEx codes [(#135)](https://github.com/NIEM/NIEM-Releases/issues/135)
- Updated UCR codes [(#136)](https://github.com/NIEM/NIEM-Releases/issues/136)
- Updated UNECE unit of measure codes to Revision 15 (2020) [(#180)](https://github.com/NIEM/NIEM-Releases/issues/180)
- Updated USPS state codes (definition formatting) [(#182)](https://github.com/NIEM/NIEM-Releases/issues/182)

## External Standards

- Replaced the full set of GML schemas with a simplified profile representing NIEM requirements [(#128)](https://github.com/NIEM/NIEM-Releases/issues/128)

## Release package updates

- Simplified folder layout [(#140)](https://github.com/NIEM/NIEM-Releases/issues/140)
- Changed the character encoding of the XML schemas from "US-ASCII" to "UTF-8" for better international support [(#125)](https://github.com/NIEM/NIEM-Releases/issues/125)
- Added attribute xml:lang to reference schemas [(#153)](https://github.com/NIEM/NIEM-Releases/issues/153)
- Normalized schema sort orders [(#179)](https://github.com/NIEM/NIEM-Releases/issues/179)

## Other updates

- Fixed definition formatting [(#132)](https://github.com/NIEM/NIEM-Releases/issues/132)
- Fixed definition inconsistencies and invalid component references [(#171)](https://github.com/NIEM/NIEM-Releases/issues/171)
- Fixed invalid augmentation names [(#78)](https://github.com/NIEM/NIEM-Releases/issues/78)
- Fixed role types that did not extend structure:ObjectType [(#170)](https://github.com/NIEM/NIEM-Releases/issues/170)
- Fixed spelling errors and added local terminology [(#131)](https://github.com/NIEM/NIEM-Releases/issues/131)
- Fixed unused elements [(#186)](https://github.com/NIEM/NIEM-Releases/issues/186)
- Moved role-of elements first under their types [(#166)](https://github.com/NIEM/NIEM-Releases/issues/166)
- Moved j:ItemMakeAbstract to Core [(#95)](https://github.com/NIEM/NIEM-Releases/issues/95)
- Moved nc:EffectiveDate from screening augmentation to nc:PersonNameType [(#96)](https://github.com/NIEM/NIEM-Releases/issues/96)
- Moved nc:ConveyanceFuelCategoryAbstract from j:EngineType to nc:ConveyanceType [(#116)](https://github.com/NIEM/NIEM-Releases/issues/116)
- Removed duplicate components [(#174)](https://github.com/NIEM/NIEM-Releases/issues/174)
- Removed or updated unused elements in Core [(#106)](https://github.com/NIEM/NIEM-Releases/issues/106)
- Updated nc:EntityType to remove requirement that it represents a legal entity; added a new legal entity indicator [(#17)](https://github.com/NIEM/NIEM-Releases/issues/17)
