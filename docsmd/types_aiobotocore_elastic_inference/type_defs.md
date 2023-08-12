# Type definitions

> [Index](../README.md) > [ElasticInference](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
    type annotations stubs module [types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).



## AcceleratorTypeOfferingTypeDef

```python
# AcceleratorTypeOfferingTypeDef definition

class AcceleratorTypeOfferingTypeDef(TypedDict):
    acceleratorType: NotRequired[str],
    locationType: NotRequired[LocationTypeType],  # (1)
    location: NotRequired[str],
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype) 
## KeyValuePairTypeDef

```python
# KeyValuePairTypeDef definition

class KeyValuePairTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[int],
```

## MemoryInfoTypeDef

```python
# MemoryInfoTypeDef definition

class MemoryInfoTypeDef(TypedDict):
    sizeInMiB: NotRequired[int],
```

## DescribeAcceleratorOfferingsRequestRequestTypeDef

```python
# DescribeAcceleratorOfferingsRequestRequestTypeDef definition

class DescribeAcceleratorOfferingsRequestRequestTypeDef(TypedDict):
    locationType: LocationTypeType,  # (1)
    acceleratorTypes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ElasticInferenceAcceleratorHealthTypeDef

```python
# ElasticInferenceAcceleratorHealthTypeDef definition

class ElasticInferenceAcceleratorHealthTypeDef(TypedDict):
    status: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AcceleratorTypeTypeDef

```python
# AcceleratorTypeTypeDef definition

class AcceleratorTypeTypeDef(TypedDict):
    acceleratorTypeName: NotRequired[str],
    memoryInfo: NotRequired[MemoryInfoTypeDef],  # (1)
    throughputInfo: NotRequired[List[KeyValuePairTypeDef]],  # (2)
```

1. See [:material-code-braces: MemoryInfoTypeDef](./type_defs.md#memoryinfotypedef) 
2. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## DescribeAcceleratorOfferingsResponseTypeDef

```python
# DescribeAcceleratorOfferingsResponseTypeDef definition

class DescribeAcceleratorOfferingsResponseTypeDef(TypedDict):
    acceleratorTypeOfferings: List[AcceleratorTypeOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorTypeOfferingTypeDef](./type_defs.md#acceleratortypeofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAcceleratorsRequestRequestTypeDef

```python
# DescribeAcceleratorsRequestRequestTypeDef definition

class DescribeAcceleratorsRequestRequestTypeDef(TypedDict):
    acceleratorIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef

```python
# DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef definition

class DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef(TypedDict):
    acceleratorIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ElasticInferenceAcceleratorTypeDef

```python
# ElasticInferenceAcceleratorTypeDef definition

class ElasticInferenceAcceleratorTypeDef(TypedDict):
    acceleratorHealth: NotRequired[ElasticInferenceAcceleratorHealthTypeDef],  # (1)
    acceleratorType: NotRequired[str],
    acceleratorId: NotRequired[str],
    availabilityZone: NotRequired[str],
    attachedResource: NotRequired[str],
```

1. See [:material-code-braces: ElasticInferenceAcceleratorHealthTypeDef](./type_defs.md#elasticinferenceacceleratorhealthtypedef) 
## DescribeAcceleratorTypesResponseTypeDef

```python
# DescribeAcceleratorTypesResponseTypeDef definition

class DescribeAcceleratorTypesResponseTypeDef(TypedDict):
    acceleratorTypes: List[AcceleratorTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorTypeTypeDef](./type_defs.md#acceleratortypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAcceleratorsResponseTypeDef

```python
# DescribeAcceleratorsResponseTypeDef definition

class DescribeAcceleratorsResponseTypeDef(TypedDict):
    acceleratorSet: List[ElasticInferenceAcceleratorTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticInferenceAcceleratorTypeDef](./type_defs.md#elasticinferenceacceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
