# Paginators

> [Index](../README.md) > [MQ](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#mq)
    type annotations stubs module [types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

## ListBrokersPaginator

Type annotations and code completion for `#!python session.create_client("mq").get_paginator("list_brokers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq/paginator/ListBrokers.html#MQ.Paginator.ListBrokers)

```python
# ListBrokersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mq.paginator import ListBrokersPaginator

session = get_session()
async with session.create_client("mq") as client:  # (1)
    paginator: ListBrokersPaginator = client.get_paginator("list_brokers")  # (2)
    async for item in paginator.paginate(...):
        item: ListBrokersResponseTypeDef
        print(item)  # (3)
```

1. client: [MQClient](./client.md)
2. paginator: [ListBrokersPaginator](./paginators.md#listbrokerspaginator)
3. item: [:material-code-braces: ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBrokersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBrokersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBrokersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBrokersRequestPaginateTypeDef](./type_defs.md#listbrokersrequestpaginatetypedef) 
