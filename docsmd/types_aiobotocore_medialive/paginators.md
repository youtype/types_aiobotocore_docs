# Paginators

> [Index](../README.md) > [MediaLive](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#medialive)
    type annotations stubs module [types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).

## DescribeSchedulePaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("describe_schedule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/DescribeSchedule.html#MediaLive.Paginator.DescribeSchedule)

```python
# DescribeSchedulePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import DescribeSchedulePaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScheduleResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [DescribeSchedulePaginator](./paginators.md#describeschedulepaginator)
3. item: [:material-code-braces: DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSchedulePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChannelId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeScheduleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScheduleRequestPaginateTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduleRequestPaginateTypeDef](./type_defs.md#describeschedulerequestpaginatetypedef) 
## ListChannelPlacementGroupsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_channel_placement_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListChannelPlacementGroups.html#MediaLive.Paginator.ListChannelPlacementGroups)

```python
# ListChannelPlacementGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListChannelPlacementGroupsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListChannelPlacementGroupsPaginator = client.get_paginator("list_channel_placement_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelPlacementGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListChannelPlacementGroupsPaginator](./paginators.md#listchannelplacementgroupspaginator)
3. item: [:material-code-braces: ListChannelPlacementGroupsResponseTypeDef](./type_defs.md#listchannelplacementgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelPlacementGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListChannelPlacementGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelPlacementGroupsResponseTypeDef](./type_defs.md#listchannelplacementgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelPlacementGroupsRequestPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelPlacementGroupsRequestPaginateTypeDef](./type_defs.md#listchannelplacementgroupsrequestpaginatetypedef) 
## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListChannels.html#MediaLive.Paginator.ListChannels)

```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestPaginateTypeDef](./type_defs.md#listchannelsrequestpaginatetypedef) 
## ListCloudWatchAlarmTemplateGroupsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_cloud_watch_alarm_template_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListCloudWatchAlarmTemplateGroups.html#MediaLive.Paginator.ListCloudWatchAlarmTemplateGroups)

```python
# ListCloudWatchAlarmTemplateGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListCloudWatchAlarmTemplateGroupsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListCloudWatchAlarmTemplateGroupsPaginator = client.get_paginator("list_cloud_watch_alarm_template_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListCloudWatchAlarmTemplateGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListCloudWatchAlarmTemplateGroupsPaginator](./paginators.md#listcloudwatchalarmtemplategroupspaginator)
3. item: [:material-code-braces: ListCloudWatchAlarmTemplateGroupsResponseTypeDef](./type_defs.md#listcloudwatchalarmtemplategroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCloudWatchAlarmTemplateGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Scope: str = ...,
    SignalMapIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCloudWatchAlarmTemplateGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCloudWatchAlarmTemplateGroupsResponseTypeDef](./type_defs.md#listcloudwatchalarmtemplategroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCloudWatchAlarmTemplateGroupsRequestPaginateTypeDef = {  # (1)
    "Scope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCloudWatchAlarmTemplateGroupsRequestPaginateTypeDef](./type_defs.md#listcloudwatchalarmtemplategroupsrequestpaginatetypedef) 
## ListCloudWatchAlarmTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_cloud_watch_alarm_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListCloudWatchAlarmTemplates.html#MediaLive.Paginator.ListCloudWatchAlarmTemplates)

```python
# ListCloudWatchAlarmTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListCloudWatchAlarmTemplatesPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListCloudWatchAlarmTemplatesPaginator = client.get_paginator("list_cloud_watch_alarm_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCloudWatchAlarmTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListCloudWatchAlarmTemplatesPaginator](./paginators.md#listcloudwatchalarmtemplatespaginator)
3. item: [:material-code-braces: ListCloudWatchAlarmTemplatesResponseTypeDef](./type_defs.md#listcloudwatchalarmtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCloudWatchAlarmTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupIdentifier: str = ...,
    Scope: str = ...,
    SignalMapIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCloudWatchAlarmTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCloudWatchAlarmTemplatesResponseTypeDef](./type_defs.md#listcloudwatchalarmtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCloudWatchAlarmTemplatesRequestPaginateTypeDef = {  # (1)
    "GroupIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCloudWatchAlarmTemplatesRequestPaginateTypeDef](./type_defs.md#listcloudwatchalarmtemplatesrequestpaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListClusters.html#MediaLive.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef) 
## ListEventBridgeRuleTemplateGroupsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_event_bridge_rule_template_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListEventBridgeRuleTemplateGroups.html#MediaLive.Paginator.ListEventBridgeRuleTemplateGroups)

```python
# ListEventBridgeRuleTemplateGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListEventBridgeRuleTemplateGroupsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListEventBridgeRuleTemplateGroupsPaginator = client.get_paginator("list_event_bridge_rule_template_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventBridgeRuleTemplateGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListEventBridgeRuleTemplateGroupsPaginator](./paginators.md#listeventbridgeruletemplategroupspaginator)
3. item: [:material-code-braces: ListEventBridgeRuleTemplateGroupsResponseTypeDef](./type_defs.md#listeventbridgeruletemplategroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventBridgeRuleTemplateGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SignalMapIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventBridgeRuleTemplateGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventBridgeRuleTemplateGroupsResponseTypeDef](./type_defs.md#listeventbridgeruletemplategroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventBridgeRuleTemplateGroupsRequestPaginateTypeDef = {  # (1)
    "SignalMapIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventBridgeRuleTemplateGroupsRequestPaginateTypeDef](./type_defs.md#listeventbridgeruletemplategroupsrequestpaginatetypedef) 
## ListEventBridgeRuleTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_event_bridge_rule_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListEventBridgeRuleTemplates.html#MediaLive.Paginator.ListEventBridgeRuleTemplates)

```python
# ListEventBridgeRuleTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListEventBridgeRuleTemplatesPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListEventBridgeRuleTemplatesPaginator = client.get_paginator("list_event_bridge_rule_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventBridgeRuleTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListEventBridgeRuleTemplatesPaginator](./paginators.md#listeventbridgeruletemplatespaginator)
3. item: [:material-code-braces: ListEventBridgeRuleTemplatesResponseTypeDef](./type_defs.md#listeventbridgeruletemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventBridgeRuleTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupIdentifier: str = ...,
    SignalMapIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventBridgeRuleTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventBridgeRuleTemplatesResponseTypeDef](./type_defs.md#listeventbridgeruletemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventBridgeRuleTemplatesRequestPaginateTypeDef = {  # (1)
    "GroupIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventBridgeRuleTemplatesRequestPaginateTypeDef](./type_defs.md#listeventbridgeruletemplatesrequestpaginatetypedef) 
## ListInputDeviceTransfersPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_input_device_transfers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListInputDeviceTransfers.html#MediaLive.Paginator.ListInputDeviceTransfers)

```python
# ListInputDeviceTransfersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputDeviceTransfersPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListInputDeviceTransfersPaginator = client.get_paginator("list_input_device_transfers")  # (2)
    async for item in paginator.paginate(...):
        item: ListInputDeviceTransfersResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListInputDeviceTransfersPaginator](./paginators.md#listinputdevicetransferspaginator)
3. item: [:material-code-braces: ListInputDeviceTransfersResponseTypeDef](./type_defs.md#listinputdevicetransfersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInputDeviceTransfersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransferType: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInputDeviceTransfersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputDeviceTransfersResponseTypeDef](./type_defs.md#listinputdevicetransfersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInputDeviceTransfersRequestPaginateTypeDef = {  # (1)
    "TransferType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputDeviceTransfersRequestPaginateTypeDef](./type_defs.md#listinputdevicetransfersrequestpaginatetypedef) 
## ListInputDevicesPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_input_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListInputDevices.html#MediaLive.Paginator.ListInputDevices)

```python
# ListInputDevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputDevicesPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListInputDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListInputDevicesPaginator](./paginators.md#listinputdevicespaginator)
3. item: [:material-code-braces: ListInputDevicesResponseTypeDef](./type_defs.md#listinputdevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInputDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInputDevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputDevicesResponseTypeDef](./type_defs.md#listinputdevicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInputDevicesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputDevicesRequestPaginateTypeDef](./type_defs.md#listinputdevicesrequestpaginatetypedef) 
## ListInputSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_input_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListInputSecurityGroups.html#MediaLive.Paginator.ListInputSecurityGroups)

```python
# ListInputSecurityGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputSecurityGroupsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListInputSecurityGroupsPaginator = client.get_paginator("list_input_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListInputSecurityGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListInputSecurityGroupsPaginator](./paginators.md#listinputsecuritygroupspaginator)
3. item: [:material-code-braces: ListInputSecurityGroupsResponseTypeDef](./type_defs.md#listinputsecuritygroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInputSecurityGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInputSecurityGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputSecurityGroupsResponseTypeDef](./type_defs.md#listinputsecuritygroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInputSecurityGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputSecurityGroupsRequestPaginateTypeDef](./type_defs.md#listinputsecuritygroupsrequestpaginatetypedef) 
## ListInputsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_inputs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListInputs.html#MediaLive.Paginator.ListInputs)

```python
# ListInputsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListInputsPaginator = client.get_paginator("list_inputs")  # (2)
    async for item in paginator.paginate(...):
        item: ListInputsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListInputsPaginator](./paginators.md#listinputspaginator)
3. item: [:material-code-braces: ListInputsResponseTypeDef](./type_defs.md#listinputsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInputsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInputsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputsResponseTypeDef](./type_defs.md#listinputsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInputsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputsRequestPaginateTypeDef](./type_defs.md#listinputsrequestpaginatetypedef) 
## ListMultiplexProgramsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_multiplex_programs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListMultiplexPrograms.html#MediaLive.Paginator.ListMultiplexPrograms)

```python
# ListMultiplexProgramsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListMultiplexProgramsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListMultiplexProgramsPaginator = client.get_paginator("list_multiplex_programs")  # (2)
    async for item in paginator.paginate(...):
        item: ListMultiplexProgramsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListMultiplexProgramsPaginator](./paginators.md#listmultiplexprogramspaginator)
3. item: [:material-code-braces: ListMultiplexProgramsResponseTypeDef](./type_defs.md#listmultiplexprogramsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMultiplexProgramsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MultiplexId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMultiplexProgramsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMultiplexProgramsResponseTypeDef](./type_defs.md#listmultiplexprogramsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMultiplexProgramsRequestPaginateTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultiplexProgramsRequestPaginateTypeDef](./type_defs.md#listmultiplexprogramsrequestpaginatetypedef) 
## ListMultiplexesPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_multiplexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListMultiplexes.html#MediaLive.Paginator.ListMultiplexes)

```python
# ListMultiplexesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListMultiplexesPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListMultiplexesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListMultiplexesPaginator](./paginators.md#listmultiplexespaginator)
3. item: [:material-code-braces: ListMultiplexesResponseTypeDef](./type_defs.md#listmultiplexesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMultiplexesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMultiplexesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMultiplexesResponseTypeDef](./type_defs.md#listmultiplexesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMultiplexesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultiplexesRequestPaginateTypeDef](./type_defs.md#listmultiplexesrequestpaginatetypedef) 
## ListNetworksPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListNetworks.html#MediaLive.Paginator.ListNetworks)

```python
# ListNetworksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListNetworksPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListNetworksPaginator = client.get_paginator("list_networks")  # (2)
    async for item in paginator.paginate(...):
        item: ListNetworksResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListNetworksPaginator](./paginators.md#listnetworkspaginator)
3. item: [:material-code-braces: ListNetworksResponseTypeDef](./type_defs.md#listnetworksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNetworksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListNetworksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNetworksResponseTypeDef](./type_defs.md#listnetworksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNetworksRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNetworksRequestPaginateTypeDef](./type_defs.md#listnetworksrequestpaginatetypedef) 
## ListNodesPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListNodes.html#MediaLive.Paginator.ListNodes)

```python
# ListNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListNodesPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListNodesPaginator = client.get_paginator("list_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ListNodesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListNodesPaginator](./paginators.md#listnodespaginator)
3. item: [:material-code-braces: ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListNodesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNodesRequestPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNodesRequestPaginateTypeDef](./type_defs.md#listnodesrequestpaginatetypedef) 
## ListOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListOfferings.html#MediaLive.Paginator.ListOfferings)

```python
# ListOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
3. item: [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChannelClass: str = ...,
    ChannelConfiguration: str = ...,
    Codec: str = ...,
    Duration: str = ...,
    MaximumBitrate: str = ...,
    MaximumFramerate: str = ...,
    Resolution: str = ...,
    ResourceType: str = ...,
    SpecialFeature: str = ...,
    VideoQuality: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOfferingsRequestPaginateTypeDef = {  # (1)
    "ChannelClass": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestPaginateTypeDef](./type_defs.md#listofferingsrequestpaginatetypedef) 
## ListReservationsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListReservations.html#MediaLive.Paginator.ListReservations)

```python
# ListReservationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListReservationsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListReservationsPaginator = client.get_paginator("list_reservations")  # (2)
    async for item in paginator.paginate(...):
        item: ListReservationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListReservationsPaginator](./paginators.md#listreservationspaginator)
3. item: [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListReservationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChannelClass: str = ...,
    Codec: str = ...,
    MaximumBitrate: str = ...,
    MaximumFramerate: str = ...,
    Resolution: str = ...,
    ResourceType: str = ...,
    SpecialFeature: str = ...,
    VideoQuality: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListReservationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListReservationsRequestPaginateTypeDef = {  # (1)
    "ChannelClass": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReservationsRequestPaginateTypeDef](./type_defs.md#listreservationsrequestpaginatetypedef) 
## ListSignalMapsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_signal_maps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/paginator/ListSignalMaps.html#MediaLive.Paginator.ListSignalMaps)

```python
# ListSignalMapsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListSignalMapsPaginator

session = get_session()
async with session.create_client("medialive") as client:  # (1)
    paginator: ListSignalMapsPaginator = client.get_paginator("list_signal_maps")  # (2)
    async for item in paginator.paginate(...):
        item: ListSignalMapsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [ListSignalMapsPaginator](./paginators.md#listsignalmapspaginator)
3. item: [:material-code-braces: ListSignalMapsResponseTypeDef](./type_defs.md#listsignalmapsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSignalMapsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CloudWatchAlarmTemplateGroupIdentifier: str = ...,
    EventBridgeRuleTemplateGroupIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSignalMapsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSignalMapsResponseTypeDef](./type_defs.md#listsignalmapsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSignalMapsRequestPaginateTypeDef = {  # (1)
    "CloudWatchAlarmTemplateGroupIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSignalMapsRequestPaginateTypeDef](./type_defs.md#listsignalmapsrequestpaginatetypedef) 
