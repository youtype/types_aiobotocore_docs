# Examples

> [Index](../README.md) > [SageMaker](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SageMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#sagemaker)
    type annotations stubs module [types-aiobotocore-sagemaker](https://pypi.org/project/types-aiobotocore-sagemaker/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker]` package installed.

Write your `SageMaker` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SageMakerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sagemaker") as client:  # (1)
    result = await client.add_association()  # (2)
```

1. client: [SageMakerClient](./client.md)
2. result: [:material-code-braces: AddAssociationResponseTypeDef](./type_defs.md#addassociationresponsetypedef)



#### Paginator usage example

```python
# CreateHubContentPresignedUrlsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sagemaker") as client:  # (1)
    paginator = client.get_paginator("create_hub_content_presigned_urls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SageMakerClient](./client.md)
2. paginator: [CreateHubContentPresignedUrlsPaginator](./paginators.md#createhubcontentpresignedurlspaginator)
3. item: [:material-code-braces: CreateHubContentPresignedUrlsResponseTypeDef](./type_defs.md#createhubcontentpresignedurlsresponsetypedef)



#### Waiter usage example

```python
# EndpointDeletedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sagemaker") as client:  # (1)
    waiter = client.get_waiter("endpoint_deleted")  # (2)
    await waiter.wait(...)
```

1. client: [SageMakerClient](./client.md)
2. waiter: [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[sagemaker]`
or a standalone `types_aiobotocore_sagemaker` package, you have to explicitly specify
`client: SageMakerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SageMakerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker.client import SageMakerClient
from types_aiobotocore_sagemaker.type_defs import AddAssociationResponseTypeDef
from types_aiobotocore_sagemaker.type_defs import AddAssociationRequestTypeDef


session = get_session()

async with session.create_client("sagemaker") as client:
    client: SageMakerClient
    kwargs: AddAssociationRequestTypeDef = {...}
    result: AddAssociationResponseTypeDef = await client.add_association(**kwargs)
```



#### Paginator usage example

```python
# CreateHubContentPresignedUrlsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker.client import SageMakerClient
from types_aiobotocore_sagemaker.paginator import CreateHubContentPresignedUrlsPaginator
from types_aiobotocore_sagemaker.type_defs import CreateHubContentPresignedUrlsResponseTypeDef


session = get_session()

async with session.create_client("sagemaker") as client:
    client: SageMakerClient
    paginator: CreateHubContentPresignedUrlsPaginator = client.get_paginator("create_hub_content_presigned_urls")
    async for item in paginator.paginate(...):
        item: CreateHubContentPresignedUrlsResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# EndpointDeletedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker.client import SageMakerClient
from types_aiobotocore_sagemaker.waiter import EndpointDeletedWaiter


session = get_session()

async with session.create_client("sagemaker") as client:
    client: SageMakerClient
    waiter: EndpointDeletedWaiter = client.get_waiter("endpoint_deleted")
    await waiter.wait(...)
```
