# Examples

> [Index](../README.md) > [SSMContacts](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSMContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#ssmcontacts)
    type annotations stubs module [types-aiobotocore-ssm-contacts](https://pypi.org/project/types-aiobotocore-ssm-contacts/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ssm-contacts]` package installed.

Write your `SSMContacts` code as usual,
type checking and code completion should work out of the box.



```python
# SSMContactsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-contacts") as client:  # (1)
    result = await client.create_contact()  # (2)
```

1. client: [SSMContactsClient](./client.md)
2. result: [:material-code-braces: CreateContactResultTypeDef](./type_defs.md#createcontactresulttypedef) 



```python
# ListContactChannelsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-contacts") as client:  # (1)
    paginator = client.get_paginator("list_contact_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SSMContactsClient](./client.md)
2. paginator: [ListContactChannelsPaginator](./paginators.md#listcontactchannelspaginator)
3. item: [:material-code-braces: ListContactChannelsResultTypeDef](./type_defs.md#listcontactchannelsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ssm-contacts]`
or a standalone `types_aiobotocore_ssm_contacts` package, you have to explicitly specify
`client: SSMContactsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SSMContactsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_contacts.client import SSMContactsClient
from types_aiobotocore_ssm_contacts.type_defs import CreateContactResultTypeDef
from types_aiobotocore_ssm_contacts.type_defs import CreateContactRequestTypeDef


session = get_session()

async with session.create_client("ssm-contacts") as client:
    client: SSMContactsClient
    kwargs: CreateContactRequestTypeDef = {...}
    result: CreateContactResultTypeDef = await client.create_contact(**kwargs)
```



```python
# ListContactChannelsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_contacts.client import SSMContactsClient
from types_aiobotocore_ssm_contacts.paginator import ListContactChannelsPaginator
from types_aiobotocore_ssm_contacts.type_defs import ListContactChannelsResultTypeDef


session = get_session()

async with session.create_client("ssm-contacts") as client:
    client: SSMContactsClient
    paginator: ListContactChannelsPaginator = client.get_paginator("list_contact_channels")
    async for item in paginator.paginate(...):
        item: ListContactChannelsResultTypeDef
        print(item)
```


