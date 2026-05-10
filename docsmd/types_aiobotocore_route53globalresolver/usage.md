# Examples

> [Index](../README.md) > [Route53GlobalResolver](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53GlobalResolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver.html#route53globalresolver)
    type annotations stubs module [types-aiobotocore-route53globalresolver](https://pypi.org/project/types-aiobotocore-route53globalresolver/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[route53globalresolver]` package installed.

Write your `Route53GlobalResolver` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# Route53GlobalResolverClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53globalresolver") as client:  # (1)
    result = await client.associate_hosted_zone()  # (2)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. result: [:material-code-braces: AssociateHostedZoneOutputTypeDef](./type_defs.md#associatehostedzoneoutputtypedef)



#### Paginator usage example

```python
# ListAccessSourcesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53globalresolver") as client:  # (1)
    paginator = client.get_paginator("list_access_sources")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListAccessSourcesPaginator](./paginators.md#listaccesssourcespaginator)
3. item: [:material-code-braces: ListAccessSourcesOutputTypeDef](./type_defs.md#listaccesssourcesoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[route53globalresolver]`
or a standalone `types_aiobotocore_route53globalresolver` package, you have to explicitly specify
`client: Route53GlobalResolverClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# Route53GlobalResolverClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.client import Route53GlobalResolverClient
from types_aiobotocore_route53globalresolver.type_defs import AssociateHostedZoneOutputTypeDef
from types_aiobotocore_route53globalresolver.type_defs import AssociateHostedZoneInputTypeDef


session = get_session()

async with session.create_client("route53globalresolver") as client:
    client: Route53GlobalResolverClient
    kwargs: AssociateHostedZoneInputTypeDef = {...}
    result: AssociateHostedZoneOutputTypeDef = await client.associate_hosted_zone(**kwargs)
```



#### Paginator usage example

```python
# ListAccessSourcesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.client import Route53GlobalResolverClient
from types_aiobotocore_route53globalresolver.paginator import ListAccessSourcesPaginator
from types_aiobotocore_route53globalresolver.type_defs import ListAccessSourcesOutputTypeDef


session = get_session()

async with session.create_client("route53globalresolver") as client:
    client: Route53GlobalResolverClient
    paginator: ListAccessSourcesPaginator = client.get_paginator("list_access_sources")
    async for item in paginator.paginate(...):
        item: ListAccessSourcesOutputTypeDef
        print(item)
```


