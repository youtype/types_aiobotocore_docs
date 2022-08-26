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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator

def get_list_group_resources_paginator() -> ListGroupResourcesPaginator:
    return client.get_paginator("list_group_resources"))
```

- [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_resource_groups.literals import GroupConfigurationStatusType

def get_value() -> GroupConfigurationStatusType:
    return "UPDATE_COMPLETE"
```

- [GroupConfigurationStatusType](./literals.md#groupconfigurationstatustype)
- [GroupFilterNameType](./literals.md#groupfilternametype)
- [ListGroupResourcesPaginatorName](./literals.md#listgroupresourcespaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [QueryErrorCodeType](./literals.md#queryerrorcodetype)
- [QueryTypeType](./literals.md#querytypetype)
- [ResourceFilterNameType](./literals.md#resourcefilternametype)
- [ResourceStatusValueType](./literals.md#resourcestatusvaluetype)
- [SearchResourcesPaginatorName](./literals.md#searchresourcespaginatorname)
- [ResourceGroupsServiceName](./literals.md#resourcegroupsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_resource_groups.type_defs import ResourceQueryTypeDef

def get_value() -> ResourceQueryTypeDef:
    return {
        "Type": ...,
        "Query": ...,
    }
```

- [ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteGroupInputRequestTypeDef](./type_defs.md#deletegroupinputrequesttypedef)
- [FailedResourceTypeDef](./type_defs.md#failedresourcetypedef)
- [GetGroupConfigurationInputRequestTypeDef](./type_defs.md#getgroupconfigurationinputrequesttypedef)
- [GetGroupInputRequestTypeDef](./type_defs.md#getgroupinputrequesttypedef)
- [GetGroupQueryInputRequestTypeDef](./type_defs.md#getgroupqueryinputrequesttypedef)
- [GetTagsInputRequestTypeDef](./type_defs.md#gettagsinputrequesttypedef)
- [GroupConfigurationParameterTypeDef](./type_defs.md#groupconfigurationparametertypedef)
- [GroupFilterTypeDef](./type_defs.md#groupfiltertypedef)
- [GroupIdentifierTypeDef](./type_defs.md#groupidentifiertypedef)
- [GroupResourcesInputRequestTypeDef](./type_defs.md#groupresourcesinputrequesttypedef)
- [PendingResourceTypeDef](./type_defs.md#pendingresourcetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef)
- [ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef)
- [ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef)
- [QueryErrorTypeDef](./type_defs.md#queryerrortypedef)
- [TagInputRequestTypeDef](./type_defs.md#taginputrequesttypedef)
- [UngroupResourcesInputRequestTypeDef](./type_defs.md#ungroupresourcesinputrequesttypedef)
- [UntagInputRequestTypeDef](./type_defs.md#untaginputrequesttypedef)
- [UpdateGroupInputRequestTypeDef](./type_defs.md#updategroupinputrequesttypedef)
- [GroupQueryTypeDef](./type_defs.md#groupquerytypedef)
- [SearchResourcesInputRequestTypeDef](./type_defs.md#searchresourcesinputrequesttypedef)
- [UpdateGroupQueryInputRequestTypeDef](./type_defs.md#updategroupqueryinputrequesttypedef)
- [DeleteGroupOutputTypeDef](./type_defs.md#deletegroupoutputtypedef)
- [GetGroupOutputTypeDef](./type_defs.md#getgroupoutputtypedef)
- [GetTagsOutputTypeDef](./type_defs.md#gettagsoutputtypedef)
- [TagOutputTypeDef](./type_defs.md#tagoutputtypedef)
- [UntagOutputTypeDef](./type_defs.md#untagoutputtypedef)
- [UpdateGroupOutputTypeDef](./type_defs.md#updategroupoutputtypedef)
- [GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef)
- [ListGroupsInputRequestTypeDef](./type_defs.md#listgroupsinputrequesttypedef)
- [ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef)
- [GroupResourcesOutputTypeDef](./type_defs.md#groupresourcesoutputtypedef)
- [UngroupResourcesOutputTypeDef](./type_defs.md#ungroupresourcesoutputtypedef)
- [ListGroupsInputListGroupsPaginateTypeDef](./type_defs.md#listgroupsinputlistgroupspaginatetypedef)
- [SearchResourcesInputSearchResourcesPaginateTypeDef](./type_defs.md#searchresourcesinputsearchresourcespaginatetypedef)
- [ListGroupResourcesInputListGroupResourcesPaginateTypeDef](./type_defs.md#listgroupresourcesinputlistgroupresourcespaginatetypedef)
- [ListGroupResourcesInputRequestTypeDef](./type_defs.md#listgroupresourcesinputrequesttypedef)
- [ListGroupResourcesItemTypeDef](./type_defs.md#listgroupresourcesitemtypedef)
- [SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef)
- [GetGroupQueryOutputTypeDef](./type_defs.md#getgroupqueryoutputtypedef)
- [UpdateGroupQueryOutputTypeDef](./type_defs.md#updategroupqueryoutputtypedef)
- [CreateGroupInputRequestTypeDef](./type_defs.md#creategroupinputrequesttypedef)
- [GroupConfigurationTypeDef](./type_defs.md#groupconfigurationtypedef)
- [PutGroupConfigurationInputRequestTypeDef](./type_defs.md#putgroupconfigurationinputrequesttypedef)
- [ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef)
- [CreateGroupOutputTypeDef](./type_defs.md#creategroupoutputtypedef)
- [GetGroupConfigurationOutputTypeDef](./type_defs.md#getgroupconfigurationoutputtypedef)

