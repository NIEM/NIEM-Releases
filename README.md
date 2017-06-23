
# NIEM 4.0

This is the NIEM 4.0 release.

This release reflects updates to the [NIEM Naming and Design Rules][NDR], as well
as the new [NIEM Code Lists Specification][Code Lists Specification].

## NDR 4.0

This release of NIEM reflects updates to the
[NIEM Naming and Design Rules][NDR], including:

- The structures schema incorporates a new attribute, uri, that supports
  cross-document and within-document references, in the style of Linked Data.
- The vocabulary for local terminology, formerly in its own namespace, has been
  moved into the appinfo namespace.
- Abstract elements now have names that end in "Abstract", other than
  augmentation points and representation elements

## Code Lists Specification 4.0

This release reflects the new [Code Lists Specification], including:

- NIEM Core contains a new type, `nc:CodeType`, which supports code lists that
  are identified at run time, including GENC (see below).
- The release contains codes for countries and subdivisions (e.g., states) that
  are provided as CSV spreadsheet files. See below for more info.

## Content

### Domains with new or updated content

- **Agriculture** (*new domain in NIEM 4.0*)
- **Biometrics**
- **Emergency Management**
- **Human Services**
  - content adopted from the former CYFS domain
- **Justice**
- **Military Operations**
- **Surface Transportation**

Note: All domains have been changed, to some degree. The list above shows
domains with additional changes beyond the regular updates to move to the 4.0
major release, apply harmonization changes, etc.

### Support for the international community

- Added **address codes**
- Added **nc:Crisis**
- Added **nc:DocumentEUDataPrivacyIndicator** to nc:DocumentType
- Added **message** elements to support message references and FATCA information
- Added **nc:ServiceDeliveryNGO** and **nc:CoordinatingAgency** organizations
- Added **nc:Payment**
- Added **nc:PublicService**
- Promoted **FinancialAccount** from the Justice domain to Core and added additional content
- Reviewed Core definitions to remove unnecessary US-specific terms

### Harmonization and issue resolution

Core-related changes include:

- Refactored **measures**
  - Created measure subtypes so that only the appropriate unit codes are available in each type
  - For example, length unit codes are now available on nc:LengthMeasureType, not nc:MeasureType itself
- Updated the representations of **GENC** codes
  - Codes for countries and administrative subdivisions (e.g., states,
    provinces) are represented according to the new [Code Lists Specification]
  - Example usage:

    ```xml
    <nc:CountryCode
      cli:codeListURI="http://api.nsgreg.nga.mil/geo-political/GENC/3/3-6"
      cli:codeListColumnName="char3">USA</nc:CountryCode>
    ```

  - The URI `http://api.nsgreg.nga.mil/geo-political/GENC/3/3-6` is resolved by
    [niem/xml-catalog.xml](niem/xml-catalog.xml) to the CSV spreadsheet
    [niem/codes/genc/geo-political/3-6/genc_geo-political_3-6_char3.csv](niem/codes/genc/geo-political/3-6/genc_geo-political_3-6_char3.csv). The
    code value `USA` appears in the spreadsheet's column headed `char3`.
  - See `niem/codes/genc/` for GENC CSV code sets provided with this release
  - See the [Code Lists Specification] for examples, more details, and how to build and use new CSVs for updated GENC codes
- Added **nc:ArrivalType** and **nc:DepartureType**
- Added / promoted additional  representations for **nc:DateType**:
  - Fiscal year
  - Quarter
  - Zulu date/time
  - Month
  - Day
  - Date ranges
- Added **nc:BinaryHash** to nc:BinaryType
- Added **nc:CountryType** and **nc:StateType**
  - Bundles multiple representations of country and state codes to allow for easier reuse
- Added additional **entity** representations
  - **nc:EntityItem**
  - **nc:GenericEntity**
    - simple name, contact info, description fields
    - for use when an entity cannot be determined to be either a person or an organization
- Added **nc:LocationFloorNumberText**
- Added **nc:OrganizationLEIIdentification**
- Added **nc:RecommendationType**
- Added **nc:TelephoneNumberDescriptionText**
- Harmonized **capability** content
- Harmonized **equipment** content
- Harmonized **hazmat** code and text elements
- Harmonized **medical condition** content
- Harmonized **mission** content
- Harmonized **permit** content
- Harmonized **PersonStolenIdentityAssociation**
- Harmonized **request** content
- Harmonized **SubjectCautionInformation** content
- Harmonized **task** content
- Moved **AnomalyType** from Maritime to Core
- Moved **CourtCase** to Core
- Moved **MGRS** (Military Grid Reference System) coordinates from Core to MilOps
- Moved **MissionID** to nc:MissionType
- Moved **OrientationType** from MilOps to Core
- Removed the **core_misc** namespace
  - Moved the existing code sets into Core
- Removed **FIPS 5-2 state** alpha codes
  - FIPS 5-2 reuses USPS state alpha code
- Removed the **FIPS 10-4** namespace (deprecated country codes)
- Removed **nc:ContactInformationAssociationType**
  - Largely overlapped nc:ContactInformationType
- Updated **nc:AngularDegreeValue** from an integer to a decimal data type
- Updated **nc:ElectronicAddressType**
- Updated **nc:PersonNationality** to correct the definition
- Updated **nc:RelativeLocationDistanceText** to a measure
- Updated **nc:ReliabilityPercent** as nc:ConfidencePercent
- Updated **nc:UTMCoordinateType** to fix the representation so it follows the common pattern
- Updated the representation of **percent** values
  - Percents should now be represented as a decimal value, with **100% represented as "100"**.
  - Values less than 0 and greater than 100 are now allowed.

### Miscellaneous
- Incorporated all 3.0-related Core Supplements
- Moved supporting schemas into a new `utility` folder to simplify the release folder layout:
  - appinfo
  - code-lists-spec
  - conformanceTargets
  - structures


[Code Lists Specification]: https://github.com/NIEM/NIEM-Code-Lists-Spec
[NDR]: https://github.com/NIEM/NIEM-NDR
