# Drs module

> [Index](../README.md) > Drs


!!! note ""

    Auto-generated documentation for [Drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#Drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

## How to install



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
- [AssociateSourceNetworkStackRequestRequestTypeDef](./type_defs.md#associatesourcenetworkstackrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CPUTypeDef](./type_defs.md#cputypedef)
- [ProductCodeTypeDef](./type_defs.md#productcodetypedef)
- [CreateExtendedSourceServerRequestRequestTypeDef](./type_defs.md#createextendedsourceserverrequestrequesttypedef)
- [LicensingTypeDef](./type_defs.md#licensingtypedef)
- [PITPolicyRuleTypeDef](./type_defs.md#pitpolicyruletypedef)
- [CreateSourceNetworkRequestRequestTypeDef](./type_defs.md#createsourcenetworkrequestrequesttypedef)
- [DataReplicationErrorTypeDef](./type_defs.md#datareplicationerrortypedef)
- [DataReplicationInfoReplicatedDiskTypeDef](./type_defs.md#datareplicationinforeplicateddisktypedef)
- [DataReplicationInitiationStepTypeDef](./type_defs.md#datareplicationinitiationsteptypedef)
- [DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef)
- [DeleteLaunchActionRequestRequestTypeDef](./type_defs.md#deletelaunchactionrequestrequesttypedef)
- [DeleteLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#deletelaunchconfigurationtemplaterequestrequesttypedef)
- [DeleteRecoveryInstanceRequestRequestTypeDef](./type_defs.md#deleterecoveryinstancerequestrequesttypedef)
- [DeleteReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#deletereplicationconfigurationtemplaterequestrequesttypedef)
- [DeleteSourceNetworkRequestRequestTypeDef](./type_defs.md#deletesourcenetworkrequestrequesttypedef)
- [DeleteSourceServerRequestRequestTypeDef](./type_defs.md#deletesourceserverrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeJobLogItemsRequestRequestTypeDef](./type_defs.md#describejoblogitemsrequestrequesttypedef)
- [DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef)
- [DescribeLaunchConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestrequesttypedef)
- [DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef)
- [DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef)
- [RecoverySnapshotTypeDef](./type_defs.md#recoverysnapshottypedef)
- [DescribeReplicationConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestrequesttypedef)
- [DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef)
- [DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef)
- [DisconnectRecoveryInstanceRequestRequestTypeDef](./type_defs.md#disconnectrecoveryinstancerequestrequesttypedef)
- [DisconnectSourceServerRequestRequestTypeDef](./type_defs.md#disconnectsourceserverrequestrequesttypedef)
- [DiskTypeDef](./type_defs.md#disktypedef)
- [SourceNetworkDataTypeDef](./type_defs.md#sourcenetworkdatatypedef)
- [ExportSourceNetworkCfnTemplateRequestRequestTypeDef](./type_defs.md#exportsourcenetworkcfntemplaterequestrequesttypedef)
- [GetFailbackReplicationConfigurationRequestRequestTypeDef](./type_defs.md#getfailbackreplicationconfigurationrequestrequesttypedef)
- [GetLaunchConfigurationRequestRequestTypeDef](./type_defs.md#getlaunchconfigurationrequestrequesttypedef)
- [GetReplicationConfigurationRequestRequestTypeDef](./type_defs.md#getreplicationconfigurationrequestrequesttypedef)
- [IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef)
- [LaunchActionParameterTypeDef](./type_defs.md#launchactionparametertypedef)
- [LaunchActionsRequestFiltersTypeDef](./type_defs.md#launchactionsrequestfilterstypedef)
- [LaunchIntoInstancePropertiesTypeDef](./type_defs.md#launchintoinstancepropertiestypedef)
- [LifeCycleLastLaunchInitiatedTypeDef](./type_defs.md#lifecyclelastlaunchinitiatedtypedef)
- [ListExtensibleSourceServersRequestRequestTypeDef](./type_defs.md#listextensiblesourceserversrequestrequesttypedef)
- [StagingSourceServerTypeDef](./type_defs.md#stagingsourceservertypedef)
- [ListStagingAccountsRequestRequestTypeDef](./type_defs.md#liststagingaccountsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
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
- [RetryDataReplicationRequestRequestTypeDef](./type_defs.md#retrydatareplicationrequestrequesttypedef)
- [ReverseReplicationRequestRequestTypeDef](./type_defs.md#reversereplicationrequestrequesttypedef)
- [SourceCloudPropertiesTypeDef](./type_defs.md#sourcecloudpropertiestypedef)
- [StagingAreaTypeDef](./type_defs.md#stagingareatypedef)
- [StartFailbackLaunchRequestRequestTypeDef](./type_defs.md#startfailbacklaunchrequestrequesttypedef)
- [StartRecoveryRequestSourceServerTypeDef](./type_defs.md#startrecoveryrequestsourceservertypedef)
- [StartReplicationRequestRequestTypeDef](./type_defs.md#startreplicationrequestrequesttypedef)
- [StartSourceNetworkRecoveryRequestNetworkEntryTypeDef](./type_defs.md#startsourcenetworkrecoveryrequestnetworkentrytypedef)
- [StartSourceNetworkReplicationRequestRequestTypeDef](./type_defs.md#startsourcenetworkreplicationrequestrequesttypedef)
- [StopFailbackRequestRequestTypeDef](./type_defs.md#stopfailbackrequestrequesttypedef)
- [StopReplicationRequestRequestTypeDef](./type_defs.md#stopreplicationrequestrequesttypedef)
- [StopSourceNetworkReplicationRequestRequestTypeDef](./type_defs.md#stopsourcenetworkreplicationrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TerminateRecoveryInstancesRequestRequestTypeDef](./type_defs.md#terminaterecoveryinstancesrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFailbackReplicationConfigurationRequestRequestTypeDef](./type_defs.md#updatefailbackreplicationconfigurationrequestrequesttypedef)
- [CreateSourceNetworkResponseTypeDef](./type_defs.md#createsourcenetworkresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportSourceNetworkCfnTemplateResponseTypeDef](./type_defs.md#exportsourcenetworkcfntemplateresponsetypedef)
- [GetFailbackReplicationConfigurationResponseTypeDef](./type_defs.md#getfailbackreplicationconfigurationresponsetypedef)
- [ListStagingAccountsResponseTypeDef](./type_defs.md#liststagingaccountsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ReverseReplicationResponseTypeDef](./type_defs.md#reversereplicationresponsetypedef)
- [ConversionPropertiesTypeDef](./type_defs.md#conversionpropertiestypedef)
- [CreateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createlaunchconfigurationtemplaterequestrequesttypedef)
- [LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef)
- [UpdateLaunchConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationtemplaterequestrequesttypedef)
- [CreateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createreplicationconfigurationtemplaterequestrequesttypedef)
- [ReplicationConfigurationTemplateResponseTypeDef](./type_defs.md#replicationconfigurationtemplateresponsetypedef)
- [ReplicationConfigurationTemplateTypeDef](./type_defs.md#replicationconfigurationtemplatetypedef)
- [UpdateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationtemplaterequestrequesttypedef)
- [DataReplicationInitiationTypeDef](./type_defs.md#datareplicationinitiationtypedef)
- [DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef](./type_defs.md#describejoblogitemsrequestdescribejoblogitemspaginatetypedef)
- [DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestdescribelaunchconfigurationtemplatespaginatetypedef)
- [DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestdescribereplicationconfigurationtemplatespaginatetypedef)
- [ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef](./type_defs.md#listextensiblesourceserversrequestlistextensiblesourceserverspaginatetypedef)
- [ListStagingAccountsRequestListStagingAccountsPaginateTypeDef](./type_defs.md#liststagingaccountsrequestliststagingaccountspaginatetypedef)
- [DescribeJobsRequestDescribeJobsPaginateTypeDef](./type_defs.md#describejobsrequestdescribejobspaginatetypedef)
- [DescribeJobsRequestRequestTypeDef](./type_defs.md#describejobsrequestrequesttypedef)
- [DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef](./type_defs.md#describerecoveryinstancesrequestdescriberecoveryinstancespaginatetypedef)
- [DescribeRecoveryInstancesRequestRequestTypeDef](./type_defs.md#describerecoveryinstancesrequestrequesttypedef)
- [DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef](./type_defs.md#describerecoverysnapshotsrequestdescriberecoverysnapshotspaginatetypedef)
- [DescribeRecoverySnapshotsRequestRequestTypeDef](./type_defs.md#describerecoverysnapshotsrequestrequesttypedef)
- [DescribeRecoverySnapshotsResponseTypeDef](./type_defs.md#describerecoverysnapshotsresponsetypedef)
- [DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef](./type_defs.md#describesourcenetworksrequestdescribesourcenetworkspaginatetypedef)
- [DescribeSourceNetworksRequestRequestTypeDef](./type_defs.md#describesourcenetworksrequestrequesttypedef)
- [DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef](./type_defs.md#describesourceserversrequestdescribesourceserverspaginatetypedef)
- [DescribeSourceServersRequestRequestTypeDef](./type_defs.md#describesourceserversrequestrequesttypedef)
- [EventResourceDataTypeDef](./type_defs.md#eventresourcedatatypedef)
- [LaunchActionTypeDef](./type_defs.md#launchactiontypedef)
- [PutLaunchActionRequestRequestTypeDef](./type_defs.md#putlaunchactionrequestrequesttypedef)
- [PutLaunchActionResponseTypeDef](./type_defs.md#putlaunchactionresponsetypedef)
- [ListLaunchActionsRequestListLaunchActionsPaginateTypeDef](./type_defs.md#listlaunchactionsrequestlistlaunchactionspaginatetypedef)
- [ListLaunchActionsRequestRequestTypeDef](./type_defs.md#listlaunchactionsrequestrequesttypedef)
- [LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef)
- [UpdateLaunchConfigurationRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationrequestrequesttypedef)
- [LifeCycleLastLaunchTypeDef](./type_defs.md#lifecyclelastlaunchtypedef)
- [ListExtensibleSourceServersResponseTypeDef](./type_defs.md#listextensiblesourceserversresponsetypedef)
- [SourcePropertiesTypeDef](./type_defs.md#sourcepropertiestypedef)
- [ParticipatingResourceTypeDef](./type_defs.md#participatingresourcetypedef)
- [RecoveryInstanceDataReplicationInitiationTypeDef](./type_defs.md#recoveryinstancedatareplicationinitiationtypedef)
- [RecoveryInstancePropertiesTypeDef](./type_defs.md#recoveryinstancepropertiestypedef)
- [SourceNetworkTypeDef](./type_defs.md#sourcenetworktypedef)
- [ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef)
- [UpdateReplicationConfigurationRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationrequestrequesttypedef)
- [StartRecoveryRequestRequestTypeDef](./type_defs.md#startrecoveryrequestrequesttypedef)
- [StartSourceNetworkRecoveryRequestRequestTypeDef](./type_defs.md#startsourcenetworkrecoveryrequestrequesttypedef)
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

