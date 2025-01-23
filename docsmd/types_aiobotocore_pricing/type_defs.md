# Type definitions

> [Index](../README.md) > [Pricing](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#pricing)
    type annotations stubs module [types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AttributeValueTypeDef

```python
# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    Value: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeServicesRequestRequestTypeDef

```python
# DescribeServicesRequestRequestTypeDef definition

class DescribeServicesRequestRequestTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    FormatVersion: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
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

## ServiceTypeDef

```python
# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    ServiceCode: str,
    AttributeNames: NotRequired[List[str]],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Type: FilterTypeType,  # (1)
    Field: str,
    Value: str,
```

1. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype) 
## GetAttributeValuesRequestRequestTypeDef

```python
# GetAttributeValuesRequestRequestTypeDef definition

class GetAttributeValuesRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    AttributeName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetPriceListFileUrlRequestRequestTypeDef

```python
# GetPriceListFileUrlRequestRequestTypeDef definition

class GetPriceListFileUrlRequestRequestTypeDef(TypedDict):
    PriceListArn: str,
    FileFormat: str,
```

## PriceListTypeDef

```python
# PriceListTypeDef definition

class PriceListTypeDef(TypedDict):
    PriceListArn: NotRequired[str],
    RegionCode: NotRequired[str],
    CurrencyCode: NotRequired[str],
    FileFormats: NotRequired[List[str]],
```

## DescribeServicesRequestPaginateTypeDef

```python
# DescribeServicesRequestPaginateTypeDef definition

class DescribeServicesRequestPaginateTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    FormatVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAttributeValuesRequestPaginateTypeDef

```python
# GetAttributeValuesRequestPaginateTypeDef definition

class GetAttributeValuesRequestPaginateTypeDef(TypedDict):
    ServiceCode: str,
    AttributeName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAttributeValuesResponseTypeDef

```python
# GetAttributeValuesResponseTypeDef definition

class GetAttributeValuesResponseTypeDef(TypedDict):
    AttributeValues: List[AttributeValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPriceListFileUrlResponseTypeDef

```python
# GetPriceListFileUrlResponseTypeDef definition

class GetPriceListFileUrlResponseTypeDef(TypedDict):
    Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProductsResponseTypeDef

```python
# GetProductsResponseTypeDef definition

class GetProductsResponseTypeDef(TypedDict):
    FormatVersion: str,
    PriceList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServicesResponseTypeDef

```python
# DescribeServicesResponseTypeDef definition

class DescribeServicesResponseTypeDef(TypedDict):
    Services: List[ServiceTypeDef],  # (1)
    FormatVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProductsRequestPaginateTypeDef

```python
# GetProductsRequestPaginateTypeDef definition

class GetProductsRequestPaginateTypeDef(TypedDict):
    ServiceCode: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    FormatVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetProductsRequestRequestTypeDef

```python
# GetProductsRequestRequestTypeDef definition

class GetProductsRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    FormatVersion: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListPriceListsRequestPaginateTypeDef

```python
# ListPriceListsRequestPaginateTypeDef definition

class ListPriceListsRequestPaginateTypeDef(TypedDict):
    ServiceCode: str,
    EffectiveDate: TimestampTypeDef,
    CurrencyCode: str,
    RegionCode: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPriceListsRequestRequestTypeDef

```python
# ListPriceListsRequestRequestTypeDef definition

class ListPriceListsRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    EffectiveDate: TimestampTypeDef,
    CurrencyCode: str,
    RegionCode: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPriceListsResponseTypeDef

```python
# ListPriceListsResponseTypeDef definition

class ListPriceListsResponseTypeDef(TypedDict):
    PriceLists: List[PriceListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PriceListTypeDef](./type_defs.md#pricelisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
