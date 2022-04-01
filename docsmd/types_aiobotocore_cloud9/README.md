# Cloud9 module

> [Index](../README.md) > Cloud9


!!! note ""

    Auto-generated documentation for [Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
    type annotations stubs module [types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Cloud9`.

### From PyPI with pip

Install `types-aiobotocore` for `Cloud9` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloud9]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloud9]'


# standalone installation
python -m pip install types-aiobotocore-cloud9
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloud9
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Cloud9Client

Type annotations and code completion for  `#!python session.create_client("cloud9")` as [Cloud9Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloud9.client import Cloud9Client


session = get_session()
async with session.create_client("cloud9") as client:
    client: Cloud9Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloud9").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_cloud9.paginator import DescribeEnvironmentMembershipsPaginator

def get_describe_environment_memberships_paginator() -> DescribeEnvironmentMembershipsPaginator:
    return client.get_paginator("describe_environment_memberships"))
```

- [DescribeEnvironmentMembershipsPaginator](./paginators.md#describeenvironmentmembershipspaginator)
- [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_cloud9.literals import ConnectionTypeType

def get_value() -> ConnectionTypeType:
    return "CONNECT_SSH"
```

- [ConnectionTypeType](./literals.md#connectiontypetype)
- [DescribeEnvironmentMembershipsPaginatorName](./literals.md#describeenvironmentmembershipspaginatorname)
- [EnvironmentLifecycleStatusType](./literals.md#environmentlifecyclestatustype)
- [EnvironmentStatusType](./literals.md#environmentstatustype)
- [EnvironmentTypeType](./literals.md#environmenttypetype)
- [ListEnvironmentsPaginatorName](./literals.md#listenvironmentspaginatorname)
- [ManagedCredentialsActionType](./literals.md#managedcredentialsactiontype)
- [ManagedCredentialsStatusType](./literals.md#managedcredentialsstatustype)
- [MemberPermissionsType](./literals.md#memberpermissionstype)
- [PermissionsType](./literals.md#permissionstype)
- [Cloud9ServiceName](./literals.md#cloud9servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_cloud9.type_defs import CreateEnvironmentEC2RequestRequestTypeDef

def get_value() -> CreateEnvironmentEC2RequestRequestTypeDef:
    return {
        "name": ...,
        "instanceType": ...,
    }
```

- [CreateEnvironmentEC2RequestRequestTypeDef](./type_defs.md#createenvironmentec2requestrequesttypedef)
- [CreateEnvironmentEC2ResultTypeDef](./type_defs.md#createenvironmentec2resulttypedef)
- [CreateEnvironmentMembershipRequestRequestTypeDef](./type_defs.md#createenvironmentmembershiprequestrequesttypedef)
- [CreateEnvironmentMembershipResultTypeDef](./type_defs.md#createenvironmentmembershipresulttypedef)
- [DeleteEnvironmentMembershipRequestRequestTypeDef](./type_defs.md#deleteenvironmentmembershiprequestrequesttypedef)
- [DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef)
- [DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef](./type_defs.md#describeenvironmentmembershipsrequestdescribeenvironmentmembershipspaginatetypedef)
- [DescribeEnvironmentMembershipsRequestRequestTypeDef](./type_defs.md#describeenvironmentmembershipsrequestrequesttypedef)
- [DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef)
- [DescribeEnvironmentStatusRequestRequestTypeDef](./type_defs.md#describeenvironmentstatusrequestrequesttypedef)
- [DescribeEnvironmentStatusResultTypeDef](./type_defs.md#describeenvironmentstatusresulttypedef)
- [DescribeEnvironmentsRequestRequestTypeDef](./type_defs.md#describeenvironmentsrequestrequesttypedef)
- [DescribeEnvironmentsResultTypeDef](./type_defs.md#describeenvironmentsresulttypedef)
- [EnvironmentLifecycleTypeDef](./type_defs.md#environmentlifecycletypedef)
- [EnvironmentMemberTypeDef](./type_defs.md#environmentmembertypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [ListEnvironmentsRequestListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsrequestlistenvironmentspaginatetypedef)
- [ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef)
- [ListEnvironmentsResultTypeDef](./type_defs.md#listenvironmentsresulttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateEnvironmentMembershipRequestRequestTypeDef](./type_defs.md#updateenvironmentmembershiprequestrequesttypedef)
- [UpdateEnvironmentMembershipResultTypeDef](./type_defs.md#updateenvironmentmembershipresulttypedef)
- [UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef)

