<a id="examples-for-aiobotocore-codeartifact-module"></a>

# Examples for aiobotocore CodeArtifact module

> [Index](../README.md) > [CodeArtifact](./README.md) > Examples

- [Examples for aiobotocore CodeArtifact module](#examples-for-aiobotocore-codeartifact-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codeartifact]` package installed.

Write your `CodeArtifact` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeArtifactClient
# and provides type checking and code completion
async with session.create_client("codeartifact") as client:
    
    # result has type AssociateExternalConnectionResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_external_connection()
    

    
    # paginator has type ListDomainsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_domains")
    async for item in paginator.paginate(...):
        # item has type ListDomainsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codeartifact]` or a standalone
`types_aiobotocore_codeartifact` package, you have to explicitly specify
`client: CodeArtifactClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.client import CodeArtifactClient
from types_aiobotocore_codeartifact.type_defs import AssociateExternalConnectionResultTypeDef
from types_aiobotocore_codeartifact.paginator import ListDomainsPaginator

from types_aiobotocore_codeartifact.literals import PaginatorName



session = get_session()

async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient

    
    result: AssociateExternalConnectionResultTypeDef = client.associate_external_connection()
    

    
    paginator_name: PaginatorName = "list_domains"
    paginator: ListDomainsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDomainsResultTypeDef
        print(item)
    

    
```
