# ManagedintegrationsforIoTDeviceManagement module

> [Index](../README.md) > ManagedintegrationsforIoTDeviceManagement


!!! note ""

    Auto-generated documentation for [ManagedintegrationsforIoTDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations.html#managedintegrationsforiotdevicemanagement)
    type annotations stubs module [types-aiobotocore-iot-managed-integrations](https://pypi.org/project/types-aiobotocore-iot-managed-integrations/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.21.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ManagedintegrationsforIoTDeviceManagement` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ManagedintegrationsforIoTDeviceManagement` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iot-managed-integrations]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iot-managed-integrations]'

# standalone installation
python -m pip install types-aiobotocore-iot-managed-integrations
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iot-managed-integrations
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ManagedintegrationsforIoTDeviceManagementClient

Type annotations and code completion for  `#!python session.create_client("iot-managed-integrations")` as [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations.html#ManagedintegrationsforIoTDeviceManagement.Client)

```python
# ManagedintegrationsforIoTDeviceManagementClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.client import ManagedintegrationsforIoTDeviceManagementClient


session = get_session()
async with session.create_client("iot-managed-integrations") as client:
    client: ManagedintegrationsforIoTDeviceManagementClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("iot-managed-integrations").get_paginator("...")`.

```python
# ListCredentialLockersPaginator usage example

from types_aiobotocore_iot_managed_integrations.paginator import ListCredentialLockersPaginator

def get_list_credential_lockers_paginator() -> ListCredentialLockersPaginator:
    return client.get_paginator("list_credential_lockers"))
```

- [ListCredentialLockersPaginator](./paginators.md#listcredentiallockerspaginator)
- [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
- [ListEventLogConfigurationsPaginator](./paginators.md#listeventlogconfigurationspaginator)
- [ListManagedThingSchemasPaginator](./paginators.md#listmanagedthingschemaspaginator)
- [ListManagedThingsPaginator](./paginators.md#listmanagedthingspaginator)
- [ListNotificationConfigurationsPaginator](./paginators.md#listnotificationconfigurationspaginator)
- [ListOtaTaskConfigurationsPaginator](./paginators.md#listotataskconfigurationspaginator)
- [ListOtaTaskExecutionsPaginator](./paginators.md#listotataskexecutionspaginator)
- [ListOtaTasksPaginator](./paginators.md#listotataskspaginator)
- [ListProvisioningProfilesPaginator](./paginators.md#listprovisioningprofilespaginator)
- [ListSchemaVersionsPaginator](./paginators.md#listschemaversionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AbortCriteriaActionType usage example

from types_aiobotocore_iot_managed_integrations.literals import AbortCriteriaActionType

def get_value() -> AbortCriteriaActionType:
    return "CANCEL"
```

- [AbortCriteriaActionType](./literals.md#abortcriteriaactiontype)
- [AbortCriteriaFailureTypeType](./literals.md#abortcriteriafailuretypetype)
- [AuthMaterialTypeType](./literals.md#authmaterialtypetype)
- [ConfigurationStateType](./literals.md#configurationstatetype)
- [DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype)
- [DeviceDiscoveryStatusType](./literals.md#devicediscoverystatustype)
- [DisconnectReasonValueType](./literals.md#disconnectreasonvaluetype)
- [DiscoveryAuthMaterialTypeType](./literals.md#discoveryauthmaterialtypetype)
- [DiscoveryTypeType](./literals.md#discoverytypetype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [EventTypeType](./literals.md#eventtypetype)
- [HubNetworkModeType](./literals.md#hubnetworkmodetype)
- [ListCredentialLockersPaginatorName](./literals.md#listcredentiallockerspaginatorname)
- [ListDestinationsPaginatorName](./literals.md#listdestinationspaginatorname)
- [ListEventLogConfigurationsPaginatorName](./literals.md#listeventlogconfigurationspaginatorname)
- [ListManagedThingSchemasPaginatorName](./literals.md#listmanagedthingschemaspaginatorname)
- [ListManagedThingsPaginatorName](./literals.md#listmanagedthingspaginatorname)
- [ListNotificationConfigurationsPaginatorName](./literals.md#listnotificationconfigurationspaginatorname)
- [ListOtaTaskConfigurationsPaginatorName](./literals.md#listotataskconfigurationspaginatorname)
- [ListOtaTaskExecutionsPaginatorName](./literals.md#listotataskexecutionspaginatorname)
- [ListOtaTasksPaginatorName](./literals.md#listotataskspaginatorname)
- [ListProvisioningProfilesPaginatorName](./literals.md#listprovisioningprofilespaginatorname)
- [ListSchemaVersionsPaginatorName](./literals.md#listschemaversionspaginatorname)
- [LogLevelType](./literals.md#logleveltype)
- [OtaMechanismType](./literals.md#otamechanismtype)
- [OtaProtocolType](./literals.md#otaprotocoltype)
- [OtaStatusType](./literals.md#otastatustype)
- [OtaTaskExecutionStatusType](./literals.md#otataskexecutionstatustype)
- [OtaTypeType](./literals.md#otatypetype)
- [ProvisioningStatusType](./literals.md#provisioningstatustype)
- [ProvisioningTypeType](./literals.md#provisioningtypetype)
- [RetryCriteriaFailureTypeType](./literals.md#retrycriteriafailuretypetype)
- [RoleType](./literals.md#roletype)
- [SchedulingConfigEndBehaviorType](./literals.md#schedulingconfigendbehaviortype)
- [SchemaVersionFormatType](./literals.md#schemaversionformattype)
- [SchemaVersionTypeType](./literals.md#schemaversiontypetype)
- [SchemaVersionVisibilityType](./literals.md#schemaversionvisibilitytype)
- [ManagedintegrationsforIoTDeviceManagementServiceName](./literals.md#managedintegrationsforiotdevicemanagementservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbortConfigCriteriaTypeDef](./type_defs.md#abortconfigcriteriatypedef)
- [CapabilityActionTypeDef](./type_defs.md#capabilityactiontypedef)
- [CapabilityReportCapabilityOutputTypeDef](./type_defs.md#capabilityreportcapabilityoutputtypedef)
- [CapabilityReportCapabilityTypeDef](./type_defs.md#capabilityreportcapabilitytypedef)
- [ConfigurationErrorTypeDef](./type_defs.md#configurationerrortypedef)
- [CreateCredentialLockerRequestTypeDef](./type_defs.md#createcredentiallockerrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateDestinationRequestTypeDef](./type_defs.md#createdestinationrequesttypedef)
- [CreateEventLogConfigurationRequestTypeDef](./type_defs.md#createeventlogconfigurationrequesttypedef)
- [CreateNotificationConfigurationRequestTypeDef](./type_defs.md#createnotificationconfigurationrequesttypedef)
- [CreateProvisioningProfileRequestTypeDef](./type_defs.md#createprovisioningprofilerequesttypedef)
- [CredentialLockerSummaryTypeDef](./type_defs.md#credentiallockersummarytypedef)
- [DeleteCredentialLockerRequestTypeDef](./type_defs.md#deletecredentiallockerrequesttypedef)
- [DeleteDestinationRequestTypeDef](./type_defs.md#deletedestinationrequesttypedef)
- [DeleteEventLogConfigurationRequestTypeDef](./type_defs.md#deleteeventlogconfigurationrequesttypedef)
- [DeleteManagedThingRequestTypeDef](./type_defs.md#deletemanagedthingrequesttypedef)
- [DeleteNotificationConfigurationRequestTypeDef](./type_defs.md#deletenotificationconfigurationrequesttypedef)
- [DeleteOtaTaskConfigurationRequestTypeDef](./type_defs.md#deleteotataskconfigurationrequesttypedef)
- [DeleteOtaTaskRequestTypeDef](./type_defs.md#deleteotataskrequesttypedef)
- [DeleteProvisioningProfileRequestTypeDef](./type_defs.md#deleteprovisioningprofilerequesttypedef)
- [DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef)
- [EventLogConfigurationSummaryTypeDef](./type_defs.md#eventlogconfigurationsummarytypedef)
- [RolloutRateIncreaseCriteriaTypeDef](./type_defs.md#rolloutrateincreasecriteriatypedef)
- [GetCredentialLockerRequestTypeDef](./type_defs.md#getcredentiallockerrequesttypedef)
- [GetDestinationRequestTypeDef](./type_defs.md#getdestinationrequesttypedef)
- [GetDeviceDiscoveryRequestTypeDef](./type_defs.md#getdevicediscoveryrequesttypedef)
- [GetEventLogConfigurationRequestTypeDef](./type_defs.md#geteventlogconfigurationrequesttypedef)
- [GetManagedThingCapabilitiesRequestTypeDef](./type_defs.md#getmanagedthingcapabilitiesrequesttypedef)
- [GetManagedThingConnectivityDataRequestTypeDef](./type_defs.md#getmanagedthingconnectivitydatarequesttypedef)
- [GetManagedThingMetaDataRequestTypeDef](./type_defs.md#getmanagedthingmetadatarequesttypedef)
- [GetManagedThingRequestTypeDef](./type_defs.md#getmanagedthingrequesttypedef)
- [GetManagedThingStateRequestTypeDef](./type_defs.md#getmanagedthingstaterequesttypedef)
- [GetNotificationConfigurationRequestTypeDef](./type_defs.md#getnotificationconfigurationrequesttypedef)
- [GetOtaTaskConfigurationRequestTypeDef](./type_defs.md#getotataskconfigurationrequesttypedef)
- [GetOtaTaskRequestTypeDef](./type_defs.md#getotataskrequesttypedef)
- [TaskProcessingDetailsTypeDef](./type_defs.md#taskprocessingdetailstypedef)
- [GetProvisioningProfileRequestTypeDef](./type_defs.md#getprovisioningprofilerequesttypedef)
- [GetRuntimeLogConfigurationRequestTypeDef](./type_defs.md#getruntimelogconfigurationrequesttypedef)
- [RuntimeLogConfigurationsTypeDef](./type_defs.md#runtimelogconfigurationstypedef)
- [GetSchemaVersionRequestTypeDef](./type_defs.md#getschemaversionrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCredentialLockersRequestTypeDef](./type_defs.md#listcredentiallockersrequesttypedef)
- [ListDestinationsRequestTypeDef](./type_defs.md#listdestinationsrequesttypedef)
- [ListEventLogConfigurationsRequestTypeDef](./type_defs.md#listeventlogconfigurationsrequesttypedef)
- [ListManagedThingSchemasRequestTypeDef](./type_defs.md#listmanagedthingschemasrequesttypedef)
- [ManagedThingSchemaListItemTypeDef](./type_defs.md#managedthingschemalistitemtypedef)
- [ListManagedThingsRequestTypeDef](./type_defs.md#listmanagedthingsrequesttypedef)
- [ManagedThingSummaryTypeDef](./type_defs.md#managedthingsummarytypedef)
- [ListNotificationConfigurationsRequestTypeDef](./type_defs.md#listnotificationconfigurationsrequesttypedef)
- [NotificationConfigurationSummaryTypeDef](./type_defs.md#notificationconfigurationsummarytypedef)
- [ListOtaTaskConfigurationsRequestTypeDef](./type_defs.md#listotataskconfigurationsrequesttypedef)
- [OtaTaskConfigurationSummaryTypeDef](./type_defs.md#otataskconfigurationsummarytypedef)
- [ListOtaTaskExecutionsRequestTypeDef](./type_defs.md#listotataskexecutionsrequesttypedef)
- [ListOtaTasksRequestTypeDef](./type_defs.md#listotatasksrequesttypedef)
- [OtaTaskSummaryTypeDef](./type_defs.md#otatasksummarytypedef)
- [ListProvisioningProfilesRequestTypeDef](./type_defs.md#listprovisioningprofilesrequesttypedef)
- [ProvisioningProfileSummaryTypeDef](./type_defs.md#provisioningprofilesummarytypedef)
- [ListSchemaVersionsRequestTypeDef](./type_defs.md#listschemaversionsrequesttypedef)
- [SchemaVersionListItemTypeDef](./type_defs.md#schemaversionlistitemtypedef)
- [RetryConfigCriteriaTypeDef](./type_defs.md#retryconfigcriteriatypedef)
- [OtaTaskExecutionSummaryTypeDef](./type_defs.md#otataskexecutionsummarytypedef)
- [ScheduleMaintenanceWindowTypeDef](./type_defs.md#schedulemaintenancewindowtypedef)
- [OtaTaskTimeoutConfigTypeDef](./type_defs.md#otatasktimeoutconfigtypedef)
- [PutDefaultEncryptionConfigurationRequestTypeDef](./type_defs.md#putdefaultencryptionconfigurationrequesttypedef)
- [PutHubConfigurationRequestTypeDef](./type_defs.md#puthubconfigurationrequesttypedef)
- [ResetRuntimeLogConfigurationRequestTypeDef](./type_defs.md#resetruntimelogconfigurationrequesttypedef)
- [StartDeviceDiscoveryRequestTypeDef](./type_defs.md#startdevicediscoveryrequesttypedef)
- [StateCapabilityTypeDef](./type_defs.md#statecapabilitytypedef)
- [UpdateDestinationRequestTypeDef](./type_defs.md#updatedestinationrequesttypedef)
- [UpdateEventLogConfigurationRequestTypeDef](./type_defs.md#updateeventlogconfigurationrequesttypedef)
- [UpdateNotificationConfigurationRequestTypeDef](./type_defs.md#updatenotificationconfigurationrequesttypedef)
- [UpdateOtaTaskRequestTypeDef](./type_defs.md#updateotataskrequesttypedef)
- [OtaTaskAbortConfigOutputTypeDef](./type_defs.md#otataskabortconfigoutputtypedef)
- [OtaTaskAbortConfigTypeDef](./type_defs.md#otataskabortconfigtypedef)
- [CommandCapabilityTypeDef](./type_defs.md#commandcapabilitytypedef)
- [CapabilityReportEndpointOutputTypeDef](./type_defs.md#capabilityreportendpointoutputtypedef)
- [CapabilityReportEndpointTypeDef](./type_defs.md#capabilityreportendpointtypedef)
- [ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef)
- [CreateCredentialLockerResponseTypeDef](./type_defs.md#createcredentiallockerresponsetypedef)
- [CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef)
- [CreateEventLogConfigurationResponseTypeDef](./type_defs.md#createeventlogconfigurationresponsetypedef)
- [CreateManagedThingResponseTypeDef](./type_defs.md#createmanagedthingresponsetypedef)
- [CreateNotificationConfigurationResponseTypeDef](./type_defs.md#createnotificationconfigurationresponsetypedef)
- [CreateOtaTaskConfigurationResponseTypeDef](./type_defs.md#createotataskconfigurationresponsetypedef)
- [CreateOtaTaskResponseTypeDef](./type_defs.md#createotataskresponsetypedef)
- [CreateProvisioningProfileResponseTypeDef](./type_defs.md#createprovisioningprofileresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetCredentialLockerResponseTypeDef](./type_defs.md#getcredentiallockerresponsetypedef)
- [GetCustomEndpointResponseTypeDef](./type_defs.md#getcustomendpointresponsetypedef)
- [GetDestinationResponseTypeDef](./type_defs.md#getdestinationresponsetypedef)
- [GetDeviceDiscoveryResponseTypeDef](./type_defs.md#getdevicediscoveryresponsetypedef)
- [GetEventLogConfigurationResponseTypeDef](./type_defs.md#geteventlogconfigurationresponsetypedef)
- [GetHubConfigurationResponseTypeDef](./type_defs.md#gethubconfigurationresponsetypedef)
- [GetManagedThingConnectivityDataResponseTypeDef](./type_defs.md#getmanagedthingconnectivitydataresponsetypedef)
- [GetManagedThingMetaDataResponseTypeDef](./type_defs.md#getmanagedthingmetadataresponsetypedef)
- [GetManagedThingResponseTypeDef](./type_defs.md#getmanagedthingresponsetypedef)
- [GetNotificationConfigurationResponseTypeDef](./type_defs.md#getnotificationconfigurationresponsetypedef)
- [GetProvisioningProfileResponseTypeDef](./type_defs.md#getprovisioningprofileresponsetypedef)
- [GetSchemaVersionResponseTypeDef](./type_defs.md#getschemaversionresponsetypedef)
- [PutHubConfigurationResponseTypeDef](./type_defs.md#puthubconfigurationresponsetypedef)
- [RegisterCustomEndpointResponseTypeDef](./type_defs.md#registercustomendpointresponsetypedef)
- [SendManagedThingCommandResponseTypeDef](./type_defs.md#sendmanagedthingcommandresponsetypedef)
- [StartDeviceDiscoveryResponseTypeDef](./type_defs.md#startdevicediscoveryresponsetypedef)
- [ListCredentialLockersResponseTypeDef](./type_defs.md#listcredentiallockersresponsetypedef)
- [ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef)
- [ListEventLogConfigurationsResponseTypeDef](./type_defs.md#listeventlogconfigurationsresponsetypedef)
- [ExponentialRolloutRateTypeDef](./type_defs.md#exponentialrolloutratetypedef)
- [GetRuntimeLogConfigurationResponseTypeDef](./type_defs.md#getruntimelogconfigurationresponsetypedef)
- [PutRuntimeLogConfigurationRequestTypeDef](./type_defs.md#putruntimelogconfigurationrequesttypedef)
- [ListCredentialLockersRequestPaginateTypeDef](./type_defs.md#listcredentiallockersrequestpaginatetypedef)
- [ListDestinationsRequestPaginateTypeDef](./type_defs.md#listdestinationsrequestpaginatetypedef)
- [ListEventLogConfigurationsRequestPaginateTypeDef](./type_defs.md#listeventlogconfigurationsrequestpaginatetypedef)
- [ListManagedThingSchemasRequestPaginateTypeDef](./type_defs.md#listmanagedthingschemasrequestpaginatetypedef)
- [ListManagedThingsRequestPaginateTypeDef](./type_defs.md#listmanagedthingsrequestpaginatetypedef)
- [ListNotificationConfigurationsRequestPaginateTypeDef](./type_defs.md#listnotificationconfigurationsrequestpaginatetypedef)
- [ListOtaTaskConfigurationsRequestPaginateTypeDef](./type_defs.md#listotataskconfigurationsrequestpaginatetypedef)
- [ListOtaTaskExecutionsRequestPaginateTypeDef](./type_defs.md#listotataskexecutionsrequestpaginatetypedef)
- [ListOtaTasksRequestPaginateTypeDef](./type_defs.md#listotatasksrequestpaginatetypedef)
- [ListProvisioningProfilesRequestPaginateTypeDef](./type_defs.md#listprovisioningprofilesrequestpaginatetypedef)
- [ListSchemaVersionsRequestPaginateTypeDef](./type_defs.md#listschemaversionsrequestpaginatetypedef)
- [ListManagedThingSchemasResponseTypeDef](./type_defs.md#listmanagedthingschemasresponsetypedef)
- [ListManagedThingsResponseTypeDef](./type_defs.md#listmanagedthingsresponsetypedef)
- [ListNotificationConfigurationsResponseTypeDef](./type_defs.md#listnotificationconfigurationsresponsetypedef)
- [ListOtaTaskConfigurationsResponseTypeDef](./type_defs.md#listotataskconfigurationsresponsetypedef)
- [ListOtaTasksResponseTypeDef](./type_defs.md#listotatasksresponsetypedef)
- [ListProvisioningProfilesResponseTypeDef](./type_defs.md#listprovisioningprofilesresponsetypedef)
- [ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef)
- [OtaTaskExecutionRetryConfigOutputTypeDef](./type_defs.md#otataskexecutionretryconfigoutputtypedef)
- [OtaTaskExecutionRetryConfigTypeDef](./type_defs.md#otataskexecutionretryconfigtypedef)
- [OtaTaskExecutionSummariesTypeDef](./type_defs.md#otataskexecutionsummariestypedef)
- [OtaTaskSchedulingConfigOutputTypeDef](./type_defs.md#otataskschedulingconfigoutputtypedef)
- [OtaTaskSchedulingConfigTypeDef](./type_defs.md#otataskschedulingconfigtypedef)
- [StateEndpointTypeDef](./type_defs.md#stateendpointtypedef)
- [CommandEndpointTypeDef](./type_defs.md#commandendpointtypedef)
- [CapabilityReportOutputTypeDef](./type_defs.md#capabilityreportoutputtypedef)
- [CapabilityReportTypeDef](./type_defs.md#capabilityreporttypedef)
- [GetDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#getdefaultencryptionconfigurationresponsetypedef)
- [PutDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#putdefaultencryptionconfigurationresponsetypedef)
- [OtaTaskExecutionRolloutConfigTypeDef](./type_defs.md#otataskexecutionrolloutconfigtypedef)
- [OtaTaskExecutionRetryConfigUnionTypeDef](./type_defs.md#otataskexecutionretryconfiguniontypedef)
- [ListOtaTaskExecutionsResponseTypeDef](./type_defs.md#listotataskexecutionsresponsetypedef)
- [GetOtaTaskResponseTypeDef](./type_defs.md#getotataskresponsetypedef)
- [OtaTaskSchedulingConfigUnionTypeDef](./type_defs.md#otataskschedulingconfiguniontypedef)
- [GetManagedThingStateResponseTypeDef](./type_defs.md#getmanagedthingstateresponsetypedef)
- [SendManagedThingCommandRequestTypeDef](./type_defs.md#sendmanagedthingcommandrequesttypedef)
- [GetManagedThingCapabilitiesResponseTypeDef](./type_defs.md#getmanagedthingcapabilitiesresponsetypedef)
- [CapabilityReportUnionTypeDef](./type_defs.md#capabilityreportuniontypedef)
- [PushConfigOutputTypeDef](./type_defs.md#pushconfigoutputtypedef)
- [PushConfigTypeDef](./type_defs.md#pushconfigtypedef)
- [CreateOtaTaskRequestTypeDef](./type_defs.md#createotataskrequesttypedef)
- [CreateManagedThingRequestTypeDef](./type_defs.md#createmanagedthingrequesttypedef)
- [UpdateManagedThingRequestTypeDef](./type_defs.md#updatemanagedthingrequesttypedef)
- [GetOtaTaskConfigurationResponseTypeDef](./type_defs.md#getotataskconfigurationresponsetypedef)
- [PushConfigUnionTypeDef](./type_defs.md#pushconfiguniontypedef)
- [CreateOtaTaskConfigurationRequestTypeDef](./type_defs.md#createotataskconfigurationrequesttypedef)

