# Type definitions

> [Index](../README.md) > [ElasticInference](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#elasticinference)
    type annotations stubs module [types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).



## AcceleratorTypeOfferingTypeDef

```python
# AcceleratorTypeOfferingTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import AcceleratorTypeOfferingTypeDef


def get_value() -> AcceleratorTypeOfferingTypeDef:
    return {
        "acceleratorType": ...,
    }


# AcceleratorTypeOfferingTypeDef definition

class AcceleratorTypeOfferingTypeDef(TypedDict):
    acceleratorType: NotRequired[str],
    locationType: NotRequired[LocationTypeType],  # (1)
    location: NotRequired[str],
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype) 
## KeyValuePairTypeDef

```python
# KeyValuePairTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import KeyValuePairTypeDef


def get_value() -> KeyValuePairTypeDef:
    return {
        "key": ...,
    }


# KeyValuePairTypeDef definition

class KeyValuePairTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[int],
```

## MemoryInfoTypeDef

```python
# MemoryInfoTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import MemoryInfoTypeDef


def get_value() -> MemoryInfoTypeDef:
    return {
        "sizeInMiB": ...,
    }


# MemoryInfoTypeDef definition

class MemoryInfoTypeDef(TypedDict):
    sizeInMiB: NotRequired[int],
```

## DescribeAcceleratorOfferingsRequestTypeDef

```python
# DescribeAcceleratorOfferingsRequestTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorOfferingsRequestTypeDef


def get_value() -> DescribeAcceleratorOfferingsRequestTypeDef:
    return {
        "locationType": ...,
    }


# DescribeAcceleratorOfferingsRequestTypeDef definition

class DescribeAcceleratorOfferingsRequestTypeDef(TypedDict):
    locationType: LocationTypeType,  # (1)
    acceleratorTypes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "name": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ElasticInferenceAcceleratorHealthTypeDef

```python
# ElasticInferenceAcceleratorHealthTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import ElasticInferenceAcceleratorHealthTypeDef


def get_value() -> ElasticInferenceAcceleratorHealthTypeDef:
    return {
        "status": ...,
    }


# ElasticInferenceAcceleratorHealthTypeDef definition

class ElasticInferenceAcceleratorHealthTypeDef(TypedDict):
    status: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AcceleratorTypeTypeDef

```python
# AcceleratorTypeTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import AcceleratorTypeTypeDef


def get_value() -> AcceleratorTypeTypeDef:
    return {
        "acceleratorTypeName": ...,
    }


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
# DescribeAcceleratorOfferingsResponseTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorOfferingsResponseTypeDef


def get_value() -> DescribeAcceleratorOfferingsResponseTypeDef:
    return {
        "acceleratorTypeOfferings": ...,
    }


# DescribeAcceleratorOfferingsResponseTypeDef definition

class DescribeAcceleratorOfferingsResponseTypeDef(TypedDict):
    acceleratorTypeOfferings: List[AcceleratorTypeOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorTypeOfferingTypeDef](./type_defs.md#acceleratortypeofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import ListTagsForResourceResultTypeDef


def get_value() -> ListTagsForResourceResultTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAcceleratorsRequestTypeDef

```python
# DescribeAcceleratorsRequestTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorsRequestTypeDef


def get_value() -> DescribeAcceleratorsRequestTypeDef:
    return {
        "acceleratorIds": ...,
    }


# DescribeAcceleratorsRequestTypeDef definition

class DescribeAcceleratorsRequestTypeDef(TypedDict):
    acceleratorIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeAcceleratorsRequestPaginateTypeDef

```python
# DescribeAcceleratorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorsRequestPaginateTypeDef


def get_value() -> DescribeAcceleratorsRequestPaginateTypeDef:
    return {
        "acceleratorIds": ...,
    }


# DescribeAcceleratorsRequestPaginateTypeDef definition

class DescribeAcceleratorsRequestPaginateTypeDef(TypedDict):
    acceleratorIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ElasticInferenceAcceleratorTypeDef

```python
# ElasticInferenceAcceleratorTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import ElasticInferenceAcceleratorTypeDef


def get_value() -> ElasticInferenceAcceleratorTypeDef:
    return {
        "acceleratorHealth": ...,
    }


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
# DescribeAcceleratorTypesResponseTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorTypesResponseTypeDef


def get_value() -> DescribeAcceleratorTypesResponseTypeDef:
    return {
        "acceleratorTypes": ...,
    }


# DescribeAcceleratorTypesResponseTypeDef definition

class DescribeAcceleratorTypesResponseTypeDef(TypedDict):
    acceleratorTypes: List[AcceleratorTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AcceleratorTypeTypeDef](./type_defs.md#acceleratortypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAcceleratorsResponseTypeDef

```python
# DescribeAcceleratorsResponseTypeDef TypedDict usage example

from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorsResponseTypeDef


def get_value() -> DescribeAcceleratorsResponseTypeDef:
    return {
        "acceleratorSet": ...,
    }


# DescribeAcceleratorsResponseTypeDef definition

class DescribeAcceleratorsResponseTypeDef(TypedDict):
    acceleratorSet: List[ElasticInferenceAcceleratorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ElasticInferenceAcceleratorTypeDef](./type_defs.md#elasticinferenceacceleratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
