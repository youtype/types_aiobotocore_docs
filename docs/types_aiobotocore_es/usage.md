<a id="examples-for-aiobotocore-elasticsearchservice-module"></a>

# Examples for aiobotocore ElasticsearchService module

> [Index](../README.md) > [ElasticsearchService](./README.md) > Examples

- [Examples for aiobotocore ElasticsearchService module](#examples-for-aiobotocore-elasticsearchservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[es]` package installed.

Write your `ElasticsearchService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ElasticsearchServiceClient
# and provides type checking and code completion
async with session.create_client("es") as client:
    
    # result has type AcceptInboundCrossClusterSearchConnectionResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_inbound_cross_cluster_search_connection()
    

    
    # paginator has type DescribeReservedElasticsearchInstanceOfferingsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_reserved_elasticsearch_instance_offerings")
    async for item in paginator.paginate(...):
        # item has type DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[es]` or a standalone `types_aiobotocore_es`
package, you have to explicitly specify `client: ElasticsearchServiceClient`
type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_es.client import ElasticsearchServiceClient
from types_aiobotocore_es.type_defs import AcceptInboundCrossClusterSearchConnectionResponseTypeDef
from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstanceOfferingsPaginator

from types_aiobotocore_es.literals import PaginatorName



session = get_session()

async with session.create_client("es") as client:
    client: ElasticsearchServiceClient

    
    result: AcceptInboundCrossClusterSearchConnectionResponseTypeDef = client.accept_inbound_cross_cluster_search_connection()
    

    
    paginator_name: PaginatorName = "describe_reserved_elasticsearch_instance_offerings"
    paginator: DescribeReservedElasticsearchInstanceOfferingsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef
        print(item)
    

    
```
