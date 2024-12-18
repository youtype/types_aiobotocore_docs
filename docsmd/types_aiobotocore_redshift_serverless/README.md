# RedshiftServerless module

> [Index](../README.md) > RedshiftServerless


!!! note ""

    Auto-generated documentation for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#redshiftserverless)
    type annotations stubs module [types-aiobotocore-redshift-serverless](https://pypi.org/project/types-aiobotocore-redshift-serverless/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `RedshiftServerless` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `RedshiftServerless` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[redshift-serverless]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[redshift-serverless]'

# standalone installation
python -m pip install types-aiobotocore-redshift-serverless
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-redshift-serverless
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RedshiftServerlessClient

Type annotations and code completion for  `#!python session.create_client("redshift-serverless")` as [RedshiftServerlessClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client)

```python
# RedshiftServerlessClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_redshift_serverless.client import RedshiftServerlessClient


session = get_session()
async with session.create_client("redshift-serverless") as client:
    client: RedshiftServerlessClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("redshift-serverless").get_paginator("...")`.

```python
# ListCustomDomainAssociationsPaginator usage example

from types_aiobotocore_redshift_serverless.paginator import ListCustomDomainAssociationsPaginator

def get_list_custom_domain_associations_paginator() -> ListCustomDomainAssociationsPaginator:
    return client.get_paginator("list_custom_domain_associations"))
```

- [ListCustomDomainAssociationsPaginator](./paginators.md#listcustomdomainassociationspaginator)
- [ListEndpointAccessPaginator](./paginators.md#listendpointaccesspaginator)
- [ListManagedWorkgroupsPaginator](./paginators.md#listmanagedworkgroupspaginator)
- [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
- [ListRecoveryPointsPaginator](./paginators.md#listrecoverypointspaginator)
- [ListScheduledActionsPaginator](./paginators.md#listscheduledactionspaginator)
- [ListSnapshotCopyConfigurationsPaginator](./paginators.md#listsnapshotcopyconfigurationspaginator)
- [ListSnapshotsPaginator](./paginators.md#listsnapshotspaginator)
- [ListTableRestoreStatusPaginator](./paginators.md#listtablerestorestatuspaginator)
- [ListUsageLimitsPaginator](./paginators.md#listusagelimitspaginator)
- [ListWorkgroupsPaginator](./paginators.md#listworkgroupspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListCustomDomainAssociationsPaginatorName usage example

from types_aiobotocore_redshift_serverless.literals import ListCustomDomainAssociationsPaginatorName

def get_value() -> ListCustomDomainAssociationsPaginatorName:
    return "list_custom_domain_associations"
```

- [ListCustomDomainAssociationsPaginatorName](./literals.md#listcustomdomainassociationspaginatorname)
- [ListEndpointAccessPaginatorName](./literals.md#listendpointaccesspaginatorname)
- [ListManagedWorkgroupsPaginatorName](./literals.md#listmanagedworkgroupspaginatorname)
- [ListNamespacesPaginatorName](./literals.md#listnamespacespaginatorname)
- [ListRecoveryPointsPaginatorName](./literals.md#listrecoverypointspaginatorname)
- [ListScheduledActionsPaginatorName](./literals.md#listscheduledactionspaginatorname)
- [ListSnapshotCopyConfigurationsPaginatorName](./literals.md#listsnapshotcopyconfigurationspaginatorname)
- [ListSnapshotsPaginatorName](./literals.md#listsnapshotspaginatorname)
- [ListTableRestoreStatusPaginatorName](./literals.md#listtablerestorestatuspaginatorname)
- [ListUsageLimitsPaginatorName](./literals.md#listusagelimitspaginatorname)
- [ListWorkgroupsPaginatorName](./literals.md#listworkgroupspaginatorname)
- [LogExportType](./literals.md#logexporttype)
- [ManagedWorkgroupStatusType](./literals.md#managedworkgroupstatustype)
- [NamespaceStatusType](./literals.md#namespacestatustype)
- [PerformanceTargetStatusType](./literals.md#performancetargetstatustype)
- [SnapshotStatusType](./literals.md#snapshotstatustype)
- [StateType](./literals.md#statetype)
- [UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype)
- [UsageLimitPeriodType](./literals.md#usagelimitperiodtype)
- [UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype)
- [WorkgroupStatusType](./literals.md#workgroupstatustype)
- [RedshiftServerlessServiceName](./literals.md#redshiftserverlessservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociationTypeDef](./type_defs.md#associationtypedef)
- [ConfigParameterTypeDef](./type_defs.md#configparametertypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SnapshotTypeDef](./type_defs.md#snapshottypedef)
- [CreateCustomDomainAssociationRequestRequestTypeDef](./type_defs.md#createcustomdomainassociationrequestrequesttypedef)
- [CreateEndpointAccessRequestRequestTypeDef](./type_defs.md#createendpointaccessrequestrequesttypedef)
- [NamespaceTypeDef](./type_defs.md#namespacetypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [CreateSnapshotCopyConfigurationRequestRequestTypeDef](./type_defs.md#createsnapshotcopyconfigurationrequestrequesttypedef)
- [SnapshotCopyConfigurationTypeDef](./type_defs.md#snapshotcopyconfigurationtypedef)
- [CreateUsageLimitRequestRequestTypeDef](./type_defs.md#createusagelimitrequestrequesttypedef)
- [UsageLimitTypeDef](./type_defs.md#usagelimittypedef)
- [PerformanceTargetTypeDef](./type_defs.md#performancetargettypedef)
- [DeleteCustomDomainAssociationRequestRequestTypeDef](./type_defs.md#deletecustomdomainassociationrequestrequesttypedef)
- [DeleteEndpointAccessRequestRequestTypeDef](./type_defs.md#deleteendpointaccessrequestrequesttypedef)
- [DeleteNamespaceRequestRequestTypeDef](./type_defs.md#deletenamespacerequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteScheduledActionRequestRequestTypeDef](./type_defs.md#deletescheduledactionrequestrequesttypedef)
- [DeleteSnapshotCopyConfigurationRequestRequestTypeDef](./type_defs.md#deletesnapshotcopyconfigurationrequestrequesttypedef)
- [DeleteSnapshotRequestRequestTypeDef](./type_defs.md#deletesnapshotrequestrequesttypedef)
- [DeleteUsageLimitRequestRequestTypeDef](./type_defs.md#deleteusagelimitrequestrequesttypedef)
- [DeleteWorkgroupRequestRequestTypeDef](./type_defs.md#deleteworkgrouprequestrequesttypedef)
- [VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef)
- [GetCredentialsRequestRequestTypeDef](./type_defs.md#getcredentialsrequestrequesttypedef)
- [GetCustomDomainAssociationRequestRequestTypeDef](./type_defs.md#getcustomdomainassociationrequestrequesttypedef)
- [GetEndpointAccessRequestRequestTypeDef](./type_defs.md#getendpointaccessrequestrequesttypedef)
- [GetNamespaceRequestRequestTypeDef](./type_defs.md#getnamespacerequestrequesttypedef)
- [GetRecoveryPointRequestRequestTypeDef](./type_defs.md#getrecoverypointrequestrequesttypedef)
- [RecoveryPointTypeDef](./type_defs.md#recoverypointtypedef)
- [GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef)
- [ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef)
- [GetScheduledActionRequestRequestTypeDef](./type_defs.md#getscheduledactionrequestrequesttypedef)
- [GetSnapshotRequestRequestTypeDef](./type_defs.md#getsnapshotrequestrequesttypedef)
- [GetTableRestoreStatusRequestRequestTypeDef](./type_defs.md#gettablerestorestatusrequestrequesttypedef)
- [TableRestoreStatusTypeDef](./type_defs.md#tablerestorestatustypedef)
- [GetUsageLimitRequestRequestTypeDef](./type_defs.md#getusagelimitrequestrequesttypedef)
- [GetWorkgroupRequestRequestTypeDef](./type_defs.md#getworkgrouprequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCustomDomainAssociationsRequestRequestTypeDef](./type_defs.md#listcustomdomainassociationsrequestrequesttypedef)
- [ListEndpointAccessRequestRequestTypeDef](./type_defs.md#listendpointaccessrequestrequesttypedef)
- [ListManagedWorkgroupsRequestRequestTypeDef](./type_defs.md#listmanagedworkgroupsrequestrequesttypedef)
- [ManagedWorkgroupListItemTypeDef](./type_defs.md#managedworkgrouplistitemtypedef)
- [ListNamespacesRequestRequestTypeDef](./type_defs.md#listnamespacesrequestrequesttypedef)
- [ListScheduledActionsRequestRequestTypeDef](./type_defs.md#listscheduledactionsrequestrequesttypedef)
- [ScheduledActionAssociationTypeDef](./type_defs.md#scheduledactionassociationtypedef)
- [ListSnapshotCopyConfigurationsRequestRequestTypeDef](./type_defs.md#listsnapshotcopyconfigurationsrequestrequesttypedef)
- [ListTableRestoreStatusRequestRequestTypeDef](./type_defs.md#listtablerestorestatusrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListUsageLimitsRequestRequestTypeDef](./type_defs.md#listusagelimitsrequestrequesttypedef)
- [ListWorkgroupsRequestRequestTypeDef](./type_defs.md#listworkgroupsrequestrequesttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [RestoreFromRecoveryPointRequestRequestTypeDef](./type_defs.md#restorefromrecoverypointrequestrequesttypedef)
- [RestoreFromSnapshotRequestRequestTypeDef](./type_defs.md#restorefromsnapshotrequestrequesttypedef)
- [RestoreTableFromRecoveryPointRequestRequestTypeDef](./type_defs.md#restoretablefromrecoverypointrequestrequesttypedef)
- [RestoreTableFromSnapshotRequestRequestTypeDef](./type_defs.md#restoretablefromsnapshotrequestrequesttypedef)
- [ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateCustomDomainAssociationRequestRequestTypeDef](./type_defs.md#updatecustomdomainassociationrequestrequesttypedef)
- [UpdateEndpointAccessRequestRequestTypeDef](./type_defs.md#updateendpointaccessrequestrequesttypedef)
- [UpdateNamespaceRequestRequestTypeDef](./type_defs.md#updatenamespacerequestrequesttypedef)
- [UpdateSnapshotCopyConfigurationRequestRequestTypeDef](./type_defs.md#updatesnapshotcopyconfigurationrequestrequesttypedef)
- [UpdateSnapshotRequestRequestTypeDef](./type_defs.md#updatesnapshotrequestrequesttypedef)
- [UpdateUsageLimitRequestRequestTypeDef](./type_defs.md#updateusagelimitrequestrequesttypedef)
- [ConvertRecoveryPointToSnapshotRequestRequestTypeDef](./type_defs.md#convertrecoverypointtosnapshotrequestrequesttypedef)
- [CreateNamespaceRequestRequestTypeDef](./type_defs.md#createnamespacerequestrequesttypedef)
- [CreateSnapshotRequestRequestTypeDef](./type_defs.md#createsnapshotrequestrequesttypedef)
- [CreateSnapshotScheduleActionParametersOutputTypeDef](./type_defs.md#createsnapshotscheduleactionparametersoutputtypedef)
- [CreateSnapshotScheduleActionParametersTypeDef](./type_defs.md#createsnapshotscheduleactionparameterstypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateCustomDomainAssociationResponseTypeDef](./type_defs.md#createcustomdomainassociationresponsetypedef)
- [GetCredentialsResponseTypeDef](./type_defs.md#getcredentialsresponsetypedef)
- [GetCustomDomainAssociationResponseTypeDef](./type_defs.md#getcustomdomainassociationresponsetypedef)
- [ListCustomDomainAssociationsResponseTypeDef](./type_defs.md#listcustomdomainassociationsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateCustomDomainAssociationResponseTypeDef](./type_defs.md#updatecustomdomainassociationresponsetypedef)
- [ConvertRecoveryPointToSnapshotResponseTypeDef](./type_defs.md#convertrecoverypointtosnapshotresponsetypedef)
- [CreateSnapshotResponseTypeDef](./type_defs.md#createsnapshotresponsetypedef)
- [DeleteSnapshotResponseTypeDef](./type_defs.md#deletesnapshotresponsetypedef)
- [GetSnapshotResponseTypeDef](./type_defs.md#getsnapshotresponsetypedef)
- [ListSnapshotsResponseTypeDef](./type_defs.md#listsnapshotsresponsetypedef)
- [UpdateSnapshotResponseTypeDef](./type_defs.md#updatesnapshotresponsetypedef)
- [CreateNamespaceResponseTypeDef](./type_defs.md#createnamespaceresponsetypedef)
- [DeleteNamespaceResponseTypeDef](./type_defs.md#deletenamespaceresponsetypedef)
- [GetNamespaceResponseTypeDef](./type_defs.md#getnamespaceresponsetypedef)
- [ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef)
- [RestoreFromRecoveryPointResponseTypeDef](./type_defs.md#restorefromrecoverypointresponsetypedef)
- [RestoreFromSnapshotResponseTypeDef](./type_defs.md#restorefromsnapshotresponsetypedef)
- [UpdateNamespaceResponseTypeDef](./type_defs.md#updatenamespaceresponsetypedef)
- [ListRecoveryPointsRequestRequestTypeDef](./type_defs.md#listrecoverypointsrequestrequesttypedef)
- [ListSnapshotsRequestRequestTypeDef](./type_defs.md#listsnapshotsrequestrequesttypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [CreateSnapshotCopyConfigurationResponseTypeDef](./type_defs.md#createsnapshotcopyconfigurationresponsetypedef)
- [DeleteSnapshotCopyConfigurationResponseTypeDef](./type_defs.md#deletesnapshotcopyconfigurationresponsetypedef)
- [ListSnapshotCopyConfigurationsResponseTypeDef](./type_defs.md#listsnapshotcopyconfigurationsresponsetypedef)
- [UpdateSnapshotCopyConfigurationResponseTypeDef](./type_defs.md#updatesnapshotcopyconfigurationresponsetypedef)
- [CreateUsageLimitResponseTypeDef](./type_defs.md#createusagelimitresponsetypedef)
- [DeleteUsageLimitResponseTypeDef](./type_defs.md#deleteusagelimitresponsetypedef)
- [GetUsageLimitResponseTypeDef](./type_defs.md#getusagelimitresponsetypedef)
- [ListUsageLimitsResponseTypeDef](./type_defs.md#listusagelimitsresponsetypedef)
- [UpdateUsageLimitResponseTypeDef](./type_defs.md#updateusagelimitresponsetypedef)
- [CreateWorkgroupRequestRequestTypeDef](./type_defs.md#createworkgrouprequestrequesttypedef)
- [UpdateWorkgroupRequestRequestTypeDef](./type_defs.md#updateworkgrouprequestrequesttypedef)
- [GetRecoveryPointResponseTypeDef](./type_defs.md#getrecoverypointresponsetypedef)
- [ListRecoveryPointsResponseTypeDef](./type_defs.md#listrecoverypointsresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)
- [GetTableRestoreStatusResponseTypeDef](./type_defs.md#gettablerestorestatusresponsetypedef)
- [ListTableRestoreStatusResponseTypeDef](./type_defs.md#listtablerestorestatusresponsetypedef)
- [RestoreTableFromRecoveryPointResponseTypeDef](./type_defs.md#restoretablefromrecoverypointresponsetypedef)
- [RestoreTableFromSnapshotResponseTypeDef](./type_defs.md#restoretablefromsnapshotresponsetypedef)
- [ListCustomDomainAssociationsRequestListCustomDomainAssociationsPaginateTypeDef](./type_defs.md#listcustomdomainassociationsrequestlistcustomdomainassociationspaginatetypedef)
- [ListEndpointAccessRequestListEndpointAccessPaginateTypeDef](./type_defs.md#listendpointaccessrequestlistendpointaccesspaginatetypedef)
- [ListManagedWorkgroupsRequestListManagedWorkgroupsPaginateTypeDef](./type_defs.md#listmanagedworkgroupsrequestlistmanagedworkgroupspaginatetypedef)
- [ListNamespacesRequestListNamespacesPaginateTypeDef](./type_defs.md#listnamespacesrequestlistnamespacespaginatetypedef)
- [ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef](./type_defs.md#listrecoverypointsrequestlistrecoverypointspaginatetypedef)
- [ListScheduledActionsRequestListScheduledActionsPaginateTypeDef](./type_defs.md#listscheduledactionsrequestlistscheduledactionspaginatetypedef)
- [ListSnapshotCopyConfigurationsRequestListSnapshotCopyConfigurationsPaginateTypeDef](./type_defs.md#listsnapshotcopyconfigurationsrequestlistsnapshotcopyconfigurationspaginatetypedef)
- [ListSnapshotsRequestListSnapshotsPaginateTypeDef](./type_defs.md#listsnapshotsrequestlistsnapshotspaginatetypedef)
- [ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef](./type_defs.md#listtablerestorestatusrequestlisttablerestorestatuspaginatetypedef)
- [ListUsageLimitsRequestListUsageLimitsPaginateTypeDef](./type_defs.md#listusagelimitsrequestlistusagelimitspaginatetypedef)
- [ListWorkgroupsRequestListWorkgroupsPaginateTypeDef](./type_defs.md#listworkgroupsrequestlistworkgroupspaginatetypedef)
- [ListManagedWorkgroupsResponseTypeDef](./type_defs.md#listmanagedworkgroupsresponsetypedef)
- [ListScheduledActionsResponseTypeDef](./type_defs.md#listscheduledactionsresponsetypedef)
- [VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef)
- [TargetActionOutputTypeDef](./type_defs.md#targetactionoutputtypedef)
- [CreateSnapshotScheduleActionParametersUnionTypeDef](./type_defs.md#createsnapshotscheduleactionparametersuniontypedef)
- [EndpointAccessTypeDef](./type_defs.md#endpointaccesstypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [ScheduledActionResponseTypeDef](./type_defs.md#scheduledactionresponsetypedef)
- [TargetActionTypeDef](./type_defs.md#targetactiontypedef)
- [CreateEndpointAccessResponseTypeDef](./type_defs.md#createendpointaccessresponsetypedef)
- [DeleteEndpointAccessResponseTypeDef](./type_defs.md#deleteendpointaccessresponsetypedef)
- [GetEndpointAccessResponseTypeDef](./type_defs.md#getendpointaccessresponsetypedef)
- [ListEndpointAccessResponseTypeDef](./type_defs.md#listendpointaccessresponsetypedef)
- [UpdateEndpointAccessResponseTypeDef](./type_defs.md#updateendpointaccessresponsetypedef)
- [WorkgroupTypeDef](./type_defs.md#workgrouptypedef)
- [CreateScheduledActionResponseTypeDef](./type_defs.md#createscheduledactionresponsetypedef)
- [DeleteScheduledActionResponseTypeDef](./type_defs.md#deletescheduledactionresponsetypedef)
- [GetScheduledActionResponseTypeDef](./type_defs.md#getscheduledactionresponsetypedef)
- [UpdateScheduledActionResponseTypeDef](./type_defs.md#updatescheduledactionresponsetypedef)
- [CreateScheduledActionRequestRequestTypeDef](./type_defs.md#createscheduledactionrequestrequesttypedef)
- [UpdateScheduledActionRequestRequestTypeDef](./type_defs.md#updatescheduledactionrequestrequesttypedef)
- [CreateWorkgroupResponseTypeDef](./type_defs.md#createworkgroupresponsetypedef)
- [DeleteWorkgroupResponseTypeDef](./type_defs.md#deleteworkgroupresponsetypedef)
- [GetWorkgroupResponseTypeDef](./type_defs.md#getworkgroupresponsetypedef)
- [ListWorkgroupsResponseTypeDef](./type_defs.md#listworkgroupsresponsetypedef)
- [UpdateWorkgroupResponseTypeDef](./type_defs.md#updateworkgroupresponsetypedef)

