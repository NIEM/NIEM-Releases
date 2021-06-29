
# NIEM Justice Domain Update 5.0.1

This is a domain update sponsored by the Justice domain for the NIEM 5.0 major release.  This update adds back NCIC code sets ([#211](https://github.com/NIEM/NIEM-Releases/issues/211)) that were intentionally removed from the 5.0 release as part of a large harmonization effort across FBI and Justice domain codes.  These code sets are being provided once again for legacy support.

This domain update creates a new code namespace (`ncic-5.0.1`), which can be added to 5.0 subsets and used in IEPDs in addition to the primary [ncic](https://raw.githubusercontent.com/NIEM/NIEM-Releases/niem-5.0/xsd/codes/ncic.xsd) code namespace that was published in the NIEM 5.0 release.  The codes in this `ncic-5.0.1` namespace will be merged back into the main NCIC namespace for the NIEM 5.1 minor release.

The new namespace defines 15 properties, 13 complex types with simple content, 13 simple types, and 450 codes.

Element | Type | Substitution Group
--- | --- | ---
ncic-5.0.1:CountryCode | ncic-5.0.1:CountryCodeType | nc:CountryRepresentation
ncic-5.0.1:EngineDisplacementUnitNCICCode | ncic-5.0.1:VehicleEPDCodeType | nc:VolumeUnitAbstract
ncic-5.0.1:JewelryGenderCode | ncic-5.0.1:SEXCodeType | j:JewelryGenderAbstract
ncic-5.0.1:PersonBirthplaceCode | ncic-5.0.1:CountryCodeType | j:PersonBirthplaceAbstract
ncic-5.0.1:PersonBloodTypeCode | ncic-5.0.1:BLTCodeType | nc:PersonBloodTypeAbstract
ncic-5.0.1:PersonEthnicityNCICCode | ncic-5.0.1:ETNCodeType | nc:PersonEthnicityAbstract
ncic-5.0.1:PersonEyeColorCode | ncic-5.0.1:EYECodeType | nc:PersonEyeColorAbstract
ncic-5.0.1:PersonHairColorCode | ncic-5.0.1:HAIRCodeType | nc:PersonHairColorAbstract
ncic-5.0.1:PersonRaceCode | ncic-5.0.1:RACECodeType | nc:PersonRaceAbstract
ncic-5.0.1:PersonSexCode | ncic-5.0.1:SEXCodeType | nc:PersonSexAbstract
ncic-5.0.1:PersonSkinToneCode | ncic-5.0.1:SKINCodeType | nc:PersonSkinToneAbstract
ncic-5.0.1:StateCanadianProvinceCode | ncic-5.0.1:CanadianCodeType | nc:StateRepresentation
ncic-5.0.1:StateUSCode | ncic-5.0.1:UnitedStatesCodeType | nc:StateRepresentation
ncic-5.0.1:StateUSTerritoriesCode | ncic-5.0.1:USTerritoriesCodeType | nc:StateRepresentation
ncic-5.0.1:VictimToSubjectRelationshipNCICCode | ncic-5.0.1:ROVCodeType | j:VictimToSubjectRelationshipAbstract

Please see the [niem-ncic-5.0.1-codes.xlsx](xlsx/niem-ncic-5.0.1-codes.xlsx) spreadsheet for both the original NCIC 5.0 codes and the NCIC 5.0.1 codes.
