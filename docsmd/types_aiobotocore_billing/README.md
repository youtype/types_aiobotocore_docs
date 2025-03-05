# Billing module

> [Index](../README.md) > Billing


!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.21.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Billing` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Billing` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[billing]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[billing]'

# standalone installation
python -m pip install types-aiobotocore-billing
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-billing
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BillingClient

Type annotations and code completion for  `#!python session.create_client("billing")` as [BillingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# BillingClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_billing.client import BillingClient


session = get_session()
async with session.create_client("billing") as client:
    client: BillingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("billing").get_paginator("...")`.

```python
# ListBillingViewsPaginator usage example

from types_aiobotocore_billing.paginator import ListBillingViewsPaginator

def get_list_billing_views_paginator() -> ListBillingViewsPaginator:
    return client.get_paginator("list_billing_views"))
```

- [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)
- [ListSourceViewsForBillingViewPaginator](./paginators.md#listsourceviewsforbillingviewpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BillingViewTypeType usage example

from types_aiobotocore_billing.literals import BillingViewTypeType

def get_value() -> BillingViewTypeType:
    return "BILLING_GROUP"
```

- [BillingViewTypeType](./literals.md#billingviewtypetype)
- [DimensionType](./literals.md#dimensiontype)
- [ListBillingViewsPaginatorName](./literals.md#listbillingviewspaginatorname)
- [ListSourceViewsForBillingViewPaginatorName](./literals.md#listsourceviewsforbillingviewpaginatorname)
- [BillingServiceName](./literals.md#billingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [BillingViewListElementTypeDef](./type_defs.md#billingviewlistelementtypedef)
- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteBillingViewRequestTypeDef](./type_defs.md#deletebillingviewrequesttypedef)
- [DimensionValuesOutputTypeDef](./type_defs.md#dimensionvaluesoutputtypedef)
- [DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef)
- [TagValuesOutputTypeDef](./type_defs.md#tagvaluesoutputtypedef)
- [TagValuesTypeDef](./type_defs.md#tagvaluestypedef)
- [GetBillingViewRequestTypeDef](./type_defs.md#getbillingviewrequesttypedef)
- [GetResourcePolicyRequestTypeDef](./type_defs.md#getresourcepolicyrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListSourceViewsForBillingViewRequestTypeDef](./type_defs.md#listsourceviewsforbillingviewrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CreateBillingViewResponseTypeDef](./type_defs.md#createbillingviewresponsetypedef)
- [DeleteBillingViewResponseTypeDef](./type_defs.md#deletebillingviewresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef)
- [ListSourceViewsForBillingViewResponseTypeDef](./type_defs.md#listsourceviewsforbillingviewresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateBillingViewResponseTypeDef](./type_defs.md#updatebillingviewresponsetypedef)
- [ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef)
- [ExpressionTypeDef](./type_defs.md#expressiontypedef)
- [ListSourceViewsForBillingViewRequestPaginateTypeDef](./type_defs.md#listsourceviewsforbillingviewrequestpaginatetypedef)
- [ListBillingViewsRequestPaginateTypeDef](./type_defs.md#listbillingviewsrequestpaginatetypedef)
- [ListBillingViewsRequestTypeDef](./type_defs.md#listbillingviewsrequesttypedef)
- [BillingViewElementTypeDef](./type_defs.md#billingviewelementtypedef)
- [ExpressionUnionTypeDef](./type_defs.md#expressionuniontypedef)
- [GetBillingViewResponseTypeDef](./type_defs.md#getbillingviewresponsetypedef)
- [CreateBillingViewRequestTypeDef](./type_defs.md#createbillingviewrequesttypedef)
- [UpdateBillingViewRequestTypeDef](./type_defs.md#updatebillingviewrequesttypedef)

