
# NIEM 4.2

This is the NIEM 4.2 minor release.

As a minor release, domains and domain code tables may be updated as needed.  Core, all Core code tables, and the NIEM architecture will remain locked until the next major release, NIEM 5.0.

NIEM 4.2 conforms to the [ReferenceSchemaDocument (REF)](https://reference.niem.gov/niem/specification/naming-and-design-rules/4.0/niem-ndr-4.0.html#section_4.1.1) target of the NIEM [Naming and Design Rules (NDR)](https://reference.niem.gov/niem/specification/naming-and-design-rules/4.0/niem-ndr-4.0.html) Specification, version 4.0.

## Key changes

The following is a summary of the content changes made in this release.

Please review the [NIEM Releases issue tracker](https://github.com/NIEM/NIEM-Releases/issues?page=1&q=is%3Aissue+label%3A4.2+is%3Aclosed) or the change log spreadsheet in the release package for a detailed list of changes.

### Domain changes

Content changes have been provided by the following domains:

- **Biometrics**: Added and updated DNA and pedigree components [(#43)](https://github.com/NIEM/NIEM-Releases/issues/43)
- **Emergency Management**: Added new components to support the Public Health Emergency Operations Center (PH EOC) Minimum Data Set [(#42)](https://github.com/NIEM/NIEM-Releases/issues/42)
- **Justice**:
  - Updated FBI NDEx codes [(#39)](https://github.com/NIEM/NIEM-Releases/issues/39)
  - Updated FBI UCR codes [(#59)](https://github.com/NIEM/NIEM-Releases/issues/59)
  - Updated FBI NCIC codes [(#63)](https://github.com/NIEM/NIEM-Releases/issues/63)
  - Removed FBI NIBRS namespace [(#60)](https://github.com/NIEM/NIEM-Releases/issues/60)
  - Removed FBI CJIS namespace [(#68)](https://github.com/NIEM/NIEM-Releases/issues/68)

In addition to the changes listed above, most domains have been updated because of cross-domain dependencies.

### Core Supplement 4.0.2

Core Supplements are additional schemas used to publish additive changes to Core between major release.  For 5.0, these supplemental changes will be merged back into the regular Core and Core code table namespaces.

- Updated Core-dependent code tables [(#35)](https://github.com/NIEM/NIEM-Releases/issues/35)
  - Census county codes [(#45)](https://github.com/NIEM/NIEM-Releases/issues/45)
  - Census / DOT commodity codes [(#48)](https://github.com/NIEM/NIEM-Releases/issues/48)
  - DEA drug codes [(#49)](https://github.com/NIEM/NIEM-Releases/issues/49)
  - Dept of Labor occupation codes [(#50)](https://github.com/NIEM/NIEM-Releases/issues/50)
  - Census FIPS state codes [(#51)](https://github.com/NIEM/NIEM-Releases/issues/51)
  - HazMat codes [(#53)](https://github.com/NIEM/NIEM-Releases/issues/53)
  - HL7 FHIR religion codes [(#54)](https://github.com/NIEM/NIEM-Releases/issues/54)
  - ISO 4217 currency codes [(#55)](https://github.com/NIEM/NIEM-Releases/issues/55)
  - ISO 639-3 language codes [(#56)](https://github.com/NIEM/NIEM-Releases/issues/56)
  - OmniClass facility codes [(#57)](https://github.com/NIEM/NIEM-Releases/issues/57)
- Merged Census county and FIPS 5-2 code namespaces into a new Census FIPS namespace for state and county codes [(#52)](https://github.com/NIEM/NIEM-Releases/issues/52)
- Updated GENC Code Lists CSVs to version 3-10 [(#30)](https://github.com/NIEM/NIEM-Releases/issues/30)
- Added GENC 3-10 country and country subdivision XML schema enumerations [(#66)](https://github.com/NIEM/NIEM-Releases/issues/66)

### Harmonization and other updates

- Harmonized physical feature elements between Biometrics and Core [(#28)](https://github.com/NIEM/NIEM-Releases/issues/28)
- Fixed wording of several Immigration element definitions [(#31)](https://github.com/NIEM/NIEM-Releases/issues/31)
- Harmonized organization name element between Emergency Management and Core [(#33)](https://github.com/NIEM/NIEM-Releases/issues/33)
- Added a Biometrics person augmentation to provide easy access to biometric information from nc:PersonType [(#34)](https://github.com/NIEM/NIEM-Releases/issues/34)
- Harmonized nibrs and ucr CriminalActivityCategoryCodeType code sets [(#36)](https://github.com/NIEM/NIEM-Releases/issues/36)
- Harmonized nibrs and ucr LocationCategoryCodeType code sets [(#37)](https://github.com/NIEM/NIEM-Releases/issues/37)
- Updated Justice elements of type ncic:CountryCodeType [(#38)](https://github.com/NIEM/NIEM-Releases/issues/38)
- Refactored fingerprint classification codes in Biometrics and Justice [(#40)](https://github.com/NIEM/NIEM-Releases/issues/40)
- Added a Justice element for type ucr:PersonAgeCodeType [(#44)](https://github.com/NIEM/NIEM-Releases/issues/44)

### Release package updates

- Fixed broken adapter type links in the documentation spreadsheet [(#18)](https://github.com/NIEM/NIEM-Releases/issues/18)
- Added issue links to the change log spreadsheet [(#69)](https://github.com/NIEM/NIEM-Releases/issues/69)
