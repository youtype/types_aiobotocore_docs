# Type definitions

> [Index](../README.md) > [LocationServiceMapsV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LocationServiceMapsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#locationservicemapsv2)
    type annotations stubs module [types-aiobotocore-geo-maps](https://pypi.org/project/types-aiobotocore-geo-maps/).



## GetGlyphsRequestRequestTypeDef

```python
# GetGlyphsRequestRequestTypeDef definition

class GetGlyphsRequestRequestTypeDef(TypedDict):
    FontStack: str,
    FontUnicodeRange: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## GetSpritesRequestRequestTypeDef

```python
# GetSpritesRequestRequestTypeDef definition

class GetSpritesRequestRequestTypeDef(TypedDict):
    FileName: str,
    Style: MapStyleType,  # (1)
    ColorScheme: ColorSchemeType,  # (2)
    Variant: VariantType,  # (3)
```

1. See [:material-code-brackets: MapStyleType](./literals.md#mapstyletype) 
2. See [:material-code-brackets: ColorSchemeType](./literals.md#colorschemetype) 
3. See [:material-code-brackets: VariantType](./literals.md#varianttype) 
## GetStaticMapRequestRequestTypeDef

```python
# GetStaticMapRequestRequestTypeDef definition

class GetStaticMapRequestRequestTypeDef(TypedDict):
    Height: int,
    FileName: str,
    Width: int,
    BoundingBox: NotRequired[str],
    BoundedPositions: NotRequired[str],
    Center: NotRequired[str],
    CompactOverlay: NotRequired[str],
    GeoJsonOverlay: NotRequired[str],
    Key: NotRequired[str],
    Padding: NotRequired[int],
    Radius: NotRequired[int],
    ScaleBarUnit: NotRequired[ScaleBarUnitType],  # (1)
    Style: NotRequired[StaticMapStyleType],  # (2)
    Zoom: NotRequired[float],
```

1. See [:material-code-brackets: ScaleBarUnitType](./literals.md#scalebarunittype) 
2. See [:material-code-brackets: StaticMapStyleType](./literals.md#staticmapstyletype) 
## GetStyleDescriptorRequestRequestTypeDef

```python
# GetStyleDescriptorRequestRequestTypeDef definition

class GetStyleDescriptorRequestRequestTypeDef(TypedDict):
    Style: MapStyleType,  # (1)
    ColorScheme: NotRequired[ColorSchemeType],  # (2)
    PoliticalView: NotRequired[str],
    Key: NotRequired[str],
```

1. See [:material-code-brackets: MapStyleType](./literals.md#mapstyletype) 
2. See [:material-code-brackets: ColorSchemeType](./literals.md#colorschemetype) 
## GetTileRequestRequestTypeDef

```python
# GetTileRequestRequestTypeDef definition

class GetTileRequestRequestTypeDef(TypedDict):
    Tileset: str,
    Z: str,
    X: str,
    Y: str,
    Key: NotRequired[str],
```

## GetGlyphsResponseTypeDef

```python
# GetGlyphsResponseTypeDef definition

class GetGlyphsResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSpritesResponseTypeDef

```python
# GetSpritesResponseTypeDef definition

class GetSpritesResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStaticMapResponseTypeDef

```python
# GetStaticMapResponseTypeDef definition

class GetStaticMapResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ETag: str,
    PricingBucket: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStyleDescriptorResponseTypeDef

```python
# GetStyleDescriptorResponseTypeDef definition

class GetStyleDescriptorResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ETag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTileResponseTypeDef

```python
# GetTileResponseTypeDef definition

class GetTileResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ETag: str,
    PricingBucket: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
