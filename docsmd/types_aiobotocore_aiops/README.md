# AIOps module

> [Index](../README.md) > AIOps


!!! note ""

    Auto-generated documentation for [AIOps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#aiops)
    type annotations stubs module [types-aiobotocore-aiops](https://pypi.org/project/types-aiobotocore-aiops/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `AIOps` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `AIOps` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[aiops]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[aiops]'

# standalone installation
python -m pip install types-aiobotocore-aiops
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-aiops
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AIOpsClient

Type annotations and code completion for  `#!python session.create_client("aiops")` as [AIOpsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#AIOps.Client)

```python
# AIOpsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_aiops.client import AIOpsClient


session = get_session()
async with session.create_client("aiops") as client:
    client: AIOpsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("aiops").get_paginator("...")`.

```python
# ListInvestigationGroupsPaginator usage example

from types_aiobotocore_aiops.paginator import ListInvestigationGroupsPaginator

def get_list_investigation_groups_paginator() -> ListInvestigationGroupsPaginator:
    return client.get_paginator("list_investigation_groups"))
```

- [ListInvestigationGroupsPaginator](./paginators.md#listinvestigationgroupspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EncryptionConfigurationTypeType usage example

from types_aiobotocore_aiops.literals import EncryptionConfigurationTypeType

def get_value() -> EncryptionConfigurationTypeType:
    return "AWS_OWNED_KEY"
```

- [EncryptionConfigurationTypeType](./literals.md#encryptionconfigurationtypetype)
- [ListInvestigationGroupsPaginatorName](./literals.md#listinvestigationgroupspaginatorname)
- [AIOpsServiceName](./literals.md#aiopsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CrossAccountConfigurationTypeDef](./type_defs.md#crossaccountconfigurationtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteInvestigationGroupPolicyRequestTypeDef](./type_defs.md#deleteinvestigationgrouppolicyrequesttypedef)
- [DeleteInvestigationGroupRequestTypeDef](./type_defs.md#deleteinvestigationgrouprequesttypedef)
- [GetInvestigationGroupPolicyRequestTypeDef](./type_defs.md#getinvestigationgrouppolicyrequesttypedef)
- [GetInvestigationGroupRequestTypeDef](./type_defs.md#getinvestigationgrouprequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListInvestigationGroupsInputTypeDef](./type_defs.md#listinvestigationgroupsinputtypedef)
- [ListInvestigationGroupsModelTypeDef](./type_defs.md#listinvestigationgroupsmodeltypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [PutInvestigationGroupPolicyRequestTypeDef](./type_defs.md#putinvestigationgrouppolicyrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [CreateInvestigationGroupInputTypeDef](./type_defs.md#createinvestigationgroupinputtypedef)
- [UpdateInvestigationGroupRequestTypeDef](./type_defs.md#updateinvestigationgrouprequesttypedef)
- [CreateInvestigationGroupOutputTypeDef](./type_defs.md#createinvestigationgroupoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetInvestigationGroupPolicyResponseTypeDef](./type_defs.md#getinvestigationgrouppolicyresponsetypedef)
- [GetInvestigationGroupResponseTypeDef](./type_defs.md#getinvestigationgroupresponsetypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [PutInvestigationGroupPolicyResponseTypeDef](./type_defs.md#putinvestigationgrouppolicyresponsetypedef)
- [ListInvestigationGroupsInputPaginateTypeDef](./type_defs.md#listinvestigationgroupsinputpaginatetypedef)
- [ListInvestigationGroupsOutputTypeDef](./type_defs.md#listinvestigationgroupsoutputtypedef)

