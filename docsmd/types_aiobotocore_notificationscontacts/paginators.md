# Paginators

> [Index](../README.md) > [UserNotificationsContacts](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [UserNotificationsContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#usernotificationscontacts)
    type annotations stubs module [types-aiobotocore-notificationscontacts](https://pypi.org/project/types-aiobotocore-notificationscontacts/).

## ListEmailContactsPaginator

Type annotations and code completion for `#!python session.create_client("notificationscontacts").get_paginator("list_email_contacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/paginator/ListEmailContacts.html#UserNotificationsContacts.Paginator.ListEmailContacts)

```python
# ListEmailContactsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_notificationscontacts.paginator import ListEmailContactsPaginator

session = get_session()
async with session.create_client("notificationscontacts") as client:  # (1)
    paginator: ListEmailContactsPaginator = client.get_paginator("list_email_contacts")  # (2)
    async for item in paginator.paginate(...):
        item: ListEmailContactsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsContactsClient](./client.md)
2. paginator: [ListEmailContactsPaginator](./paginators.md#listemailcontactspaginator)
3. item: [:material-code-braces: ListEmailContactsResponseTypeDef](./type_defs.md#listemailcontactsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEmailContactsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEmailContactsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEmailContactsResponseTypeDef](./type_defs.md#listemailcontactsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEmailContactsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEmailContactsRequestPaginateTypeDef](./type_defs.md#listemailcontactsrequestpaginatetypedef) 
