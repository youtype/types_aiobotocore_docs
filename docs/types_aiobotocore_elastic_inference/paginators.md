<a id="paginators-for-aiobotocore-elasticinference-module"></a>

# Paginators for aiobotocore ElasticInference module

> [Index](../README.md) > [ElasticInference](./README.md) > Paginators

Auto-generated documentation for
[ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
type annotations stubs module
[types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).

- [Paginators for aiobotocore ElasticInference module](#paginators-for-aiobotocore-elasticinference-module)
  - [DescribeAcceleratorsPaginator](#describeacceleratorspaginator)

<a id="describeacceleratorspaginator"></a>

## DescribeAcceleratorsPaginator

Type annotations for
`session.create_client("elastic-inference").get_paginator("describe_accelerators")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elastic_inference.paginator import DescribeAcceleratorsPaginator

session = get_session()
async with session.create_client("elastic-inference") as client:
    client: ElasticInferenceClient
    paginator: DescribeAcceleratorsPaginator = client.get_paginator("describe_accelerators")
```

Boto3 documentation:
[ElasticInference.Paginator.DescribeAccelerators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators)

Arguments for `DescribeAcceleratorsPaginator.paginate` method:

- `acceleratorIds`: `Sequence`\[`str`\]
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAcceleratorsPaginator.paginate` returns
`AsyncIterator`\[[DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef)\].
