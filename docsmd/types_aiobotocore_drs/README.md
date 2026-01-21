# Drs module

> [Index](../README.md) > Drs


!!! note ""

    Auto-generated documentation for [Drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Drs` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Drs` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[drs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[drs]'

# standalone installation
python -m pip install types-aiobotocore-drs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-drs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DrsClient

Type annotations and code completion for  `#!python session.create_client("drs")` as [DrsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#Drs.Client)

```python
# DrsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.client import DrsClient


session = get_session()
async with session.create_client("drs") as client:
    client: DrsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("drs").get_paginator("...")`.

```python
# DescribeJobLogItemsPaginator usage example

from types_aiobotocore_drs.paginator import DescribeJobLogItemsPaginator

def get_describe_job_log_items_paginator() -> DescribeJobLogItemsPaginator:
    return client.get_paginator("describe_job_log_items"))
```

- [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
- [DescribeJobsPaginator](./paginators.md#describejobspaginator)
- [DescribeLaunchConfigurationTemplatesPaginator](./paginators.md#describelaunchconfigurationtemplatespaginator)
- [DescribeRecoveryInstancesPaginator](./paginators.md#describerecoveryinstancespaginator)
- [DescribeRecoverySnapshotsPaginator](./paginators.md#describerecoverysnapshotspaginator)
- [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
- [DescribeSourceNetworksPaginator](./paginators.md#describesourcenetworkspaginator)
- [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
- [ListExtensibleSourceServersPaginator](./paginators.md#listextensiblesourceserverspaginator)
- [ListLaunchActionsPaginator](./paginators.md#listlaunchactionspaginator)
- [ListStagingAccountsPaginator](./paginators.md#liststagingaccountspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DataReplicationErrorStringType usage example

from types_aiobotocore_drs.literals import DataReplicationErrorStringType

def get_value() -> DataReplicationErrorStringType:
    return "AGENT_NOT_SEEN"
```

- [DataReplicationErrorStringType](./literals.md#datareplicationerrorstringtype)
- [DataReplicationInitiationStepNameType](./literals.md#datareplicationinitiationstepnametype)
- [DataReplicationInitiationStepStatusType](./literals.md#datareplicationinitiationstepstatustype)
- [DataReplicationStateType](./literals.md#datareplicationstatetype)
- [DescribeJobLogItemsPaginatorName](./literals.md#describejoblogitemspaginatorname)
- [DescribeJobsPaginatorName](./literals.md#describejobspaginatorname)
- [DescribeLaunchConfigurationTemplatesPaginatorName](./literals.md#describelaunchconfigurationtemplatespaginatorname)
- [DescribeRecoveryInstancesPaginatorName](./literals.md#describerecoveryinstancespaginatorname)
- [DescribeRecoverySnapshotsPaginatorName](./literals.md#describerecoverysnapshotspaginatorname)
- [DescribeReplicationConfigurationTemplatesPaginatorName](./literals.md#describereplicationconfigurationtemplatespaginatorname)
- [DescribeSourceNetworksPaginatorName](./literals.md#describesourcenetworkspaginatorname)
- [DescribeSourceServersPaginatorName](./literals.md#describesourceserverspaginatorname)
- [EC2InstanceStateType](./literals.md#ec2instancestatetype)
- [ExtensionStatusType](./literals.md#extensionstatustype)
- [FailbackLaunchTypeType](./literals.md#failbacklaunchtypetype)
- [FailbackReplicationErrorType](./literals.md#failbackreplicationerrortype)
- [FailbackStateType](./literals.md#failbackstatetype)
- [InitiatedByType](./literals.md#initiatedbytype)
- [JobLogEventType](./literals.md#joblogeventtype)
- [JobStatusType](./literals.md#jobstatustype)
- [JobTypeType](./literals.md#jobtypetype)
- [LastLaunchResultType](./literals.md#lastlaunchresulttype)
- [LastLaunchTypeType](./literals.md#lastlaunchtypetype)
- [LaunchActionCategoryType](./literals.md#launchactioncategorytype)
- [LaunchActionParameterTypeType](./literals.md#launchactionparametertypetype)
- [LaunchActionRunStatusType](./literals.md#launchactionrunstatustype)
- [LaunchActionTypeType](./literals.md#launchactiontypetype)
- [LaunchDispositionType](./literals.md#launchdispositiontype)
- [LaunchStatusType](./literals.md#launchstatustype)
- [ListExtensibleSourceServersPaginatorName](./literals.md#listextensiblesourceserverspaginatorname)
- [ListLaunchActionsPaginatorName](./literals.md#listlaunchactionspaginatorname)
- [ListStagingAccountsPaginatorName](./literals.md#liststagingaccountspaginatorname)
- [OriginEnvironmentType](./literals.md#originenvironmenttype)
- [PITPolicyRuleUnitsType](./literals.md#pitpolicyruleunitstype)
- [ProductCodeModeType](./literals.md#productcodemodetype)
- [RecoveryInstanceDataReplicationInitiationStepNameType](./literals.md#recoveryinstancedatareplicationinitiationstepnametype)
- [RecoveryInstanceDataReplicationInitiationStepStatusType](./literals.md#recoveryinstancedatareplicationinitiationstepstatustype)
- [RecoveryInstanceDataReplicationStateType](./literals.md#recoveryinstancedatareplicationstatetype)
- [RecoveryResultType](./literals.md#recoveryresulttype)
- [RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype)
- [ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
- [ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
- [ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
- [ReplicationConfigurationReplicatedDiskStagingDiskTypeType](./literals.md#replicationconfigurationreplicateddiskstagingdisktypetype)
- [ReplicationDirectionType](./literals.md#replicationdirectiontype)
- [ReplicationStatusType](./literals.md#replicationstatustype)
- [TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)
- [VolumeStatusType](./literals.md#volumestatustype)
- [DrsServiceName](./literals.md#drsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountTypeDef](./type_defs.md#accounttypedef)
- [AssociateSourceNetworkStackRequestTypeDef](./type_defs.md#associatesourcenetworkstackrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CPUTypeDef](./type_defs.md#cputypedef)
- [ProductCodeTypeDef](./type_defs.md#productcodetypedef)
- [CreateExtendedSourceServerRequestTypeDef](./type_defs.md#createextendedsourceserverrequesttypedef)
- [LicensingTypeDef](./type_defs.md#licensingtypedef)
- [PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef)
- [CreateSourceNetworkRequestTypeDef](./type_defs.md#createsourcenetworkrequesttypedef)
- [DataReplicationErrorTypeDef](./type_defs.md#datareplicationerrortypedef)
- [DataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#datareplicationinforeplicateddisktypedef)
- [DataReplicationInitiationStepTypeDef](./type_defs.md#datareplicationinitiationsteptypedef)
- [DeleteJobRequestTypeDef](./type_defs.md#deletejobrequesttypedef)
- [DeleteLaunchActionRequestTypeDef](./type_defs.md#deletelaunchactionrequesttypedef)
- [DeleteLaunchConfigurationTemplateRequestTypeDef](./type_defs.md#deletelaunchconfigurationtemplaterequesttypedef)
- [DeleteRecoveryInstanceRequestTypeDef](./type_defs.md#deleterecoveryinstancerequesttypedef)
- [DeleteReplicationConfigurationTemplateRequestTypeDef](./type_defs.md#deletereplicationconfigurationtemplaterequesttypedef)
- [DeleteSourceNetworkRequestTypeDef](./type_defs.md#deletesourcenetworkrequesttypedef)
- [DeleteSourceServerRequestTypeDef](./type_defs.md#deletesourceserverrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeJobLogItemsRequestTypeDef](./type_defs.md#describejoblogitemsrequesttypedef)
- [DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef)
- [DescribeLaunchConfigurationTemplatesRequestTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequesttypedef)
- [DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef)
- [DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef)
- [RecoverySnapshotTypeDef](./type_defs.md#recoverysnapshottypedef)
- [DescribeReplicationConfigurationTemplatesRequestTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequesttypedef)
- [DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef)
- [DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef)
- [DisconnectRecoveryInstanceRequestTypeDef](./type_defs.md#disconnectrecoveryinstancerequesttypedef)
- [DisconnectSourceServerRequestTypeDef](./type_defs.md#disconnectsourceserverrequesttypedef)
- [DiskTypeDef](./type_defs.md#disktypedef)
- [SourceNetworkDataTypeDef](./type_defs.md#sourcenetworkdatatypedef)
- [ExportSourceNetworkCfnTemplateRequestTypeDef](./type_defs.md#exportsourcenetworkcfntemplaterequesttypedef)
- [GetFailbackReplicationConfigurationRequestTypeDef](./type_defs.md#getfailbackreplicationconfigurationrequesttypedef)
- [GetLaunchConfigurationRequestTypeDef](./type_defs.md#getlaunchconfigurationrequesttypedef)
- [GetReplicationConfigurationRequestTypeDef](./type_defs.md#getreplicationconfigurationrequesttypedef)
- [IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef)
- [LaunchActionParameterTypeDef](./type_defs.md#launchactionparametertypedef)
- [LaunchActionsRequestFiltersTypeDef](./type_defs.md#launchactionsrequestfilterstypedef)
- [LaunchIntoInstancePropertiesTypeDef](./type_defs.md#launchintoinstancepropertiestypedef)
- [LifeCycleLastLaunchInitiatedTypeDef](./type_defs.md#lifecyclelastlaunchinitiatedtypedef)
- [ListExtensibleSourceServersRequestTypeDef](./type_defs.md#listextensiblesourceserversrequesttypedef)
- [StagingSourceServerTypeDef](./type_defs.md#stagingsourceservertypedef)
- [ListStagingAccountsRequestTypeDef](./type_defs.md#liststagingaccountsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [OSTypeDef](./type_defs.md#ostypedef)
- [ParticipatingResourceIDTypeDef](./type_defs.md#participatingresourceidtypedef)
- [RecoveryInstanceDataReplicationErrorTypeDef](./type_defs.md#recoveryinstancedatareplicationerrortypedef)
- [RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#recoveryinstancedatareplicationinforeplicateddisktypedef)
- [RecoveryInstanceDataReplicationInitiationStepTypeDef](./type_defs.md#recoveryinstancedatareplicationinitiationsteptypedef)
- [RecoveryInstanceDiskTypeDef](./type_defs.md#recoveryinstancedisktypedef)
- [RecoveryInstanceFailbackTypeDef](./type_defs.md#recoveryinstancefailbacktypedef)
- [RecoveryLifeCycleTypeDef](./type_defs.md#recoverylifecycletypedef)
- [ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef)
- [RetryDataReplicationRequestTypeDef](./type_defs.md#retrydatareplicationrequesttypedef)
- [ReverseReplicationRequestTypeDef](./type_defs.md#reversereplicationrequesttypedef)
- [SourceCloudPropertiesTypeDef](./type_defs.md#sourcecloudpropertiestypedef)
- [StagingAreaTypeDef](./type_defs.md#stagingareatypedef)
- [StartFailbackLaunchRequestTypeDef](./type_defs.md#startfailbacklaunchrequesttypedef)
- [StartRecoveryRequestSourceServerTypeDef](./type_defs.md#startrecoveryrequestsourceservertypedef)
- [StartReplicationRequestTypeDef](./type_defs.md#startreplicationrequesttypedef)
- [StartSourceNetworkRecoveryRequestNetworkEntryTypeDef](./type_defs.md#startsourcenetworkrecoveryrequestnetworkentrytypedef)
- [StartSourceNetworkReplicationRequestTypeDef](./type_defs.md#startsourcenetworkreplicationrequesttypedef)
- [StopFailbackRequestTypeDef](./type_defs.md#stopfailbackrequesttypedef)
- [StopReplicationRequestTypeDef](./type_defs.md#stopreplicationrequesttypedef)
- [StopSourceNetworkReplicationRequestTypeDef](./type_defs.md#stopsourcenetworkreplicationrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TerminateRecoveryInstancesRequestTypeDef](./type_defs.md#terminaterecoveryinstancesrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateFailbackReplicationConfigurationRequestTypeDef](./type_defs.md#updatefailbackreplicationconfigurationrequesttypedef)
- [CreateSourceNetworkResponseTypeDef](./type_defs.md#createsourcenetworkresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportSourceNetworkCfnTemplateResponseTypeDef](./type_defs.md#exportsourcenetworkcfntemplateresponsetypedef)
- [GetFailbackReplicationConfigurationResponseTypeDef](./type_defs.md#getfailbackreplicationconfigurationresponsetypedef)
- [ListStagingAccountsResponseTypeDef](./type_defs.md#liststagingaccountsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ReverseReplicationResponseTypeDef](./type_defs.md#reversereplicationresponsetypedef)
- [ConversionPropertiesTypeDef](./type_defs.md#conversionpropertiestypedef)
- [CreateLaunchConfigurationTemplateRequestTypeDef](./type_defs.md#createlaunchconfigurationtemplaterequesttypedef)
- [LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef)
- [UpdateLaunchConfigurationTemplateRequestTypeDef](./type_defs.md#updatelaunchconfigurationtemplaterequesttypedef)
- [CreateReplicationConfigurationTemplateRequestTypeDef](./type_defs.md#createreplicationconfigurationtemplaterequesttypedef)
- [ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef)
- [ReplicationConfigurationTemplateTypeDef](./type_defs.md#replicationconfigurationtemplatetypedef)
- [UpdateReplicationConfigurationTemplateRequestTypeDef](./type_defs.md#updatereplicationconfigurationtemplaterequesttypedef)
- [DataReplicationInitiationTypeDef](./type_defs.md#datareplicationinitiationtypedef)
- [DescribeJobLogItemsRequestPaginateTypeDef](./type_defs.md#describejoblogitemsrequestpaginatetypedef)
- [DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestpaginatetypedef)
- [DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestpaginatetypedef)
- [ListExtensibleSourceServersRequestPaginateTypeDef](./type_defs.md#listextensiblesourceserversrequestpaginatetypedef)
- [ListStagingAccountsRequestPaginateTypeDef](./type_defs.md#liststagingaccountsrequestpaginatetypedef)
- [DescribeJobsRequestPaginateTypeDef](./type_defs.md#describejobsrequestpaginatetypedef)
- [DescribeJobsRequestTypeDef](./type_defs.md#describejobsrequesttypedef)
- [DescribeRecoveryInstancesRequestPaginateTypeDef](./type_defs.md#describerecoveryinstancesrequestpaginatetypedef)
- [DescribeRecoveryInstancesRequestTypeDef](./type_defs.md#describerecoveryinstancesrequesttypedef)
- [DescribeRecoverySnapshotsRequestPaginateTypeDef](./type_defs.md#describerecoverysnapshotsrequestpaginatetypedef)
- [DescribeRecoverySnapshotsRequestTypeDef](./type_defs.md#describerecoverysnapshotsrequesttypedef)
- [DescribeRecoverySnapshotsResponseTypeDef](./type_defs.md#describerecoverysnapshotsresponsetypedef)
- [DescribeSourceNetworksRequestPaginateTypeDef](./type_defs.md#describesourcenetworksrequestpaginatetypedef)
- [DescribeSourceNetworksRequestTypeDef](./type_defs.md#describesourcenetworksrequesttypedef)
- [DescribeSourceServersRequestPaginateTypeDef](./type_defs.md#describesourceserversrequestpaginatetypedef)
- [DescribeSourceServersRequestTypeDef](./type_defs.md#describesourceserversrequesttypedef)
- [EventResourceDataTypeDef](./type_defs.md#eventresourcedatatypedef)
- [LaunchActionTypeDef](./type_defs.md#launchactiontypedef)
- [PutLaunchActionRequestTypeDef](./type_defs.md#putlaunchactionrequesttypedef)
- [PutLaunchActionResponseTypeDef](./type_defs.md#putlaunchactionresponsetypedef)
- [ListLaunchActionsRequestPaginateTypeDef](./type_defs.md#listlaunchactionsrequestpaginatetypedef)
- [ListLaunchActionsRequestTypeDef](./type_defs.md#listlaunchactionsrequesttypedef)
- [LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef)
- [UpdateLaunchConfigurationRequestTypeDef](./type_defs.md#updatelaunchconfigurationrequesttypedef)
- [LifeCycleLastLaunchTypeDef](./type_defs.md#lifecyclelastlaunchtypedef)
- [ListExtensibleSourceServersResponseTypeDef](./type_defs.md#listextensiblesourceserversresponsetypedef)
- [SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef)
- [ParticipatingResourceTypeDef](./type_defs.md#participatingresourcetypedef)
- [RecoveryInstanceDataReplicationInitiationTypeDef](./type_defs.md#recoveryinstancedatareplicationinitiationtypedef)
- [RecoveryInstancePropertiesTypeDef](./type_defs.md#recoveryinstancepropertiestypedef)
- [SourceNetworkTypeDef](./type_defs.md#sourcenetworktypedef)
- [ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef)
- [UpdateReplicationConfigurationRequestTypeDef](./type_defs.md#updatereplicationconfigurationrequesttypedef)
- [StartRecoveryRequestTypeDef](./type_defs.md#startrecoveryrequesttypedef)
- [StartSourceNetworkRecoveryRequestTypeDef](./type_defs.md#startsourcenetworkrecoveryrequesttypedef)
- [CreateLaunchConfigurationTemplateResponseTypeDef](./type_defs.md#createlaunchconfigurationtemplateresponsetypedef)
- [DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef)
- [UpdateLaunchConfigurationTemplateResponseTypeDef](./type_defs.md#updatelaunchconfigurationtemplateresponsetypedef)
- [DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef)
- [DataReplicationInfoTypeDef](./type_defs.md#datareplicationinfotypedef)
- [JobLogEventDataTypeDef](./type_defs.md#joblogeventdatatypedef)
- [LaunchActionRunTypeDef](./type_defs.md#launchactionruntypedef)
- [ListLaunchActionsResponseTypeDef](./type_defs.md#listlaunchactionsresponsetypedef)
- [LifeCycleTypeDef](./type_defs.md#lifecycletypedef)
- [RecoveryInstanceDataReplicationInfoTypeDef](./type_defs.md#recoveryinstancedatareplicationinfotypedef)
- [DescribeSourceNetworksResponseTypeDef](./type_defs.md#describesourcenetworksresponsetypedef)
- [StartSourceNetworkReplicationResponseTypeDef](./type_defs.md#startsourcenetworkreplicationresponsetypedef)
- [StopSourceNetworkReplicationResponseTypeDef](./type_defs.md#stopsourcenetworkreplicationresponsetypedef)
- [JobLogTypeDef](./type_defs.md#joblogtypedef)
- [LaunchActionsStatusTypeDef](./type_defs.md#launchactionsstatustypedef)
- [SourceServerResponseTypeDef](./type_defs.md#sourceserverresponsetypedef)
- [SourceServerTypeDef](./type_defs.md#sourceservertypedef)
- [RecoveryInstanceTypeDef](./type_defs.md#recoveryinstancetypedef)
- [DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef)
- [ParticipatingServerTypeDef](./type_defs.md#participatingservertypedef)
- [CreateExtendedSourceServerResponseTypeDef](./type_defs.md#createextendedsourceserverresponsetypedef)
- [DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef)
- [StartReplicationResponseTypeDef](./type_defs.md#startreplicationresponsetypedef)
- [StopReplicationResponseTypeDef](./type_defs.md#stopreplicationresponsetypedef)
- [DescribeRecoveryInstancesResponseTypeDef](./type_defs.md#describerecoveryinstancesresponsetypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [AssociateSourceNetworkStackResponseTypeDef](./type_defs.md#associatesourcenetworkstackresponsetypedef)
- [DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef)
- [StartFailbackLaunchResponseTypeDef](./type_defs.md#startfailbacklaunchresponsetypedef)
- [StartRecoveryResponseTypeDef](./type_defs.md#startrecoveryresponsetypedef)
- [StartSourceNetworkRecoveryResponseTypeDef](./type_defs.md#startsourcenetworkrecoveryresponsetypedef)
- [TerminateRecoveryInstancesResponseTypeDef](./type_defs.md#terminaterecoveryinstancesresponsetypedef)

