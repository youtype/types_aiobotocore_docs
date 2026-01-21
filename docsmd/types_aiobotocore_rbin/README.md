# RecycleBin module

> [Index](../README.md) > RecycleBin


!!! note ""

    Auto-generated documentation for [RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#recyclebin)
    type annotations stubs module [types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `RecycleBin` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `RecycleBin` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[rbin]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[rbin]'

# standalone installation
python -m pip install types-aiobotocore-rbin
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rbin
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RecycleBinClient

Type annotations and code completion for  `#!python session.create_client("rbin")` as [RecycleBinClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# RecycleBinClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_rbin.client import RecycleBinClient


session = get_session()
async with session.create_client("rbin") as client:
    client: RecycleBinClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("rbin").get_paginator("...")`.

```python
# ListRulesPaginator usage example

from types_aiobotocore_rbin.paginator import ListRulesPaginator

def get_list_rules_paginator() -> ListRulesPaginator:
    return client.get_paginator("list_rules"))
```

- [ListRulesPaginator](./paginators.md#listrulespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListRulesPaginatorName usage example

from types_aiobotocore_rbin.literals import ListRulesPaginatorName

def get_value() -> ListRulesPaginatorName:
    return "list_rules"
```

- [ListRulesPaginatorName](./literals.md#listrulespaginatorname)
- [LockStateType](./literals.md#lockstatetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RetentionPeriodUnitType](./literals.md#retentionperiodunittype)
- [RuleStatusType](./literals.md#rulestatustype)
- [UnlockDelayUnitType](./literals.md#unlockdelayunittype)
- [RecycleBinServiceName](./literals.md#recyclebinservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteRuleRequestTypeDef](./type_defs.md#deleterulerequesttypedef)
- [GetRuleRequestTypeDef](./type_defs.md#getrulerequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [UnlockDelayTypeDef](./type_defs.md#unlockdelaytypedef)
- [UnlockRuleRequestTypeDef](./type_defs.md#unlockrulerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ListRulesRequestTypeDef](./type_defs.md#listrulesrequesttypedef)
- [RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef)
- [UpdateRuleRequestTypeDef](./type_defs.md#updaterulerequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef)
- [ListRulesRequestPaginateTypeDef](./type_defs.md#listrulesrequestpaginatetypedef)
- [LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef)
- [ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)
- [CreateRuleRequestTypeDef](./type_defs.md#createrulerequesttypedef)
- [CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef)
- [GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef)
- [LockRuleRequestTypeDef](./type_defs.md#lockrulerequesttypedef)
- [LockRuleResponseTypeDef](./type_defs.md#lockruleresponsetypedef)
- [UnlockRuleResponseTypeDef](./type_defs.md#unlockruleresponsetypedef)

