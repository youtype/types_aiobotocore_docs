# ElasticInference module

> [Index](../README.md) > ElasticInference


!!! note ""

    Auto-generated documentation for [ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#elasticinference)
    type annotations stubs module [types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ElasticInference` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ElasticInference` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[elastic-inference]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[elastic-inference]'

# standalone installation
python -m pip install types-aiobotocore-elastic-inference
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-elastic-inference
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ElasticInferenceClient

Type annotations and code completion for  `#!python session.create_client("elastic-inference")` as [ElasticInferenceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# ElasticInferenceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_elastic_inference.client import ElasticInferenceClient


session = get_session()
async with session.create_client("elastic-inference") as client:
    client: ElasticInferenceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("elastic-inference").get_paginator("...")`.

```python
# DescribeAcceleratorsPaginator usage example

from types_aiobotocore_elastic_inference.paginator import DescribeAcceleratorsPaginator

def get_describe_accelerators_paginator() -> DescribeAcceleratorsPaginator:
    return client.get_paginator("describe_accelerators"))
```

- [DescribeAcceleratorsPaginator](./paginators.md#describeacceleratorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DescribeAcceleratorsPaginatorName usage example

from types_aiobotocore_elastic_inference.literals import DescribeAcceleratorsPaginatorName

def get_value() -> DescribeAcceleratorsPaginatorName:
    return "describe_accelerators"
```

- [DescribeAcceleratorsPaginatorName](./literals.md#describeacceleratorspaginatorname)
- [LocationTypeType](./literals.md#locationtypetype)
- [ElasticInferenceServiceName](./literals.md#elasticinferenceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceleratorTypeOfferingTypeDef](./type_defs.md#acceleratortypeofferingtypedef)
- [KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef)
- [MemoryInfoTypeDef](./type_defs.md#memoryinfotypedef)
- [DescribeAcceleratorOfferingsRequestRequestTypeDef](./type_defs.md#describeacceleratorofferingsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ElasticInferenceAcceleratorHealthTypeDef](./type_defs.md#elasticinferenceacceleratorhealthtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AcceleratorTypeTypeDef](./type_defs.md#acceleratortypetypedef)
- [DescribeAcceleratorOfferingsResponseTypeDef](./type_defs.md#describeacceleratorofferingsresponsetypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [DescribeAcceleratorsRequestRequestTypeDef](./type_defs.md#describeacceleratorsrequestrequesttypedef)
- [DescribeAcceleratorsRequestPaginateTypeDef](./type_defs.md#describeacceleratorsrequestpaginatetypedef)
- [ElasticInferenceAcceleratorTypeDef](./type_defs.md#elasticinferenceacceleratortypedef)
- [DescribeAcceleratorTypesResponseTypeDef](./type_defs.md#describeacceleratortypesresponsetypedef)
- [DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef)

