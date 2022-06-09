# DAX module

> [Index](../README.md) > DAX


!!! note ""

    Auto-generated documentation for [DAX](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
    type annotations stubs module [types-aiobotocore-dax](https://pypi.org/project/types-aiobotocore-dax/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `DAX`.

### From PyPI with pip

Install `types-aiobotocore` for `DAX` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[dax]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[dax]'


# standalone installation
python -m pip install types-aiobotocore-dax
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-dax
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DAXClient

Type annotations and code completion for  `#!python session.create_client("dax")` as [DAXClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.client import DAXClient


session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("dax").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_dax.paginator import DescribeClustersPaginator

def get_describe_clusters_paginator() -> DescribeClustersPaginator:
    return client.get_paginator("describe_clusters"))
```

- [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
- [DescribeDefaultParametersPaginator](./paginators.md#describedefaultparameterspaginator)
- [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- [DescribeParameterGroupsPaginator](./paginators.md#describeparametergroupspaginator)
- [DescribeParametersPaginator](./paginators.md#describeparameterspaginator)
- [DescribeSubnetGroupsPaginator](./paginators.md#describesubnetgroupspaginator)
- [ListTagsPaginator](./paginators.md#listtagspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_dax.literals import ChangeTypeType

def get_value() -> ChangeTypeType:
    return "IMMEDIATE"
```

- [ChangeTypeType](./literals.md#changetypetype)
- [ClusterEndpointEncryptionTypeType](./literals.md#clusterendpointencryptiontypetype)
- [DescribeClustersPaginatorName](./literals.md#describeclusterspaginatorname)
- [DescribeDefaultParametersPaginatorName](./literals.md#describedefaultparameterspaginatorname)
- [DescribeEventsPaginatorName](./literals.md#describeeventspaginatorname)
- [DescribeParameterGroupsPaginatorName](./literals.md#describeparametergroupspaginatorname)
- [DescribeParametersPaginatorName](./literals.md#describeparameterspaginatorname)
- [DescribeSubnetGroupsPaginatorName](./literals.md#describesubnetgroupspaginatorname)
- [IsModifiableType](./literals.md#ismodifiabletype)
- [ListTagsPaginatorName](./literals.md#listtagspaginatorname)
- [ParameterTypeType](./literals.md#parametertypetype)
- [SSEStatusType](./literals.md#ssestatustype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [DAXServiceName](./literals.md#daxservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_dax.type_defs import EndpointTypeDef

def get_value() -> EndpointTypeDef:
    return {
        "Address": ...,
    }
```

- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [ParameterGroupStatusTypeDef](./type_defs.md#parametergroupstatustypedef)
- [SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef)
- [SecurityGroupMembershipTypeDef](./type_defs.md#securitygroupmembershiptypedef)
- [SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateParameterGroupRequestRequestTypeDef](./type_defs.md#createparametergrouprequestrequesttypedef)
- [ParameterGroupTypeDef](./type_defs.md#parametergrouptypedef)
- [CreateSubnetGroupRequestRequestTypeDef](./type_defs.md#createsubnetgrouprequestrequesttypedef)
- [DecreaseReplicationFactorRequestRequestTypeDef](./type_defs.md#decreasereplicationfactorrequestrequesttypedef)
- [DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef)
- [DeleteParameterGroupRequestRequestTypeDef](./type_defs.md#deleteparametergrouprequestrequesttypedef)
- [DeleteSubnetGroupRequestRequestTypeDef](./type_defs.md#deletesubnetgrouprequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeClustersRequestRequestTypeDef](./type_defs.md#describeclustersrequestrequesttypedef)
- [DescribeDefaultParametersRequestRequestTypeDef](./type_defs.md#describedefaultparametersrequestrequesttypedef)
- [DescribeEventsRequestRequestTypeDef](./type_defs.md#describeeventsrequestrequesttypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [DescribeParameterGroupsRequestRequestTypeDef](./type_defs.md#describeparametergroupsrequestrequesttypedef)
- [DescribeParametersRequestRequestTypeDef](./type_defs.md#describeparametersrequestrequesttypedef)
- [DescribeSubnetGroupsRequestRequestTypeDef](./type_defs.md#describesubnetgroupsrequestrequesttypedef)
- [IncreaseReplicationFactorRequestRequestTypeDef](./type_defs.md#increasereplicationfactorrequestrequesttypedef)
- [ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef)
- [NodeTypeSpecificValueTypeDef](./type_defs.md#nodetypespecificvaluetypedef)
- [ParameterNameValueTypeDef](./type_defs.md#parameternamevaluetypedef)
- [RebootNodeRequestRequestTypeDef](./type_defs.md#rebootnoderequestrequesttypedef)
- [SubnetTypeDef](./type_defs.md#subnettypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef)
- [UpdateSubnetGroupRequestRequestTypeDef](./type_defs.md#updatesubnetgrouprequestrequesttypedef)
- [NodeTypeDef](./type_defs.md#nodetypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [DeleteParameterGroupResponseTypeDef](./type_defs.md#deleteparametergroupresponsetypedef)
- [DeleteSubnetGroupResponseTypeDef](./type_defs.md#deletesubnetgroupresponsetypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [TagResourceResponseTypeDef](./type_defs.md#tagresourceresponsetypedef)
- [UntagResourceResponseTypeDef](./type_defs.md#untagresourceresponsetypedef)
- [CreateParameterGroupResponseTypeDef](./type_defs.md#createparametergroupresponsetypedef)
- [DescribeParameterGroupsResponseTypeDef](./type_defs.md#describeparametergroupsresponsetypedef)
- [UpdateParameterGroupResponseTypeDef](./type_defs.md#updateparametergroupresponsetypedef)
- [DescribeClustersRequestDescribeClustersPaginateTypeDef](./type_defs.md#describeclustersrequestdescribeclusterspaginatetypedef)
- [DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef](./type_defs.md#describedefaultparametersrequestdescribedefaultparameterspaginatetypedef)
- [DescribeEventsRequestDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsrequestdescribeeventspaginatetypedef)
- [DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef](./type_defs.md#describeparametergroupsrequestdescribeparametergroupspaginatetypedef)
- [DescribeParametersRequestDescribeParametersPaginateTypeDef](./type_defs.md#describeparametersrequestdescribeparameterspaginatetypedef)
- [DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef](./type_defs.md#describesubnetgroupsrequestdescribesubnetgroupspaginatetypedef)
- [ListTagsRequestListTagsPaginateTypeDef](./type_defs.md#listtagsrequestlisttagspaginatetypedef)
- [DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef)
- [ParameterTypeDef](./type_defs.md#parametertypedef)
- [UpdateParameterGroupRequestRequestTypeDef](./type_defs.md#updateparametergrouprequestrequesttypedef)
- [SubnetGroupTypeDef](./type_defs.md#subnetgrouptypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [DescribeDefaultParametersResponseTypeDef](./type_defs.md#describedefaultparametersresponsetypedef)
- [DescribeParametersResponseTypeDef](./type_defs.md#describeparametersresponsetypedef)
- [CreateSubnetGroupResponseTypeDef](./type_defs.md#createsubnetgroupresponsetypedef)
- [DescribeSubnetGroupsResponseTypeDef](./type_defs.md#describesubnetgroupsresponsetypedef)
- [UpdateSubnetGroupResponseTypeDef](./type_defs.md#updatesubnetgroupresponsetypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [DecreaseReplicationFactorResponseTypeDef](./type_defs.md#decreasereplicationfactorresponsetypedef)
- [DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef)
- [DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef)
- [IncreaseReplicationFactorResponseTypeDef](./type_defs.md#increasereplicationfactorresponsetypedef)
- [RebootNodeResponseTypeDef](./type_defs.md#rebootnoderesponsetypedef)
- [UpdateClusterResponseTypeDef](./type_defs.md#updateclusterresponsetypedef)

