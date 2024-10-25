# Paginators

> [Index](../README.md) > [CustomerProfiles](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## ListEventStreamsPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_event_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams)

```python
# ListEventStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListEventStreamsPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListEventStreamsPaginator = client.get_paginator("list_event_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventStreamsResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListEventStreamsPaginator](./paginators.md#listeventstreamspaginator)
3. item: [:material-code-braces: ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEventStreamsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventStreamsRequestListEventStreamsPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventStreamsRequestListEventStreamsPaginateTypeDef](./type_defs.md#listeventstreamsrequestlisteventstreamspaginatetypedef) 
