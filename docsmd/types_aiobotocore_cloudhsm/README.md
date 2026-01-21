# CloudHSM module

> [Index](../README.md) > CloudHSM


!!! note ""

    Auto-generated documentation for [CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#cloudhsm)
    type annotations stubs module [types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudHSM` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudHSM` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudhsm]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudhsm]'

# standalone installation
python -m pip install types-aiobotocore-cloudhsm
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudhsm
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudHSMClient

Type annotations and code completion for  `#!python session.create_client("cloudhsm")` as [CloudHSMClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client)

```python
# CloudHSMClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudhsm.client import CloudHSMClient


session = get_session()
async with session.create_client("cloudhsm") as client:
    client: CloudHSMClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloudhsm").get_paginator("...")`.

```python
# ListHapgsPaginator usage example

from types_aiobotocore_cloudhsm.paginator import ListHapgsPaginator

def get_list_hapgs_paginator() -> ListHapgsPaginator:
    return client.get_paginator("list_hapgs"))
```

- [ListHapgsPaginator](./paginators.md#listhapgspaginator)
- [ListHsmsPaginator](./paginators.md#listhsmspaginator)
- [ListLunaClientsPaginator](./paginators.md#listlunaclientspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ClientVersionType usage example

from types_aiobotocore_cloudhsm.literals import ClientVersionType

def get_value() -> ClientVersionType:
    return "5.1"
```

- [ClientVersionType](./literals.md#clientversiontype)
- [CloudHsmObjectStateType](./literals.md#cloudhsmobjectstatetype)
- [HsmStatusType](./literals.md#hsmstatustype)
- [ListHapgsPaginatorName](./literals.md#listhapgspaginatorname)
- [ListHsmsPaginatorName](./literals.md#listhsmspaginatorname)
- [ListLunaClientsPaginatorName](./literals.md#listlunaclientspaginatorname)
- [SubscriptionTypeType](./literals.md#subscriptiontypetype)
- [CloudHSMServiceName](./literals.md#cloudhsmservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateHapgRequestTypeDef](./type_defs.md#createhapgrequesttypedef)
- [CreateHsmRequestTypeDef](./type_defs.md#createhsmrequesttypedef)
- [CreateLunaClientRequestTypeDef](./type_defs.md#createlunaclientrequesttypedef)
- [DeleteHapgRequestTypeDef](./type_defs.md#deletehapgrequesttypedef)
- [DeleteHsmRequestTypeDef](./type_defs.md#deletehsmrequesttypedef)
- [DeleteLunaClientRequestTypeDef](./type_defs.md#deletelunaclientrequesttypedef)
- [DescribeHapgRequestTypeDef](./type_defs.md#describehapgrequesttypedef)
- [DescribeHsmRequestTypeDef](./type_defs.md#describehsmrequesttypedef)
- [DescribeLunaClientRequestTypeDef](./type_defs.md#describelunaclientrequesttypedef)
- [GetConfigRequestTypeDef](./type_defs.md#getconfigrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListHapgsRequestTypeDef](./type_defs.md#listhapgsrequesttypedef)
- [ListHsmsRequestTypeDef](./type_defs.md#listhsmsrequesttypedef)
- [ListLunaClientsRequestTypeDef](./type_defs.md#listlunaclientsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ModifyHapgRequestTypeDef](./type_defs.md#modifyhapgrequesttypedef)
- [ModifyHsmRequestTypeDef](./type_defs.md#modifyhsmrequesttypedef)
- [ModifyLunaClientRequestTypeDef](./type_defs.md#modifylunaclientrequesttypedef)
- [RemoveTagsFromResourceRequestTypeDef](./type_defs.md#removetagsfromresourcerequesttypedef)
- [AddTagsToResourceRequestTypeDef](./type_defs.md#addtagstoresourcerequesttypedef)
- [AddTagsToResourceResponseTypeDef](./type_defs.md#addtagstoresourceresponsetypedef)
- [CreateHapgResponseTypeDef](./type_defs.md#createhapgresponsetypedef)
- [CreateHsmResponseTypeDef](./type_defs.md#createhsmresponsetypedef)
- [CreateLunaClientResponseTypeDef](./type_defs.md#createlunaclientresponsetypedef)
- [DeleteHapgResponseTypeDef](./type_defs.md#deletehapgresponsetypedef)
- [DeleteHsmResponseTypeDef](./type_defs.md#deletehsmresponsetypedef)
- [DeleteLunaClientResponseTypeDef](./type_defs.md#deletelunaclientresponsetypedef)
- [DescribeHapgResponseTypeDef](./type_defs.md#describehapgresponsetypedef)
- [DescribeHsmResponseTypeDef](./type_defs.md#describehsmresponsetypedef)
- [DescribeLunaClientResponseTypeDef](./type_defs.md#describelunaclientresponsetypedef)
- [GetConfigResponseTypeDef](./type_defs.md#getconfigresponsetypedef)
- [ListAvailableZonesResponseTypeDef](./type_defs.md#listavailablezonesresponsetypedef)
- [ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef)
- [ListHsmsResponseTypeDef](./type_defs.md#listhsmsresponsetypedef)
- [ListLunaClientsResponseTypeDef](./type_defs.md#listlunaclientsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ModifyHapgResponseTypeDef](./type_defs.md#modifyhapgresponsetypedef)
- [ModifyHsmResponseTypeDef](./type_defs.md#modifyhsmresponsetypedef)
- [ModifyLunaClientResponseTypeDef](./type_defs.md#modifylunaclientresponsetypedef)
- [RemoveTagsFromResourceResponseTypeDef](./type_defs.md#removetagsfromresourceresponsetypedef)
- [ListHapgsRequestPaginateTypeDef](./type_defs.md#listhapgsrequestpaginatetypedef)
- [ListHsmsRequestPaginateTypeDef](./type_defs.md#listhsmsrequestpaginatetypedef)
- [ListLunaClientsRequestPaginateTypeDef](./type_defs.md#listlunaclientsrequestpaginatetypedef)

