# Examples

> [Index](../README.md) > [KinesisVideo](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#kinesisvideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesisvideo]` package installed.

Write your `KinesisVideo` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisVideoClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesisvideo") as client:  # (1)
    result = await client.create_signaling_channel()  # (2)
```

1. client: [KinesisVideoClient](./client.md)
2. result: [:material-code-braces: CreateSignalingChannelOutputTypeDef](./type_defs.md#createsignalingchanneloutputtypedef) 



```python
# DescribeMappedResourceConfigurationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesisvideo") as client:  # (1)
    paginator = client.get_paginator("describe_mapped_resource_configuration")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KinesisVideoClient](./client.md)
2. paginator: [DescribeMappedResourceConfigurationPaginator](./paginators.md#describemappedresourceconfigurationpaginator)
3. item: [:material-code-braces: DescribeMappedResourceConfigurationOutputTypeDef](./type_defs.md#describemappedresourceconfigurationoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kinesisvideo]`
or a standalone `types_aiobotocore_kinesisvideo` package, you have to explicitly specify
`client: KinesisVideoClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisVideoClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
from types_aiobotocore_kinesisvideo.type_defs import CreateSignalingChannelOutputTypeDef
from types_aiobotocore_kinesisvideo.type_defs import CreateSignalingChannelInputTypeDef


session = get_session()

async with session.create_client("kinesisvideo") as client:
    client: KinesisVideoClient
    kwargs: CreateSignalingChannelInputTypeDef = {...}
    result: CreateSignalingChannelOutputTypeDef = await client.create_signaling_channel(**kwargs)
```



```python
# DescribeMappedResourceConfigurationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
from types_aiobotocore_kinesisvideo.paginator import DescribeMappedResourceConfigurationPaginator
from types_aiobotocore_kinesisvideo.type_defs import DescribeMappedResourceConfigurationOutputTypeDef


session = get_session()

async with session.create_client("kinesisvideo") as client:
    client: KinesisVideoClient
    paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
    async for item in paginator.paginate(...):
        item: DescribeMappedResourceConfigurationOutputTypeDef
        print(item)
```


