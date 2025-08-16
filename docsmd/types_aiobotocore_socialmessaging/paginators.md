# Paginators

> [Index](../README.md) > [EndUserMessagingSocial](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial)
    type annotations stubs module [types-aiobotocore-socialmessaging](https://pypi.org/project/types-aiobotocore-socialmessaging/).

## ListLinkedWhatsAppBusinessAccountsPaginator

Type annotations and code completion for `#!python session.create_client("socialmessaging").get_paginator("list_linked_whatsapp_business_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/paginator/ListLinkedWhatsAppBusinessAccounts.html#EndUserMessagingSocial.Paginator.ListLinkedWhatsAppBusinessAccounts)

```python
# ListLinkedWhatsAppBusinessAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_socialmessaging.paginator import ListLinkedWhatsAppBusinessAccountsPaginator

session = get_session()
async with session.create_client("socialmessaging") as client:  # (1)
    paginator: ListLinkedWhatsAppBusinessAccountsPaginator = client.get_paginator("list_linked_whatsapp_business_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListLinkedWhatsAppBusinessAccountsOutputTypeDef
        print(item)  # (3)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. paginator: [ListLinkedWhatsAppBusinessAccountsPaginator](./paginators.md#listlinkedwhatsappbusinessaccountspaginator)
3. item: `AioPageIterator[ListLinkedWhatsAppBusinessAccountsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLinkedWhatsAppBusinessAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLinkedWhatsAppBusinessAccountsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLinkedWhatsAppBusinessAccountsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsinputpaginatetypedef)
## ListWhatsAppMessageTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("socialmessaging").get_paginator("list_whatsapp_message_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/paginator/ListWhatsAppMessageTemplates.html#EndUserMessagingSocial.Paginator.ListWhatsAppMessageTemplates)

```python
# ListWhatsAppMessageTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_socialmessaging.paginator import ListWhatsAppMessageTemplatesPaginator

session = get_session()
async with session.create_client("socialmessaging") as client:  # (1)
    paginator: ListWhatsAppMessageTemplatesPaginator = client.get_paginator("list_whatsapp_message_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListWhatsAppMessageTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. paginator: [ListWhatsAppMessageTemplatesPaginator](./paginators.md#listwhatsappmessagetemplatespaginator)
3. item: `AioPageIterator[ListWhatsAppMessageTemplatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWhatsAppMessageTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWhatsAppMessageTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWhatsAppMessageTemplatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWhatsAppMessageTemplatesInputPaginateTypeDef = {  # (1)
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWhatsAppMessageTemplatesInputPaginateTypeDef](./type_defs.md#listwhatsappmessagetemplatesinputpaginatetypedef)
## ListWhatsAppTemplateLibraryPaginator

Type annotations and code completion for `#!python session.create_client("socialmessaging").get_paginator("list_whatsapp_template_library")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/paginator/ListWhatsAppTemplateLibrary.html#EndUserMessagingSocial.Paginator.ListWhatsAppTemplateLibrary)

```python
# ListWhatsAppTemplateLibraryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_socialmessaging.paginator import ListWhatsAppTemplateLibraryPaginator

session = get_session()
async with session.create_client("socialmessaging") as client:  # (1)
    paginator: ListWhatsAppTemplateLibraryPaginator = client.get_paginator("list_whatsapp_template_library")  # (2)
    async for item in paginator.paginate(...):
        item: ListWhatsAppTemplateLibraryOutputTypeDef
        print(item)  # (3)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. paginator: [ListWhatsAppTemplateLibraryPaginator](./paginators.md#listwhatsapptemplatelibrarypaginator)
3. item: `AioPageIterator[ListWhatsAppTemplateLibraryOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWhatsAppTemplateLibraryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    id: str,
    filters: Mapping[str, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWhatsAppTemplateLibraryOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWhatsAppTemplateLibraryOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWhatsAppTemplateLibraryInputPaginateTypeDef = {  # (1)
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWhatsAppTemplateLibraryInputPaginateTypeDef](./type_defs.md#listwhatsapptemplatelibraryinputpaginatetypedef)
