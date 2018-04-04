
# NIEM 4.1

This is the NIEM 4.1 beta 1 pre-release.

NIEM 4.1 will be a minor release and is scheduled to be published Summer 2018.

The full beta release package may be downloaded from the [NIEM Releases repository on GitHub](https://github.com/NIEM/NIEM-Releases/tree/niem-4.1beta1) as a zip file by clicking on the green "Clone or download" button and then clicking "Download ZIP", or by downloading the package from the traditional release site at  https://release.niem.gov/niem/4.1/niem-4.1beta1.zip.

## Minor release

In a minor release, domains may update their content as needed.

Core and all namespaces imported by Core are locked until the next major release (NIEM 5.0). A core supplement may be published as an interim solution, with changes published in newly created schemas.

The NIEM architecture also remains locked in minor releases. Only additive changes that do not affect Core are permitted.

## Content changes

### Domain changes

Content changes have been made in the following domains:

- Biometrics
- Emergency Management
- Human Services
- Justice
- Military Operations

Most domains have been updated because of cross-domain dependencies.

**Issue resolutions**:

The following domain-related issues from the [issue tracker](https://github.com/NIEM/NIEM-Releases/issues) have been addressed:

- Remove references to "cyfs" from Human Services definitions ([#4](https://github.com/NIEM/NIEM-Releases/issues/4))
- Add keyword "GVWR" to nc:VehicleMaximumLoadWeightMeasure ([#10](https://github.com/NIEM/NIEM-Releases/issues/10))
- Fix type of element mo:MGRSUTM100000MeterCoordinateValue ([#11](https://github.com/NIEM/NIEM-Releases/issues/11))

### Core Supplement 4.0.1

Core Supplement 4.0.1 will be published concurrently with the 4.1 release.  This will provide bug fixes for Core content in a separate schema that can be used along with the existing Core 4.0 schema.  Learn more about Core Supplements at [niem.github.io](http://niem.github.io/normative-rules-guidelines/core-supplement/).

The Core Supplement schema may be found bundled with the other schemas at `niem/niem-core/4.0/1/niem-core.xsd` or by [clicking here](https://github.com/NIEM/NIEM-Releases/tree/niem-4.1beta1/niem/niem-core/4.0/1/niem-core.xsd).

**Issue resolutions**:

The following core-related issues from the [issue tracker](https://github.com/NIEM/NIEM-Releases/issues) have been addressed in the Core Supplement:

- Create a polygon node element of type nc:LocationType ([#9](https://github.com/NIEM/NIEM-Releases/issues/9))
- nc:LocationHeightMeasureType should extend nc:LengthMeasureType instead of nc:MeasureType ([#13](https://github.com/NIEM/NIEM-Releases/issues/13))

## SSGT

The SSGT is available for testing purposes to search, explore, and build XML Schema subsets with the 4.1 beta1 release.  It is available [here](https://tools.niem.gov/niemtools-4.1beta1/ssgt/index.iepd).

Please note that this is the development version of the tool and thus may run more slowly than the regular production version.

## Feedback

Please submit feedback by Friday, April 20, 2018.

Feedback may be submitted by either creating a [new issue](https://github.com/NIEM/NIEM-Releases/issues) or by emailing niem-comments@lists.gatech.edu.
