
# NIEM 4.1

This is the NIEM 4.1 release.

## What is a minor release?

NIEM 4.1 is a minor release, which allows domains to update their content as needed.  Core, all namespaces that Core imports, and the architecture will remain locked until the next major release, NIEM 5.0.

## Content changes

The following is a summary of the content changes made in this release.  Please review the change log spreadsheet for a detailed list.

### Domain changes

Content changes have been provided by the following domains:

- Biometrics
- Emergency Management
- Human Services
- Justice
- Military Operations

In addition to those listed above, most domains have been updated because of cross-domain dependencies.

### Issue resolutions

The following domain-related issues from the [issue tracker](https://github.com/NIEM/NIEM-Releases/issues) have been addressed:

- Remove references to "cyfs" from Human Services definitions ([#4](https://github.com/NIEM/NIEM-Releases/issues/4))
- Add keyword "GVWR" to nc:VehicleMaximumLoadWeightMeasure ([#10](https://github.com/NIEM/NIEM-Releases/issues/10))
- Fix type of element mo:MGRSUTM100000MeterCoordinateValue ([#11](https://github.com/NIEM/NIEM-Releases/issues/11))
- Fix special characters in definitions ([#14](https://github.com/NIEM/NIEM-Releases/issues/14))

### Core Supplement 4.0.1

Core Supplement 4.0.1 is being published concurrently with the 4.1 release.  This  provides bug fixes for Core content in a separate schema that can be used along with the existing Core 4.0 schema.

The Core Supplement schema may be found bundled with the other schemas in the subdirectory:

```
niem/niem-core/4.0/1/niem-core.xsd
```

This schema is in subdirectory "1" under the path for Core, identifying it as the first supplement to that namespace.

**Issue resolutions**:

The following core-related issues from the [issue tracker](https://github.com/NIEM/NIEM-Releases/issues) have been addressed in the Core Supplement:

- Create a polygon node element of type nc:LocationType ([#9](https://github.com/NIEM/NIEM-Releases/issues/9))
- nc:LocationHeightMeasureType should extend nc:LengthMeasureType instead of nc:MeasureType ([#13](https://github.com/NIEM/NIEM-Releases/issues/13))
