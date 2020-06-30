
# NIEM 5.0-alpha1

This is the alpha 1 draft of the NIEM 5.0 major release.

In a major release, content may be updated in any namespace, including Core.  Changes may also be made to the NIEM architecture, which may be reflected in the structure and layout of the NIEM schemas.

The final NIEM 5.0 release is targeted for Fall 2020.

## Feedback

Please submit feedback by Friday, April 17.  Feedback can be posted directly to the [NIEM Releases issue tracker](https://github.com/NIEM/NIEM-Releases/issues) or emailed to niem-comments@lists.gatech.edu .

## Key changes

The following is a summary of the content changes made in this release.  Please review the [5.0 issues](https://github.com/NIEM/NIEM-Releases/issues?page=1&q=is%3Aissue+label%3A5.0) in the NIEM Releases issue tracker or the change log spreadsheet in the release package for a detailed list of changes.

Note that schema updates have been committed per issue, so issue-specific file diffs are available from the issue links below or by reviewing the commit history in a git client.

### Core

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

### Code Tables

- Simplified namespace definitions [(#139)](https://github.com/NIEM/NIEM-Releases/issues/139)
- Merged FIPS 5-2 state codes and Census county codes into consolidated FIPS namespaces [(#52)](https://github.com/NIEM/NIEM-Releases/issues/52)
- Replaced non-breaking spaces in OmniClass facility codes [(#133)](https://github.com/NIEM/NIEM-Releases/issues/133)
- Added GENC alpha-2 and numeric country codes [(#94)](https://github.com/NIEM/NIEM-Releases/issues/94)
- Updated the definition of deprecated aamva:DriverLicenseClassCodeSimpleType code "M" [(#108)](https://github.com/NIEM/NIEM-Releases/issues/108)
- Updated FBI NCIC codes [(#134)](https://github.com/NIEM/NIEM-Releases/issues/134) and replaced the VMO code set with unique code values
- Updated FBI NDEx codes [(#135)](https://github.com/NIEM/NIEM-Releases/issues/135)
- Updated FBI UCR codes [(#136)](https://github.com/NIEM/NIEM-Releases/issues/136)
- Updated FBI Justice domain codes [(#137)](https://github.com/NIEM/NIEM-Releases/issues/137)

### Auxiliary content

- Added content from the Generic Statistical Information Model (GSIM) content as a precursor to the new Statistics domain [(#155)](https://github.com/NIEM/NIEM-Releases/issues/155)
- Added Controlled Unclassified Information (CUI) metadata [(#156)](https://github.com/NIEM/NIEM-Releases/issues/156)

### Harmonization and QA

- Added new nc:PersonContactInformation element to nc:PersonType [(#29)](https://github.com/NIEM/NIEM-Releases/issues/29)
- Added substitution groups for street direction codes [(#65)](https://github.com/NIEM/NIEM-Releases/issues/65)
- Added street category codes and updated directionals [(#80)](https://github.com/NIEM/NIEM-Releases/issues/80)
- Added new nc:ActivityLocation element to nc:ActivityType [(#71)](https://github.com/NIEM/NIEM-Releases/issues/71)
- Added nc:MailingAddress and nc:PhysicalAddress as substitutions for nc:Address [(#72)](https://github.com/NIEM/NIEM-Releases/issues/72)
- Fixed invalid augmentation names [(#78)](https://github.com/NIEM/NIEM-Releases/issues/78)
- Fixed definition of j:PersonSignature [(#92)](https://github.com/NIEM/NIEM-Releases/issues/92)
- Fixed spelling errors and added local terminology [(#131)](https://github.com/NIEM/NIEM-Releases/issues/131) - *in progress*
- Fixed definition formatting [(#132)](https://github.com/NIEM/NIEM-Releases/issues/132) - *in progress*
- Harmonized warrant components in Justice and Screening [(#62)](https://github.com/NIEM/NIEM-Releases/issues/62)
- Harmonized biom:ImageType [(#99)](https://github.com/NIEM/NIEM-Releases/issues/99)
- Harmonized location area elements and GML adapters [(#101)](https://github.com/NIEM/NIEM-Releases/issues/101) - *in progress*
- Harmonized education components [(#113)](https://github.com/NIEM/NIEM-Releases/issues/113)
- Harmonized conveyance components [(#119)](https://github.com/NIEM/NIEM-Releases/issues/119)
- Harmonized vehicle components [(#122)](https://github.com/NIEM/NIEM-Releases/issues/122)
- Merged scr:PersonNameAugmentation and scr:PersonNameTextAugmentation [(#77)](https://github.com/NIEM/NIEM-Releases/issues/77)
- Moved nc:PleaCategoryCodeType to the Justice domain [(#24)](https://github.com/NIEM/NIEM-Releases/issues/24)
- Moved additional Justice-specific types from Core to Justice [(#79)](https://github.com/NIEM/NIEM-Releases/issues/79)
- Moved Core code elements to code namespaces to enable easier code set updates during minor releases (#90)
- Moved j:ItemMakeAbstract to Core [(#95)](https://github.com/NIEM/NIEM-Releases/issues/95)
- Moved nc:EffectiveDate from screening augmentation to nc:PersonNameType [(#96)](https://github.com/NIEM/NIEM-Releases/issues/96)
- Refactored scr:AddressAugmentationType [(#110)](https://github.com/NIEM/NIEM-Releases/issues/110)
- Refactored im:CountryType [(#112)](https://github.com/NIEM/NIEM-Releases/issues/112)
- Refactored intel:PersonAugmentationType [(#114)](https://github.com/NIEM/NIEM-Releases/issues/114)
- Refactored citizenship and nationality into separate types [(#124)](https://github.com/NIEM/NIEM-Releases/issues/124)
- Updated inconsistent code set folder paths, file names, and target namespaces [(#58)](https://github.com/NIEM/NIEM-Releases/issues/58)
- Updated country and state element class terms [(#67)](https://github.com/NIEM/NIEM-Releases/issues/67)
- Updated location elements [(#100)](https://github.com/NIEM/NIEM-Releases/issues/100)
- Updated address elements [(#111)](https://github.com/NIEM/NIEM-Releases/issues/111)
- Used nc:CountryType instead of custom substitution groups for citizenship and nationality elements [(#93)](https://github.com/NIEM/NIEM-Releases/issues/93)

### Release package updates

- Simplified folder layout [(#140)](https://github.com/NIEM/NIEM-Releases/issues/140)
- Changed the character encoding of the XML schemas from "US-ASCII" to "UTF-8" for better international support [(#125)](https://github.com/NIEM/NIEM-Releases/issues/125)
- Normalized schema sort orders:
  - Sorted namespace prefix declarations by prefix
  - Sorted import statements by target namespace
  - Sorted local terminology by term
  - Sorted type union members by qname
  - Sorted metadata appliesTo values by qname
  - Sorted components using case-insensitive order, with spaces sorting above other characters
  - Sorted facets by style (alphabetically with the exception of sorting min facets before max facets), value, and definition
- Updated target namespaces and dependencies for 5.0.

## Expected updates for beta

Additional updates are being considered or are expected for the beta draft, including:

- Additional content from the Public Health Emergency Operations Center (PH-EOC) Minimum Data Set added to the Emergency Management domain
- Code table updates, including AAMVA and GENC edition 3.0 update 11
- Continued harmonization and QA fixes across the model
- Harmonization of updated Model Minimum Uniform Crash Criteria (MMUCC) content with the Justice domain
