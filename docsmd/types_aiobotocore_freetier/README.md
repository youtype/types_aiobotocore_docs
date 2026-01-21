# FreeTier module

> [Index](../README.md) > FreeTier


!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `FreeTier` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `FreeTier` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[freetier]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[freetier]'

# standalone installation
python -m pip install types-aiobotocore-freetier
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-freetier
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FreeTierClient

Type annotations and code completion for  `#!python session.create_client("freetier")` as [FreeTierClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#FreeTier.Client)

```python
# FreeTierClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_freetier.client import FreeTierClient


session = get_session()
async with session.create_client("freetier") as client:
    client: FreeTierClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("freetier").get_paginator("...")`.

```python
# GetFreeTierUsagePaginator usage example

from types_aiobotocore_freetier.paginator import GetFreeTierUsagePaginator

def get_get_free_tier_usage_paginator() -> GetFreeTierUsagePaginator:
    return client.get_paginator("get_free_tier_usage"))
```

- [GetFreeTierUsagePaginator](./paginators.md#getfreetierusagepaginator)
- [ListAccountActivitiesPaginator](./paginators.md#listaccountactivitiespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountPlanStatusType usage example

from types_aiobotocore_freetier.literals import AccountPlanStatusType

def get_value() -> AccountPlanStatusType:
    return "ACTIVE"
```

- [AccountPlanStatusType](./literals.md#accountplanstatustype)
- [AccountPlanTypeType](./literals.md#accountplantypetype)
- [ActivityStatusType](./literals.md#activitystatustype)
- [CurrencyCodeType](./literals.md#currencycodetype)
- [DimensionType](./literals.md#dimensiontype)
- [GetFreeTierUsagePaginatorName](./literals.md#getfreetierusagepaginatorname)
- [LanguageCodeType](./literals.md#languagecodetype)
- [ListAccountActivitiesPaginatorName](./literals.md#listaccountactivitiespaginatorname)
- [MatchOptionType](./literals.md#matchoptiontype)
- [FreeTierServiceName](./literals.md#freetierservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [MonetaryAmountTypeDef](./type_defs.md#monetaryamounttypedef)
- [DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef)
- [FreeTierUsageTypeDef](./type_defs.md#freetierusagetypedef)
- [GetAccountActivityRequestTypeDef](./type_defs.md#getaccountactivityrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccountActivitiesRequestTypeDef](./type_defs.md#listaccountactivitiesrequesttypedef)
- [UpgradeAccountPlanRequestTypeDef](./type_defs.md#upgradeaccountplanrequesttypedef)
- [ActivityRewardTypeDef](./type_defs.md#activityrewardtypedef)
- [ExpressionPaginatorTypeDef](./type_defs.md#expressionpaginatortypedef)
- [ExpressionTypeDef](./type_defs.md#expressiontypedef)
- [GetAccountPlanStateResponseTypeDef](./type_defs.md#getaccountplanstateresponsetypedef)
- [GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef)
- [UpgradeAccountPlanResponseTypeDef](./type_defs.md#upgradeaccountplanresponsetypedef)
- [ListAccountActivitiesRequestPaginateTypeDef](./type_defs.md#listaccountactivitiesrequestpaginatetypedef)
- [ActivitySummaryTypeDef](./type_defs.md#activitysummarytypedef)
- [GetAccountActivityResponseTypeDef](./type_defs.md#getaccountactivityresponsetypedef)
- [GetFreeTierUsageRequestPaginateTypeDef](./type_defs.md#getfreetierusagerequestpaginatetypedef)
- [GetFreeTierUsageRequestTypeDef](./type_defs.md#getfreetierusagerequesttypedef)
- [ListAccountActivitiesResponseTypeDef](./type_defs.md#listaccountactivitiesresponsetypedef)

