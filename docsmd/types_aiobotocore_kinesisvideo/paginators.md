# Paginators

> [Index](../README.md) > [KinesisVideo](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#kinesisvideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## DescribeMappedResourceConfigurationPaginator

Type annotations and code completion for `#!python session.create_client("kinesisvideo").get_paginator("describe_mapped_resource_configuration")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo/paginator/DescribeMappedResourceConfiguration.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration)

```python
# DescribeMappedResourceConfigurationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.paginator import DescribeMappedResourceConfigurationPaginator

session = get_session()
async with session.create_client("kinesisvideo") as client:  # (1)
    paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMappedResourceConfigurationOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoClient](./client.md)
2. paginator: [DescribeMappedResourceConfigurationPaginator](./paginators.md#describemappedresourceconfigurationpaginator)
3. item: [:material-code-braces: DescribeMappedResourceConfigurationOutputTypeDef](./type_defs.md#describemappedresourceconfigurationoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeMappedResourceConfigurationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeMappedResourceConfigurationOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMappedResourceConfigurationOutputTypeDef](./type_defs.md#describemappedresourceconfigurationoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMappedResourceConfigurationInputPaginateTypeDef = {  # (1)
    "StreamName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMappedResourceConfigurationInputPaginateTypeDef](./type_defs.md#describemappedresourceconfigurationinputpaginatetypedef) 
## ListEdgeAgentConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("kinesisvideo").get_paginator("list_edge_agent_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo/paginator/ListEdgeAgentConfigurations.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations)

```python
# ListEdgeAgentConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.paginator import ListEdgeAgentConfigurationsPaginator

session = get_session()
async with session.create_client("kinesisvideo") as client:  # (1)
    paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListEdgeAgentConfigurationsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoClient](./client.md)
2. paginator: [ListEdgeAgentConfigurationsPaginator](./paginators.md#listedgeagentconfigurationspaginator)
3. item: [:material-code-braces: ListEdgeAgentConfigurationsOutputTypeDef](./type_defs.md#listedgeagentconfigurationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEdgeAgentConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HubDeviceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEdgeAgentConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEdgeAgentConfigurationsOutputTypeDef](./type_defs.md#listedgeagentconfigurationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEdgeAgentConfigurationsInputPaginateTypeDef = {  # (1)
    "HubDeviceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEdgeAgentConfigurationsInputPaginateTypeDef](./type_defs.md#listedgeagentconfigurationsinputpaginatetypedef) 
## ListSignalingChannelsPaginator

Type annotations and code completion for `#!python session.create_client("kinesisvideo").get_paginator("list_signaling_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo/paginator/ListSignalingChannels.html#KinesisVideo.Paginator.ListSignalingChannels)

```python
# ListSignalingChannelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.paginator import ListSignalingChannelsPaginator

session = get_session()
async with session.create_client("kinesisvideo") as client:  # (1)
    paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListSignalingChannelsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoClient](./client.md)
2. paginator: [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
3. item: [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSignalingChannelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChannelNameCondition: ChannelNameConditionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSignalingChannelsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ChannelNameConditionTypeDef](./type_defs.md#channelnameconditiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSignalingChannelsInputPaginateTypeDef = {  # (1)
    "ChannelNameCondition": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSignalingChannelsInputPaginateTypeDef](./type_defs.md#listsignalingchannelsinputpaginatetypedef) 
## ListStreamsPaginator

Type annotations and code completion for `#!python session.create_client("kinesisvideo").get_paginator("list_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo/paginator/ListStreams.html#KinesisVideo.Paginator.ListStreams)

```python
# ListStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesisvideo.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("kinesisvideo") as client:  # (1)
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisVideoClient](./client.md)
2. paginator: [ListStreamsPaginator](./paginators.md#liststreamspaginator)
3. item: [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StreamNameCondition: StreamNameConditionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListStreamsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: StreamNameConditionTypeDef](./type_defs.md#streamnameconditiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamsInputPaginateTypeDef = {  # (1)
    "StreamNameCondition": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamsInputPaginateTypeDef](./type_defs.md#liststreamsinputpaginatetypedef) 
