
# NIEM 5.0-alpha1

This is a preliminary draft of the NIEM 5.0 alpha 1 major release.  Additional changes will be applied before alpha1 is published for review.

In a major release, content may be updated in any namespace, including Core.  Changes may also be made to the NIEM architecture, which may be reflected in the structure and layout of the NIEM schemas.

## Key changes

The following is a summary of the content changes made in this release.

Please review the [5.0 issues in the NIEM Releases issue tracker](https://github.com/NIEM/NIEM-Releases/issues?page=1&q=is%3Aissue+label%3A5.0+is%3Aclosed) or the change log spreadsheet in the release package for a detailed list of changes.

### Core

- Merged Core Supplement 4.0.1. (#127)
  - Replaced nc:PolygonCoordinate (nc:Location2DGeospatialCoordinateType) with new nc:PolygonNodeLocation (nc:LocationType) (#9)
  - Changed the parent type of nc:LocationHeightMeasureType from nc:MeasureType to nc:LengthMeasureType (#13).
- Merged Core Supplement 4.0.2 (#127)
  - Updated Census county codes (#45)
  - Updated Census / DOT commodity codes (#48)
  - Updated DEA drug codes (#49)
  - Updated Dept of Labor occupation codes (#50)
  - Updated Census FIPS state codes (#51)
  - Updated HazMat codes (#53)
  - Updated HL7 religion codes (#54)
  - Updated ISO 4217 currency codes (#55)
  - Updated ISO 639-3 language codes (#56)
  - Updated OmniClass facility codes (#57)
  - Added GENC XML Schema enumerations (#66)

### Code Tables

- Merged FIPS 5-2 state codes and Census county codes into consolidated FIPS namespaces (#52)
- Replaced non-breaking spaces in OmniClass facility codes (#133)
- Added GENC alpha-2 and numeric country codes (#94)

### Harmonization and QA

- Added new nc:PersonContactInformation element to nc:PersonType (#29)
- Added substitution groups for street direction codes (#65)
- Added street category codes and updated directionals (#80)
- Added new nc:ActivityLocation element to nc:ActivityType (#71)
- Added nc:MailingAddress and nc:PhysicalAddress as substitutions for nc:Address (#72)
- Fixed invalid augmentation names (#78)
- Fixed definition of j:PersonSignature (#92)
- Fixed spelling errors and added local terminology (#131) - *in progress*
- Fixed definition formatting (#132) - *in progress*
- Harmonized warrant components in Justice and Screening (#62)
- Harmonized biom:ImageType (#99)
- Merged scr:PersonNameAugmentation and scr:PersonNameTextAugmentation (#77)
- Moved nc:PleaCategoryCodeType to the Justice domain (#24)
- Moved additional Justice-specific types from Core to Justice (#79)
- Moved j:ItemMakeAbstract to Core (#95)
- Moved nc:EffectiveDate from screening augmentation to nc:PersonNameType (#96)
- Updated inconsistent code set folder paths, file names, and target namespaces (#58)
- Updated country and state element class terms (#67)
- Used nc:CountryType instead of custom substitution groups for citizenship and nationality elements (#93)

### Release package updates

- Changed the character encoding of the XML schemas from "US-ASCII" to "UTF-8" for better international support (#125)
- Normalized schema sort orders:
  - Sorted namespace prefix declarations by prefix
  - Sorted import statements by target namespace
  - Sorted local terminology by term
  - Sorted type union members by qname
  - Sorted metadata appliesTo values by qname
  - Sorted components using case-insensitive order, with spaces sorting above other characters
  - Sorted facets by style (alphabetically with the exception of sorting min facets before max facets), value, and definition
- Updated target namespaces and dependencies for 5.0.
