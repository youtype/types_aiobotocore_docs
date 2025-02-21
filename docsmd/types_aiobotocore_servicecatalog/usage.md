# Examples

> [Index](../README.md) > [ServiceCatalog](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ServiceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#servicecatalog)
    type annotations stubs module [types-aiobotocore-servicecatalog](https://pypi.org/project/types-aiobotocore-servicecatalog/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[servicecatalog]` package installed.

Write your `ServiceCatalog` code as usual,
type checking and code completion should work out of the box.



```python
# ServiceCatalogClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("servicecatalog") as client:  # (1)
    result = await client.batch_associate_service_action_with_provisioning_artifact()  # (2)
```

1. client: [ServiceCatalogClient](./client.md)
2. result: [:material-code-braces: BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef](./type_defs.md#batchassociateserviceactionwithprovisioningartifactoutputtypedef) 



```python
# ListAcceptedPortfolioSharesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("servicecatalog") as client:  # (1)
    paginator = client.get_paginator("list_accepted_portfolio_shares")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListAcceptedPortfolioSharesPaginator](./paginators.md#listacceptedportfoliosharespaginator)
3. item: [:material-code-braces: ListAcceptedPortfolioSharesOutputTypeDef](./type_defs.md#listacceptedportfoliosharesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[servicecatalog]`
or a standalone `types_aiobotocore_servicecatalog` package, you have to explicitly specify
`client: ServiceCatalogClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ServiceCatalogClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog.client import ServiceCatalogClient
from types_aiobotocore_servicecatalog.type_defs import BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef
from types_aiobotocore_servicecatalog.type_defs import BatchAssociateServiceActionWithProvisioningArtifactInputTypeDef


session = get_session()

async with session.create_client("servicecatalog") as client:
    client: ServiceCatalogClient
    kwargs: BatchAssociateServiceActionWithProvisioningArtifactInputTypeDef = {...}
    result: BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef = await client.batch_associate_service_action_with_provisioning_artifact(**kwargs)
```



```python
# ListAcceptedPortfolioSharesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog.client import ServiceCatalogClient
from types_aiobotocore_servicecatalog.paginator import ListAcceptedPortfolioSharesPaginator
from types_aiobotocore_servicecatalog.type_defs import ListAcceptedPortfolioSharesOutputTypeDef


session = get_session()

async with session.create_client("servicecatalog") as client:
    client: ServiceCatalogClient
    paginator: ListAcceptedPortfolioSharesPaginator = client.get_paginator("list_accepted_portfolio_shares")
    async for item in paginator.paginate(...):
        item: ListAcceptedPortfolioSharesOutputTypeDef
        print(item)
```


