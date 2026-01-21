# CloudFrontKeyValueStore module

> [Index](../README.md) > CloudFrontKeyValueStore


!!! note ""

    Auto-generated documentation for [CloudFrontKeyValueStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#cloudfrontkeyvaluestore)
    type annotations stubs module [types-aiobotocore-cloudfront-keyvaluestore](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudFrontKeyValueStore` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudFrontKeyValueStore` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudfront-keyvaluestore]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudfront-keyvaluestore]'

# standalone installation
python -m pip install types-aiobotocore-cloudfront-keyvaluestore
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudfront-keyvaluestore
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudFrontKeyValueStoreClient

Type annotations and code completion for  `#!python session.create_client("cloudfront-keyvaluestore")` as [CloudFrontKeyValueStoreClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore.Client)

```python
# CloudFrontKeyValueStoreClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudfront_keyvaluestore.client import CloudFrontKeyValueStoreClient


session = get_session()
async with session.create_client("cloudfront-keyvaluestore") as client:
    client: CloudFrontKeyValueStoreClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloudfront-keyvaluestore").get_paginator("...")`.

```python
# ListKeysPaginator usage example

from types_aiobotocore_cloudfront_keyvaluestore.paginator import ListKeysPaginator

def get_list_keys_paginator() -> ListKeysPaginator:
    return client.get_paginator("list_keys"))
```

- [ListKeysPaginator](./paginators.md#listkeyspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListKeysPaginatorName usage example

from types_aiobotocore_cloudfront_keyvaluestore.literals import ListKeysPaginatorName

def get_value() -> ListKeysPaginatorName:
    return "list_keys"
```

- [ListKeysPaginatorName](./literals.md#listkeyspaginatorname)
- [CloudFrontKeyValueStoreServiceName](./literals.md#cloudfrontkeyvaluestoreservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeleteKeyRequestListItemTypeDef](./type_defs.md#deletekeyrequestlistitemtypedef)
- [DeleteKeyRequestTypeDef](./type_defs.md#deletekeyrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DescribeKeyValueStoreRequestTypeDef](./type_defs.md#describekeyvaluestorerequesttypedef)
- [GetKeyRequestTypeDef](./type_defs.md#getkeyrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListKeysRequestTypeDef](./type_defs.md#listkeysrequesttypedef)
- [ListKeysResponseListItemTypeDef](./type_defs.md#listkeysresponselistitemtypedef)
- [PutKeyRequestListItemTypeDef](./type_defs.md#putkeyrequestlistitemtypedef)
- [PutKeyRequestTypeDef](./type_defs.md#putkeyrequesttypedef)
- [DeleteKeyResponseTypeDef](./type_defs.md#deletekeyresponsetypedef)
- [DescribeKeyValueStoreResponseTypeDef](./type_defs.md#describekeyvaluestoreresponsetypedef)
- [GetKeyResponseTypeDef](./type_defs.md#getkeyresponsetypedef)
- [PutKeyResponseTypeDef](./type_defs.md#putkeyresponsetypedef)
- [UpdateKeysResponseTypeDef](./type_defs.md#updatekeysresponsetypedef)
- [ListKeysRequestPaginateTypeDef](./type_defs.md#listkeysrequestpaginatetypedef)
- [ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef)
- [UpdateKeysRequestTypeDef](./type_defs.md#updatekeysrequesttypedef)

