# Examples

> [Index](../README.md) > [Route53Domains](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53Domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#route53domains)
    type annotations stubs module [types-aiobotocore-route53domains](https://pypi.org/project/types-aiobotocore-route53domains/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[route53domains]` package installed.

Write your `Route53Domains` code as usual,
type checking and code completion should work out of the box.



```python
# Route53DomainsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53domains") as client:  # (1)
    result = await client.accept_domain_transfer_from_another_aws_account()  # (2)
```

1. client: [Route53DomainsClient](./client.md)
2. result: [:material-code-braces: AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef](./type_defs.md#acceptdomaintransferfromanotherawsaccountresponsetypedef) 



```python
# ListDomainsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53domains") as client:  # (1)
    paginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[route53domains]`
or a standalone `types_aiobotocore_route53domains` package, you have to explicitly specify
`client: Route53DomainsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Route53DomainsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53domains.client import Route53DomainsClient
from types_aiobotocore_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef
from types_aiobotocore_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountRequestTypeDef


session = get_session()

async with session.create_client("route53domains") as client:
    client: Route53DomainsClient
    kwargs: AcceptDomainTransferFromAnotherAwsAccountRequestTypeDef = {...}
    result: AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = await client.accept_domain_transfer_from_another_aws_account(**kwargs)
```



```python
# ListDomainsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53domains.client import Route53DomainsClient
from types_aiobotocore_route53domains.paginator import ListDomainsPaginator
from types_aiobotocore_route53domains.type_defs import ListDomainsResponseTypeDef


session = get_session()

async with session.create_client("route53domains") as client:
    client: Route53DomainsClient
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)
```


