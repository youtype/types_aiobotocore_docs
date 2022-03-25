<a id="type-annotations-for-aiobotocore-recyclebin-module"></a>

# Type annotations for aiobotocore RecycleBin module

> [Index](../README.md) > RecycleBin

Auto-generated documentation for
[RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
type annotations stubs module
[types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).

- [Type annotations for aiobotocore RecycleBin module](#type-annotations-for-aiobotocore-recyclebin-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [Usage](#usage)
  - [RecycleBinClient](#recyclebinclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `RecycleBin`.

<a id="from-pypi-with-pip"></a>

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

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rbin
```

<a id="usage"></a>

## Usage

Code samples can be found [here](./usage.md).

<a id="recyclebinclient"></a>

## RecycleBinClient

Type annotations for `session.create_client("rbin")` as
[RecycleBinClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_rbin.client import RecycleBinClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [create_rule](./client.md#create_rule)
- [delete_rule](./client.md#delete_rule)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_paginator](./client.md#get_paginator)
- [get_rule](./client.md#get_rule)
- [list_rules](./client.md#list_rules)
- [list_tags_for_resource](./client.md#list_tags_for_resource)
- [tag_resource](./client.md#tag_resource)
- [untag_resource](./client.md#untag_resource)
- [update_rule](./client.md#update_rule)

<a id="exceptions"></a>

### Exceptions

RecycleBinClient [exceptions](./client.md#exceptions)

- ClientError
- InternalServerException
- ResourceNotFoundException
- ServiceQuotaExceededException
- ValidationException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("rbin").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_rbin.paginator import ListRulesPaginator, ...
```

- [ListRulesPaginator](./paginators.md#listrulespaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_rbin.literals import ListRulesPaginatorName, ...
```

- [ListRulesPaginatorName](./literals.md#listrulespaginatorname)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RetentionPeriodUnitType](./literals.md#retentionperiodunittype)
- [RuleStatusType](./literals.md#rulestatustype)
- [RecycleBinServiceName](./literals.md#recyclebinservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from types_aiobotocore_rbin.type_defs import CreateRuleRequestRequestTypeDef, ...
```

- [CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef)
- [CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef)
- [DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef)
- [GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef)
- [GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef)
- [ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef)
- [ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)
- [RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef)
- [UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef)