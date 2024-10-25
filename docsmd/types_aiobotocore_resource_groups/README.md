# ResourceGroups module

> [Index](../README.md) > ResourceGroups


!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ResourceGroups` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[resource-groups]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[resource-groups]'


# standalone installation
python -m pip install types-aiobotocore-resource-groups
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-resource-groups
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ResourceGroupsClient

Type annotations and code completion for  `#!python session.create_client("resource-groups")` as [ResourceGroupsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# ResourceGroupsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.client import ResourceGroupsClient


session = get_session()
async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("resource-groups").get_paginator("...")`.

```python
# ListGroupResourcesPaginator usage example

from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator

def get_list_group_resources_paginator() -> ListGroupResourcesPaginator:
    return client.get_paginator("list_group_resources"))
```

- [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
- [ListGroupingStatusesPaginator](./paginators.md#listgroupingstatusespaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListTagSyncTasksPaginator](./paginators.md#listtagsynctaskspaginator)
- [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# GroupConfigurationStatusType usage example

from types_aiobotocore_resource_groups.literals import GroupConfigurationStatusType

def get_value() -> GroupConfigurationStatusType:
    return "UPDATE_COMPLETE"
```

- [GroupConfigurationStatusType](./literals.md#groupconfigurationstatustype)
- [GroupFilterNameType](./literals.md#groupfilternametype)
- [GroupLifecycleEventsDesiredStatusType](./literals.md#grouplifecycleeventsdesiredstatustype)
- [GroupLifecycleEventsStatusType](./literals.md#grouplifecycleeventsstatustype)
- [GroupingStatusType](./literals.md#groupingstatustype)
- [GroupingTypeType](./literals.md#groupingtypetype)
- [ListGroupResourcesPaginatorName](./literals.md#listgroupresourcespaginatorname)
- [ListGroupingStatusesFilterNameType](./literals.md#listgroupingstatusesfilternametype)
- [ListGroupingStatusesPaginatorName](./literals.md#listgroupingstatusespaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListTagSyncTasksPaginatorName](./literals.md#listtagsynctaskspaginatorname)
- [QueryErrorCodeType](./literals.md#queryerrorcodetype)
- [QueryTypeType](./literals.md#querytypetype)
- [ResourceFilterNameType](./literals.md#resourcefilternametype)
- [ResourceStatusValueType](./literals.md#resourcestatusvaluetype)
- [SearchResourcesPaginatorName](./literals.md#searchresourcespaginatorname)
- [TagSyncTaskStatusType](./literals.md#tagsynctaskstatustype)
- [ResourceGroupsServiceName](./literals.md#resourcegroupsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef)
- [CancelTagSyncTaskInputRequestTypeDef](./type_defs.md#canceltagsynctaskinputrequesttypedef)
- [ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteGroupInputRequestTypeDef](./type_defs.md#deletegroupinputrequesttypedef)
- [FailedResourceTypeDef](./type_defs.md#failedresourcetypedef)
- [GetGroupConfigurationInputRequestTypeDef](./type_defs.md#getgroupconfigurationinputrequesttypedef)
- [GetGroupInputRequestTypeDef](./type_defs.md#getgroupinputrequesttypedef)
- [GetGroupQueryInputRequestTypeDef](./type_defs.md#getgroupqueryinputrequesttypedef)
- [GetTagSyncTaskInputRequestTypeDef](./type_defs.md#gettagsynctaskinputrequesttypedef)
- [GetTagsInputRequestTypeDef](./type_defs.md#gettagsinputrequesttypedef)
- [GroupConfigurationParameterOutputTypeDef](./type_defs.md#groupconfigurationparameteroutputtypedef)
- [GroupConfigurationParameterTypeDef](./type_defs.md#groupconfigurationparametertypedef)
- [GroupFilterTypeDef](./type_defs.md#groupfiltertypedef)
- [GroupIdentifierTypeDef](./type_defs.md#groupidentifiertypedef)
- [GroupResourcesInputRequestTypeDef](./type_defs.md#groupresourcesinputrequesttypedef)
- [PendingResourceTypeDef](./type_defs.md#pendingresourcetypedef)
- [GroupingStatusesItemTypeDef](./type_defs.md#groupingstatusesitemtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef)
- [ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef)
- [ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef)
- [QueryErrorTypeDef](./type_defs.md#queryerrortypedef)
- [ListGroupingStatusesFilterTypeDef](./type_defs.md#listgroupingstatusesfiltertypedef)
- [ListTagSyncTasksFilterTypeDef](./type_defs.md#listtagsynctasksfiltertypedef)
- [TagSyncTaskItemTypeDef](./type_defs.md#tagsynctaskitemtypedef)
- [StartTagSyncTaskInputRequestTypeDef](./type_defs.md#starttagsynctaskinputrequesttypedef)
- [TagInputRequestTypeDef](./type_defs.md#taginputrequesttypedef)
- [UngroupResourcesInputRequestTypeDef](./type_defs.md#ungroupresourcesinputrequesttypedef)
- [UntagInputRequestTypeDef](./type_defs.md#untaginputrequesttypedef)
- [UpdateAccountSettingsInputRequestTypeDef](./type_defs.md#updateaccountsettingsinputrequesttypedef)
- [UpdateGroupInputRequestTypeDef](./type_defs.md#updategroupinputrequesttypedef)
- [GroupQueryTypeDef](./type_defs.md#groupquerytypedef)
- [SearchResourcesInputRequestTypeDef](./type_defs.md#searchresourcesinputrequesttypedef)
- [UpdateGroupQueryInputRequestTypeDef](./type_defs.md#updategroupqueryinputrequesttypedef)
- [DeleteGroupOutputTypeDef](./type_defs.md#deletegroupoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAccountSettingsOutputTypeDef](./type_defs.md#getaccountsettingsoutputtypedef)
- [GetGroupOutputTypeDef](./type_defs.md#getgroupoutputtypedef)
- [GetTagSyncTaskOutputTypeDef](./type_defs.md#gettagsynctaskoutputtypedef)
- [GetTagsOutputTypeDef](./type_defs.md#gettagsoutputtypedef)
- [StartTagSyncTaskOutputTypeDef](./type_defs.md#starttagsynctaskoutputtypedef)
- [TagOutputTypeDef](./type_defs.md#tagoutputtypedef)
- [UntagOutputTypeDef](./type_defs.md#untagoutputtypedef)
- [UpdateAccountSettingsOutputTypeDef](./type_defs.md#updateaccountsettingsoutputtypedef)
- [UpdateGroupOutputTypeDef](./type_defs.md#updategroupoutputtypedef)
- [GroupConfigurationItemOutputTypeDef](./type_defs.md#groupconfigurationitemoutputtypedef)
- [GroupConfigurationParameterUnionTypeDef](./type_defs.md#groupconfigurationparameteruniontypedef)
- [ListGroupsInputRequestTypeDef](./type_defs.md#listgroupsinputrequesttypedef)
- [ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef)
- [GroupResourcesOutputTypeDef](./type_defs.md#groupresourcesoutputtypedef)
- [UngroupResourcesOutputTypeDef](./type_defs.md#ungroupresourcesoutputtypedef)
- [ListGroupingStatusesOutputTypeDef](./type_defs.md#listgroupingstatusesoutputtypedef)
- [ListGroupsInputListGroupsPaginateTypeDef](./type_defs.md#listgroupsinputlistgroupspaginatetypedef)
- [SearchResourcesInputSearchResourcesPaginateTypeDef](./type_defs.md#searchresourcesinputsearchresourcespaginatetypedef)
- [ListGroupResourcesInputListGroupResourcesPaginateTypeDef](./type_defs.md#listgroupresourcesinputlistgroupresourcespaginatetypedef)
- [ListGroupResourcesInputRequestTypeDef](./type_defs.md#listgroupresourcesinputrequesttypedef)
- [ListGroupResourcesItemTypeDef](./type_defs.md#listgroupresourcesitemtypedef)
- [SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef)
- [ListGroupingStatusesInputListGroupingStatusesPaginateTypeDef](./type_defs.md#listgroupingstatusesinputlistgroupingstatusespaginatetypedef)
- [ListGroupingStatusesInputRequestTypeDef](./type_defs.md#listgroupingstatusesinputrequesttypedef)
- [ListTagSyncTasksInputListTagSyncTasksPaginateTypeDef](./type_defs.md#listtagsynctasksinputlisttagsynctaskspaginatetypedef)
- [ListTagSyncTasksInputRequestTypeDef](./type_defs.md#listtagsynctasksinputrequesttypedef)
- [ListTagSyncTasksOutputTypeDef](./type_defs.md#listtagsynctasksoutputtypedef)
- [GetGroupQueryOutputTypeDef](./type_defs.md#getgroupqueryoutputtypedef)
- [UpdateGroupQueryOutputTypeDef](./type_defs.md#updategroupqueryoutputtypedef)
- [GroupConfigurationTypeDef](./type_defs.md#groupconfigurationtypedef)
- [GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef)
- [ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef)
- [CreateGroupOutputTypeDef](./type_defs.md#creategroupoutputtypedef)
- [GetGroupConfigurationOutputTypeDef](./type_defs.md#getgroupconfigurationoutputtypedef)
- [GroupConfigurationItemUnionTypeDef](./type_defs.md#groupconfigurationitemuniontypedef)
- [PutGroupConfigurationInputRequestTypeDef](./type_defs.md#putgroupconfigurationinputrequesttypedef)
- [CreateGroupInputRequestTypeDef](./type_defs.md#creategroupinputrequesttypedef)

