<a id="paginators-for-aiobotocore-mq-module"></a>

# Paginators for aiobotocore MQ module

> [Index](..) > [MQ](.) > Paginators

Auto-generated documentation for
[MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
type annotations stubs module
[types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

- [Paginators for aiobotocore MQ module](#paginators-for-aiobotocore-mq-module)
  - [ListBrokersPaginator](#listbrokerspaginator)

<a id="listbrokerspaginator"></a>

## ListBrokersPaginator

Type annotations for
`session.create_client("mq").get_paginator("list_brokers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mq.paginator import ListBrokersPaginator

session = get_session()
async with session.create_client("mq") as client:
    client: MQClient
    paginator: ListBrokersPaginator = client.get_paginator("list_brokers")
```

Boto3 documentation:
[MQ.Paginator.ListBrokers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers)

Arguments for `ListBrokersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBrokersPaginator.paginate` returns
`_PageIterator`\[[ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef)\].
