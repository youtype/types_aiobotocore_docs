# Examples

> [Index](../README.md) > [AgreementService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AgreementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#agreementservice)
    type annotations stubs module [types-aiobotocore-marketplace-agreement](https://pypi.org/project/types-aiobotocore-marketplace-agreement/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-agreement]` package installed.

Write your `AgreementService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AgreementServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-agreement") as client:  # (1)
    result = await client.accept_agreement_cancellation_request()  # (2)
```

1. client: [AgreementServiceClient](./client.md)
2. result: [:material-code-braces: AcceptAgreementCancellationRequestOutputTypeDef](./type_defs.md#acceptagreementcancellationrequestoutputtypedef)



#### Paginator usage example

```python
# GetAgreementEntitlementsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-agreement") as client:  # (1)
    paginator = client.get_paginator("get_agreement_entitlements")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AgreementServiceClient](./client.md)
2. paginator: [GetAgreementEntitlementsPaginator](./paginators.md#getagreemententitlementspaginator)
3. item: [:material-code-braces: GetAgreementEntitlementsOutputTypeDef](./type_defs.md#getagreemententitlementsoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[marketplace-agreement]`
or a standalone `types_aiobotocore_marketplace_agreement` package, you have to explicitly specify
`client: AgreementServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AgreementServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_agreement.client import AgreementServiceClient
from types_aiobotocore_marketplace_agreement.type_defs import AcceptAgreementCancellationRequestOutputTypeDef
from types_aiobotocore_marketplace_agreement.type_defs import AcceptAgreementCancellationRequestInputTypeDef


session = get_session()

async with session.create_client("marketplace-agreement") as client:
    client: AgreementServiceClient
    kwargs: AcceptAgreementCancellationRequestInputTypeDef = {...}
    result: AcceptAgreementCancellationRequestOutputTypeDef = await client.accept_agreement_cancellation_request(**kwargs)
```



#### Paginator usage example

```python
# GetAgreementEntitlementsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_agreement.client import AgreementServiceClient
from types_aiobotocore_marketplace_agreement.paginator import GetAgreementEntitlementsPaginator
from types_aiobotocore_marketplace_agreement.type_defs import GetAgreementEntitlementsOutputTypeDef


session = get_session()

async with session.create_client("marketplace-agreement") as client:
    client: AgreementServiceClient
    paginator: GetAgreementEntitlementsPaginator = client.get_paginator("get_agreement_entitlements")
    async for item in paginator.paginate(...):
        item: GetAgreementEntitlementsOutputTypeDef
        print(item)
```


