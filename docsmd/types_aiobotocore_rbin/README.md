# RecycleBin module

> [Index](../README.md) > RecycleBin


!!! note ""

    Auto-generated documentation for [RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
    type annotations stubs module [types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `RecycleBin`.

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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_rbin.paginator import ListRulesPaginator

def get_list_rules_paginator() -> ListRulesPaginator:
    return client.get_paginator("list_rules"))
```

- [ListRulesPaginator](./paginators.md#listrulespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rbin.literals import ListRulesPaginatorName

def get_value() -> ListRulesPaginatorName:
    return "list_rules"
```

- [ListRulesPaginatorName](./literals.md#listrulespaginatorname)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RetentionPeriodUnitType](./literals.md#retentionperiodunittype)
- [RuleStatusType](./literals.md#rulestatustype)
- [RecycleBinServiceName](./literals.md#recyclebinservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rbin.type_defs import ResourceTagTypeDef

def get_value() -> ResourceTagTypeDef:
    return {
        "ResourceTagKey": ...,
    }
```

- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef)
- [GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef)
- [RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef)
- [UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef)
- [CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef)
- [GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef)
- [ListRulesRequestListRulesPaginateTypeDef](./type_defs.md#listrulesrequestlistrulespaginatetypedef)
- [ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)

