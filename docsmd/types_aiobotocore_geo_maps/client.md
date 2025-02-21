# LocationServiceMapsV2Client

> [Index](../README.md) > [LocationServiceMapsV2](./README.md) > LocationServiceMapsV2Client

!!! note ""

    Auto-generated documentation for [LocationServiceMapsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#locationservicemapsv2)
    type annotations stubs module [types-aiobotocore-geo-maps](https://pypi.org/project/types-aiobotocore-geo-maps/).

## LocationServiceMapsV2Client

Type annotations and code completion for `#!python session.create_client("geo-maps")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#LocationServiceMapsV2.Client)

```python
# LocationServiceMapsV2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_geo_maps.client import LocationServiceMapsV2Client

session = get_session()
async with session.create_client("geo-maps") as client:
    client: LocationServiceMapsV2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("geo-maps").exceptions` structure.

```python
# LocationServiceMapsV2Client.exceptions usage example

async with session.create_client("geo-maps") as client:
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
# LocationServiceMapsV2Client usage type checking example

from types_aiobotocore_geo_maps.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("geo-maps").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("geo-maps").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps/client/generate_presigned_url.html)

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


### get\_glyphs

Returns the map's glyphs.

Type annotations and code completion for `#!python session.create_client("geo-maps").get_glyphs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps/client/get_glyphs.html)

```python
# get_glyphs method definition

await def get_glyphs(
    self,
    *,
    FontStack: str,
    FontUnicodeRange: str,
) -> GetGlyphsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGlyphsResponseTypeDef](./type_defs.md#getglyphsresponsetypedef) 


```python
# get_glyphs method usage example with argument unpacking

kwargs: GetGlyphsRequestTypeDef = {  # (1)
    "FontStack": ...,
    "FontUnicodeRange": ...,
}

parent.get_glyphs(**kwargs)
```

1. See [:material-code-braces: GetGlyphsRequestTypeDef](./type_defs.md#getglyphsrequesttypedef) 

### get\_sprites

Returns the map's sprites.

Type annotations and code completion for `#!python session.create_client("geo-maps").get_sprites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps/client/get_sprites.html)

```python
# get_sprites method definition

await def get_sprites(
    self,
    *,
    FileName: str,
    Style: MapStyleType,  # (1)
    ColorScheme: ColorSchemeType,  # (2)
    Variant: VariantType,  # (3)
) -> GetSpritesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MapStyleType](./literals.md#mapstyletype) 
2. See [:material-code-brackets: ColorSchemeType](./literals.md#colorschemetype) 
3. See [:material-code-brackets: VariantType](./literals.md#varianttype) 
4. See [:material-code-braces: GetSpritesResponseTypeDef](./type_defs.md#getspritesresponsetypedef) 


```python
# get_sprites method usage example with argument unpacking

kwargs: GetSpritesRequestTypeDef = {  # (1)
    "FileName": ...,
    "Style": ...,
    "ColorScheme": ...,
    "Variant": ...,
}

parent.get_sprites(**kwargs)
```

1. See [:material-code-braces: GetSpritesRequestTypeDef](./type_defs.md#getspritesrequesttypedef) 

### get\_static\_map

Provides high-quality static map images with customizable options.

Type annotations and code completion for `#!python session.create_client("geo-maps").get_static_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps/client/get_static_map.html)

```python
# get_static_map method definition

await def get_static_map(
    self,
    *,
    Height: int,
    FileName: str,
    Width: int,
    BoundingBox: str = ...,
    BoundedPositions: str = ...,
    Center: str = ...,
    CompactOverlay: str = ...,
    GeoJsonOverlay: str = ...,
    Key: str = ...,
    Padding: int = ...,
    Radius: int = ...,
    ScaleBarUnit: ScaleBarUnitType = ...,  # (1)
    Style: StaticMapStyleType = ...,  # (2)
    Zoom: float = ...,
) -> GetStaticMapResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScaleBarUnitType](./literals.md#scalebarunittype) 
2. See [:material-code-brackets: StaticMapStyleType](./literals.md#staticmapstyletype) 
3. See [:material-code-braces: GetStaticMapResponseTypeDef](./type_defs.md#getstaticmapresponsetypedef) 


```python
# get_static_map method usage example with argument unpacking

kwargs: GetStaticMapRequestTypeDef = {  # (1)
    "Height": ...,
    "FileName": ...,
    "Width": ...,
}

parent.get_static_map(**kwargs)
```

1. See [:material-code-braces: GetStaticMapRequestTypeDef](./type_defs.md#getstaticmaprequesttypedef) 

### get\_style\_descriptor

Returns information about the style.

Type annotations and code completion for `#!python session.create_client("geo-maps").get_style_descriptor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps/client/get_style_descriptor.html)

```python
# get_style_descriptor method definition

await def get_style_descriptor(
    self,
    *,
    Style: MapStyleType,  # (1)
    ColorScheme: ColorSchemeType = ...,  # (2)
    PoliticalView: str = ...,
    Key: str = ...,
) -> GetStyleDescriptorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MapStyleType](./literals.md#mapstyletype) 
2. See [:material-code-brackets: ColorSchemeType](./literals.md#colorschemetype) 
3. See [:material-code-braces: GetStyleDescriptorResponseTypeDef](./type_defs.md#getstyledescriptorresponsetypedef) 


```python
# get_style_descriptor method usage example with argument unpacking

kwargs: GetStyleDescriptorRequestTypeDef = {  # (1)
    "Style": ...,
}

parent.get_style_descriptor(**kwargs)
```

1. See [:material-code-braces: GetStyleDescriptorRequestTypeDef](./type_defs.md#getstyledescriptorrequesttypedef) 

### get\_tile

Returns a tile.

Type annotations and code completion for `#!python session.create_client("geo-maps").get_tile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps/client/get_tile.html)

```python
# get_tile method definition

await def get_tile(
    self,
    *,
    Tileset: str,
    Z: str,
    X: str,
    Y: str,
    Key: str = ...,
) -> GetTileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTileResponseTypeDef](./type_defs.md#gettileresponsetypedef) 


```python
# get_tile method usage example with argument unpacking

kwargs: GetTileRequestTypeDef = {  # (1)
    "Tileset": ...,
    "Z": ...,
    "X": ...,
    "Y": ...,
}

parent.get_tile(**kwargs)
```

1. See [:material-code-braces: GetTileRequestTypeDef](./type_defs.md#gettilerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("geo-maps").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#LocationServiceMapsV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("geo-maps").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#LocationServiceMapsV2.Client)

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





