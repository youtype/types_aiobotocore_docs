# Detective module

> [Index](../README.md) > Detective


!!! note ""

    Auto-generated documentation for [Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
    type annotations stubs module [types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Detective` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[detective]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[detective]'


# standalone installation
python -m pip install types-aiobotocore-detective
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-detective
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DetectiveClient

Type annotations and code completion for  `#!python session.create_client("detective")` as [DetectiveClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_detective.client import DetectiveClient


session = get_session()
async with session.create_client("detective") as client:
    client: DetectiveClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_detective.literals import DatasourcePackageIngestStateType

def get_value() -> DatasourcePackageIngestStateType:
    return "DISABLED"
```

- [DatasourcePackageIngestStateType](./literals.md#datasourcepackageingeststatetype)
- [DatasourcePackageType](./literals.md#datasourcepackagetype)
- [InvitationTypeType](./literals.md#invitationtypetype)
- [MemberDisabledReasonType](./literals.md#memberdisabledreasontype)
- [MemberStatusType](./literals.md#memberstatustype)
- [DetectiveServiceName](./literals.md#detectiveservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_detective.type_defs import AcceptInvitationRequestRequestTypeDef

def get_value() -> AcceptInvitationRequestRequestTypeDef:
    return {
        "GraphArn": ...,
    }
```

- [AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef)
- [AccountTypeDef](./type_defs.md#accounttypedef)
- [AdministratorTypeDef](./type_defs.md#administratortypedef)
- [BatchGetGraphMemberDatasourcesRequestRequestTypeDef](./type_defs.md#batchgetgraphmemberdatasourcesrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef)
- [BatchGetMembershipDatasourcesRequestRequestTypeDef](./type_defs.md#batchgetmembershipdatasourcesrequestrequesttypedef)
- [UnprocessedGraphTypeDef](./type_defs.md#unprocessedgraphtypedef)
- [CreateGraphRequestRequestTypeDef](./type_defs.md#creategraphrequestrequesttypedef)
- [TimestampForCollectionTypeDef](./type_defs.md#timestampforcollectiontypedef)
- [DatasourcePackageUsageInfoTypeDef](./type_defs.md#datasourcepackageusageinfotypedef)
- [DeleteGraphRequestRequestTypeDef](./type_defs.md#deletegraphrequestrequesttypedef)
- [DeleteMembersRequestRequestTypeDef](./type_defs.md#deletemembersrequestrequesttypedef)
- [DescribeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#describeorganizationconfigurationrequestrequesttypedef)
- [DisassociateMembershipRequestRequestTypeDef](./type_defs.md#disassociatemembershiprequestrequesttypedef)
- [EnableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#enableorganizationadminaccountrequestrequesttypedef)
- [GetMembersRequestRequestTypeDef](./type_defs.md#getmembersrequestrequesttypedef)
- [GraphTypeDef](./type_defs.md#graphtypedef)
- [ListDatasourcePackagesRequestRequestTypeDef](./type_defs.md#listdatasourcepackagesrequestrequesttypedef)
- [ListGraphsRequestRequestTypeDef](./type_defs.md#listgraphsrequestrequesttypedef)
- [ListInvitationsRequestRequestTypeDef](./type_defs.md#listinvitationsrequestrequesttypedef)
- [ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef)
- [ListOrganizationAdminAccountsRequestRequestTypeDef](./type_defs.md#listorganizationadminaccountsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RejectInvitationRequestRequestTypeDef](./type_defs.md#rejectinvitationrequestrequesttypedef)
- [StartMonitoringMemberRequestRequestTypeDef](./type_defs.md#startmonitoringmemberrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDatasourcePackagesRequestRequestTypeDef](./type_defs.md#updatedatasourcepackagesrequestrequesttypedef)
- [UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef)
- [CreateMembersRequestRequestTypeDef](./type_defs.md#createmembersrequestrequesttypedef)
- [CreateGraphResponseTypeDef](./type_defs.md#creategraphresponsetypedef)
- [DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DeleteMembersResponseTypeDef](./type_defs.md#deletemembersresponsetypedef)
- [DatasourcePackageIngestDetailTypeDef](./type_defs.md#datasourcepackageingestdetailtypedef)
- [MembershipDatasourcesTypeDef](./type_defs.md#membershipdatasourcestypedef)
- [MemberDetailTypeDef](./type_defs.md#memberdetailtypedef)
- [ListGraphsResponseTypeDef](./type_defs.md#listgraphsresponsetypedef)
- [ListDatasourcePackagesResponseTypeDef](./type_defs.md#listdatasourcepackagesresponsetypedef)
- [BatchGetGraphMemberDatasourcesResponseTypeDef](./type_defs.md#batchgetgraphmemberdatasourcesresponsetypedef)
- [BatchGetMembershipDatasourcesResponseTypeDef](./type_defs.md#batchgetmembershipdatasourcesresponsetypedef)
- [CreateMembersResponseTypeDef](./type_defs.md#createmembersresponsetypedef)
- [GetMembersResponseTypeDef](./type_defs.md#getmembersresponsetypedef)
- [ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef)
- [ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)

