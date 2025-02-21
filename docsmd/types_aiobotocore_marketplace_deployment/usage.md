# Examples

> [Index](../README.md) > [MarketplaceDeploymentService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceDeploymentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#marketplacedeploymentservice)
    type annotations stubs module [types-aiobotocore-marketplace-deployment](https://pypi.org/project/types-aiobotocore-marketplace-deployment/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-deployment]` package installed.

Write your `MarketplaceDeploymentService` code as usual,
type checking and code completion should work out of the box.



```python
# MarketplaceDeploymentServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-deployment") as client:  # (1)
    result = await client.list_tags_for_resource()  # (2)
```

1. client: [MarketplaceDeploymentServiceClient](./client.md)
2. result: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[marketplace-deployment]`
or a standalone `types_aiobotocore_marketplace_deployment` package, you have to explicitly specify
`client: MarketplaceDeploymentServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MarketplaceDeploymentServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_deployment.client import MarketplaceDeploymentServiceClient
from types_aiobotocore_marketplace_deployment.type_defs import ListTagsForResourceResponseTypeDef
from types_aiobotocore_marketplace_deployment.type_defs import ListTagsForResourceRequestTypeDef


session = get_session()

async with session.create_client("marketplace-deployment") as client:
    client: MarketplaceDeploymentServiceClient
    kwargs: ListTagsForResourceRequestTypeDef = {...}
    result: ListTagsForResourceResponseTypeDef = await client.list_tags_for_resource(**kwargs)
```




