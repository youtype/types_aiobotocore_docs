<a id="examples-for-aiobotocore-ssmcontacts-module"></a>

# Examples for aiobotocore SSMContacts module

> [Index](../README.md) > [SSMContacts](./README.md) > Examples

- [Examples for aiobotocore SSMContacts module](#examples-for-aiobotocore-ssmcontacts-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ssm-contacts]` package installed.

Write your `SSMContacts` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SSMContactsClient
# and provides type checking and code completion
async with session.create_client("ssm-contacts") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_page()
    

    
    # paginator has type ListContactChannelsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_contact_channels")
    async for item in paginator.paginate(...):
        # item has type ListContactChannelsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ssm-contacts]` or a standalone
`types_aiobotocore_ssm_contacts` package, you have to explicitly specify
`client: SSMContactsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ssm_contacts.client import SSMContactsClient
from types_aiobotocore_ssm_contacts.type_defs import Dict[str, Any]
from types_aiobotocore_ssm_contacts.paginator import ListContactChannelsPaginator

from types_aiobotocore_ssm_contacts.literals import PaginatorName



session = get_session()

async with session.create_client("ssm-contacts") as client:
    client: SSMContactsClient

    
    result: Dict[str, Any] = client.accept_page()
    

    
    paginator_name: PaginatorName = "list_contact_channels"
    paginator: ListContactChannelsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListContactChannelsResultTypeDef
        print(item)
    

    
```
