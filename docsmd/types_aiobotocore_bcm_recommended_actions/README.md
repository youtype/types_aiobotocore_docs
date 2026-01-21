# BillingandCostManagementRecommendedActions module

> [Index](../README.md) > BillingandCostManagementRecommendedActions


!!! note ""

    Auto-generated documentation for [BillingandCostManagementRecommendedActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#billingandcostmanagementrecommendedactions)
    type annotations stubs module [types-aiobotocore-bcm-recommended-actions](https://pypi.org/project/types-aiobotocore-bcm-recommended-actions/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `BillingandCostManagementRecommendedActions` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `BillingandCostManagementRecommendedActions` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bcm-recommended-actions]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bcm-recommended-actions]'

# standalone installation
python -m pip install types-aiobotocore-bcm-recommended-actions
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bcm-recommended-actions
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BillingandCostManagementRecommendedActionsClient

Type annotations and code completion for  `#!python session.create_client("bcm-recommended-actions")` as [BillingandCostManagementRecommendedActionsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#BillingandCostManagementRecommendedActions.Client)

```python
# BillingandCostManagementRecommendedActionsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_recommended_actions.client import BillingandCostManagementRecommendedActionsClient


session = get_session()
async with session.create_client("bcm-recommended-actions") as client:
    client: BillingandCostManagementRecommendedActionsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bcm-recommended-actions").get_paginator("...")`.

```python
# ListRecommendedActionsPaginator usage example

from types_aiobotocore_bcm_recommended_actions.paginator import ListRecommendedActionsPaginator

def get_list_recommended_actions_paginator() -> ListRecommendedActionsPaginator:
    return client.get_paginator("list_recommended_actions"))
```

- [ListRecommendedActionsPaginator](./paginators.md#listrecommendedactionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionTypeType usage example

from types_aiobotocore_bcm_recommended_actions.literals import ActionTypeType

def get_value() -> ActionTypeType:
    return "ADD_ALTERNATE_BILLING_CONTACT"
```

- [ActionTypeType](./literals.md#actiontypetype)
- [FeatureType](./literals.md#featuretype)
- [FilterNameType](./literals.md#filternametype)
- [ListRecommendedActionsPaginatorName](./literals.md#listrecommendedactionspaginatorname)
- [MatchOptionType](./literals.md#matchoptiontype)
- [SeverityType](./literals.md#severitytype)
- [BillingandCostManagementRecommendedActionsServiceName](./literals.md#billingandcostmanagementrecommendedactionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionFilterTypeDef](./type_defs.md#actionfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [RecommendedActionTypeDef](./type_defs.md#recommendedactiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RequestFilterTypeDef](./type_defs.md#requestfiltertypedef)
- [ListRecommendedActionsResponseTypeDef](./type_defs.md#listrecommendedactionsresponsetypedef)
- [ListRecommendedActionsRequestPaginateTypeDef](./type_defs.md#listrecommendedactionsrequestpaginatetypedef)
- [ListRecommendedActionsRequestTypeDef](./type_defs.md#listrecommendedactionsrequesttypedef)

