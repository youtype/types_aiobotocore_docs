# LocationServicePlacesV2 module

> [Index](../README.md) > LocationServicePlacesV2


!!! note ""

    Auto-generated documentation for [LocationServicePlacesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#locationserviceplacesv2)
    type annotations stubs module [types-aiobotocore-geo-places](https://pypi.org/project/types-aiobotocore-geo-places/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LocationServicePlacesV2` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LocationServicePlacesV2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[geo-places]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[geo-places]'

# standalone installation
python -m pip install types-aiobotocore-geo-places
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-geo-places
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LocationServicePlacesV2Client

Type annotations and code completion for  `#!python session.create_client("geo-places")` as [LocationServicePlacesV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#LocationServicePlacesV2.Client)

```python
# LocationServicePlacesV2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_geo_places.client import LocationServicePlacesV2Client


session = get_session()
async with session.create_client("geo-places") as client:
    client: LocationServicePlacesV2Client
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutocompleteAdditionalFeatureType usage example

from types_aiobotocore_geo_places.literals import AutocompleteAdditionalFeatureType

def get_value() -> AutocompleteAdditionalFeatureType:
    return "Core"
```

- [AutocompleteAdditionalFeatureType](./literals.md#autocompleteadditionalfeaturetype)
- [AutocompleteFilterPlaceTypeType](./literals.md#autocompletefilterplacetypetype)
- [AutocompleteIntendedUseType](./literals.md#autocompleteintendedusetype)
- [GeocodeAdditionalFeatureType](./literals.md#geocodeadditionalfeaturetype)
- [GeocodeFilterPlaceTypeType](./literals.md#geocodefilterplacetypetype)
- [GeocodeIntendedUseType](./literals.md#geocodeintendedusetype)
- [GetPlaceAdditionalFeatureType](./literals.md#getplaceadditionalfeaturetype)
- [GetPlaceIntendedUseType](./literals.md#getplaceintendedusetype)
- [PlaceTypeType](./literals.md#placetypetype)
- [PostalAuthorityType](./literals.md#postalauthoritytype)
- [PostalCodeModeType](./literals.md#postalcodemodetype)
- [PostalCodeTypeType](./literals.md#postalcodetypetype)
- [QueryTypeType](./literals.md#querytypetype)
- [RecordTypeCodeType](./literals.md#recordtypecodetype)
- [ReverseGeocodeAdditionalFeatureType](./literals.md#reversegeocodeadditionalfeaturetype)
- [ReverseGeocodeFilterPlaceTypeType](./literals.md#reversegeocodefilterplacetypetype)
- [ReverseGeocodeIntendedUseType](./literals.md#reversegeocodeintendedusetype)
- [SearchNearbyAdditionalFeatureType](./literals.md#searchnearbyadditionalfeaturetype)
- [SearchNearbyIntendedUseType](./literals.md#searchnearbyintendedusetype)
- [SearchTextAdditionalFeatureType](./literals.md#searchtextadditionalfeaturetype)
- [SearchTextIntendedUseType](./literals.md#searchtextintendedusetype)
- [SuggestAdditionalFeatureType](./literals.md#suggestadditionalfeaturetype)
- [SuggestIntendedUseType](./literals.md#suggestintendedusetype)
- [SuggestResultItemTypeType](./literals.md#suggestresultitemtypetype)
- [TypePlacementType](./literals.md#typeplacementtype)
- [ZipClassificationCodeType](./literals.md#zipclassificationcodetype)
- [LocationServicePlacesV2ServiceName](./literals.md#locationserviceplacesv2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessPointTypeDef](./type_defs.md#accesspointtypedef)
- [CategoryTypeDef](./type_defs.md#categorytypedef)
- [SecondaryAddressComponentMatchScoreTypeDef](./type_defs.md#secondaryaddresscomponentmatchscoretypedef)
- [PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef)
- [CountryTypeDef](./type_defs.md#countrytypedef)
- [RegionTypeDef](./type_defs.md#regiontypedef)
- [SecondaryAddressComponentTypeDef](./type_defs.md#secondaryaddresscomponenttypedef)
- [StreetComponentsTypeDef](./type_defs.md#streetcomponentstypedef)
- [SubRegionTypeDef](./type_defs.md#subregiontypedef)
- [HighlightTypeDef](./type_defs.md#highlighttypedef)
- [FilterCircleTypeDef](./type_defs.md#filtercircletypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BusinessChainTypeDef](./type_defs.md#businesschaintypedef)
- [FoodTypeTypeDef](./type_defs.md#foodtypetypedef)
- [GeocodeFilterTypeDef](./type_defs.md#geocodefiltertypedef)
- [ParsedQueryComponentTypeDef](./type_defs.md#parsedquerycomponenttypedef)
- [ParsedQuerySecondaryAddressComponentTypeDef](./type_defs.md#parsedquerysecondaryaddresscomponenttypedef)
- [GeocodeQueryComponentsTypeDef](./type_defs.md#geocodequerycomponentstypedef)
- [TimeZoneTypeDef](./type_defs.md#timezonetypedef)
- [GetPlaceRequestTypeDef](./type_defs.md#getplacerequesttypedef)
- [OpeningHoursComponentsTypeDef](./type_defs.md#openinghourscomponentstypedef)
- [UspsZipPlus4TypeDef](./type_defs.md#uspszipplus4typedef)
- [UspsZipTypeDef](./type_defs.md#uspsziptypedef)
- [QueryRefinementTypeDef](./type_defs.md#queryrefinementtypedef)
- [ReverseGeocodeFilterTypeDef](./type_defs.md#reversegeocodefiltertypedef)
- [SearchNearbyFilterTypeDef](./type_defs.md#searchnearbyfiltertypedef)
- [SuggestQueryResultTypeDef](./type_defs.md#suggestqueryresulttypedef)
- [AccessRestrictionTypeDef](./type_defs.md#accessrestrictiontypedef)
- [ContactDetailsTypeDef](./type_defs.md#contactdetailstypedef)
- [AddressComponentMatchScoresTypeDef](./type_defs.md#addresscomponentmatchscorestypedef)
- [AddressComponentPhonemesTypeDef](./type_defs.md#addresscomponentphonemestypedef)
- [AddressTypeDef](./type_defs.md#addresstypedef)
- [CountryHighlightsTypeDef](./type_defs.md#countryhighlightstypedef)
- [RegionHighlightsTypeDef](./type_defs.md#regionhighlightstypedef)
- [SubRegionHighlightsTypeDef](./type_defs.md#subregionhighlightstypedef)
- [SuggestAddressHighlightsTypeDef](./type_defs.md#suggestaddresshighlightstypedef)
- [AutocompleteFilterTypeDef](./type_defs.md#autocompletefiltertypedef)
- [SearchTextFilterTypeDef](./type_defs.md#searchtextfiltertypedef)
- [SuggestFilterTypeDef](./type_defs.md#suggestfiltertypedef)
- [GeocodeParsedQueryAddressComponentsTypeDef](./type_defs.md#geocodeparsedqueryaddresscomponentstypedef)
- [GeocodeRequestTypeDef](./type_defs.md#geocoderequesttypedef)
- [OpeningHoursTypeDef](./type_defs.md#openinghourstypedef)
- [PostalCodeDetailsTypeDef](./type_defs.md#postalcodedetailstypedef)
- [ReverseGeocodeRequestTypeDef](./type_defs.md#reversegeocoderequesttypedef)
- [SearchNearbyRequestTypeDef](./type_defs.md#searchnearbyrequesttypedef)
- [ContactsTypeDef](./type_defs.md#contactstypedef)
- [ComponentMatchScoresTypeDef](./type_defs.md#componentmatchscorestypedef)
- [PhonemeDetailsTypeDef](./type_defs.md#phonemedetailstypedef)
- [IntersectionTypeDef](./type_defs.md#intersectiontypedef)
- [RelatedPlaceTypeDef](./type_defs.md#relatedplacetypedef)
- [AutocompleteAddressHighlightsTypeDef](./type_defs.md#autocompleteaddresshighlightstypedef)
- [SuggestHighlightsTypeDef](./type_defs.md#suggesthighlightstypedef)
- [AutocompleteRequestTypeDef](./type_defs.md#autocompleterequesttypedef)
- [SearchTextRequestTypeDef](./type_defs.md#searchtextrequesttypedef)
- [SuggestRequestTypeDef](./type_defs.md#suggestrequesttypedef)
- [GeocodeParsedQueryTypeDef](./type_defs.md#geocodeparsedquerytypedef)
- [MatchScoreDetailsTypeDef](./type_defs.md#matchscoredetailstypedef)
- [SearchNearbyResultItemTypeDef](./type_defs.md#searchnearbyresultitemtypedef)
- [SearchTextResultItemTypeDef](./type_defs.md#searchtextresultitemtypedef)
- [SuggestPlaceResultTypeDef](./type_defs.md#suggestplaceresulttypedef)
- [ReverseGeocodeResultItemTypeDef](./type_defs.md#reversegeocoderesultitemtypedef)
- [GetPlaceResponseTypeDef](./type_defs.md#getplaceresponsetypedef)
- [AutocompleteHighlightsTypeDef](./type_defs.md#autocompletehighlightstypedef)
- [GeocodeResultItemTypeDef](./type_defs.md#geocoderesultitemtypedef)
- [SearchNearbyResponseTypeDef](./type_defs.md#searchnearbyresponsetypedef)
- [SearchTextResponseTypeDef](./type_defs.md#searchtextresponsetypedef)
- [SuggestResultItemTypeDef](./type_defs.md#suggestresultitemtypedef)
- [ReverseGeocodeResponseTypeDef](./type_defs.md#reversegeocoderesponsetypedef)
- [AutocompleteResultItemTypeDef](./type_defs.md#autocompleteresultitemtypedef)
- [GeocodeResponseTypeDef](./type_defs.md#geocoderesponsetypedef)
- [SuggestResponseTypeDef](./type_defs.md#suggestresponsetypedef)
- [AutocompleteResponseTypeDef](./type_defs.md#autocompleteresponsetypedef)

