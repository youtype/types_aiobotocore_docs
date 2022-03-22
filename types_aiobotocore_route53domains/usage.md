<a id="examples-for-aiobotocore-route53domains-module"></a>

# Examples for aiobotocore Route53Domains module

> [Index](../README.md) > [Route53Domains](./README.md) > Examples

- [Examples for aiobotocore Route53Domains module](#examples-for-aiobotocore-route53domains-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[route53domains]` package installed.

Write your `Route53Domains` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Route53DomainsClient
# and provides type checking and code completion
async with session.create_client("route53domains") as client:
    
    # result has type AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_domain_transfer_from_another_aws_account()
    

    
    # paginator has type ListDomainsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_domains")
    async for item in paginator.paginate(...):
        # item has type ListDomainsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[route53domains]` or a standalone
`types_aiobotocore_route53domains` package, you have to explicitly specify
`client: Route53DomainsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53domains.client import Route53DomainsClient
from types_aiobotocore_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef
from types_aiobotocore_route53domains.paginator import ListDomainsPaginator

from types_aiobotocore_route53domains.literals import PaginatorName



session = get_session()

async with session.create_client("route53domains") as client:
    client: Route53DomainsClient

    
    result: AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = client.accept_domain_transfer_from_another_aws_account()
    

    
    paginator_name: PaginatorName = "list_domains"
    paginator: ListDomainsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)
    

    
```
