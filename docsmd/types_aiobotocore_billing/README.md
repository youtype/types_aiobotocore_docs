# Billing module

> [Index](../README.md) > Billing


!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
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








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BillingViewTypeType usage example

from types_aiobotocore_billing.literals import BillingViewTypeType

def get_value() -> BillingViewTypeType:
    return "BILLING_GROUP"
```

- [BillingViewTypeType](./literals.md#billingviewtypetype)
- [ListBillingViewsPaginatorName](./literals.md#listbillingviewspaginatorname)
- [BillingServiceName](./literals.md#billingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [BillingViewListElementTypeDef](./type_defs.md#billingviewlistelementtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef)
- [ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef)
- [ListBillingViewsRequestListBillingViewsPaginateTypeDef](./type_defs.md#listbillingviewsrequestlistbillingviewspaginatetypedef)
- [ListBillingViewsRequestRequestTypeDef](./type_defs.md#listbillingviewsrequestrequesttypedef)

