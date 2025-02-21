# LocationServicePlacesV2Client

> [Index](../README.md) > [LocationServicePlacesV2](./README.md) > LocationServicePlacesV2Client

!!! note ""

    Auto-generated documentation for [LocationServicePlacesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#locationserviceplacesv2)
    type annotations stubs module [types-aiobotocore-geo-places](https://pypi.org/project/types-aiobotocore-geo-places/).

## LocationServicePlacesV2Client

Type annotations and code completion for `#!python session.create_client("geo-places")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#LocationServicePlacesV2.Client)

```python
# LocationServicePlacesV2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_geo_places.client import LocationServicePlacesV2Client

session = get_session()
async with session.create_client("geo-places") as client:
    client: LocationServicePlacesV2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("geo-places").exceptions` structure.

```python
# LocationServicePlacesV2Client.exceptions usage example

async with session.create_client("geo-places") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# LocationServicePlacesV2Client usage type checking example

from types_aiobotocore_geo_places.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("geo-places").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("geo-places").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### autocomplete

The autocomplete operation speeds up and increases the accuracy of entering
addresses by providing a list of address candidates matching a partially
entered address.

Type annotations and code completion for `#!python session.create_client("geo-places").autocomplete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/autocomplete.html)

```python
# autocomplete method definition

await def autocomplete(
    self,
    *,
    QueryText: str,
    MaxResults: int = ...,
    BiasPosition: Sequence[float] = ...,
    Filter: AutocompleteFilterTypeDef = ...,  # (1)
    PostalCodeMode: PostalCodeModeType = ...,  # (2)
    AdditionalFeatures: Sequence[AutocompleteAdditionalFeatureType] = ...,  # (3)
    Language: str = ...,
    PoliticalView: str = ...,
    IntendedUse: AutocompleteIntendedUseType = ...,  # (4)
    Key: str = ...,
) -> AutocompleteResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AutocompleteFilterTypeDef](./type_defs.md#autocompletefiltertypedef) 
2. See [:material-code-brackets: PostalCodeModeType](./literals.md#postalcodemodetype) 
3. See [:material-code-brackets: AutocompleteAdditionalFeatureType](./literals.md#autocompleteadditionalfeaturetype) 
4. See [:material-code-brackets: AutocompleteIntendedUseType](./literals.md#autocompleteintendedusetype) 
5. See [:material-code-braces: AutocompleteResponseTypeDef](./type_defs.md#autocompleteresponsetypedef) 


```python
# autocomplete method usage example with argument unpacking

kwargs: AutocompleteRequestTypeDef = {  # (1)
    "QueryText": ...,
}

parent.autocomplete(**kwargs)
```

1. See [:material-code-braces: AutocompleteRequestTypeDef](./type_defs.md#autocompleterequesttypedef) 

### geocode

The <code>Geocode</code> action allows you to obtain coordinates, addresses,
and other information about places.

Type annotations and code completion for `#!python session.create_client("geo-places").geocode` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/geocode.html)

```python
# geocode method definition

await def geocode(
    self,
    *,
    QueryText: str = ...,
    QueryComponents: GeocodeQueryComponentsTypeDef = ...,  # (1)
    MaxResults: int = ...,
    BiasPosition: Sequence[float] = ...,
    Filter: GeocodeFilterTypeDef = ...,  # (2)
    AdditionalFeatures: Sequence[GeocodeAdditionalFeatureType] = ...,  # (3)
    Language: str = ...,
    PoliticalView: str = ...,
    IntendedUse: GeocodeIntendedUseType = ...,  # (4)
    Key: str = ...,
) -> GeocodeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: GeocodeQueryComponentsTypeDef](./type_defs.md#geocodequerycomponentstypedef) 
2. See [:material-code-braces: GeocodeFilterTypeDef](./type_defs.md#geocodefiltertypedef) 
3. See [:material-code-brackets: GeocodeAdditionalFeatureType](./literals.md#geocodeadditionalfeaturetype) 
4. See [:material-code-brackets: GeocodeIntendedUseType](./literals.md#geocodeintendedusetype) 
5. See [:material-code-braces: GeocodeResponseTypeDef](./type_defs.md#geocoderesponsetypedef) 


```python
# geocode method usage example with argument unpacking

kwargs: GeocodeRequestTypeDef = {  # (1)
    "QueryText": ...,
}

parent.geocode(**kwargs)
```

1. See [:material-code-braces: GeocodeRequestTypeDef](./type_defs.md#geocoderequesttypedef) 

### get\_place

Finds a place by its unique ID.

Type annotations and code completion for `#!python session.create_client("geo-places").get_place` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/get_place.html)

```python
# get_place method definition

await def get_place(
    self,
    *,
    PlaceId: str,
    AdditionalFeatures: Sequence[GetPlaceAdditionalFeatureType] = ...,  # (1)
    Language: str = ...,
    PoliticalView: str = ...,
    IntendedUse: GetPlaceIntendedUseType = ...,  # (2)
    Key: str = ...,
) -> GetPlaceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GetPlaceAdditionalFeatureType](./literals.md#getplaceadditionalfeaturetype) 
2. See [:material-code-brackets: GetPlaceIntendedUseType](./literals.md#getplaceintendedusetype) 
3. See [:material-code-braces: GetPlaceResponseTypeDef](./type_defs.md#getplaceresponsetypedef) 


```python
# get_place method usage example with argument unpacking

kwargs: GetPlaceRequestTypeDef = {  # (1)
    "PlaceId": ...,
}

parent.get_place(**kwargs)
```

1. See [:material-code-braces: GetPlaceRequestTypeDef](./type_defs.md#getplacerequesttypedef) 

### reverse\_geocode

The <code>ReverseGeocode</code> operation allows you to retrieve addresses and
place information from coordinates.

Type annotations and code completion for `#!python session.create_client("geo-places").reverse_geocode` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/reverse_geocode.html)

```python
# reverse_geocode method definition

await def reverse_geocode(
    self,
    *,
    QueryPosition: Sequence[float],
    QueryRadius: int = ...,
    MaxResults: int = ...,
    Filter: ReverseGeocodeFilterTypeDef = ...,  # (1)
    AdditionalFeatures: Sequence[ReverseGeocodeAdditionalFeatureType] = ...,  # (2)
    Language: str = ...,
    PoliticalView: str = ...,
    IntendedUse: ReverseGeocodeIntendedUseType = ...,  # (3)
    Key: str = ...,
) -> ReverseGeocodeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ReverseGeocodeFilterTypeDef](./type_defs.md#reversegeocodefiltertypedef) 
2. See [:material-code-brackets: ReverseGeocodeAdditionalFeatureType](./literals.md#reversegeocodeadditionalfeaturetype) 
3. See [:material-code-brackets: ReverseGeocodeIntendedUseType](./literals.md#reversegeocodeintendedusetype) 
4. See [:material-code-braces: ReverseGeocodeResponseTypeDef](./type_defs.md#reversegeocoderesponsetypedef) 


```python
# reverse_geocode method usage example with argument unpacking

kwargs: ReverseGeocodeRequestTypeDef = {  # (1)
    "QueryPosition": ...,
}

parent.reverse_geocode(**kwargs)
```

1. See [:material-code-braces: ReverseGeocodeRequestTypeDef](./type_defs.md#reversegeocoderequesttypedef) 

### search\_nearby

Search nearby a specified location.

Type annotations and code completion for `#!python session.create_client("geo-places").search_nearby` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/search_nearby.html)

```python
# search_nearby method definition

await def search_nearby(
    self,
    *,
    QueryPosition: Sequence[float],
    QueryRadius: int = ...,
    MaxResults: int = ...,
    Filter: SearchNearbyFilterTypeDef = ...,  # (1)
    AdditionalFeatures: Sequence[SearchNearbyAdditionalFeatureType] = ...,  # (2)
    Language: str = ...,
    PoliticalView: str = ...,
    IntendedUse: SearchNearbyIntendedUseType = ...,  # (3)
    NextToken: str = ...,
    Key: str = ...,
) -> SearchNearbyResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SearchNearbyFilterTypeDef](./type_defs.md#searchnearbyfiltertypedef) 
2. See [:material-code-brackets: SearchNearbyAdditionalFeatureType](./literals.md#searchnearbyadditionalfeaturetype) 
3. See [:material-code-brackets: SearchNearbyIntendedUseType](./literals.md#searchnearbyintendedusetype) 
4. See [:material-code-braces: SearchNearbyResponseTypeDef](./type_defs.md#searchnearbyresponsetypedef) 


```python
# search_nearby method usage example with argument unpacking

kwargs: SearchNearbyRequestTypeDef = {  # (1)
    "QueryPosition": ...,
}

parent.search_nearby(**kwargs)
```

1. See [:material-code-braces: SearchNearbyRequestTypeDef](./type_defs.md#searchnearbyrequesttypedef) 

### search\_text

Use the <code>SearchText</code> operation to search for geocode and place
information.

Type annotations and code completion for `#!python session.create_client("geo-places").search_text` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/search_text.html)

```python
# search_text method definition

await def search_text(
    self,
    *,
    QueryText: str = ...,
    QueryId: str = ...,
    MaxResults: int = ...,
    BiasPosition: Sequence[float] = ...,
    Filter: SearchTextFilterTypeDef = ...,  # (1)
    AdditionalFeatures: Sequence[SearchTextAdditionalFeatureType] = ...,  # (2)
    Language: str = ...,
    PoliticalView: str = ...,
    IntendedUse: SearchTextIntendedUseType = ...,  # (3)
    NextToken: str = ...,
    Key: str = ...,
) -> SearchTextResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SearchTextFilterTypeDef](./type_defs.md#searchtextfiltertypedef) 
2. See [:material-code-brackets: SearchTextAdditionalFeatureType](./literals.md#searchtextadditionalfeaturetype) 
3. See [:material-code-brackets: SearchTextIntendedUseType](./literals.md#searchtextintendedusetype) 
4. See [:material-code-braces: SearchTextResponseTypeDef](./type_defs.md#searchtextresponsetypedef) 


```python
# search_text method usage example with argument unpacking

kwargs: SearchTextRequestTypeDef = {  # (1)
    "QueryText": ...,
}

parent.search_text(**kwargs)
```

1. See [:material-code-braces: SearchTextRequestTypeDef](./type_defs.md#searchtextrequesttypedef) 

### suggest

The <code>Suggest</code> operation finds addresses or place candidates based on
incomplete or misspelled queries.

Type annotations and code completion for `#!python session.create_client("geo-places").suggest` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places/client/suggest.html)

```python
# suggest method definition

await def suggest(
    self,
    *,
    QueryText: str,
    MaxResults: int = ...,
    MaxQueryRefinements: int = ...,
    BiasPosition: Sequence[float] = ...,
    Filter: SuggestFilterTypeDef = ...,  # (1)
    AdditionalFeatures: Sequence[SuggestAdditionalFeatureType] = ...,  # (2)
    Language: str = ...,
    PoliticalView: str = ...,
    IntendedUse: SuggestIntendedUseType = ...,  # (3)
    Key: str = ...,
) -> SuggestResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SuggestFilterTypeDef](./type_defs.md#suggestfiltertypedef) 
2. See [:material-code-brackets: SuggestAdditionalFeatureType](./literals.md#suggestadditionalfeaturetype) 
3. See [:material-code-brackets: SuggestIntendedUseType](./literals.md#suggestintendedusetype) 
4. See [:material-code-braces: SuggestResponseTypeDef](./type_defs.md#suggestresponsetypedef) 


```python
# suggest method usage example with argument unpacking

kwargs: SuggestRequestTypeDef = {  # (1)
    "QueryText": ...,
}

parent.suggest(**kwargs)
```

1. See [:material-code-braces: SuggestRequestTypeDef](./type_defs.md#suggestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("geo-places").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#LocationServicePlacesV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("geo-places").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#LocationServicePlacesV2.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





