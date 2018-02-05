
# NIEM 4.1

This is the NIEM 4.1 alpha 1 pre-release.

NIEM 4.1 will be a minor release and is scheduled to be published in summer 2018.

## Minor releases

In a minor release, domains may update their content as needed.

Core and all namespaces imported by Core are locked until the next major release (5.0). A core supplement may be published as an interim solution, with changes published in newly created schemas.

The NIEM architecture also remains locked in minor releases. Only additive changes that do not affect are permitted.

## Core Supplement

Because Core is locked until the next major release, a supplemental file can be published to provide access to new or harmonized content in the interim.

Core Supplement 4.0.1 is scheduleded to be published as part of the 4.1 release.  This will provide updates to Core content and code tables in an additive manner, and can be used along side the existing Core 4.0 namespace.

## Content changes

### Domain changes

Content changes have been made in the following domains:

- Biometrics
- Human Services
- Military Operations

Most domains have been updated because of cross-domain dependencies.

### Issue resolution

The following issues from the [issue tracker](https://github.com/NIEM/NIEM-Releases/issues) have been addressed:

- Remove references to "cyfs" from Human Services definitions (#4)
- Create a polygon node element of type nc:LocationType (#9)
- Add keyword "GVWR" to nc:VehicleMaximumLoadWeightMeasure (#10)
- Fix type of element mo:MGRSUTM100000MeterCoordinateValue (#11)

## Feedback

Please submit feedback by Wednesday, February 21.

Feedback may be submitted by either creating a [new issue](https://github.com/NIEM/NIEM-Releases/issues) or by emailing niem-comments@lists.gatech.edu.
