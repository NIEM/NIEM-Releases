
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

### Code Tables

- Merged FIPS 5-2 state codes and Census county codes into consolidated FIPS namespaces (#52)

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
