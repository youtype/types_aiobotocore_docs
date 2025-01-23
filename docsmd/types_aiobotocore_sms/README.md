# SMS module

> [Index](../README.md) > SMS


!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#sms)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SMS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SMS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sms]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sms]'

# standalone installation
python -m pip install types-aiobotocore-sms
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sms
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SMSClient

Type annotations and code completion for  `#!python session.create_client("sms")` as [SMSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client)

```python
# SMSClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_sms.client import SMSClient


session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("sms").get_paginator("...")`.

```python
# GetConnectorsPaginator usage example

from types_aiobotocore_sms.paginator import GetConnectorsPaginator

def get_get_connectors_paginator() -> GetConnectorsPaginator:
    return client.get_paginator("get_connectors"))
```

- [GetConnectorsPaginator](./paginators.md#getconnectorspaginator)
- [GetReplicationJobsPaginator](./paginators.md#getreplicationjobspaginator)
- [GetReplicationRunsPaginator](./paginators.md#getreplicationrunspaginator)
- [GetServersPaginator](./paginators.md#getserverspaginator)
- [ListAppsPaginator](./paginators.md#listappspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AppLaunchConfigurationStatusType usage example

from types_aiobotocore_sms.literals import AppLaunchConfigurationStatusType

def get_value() -> AppLaunchConfigurationStatusType:
    return "CONFIGURED"
```

- [AppLaunchConfigurationStatusType](./literals.md#applaunchconfigurationstatustype)
- [AppLaunchStatusType](./literals.md#applaunchstatustype)
- [AppReplicationConfigurationStatusType](./literals.md#appreplicationconfigurationstatustype)
- [AppReplicationStatusType](./literals.md#appreplicationstatustype)
- [AppStatusType](./literals.md#appstatustype)
- [AppValidationStrategyType](./literals.md#appvalidationstrategytype)
- [ConnectorCapabilityType](./literals.md#connectorcapabilitytype)
- [ConnectorStatusType](./literals.md#connectorstatustype)
- [GetConnectorsPaginatorName](./literals.md#getconnectorspaginatorname)
- [GetReplicationJobsPaginatorName](./literals.md#getreplicationjobspaginatorname)
- [GetReplicationRunsPaginatorName](./literals.md#getreplicationrunspaginatorname)
- [GetServersPaginatorName](./literals.md#getserverspaginatorname)
- [LicenseTypeType](./literals.md#licensetypetype)
- [ListAppsPaginatorName](./literals.md#listappspaginatorname)
- [OutputFormatType](./literals.md#outputformattype)
- [ReplicationJobStateType](./literals.md#replicationjobstatetype)
- [ReplicationRunStateType](./literals.md#replicationrunstatetype)
- [ReplicationRunTypeType](./literals.md#replicationruntypetype)
- [ScriptTypeType](./literals.md#scripttypetype)
- [ServerCatalogStatusType](./literals.md#servercatalogstatustype)
- [ServerTypeType](./literals.md#servertypetype)
- [ServerValidationStrategyType](./literals.md#servervalidationstrategytype)
- [ValidationStatusType](./literals.md#validationstatustype)
- [VmManagerTypeType](./literals.md#vmmanagertypetype)
- [SMSServiceName](./literals.md#smsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [LaunchDetailsTypeDef](./type_defs.md#launchdetailstypedef)
- [ConnectorTypeDef](./type_defs.md#connectortypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DeleteAppLaunchConfigurationRequestRequestTypeDef](./type_defs.md#deleteapplaunchconfigurationrequestrequesttypedef)
- [DeleteAppReplicationConfigurationRequestRequestTypeDef](./type_defs.md#deleteappreplicationconfigurationrequestrequesttypedef)
- [DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef)
- [DeleteAppValidationConfigurationRequestRequestTypeDef](./type_defs.md#deleteappvalidationconfigurationrequestrequesttypedef)
- [DeleteReplicationJobRequestRequestTypeDef](./type_defs.md#deletereplicationjobrequestrequesttypedef)
- [DisassociateConnectorRequestRequestTypeDef](./type_defs.md#disassociateconnectorrequestrequesttypedef)
- [GenerateChangeSetRequestRequestTypeDef](./type_defs.md#generatechangesetrequestrequesttypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [GenerateTemplateRequestRequestTypeDef](./type_defs.md#generatetemplaterequestrequesttypedef)
- [GetAppLaunchConfigurationRequestRequestTypeDef](./type_defs.md#getapplaunchconfigurationrequestrequesttypedef)
- [GetAppReplicationConfigurationRequestRequestTypeDef](./type_defs.md#getappreplicationconfigurationrequestrequesttypedef)
- [GetAppRequestRequestTypeDef](./type_defs.md#getapprequestrequesttypedef)
- [GetAppValidationConfigurationRequestRequestTypeDef](./type_defs.md#getappvalidationconfigurationrequestrequesttypedef)
- [GetAppValidationOutputRequestRequestTypeDef](./type_defs.md#getappvalidationoutputrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetConnectorsRequestRequestTypeDef](./type_defs.md#getconnectorsrequestrequesttypedef)
- [GetReplicationJobsRequestRequestTypeDef](./type_defs.md#getreplicationjobsrequestrequesttypedef)
- [GetReplicationRunsRequestRequestTypeDef](./type_defs.md#getreplicationrunsrequestrequesttypedef)
- [VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef)
- [ImportAppCatalogRequestRequestTypeDef](./type_defs.md#importappcatalogrequestrequesttypedef)
- [LaunchAppRequestRequestTypeDef](./type_defs.md#launchapprequestrequesttypedef)
- [ListAppsRequestRequestTypeDef](./type_defs.md#listappsrequestrequesttypedef)
- [NotificationContextTypeDef](./type_defs.md#notificationcontexttypedef)
- [ReplicationRunStageDetailsTypeDef](./type_defs.md#replicationrunstagedetailstypedef)
- [ServerReplicationParametersOutputTypeDef](./type_defs.md#serverreplicationparametersoutputtypedef)
- [StartAppReplicationRequestRequestTypeDef](./type_defs.md#startappreplicationrequestrequesttypedef)
- [StartOnDemandAppReplicationRequestRequestTypeDef](./type_defs.md#startondemandappreplicationrequestrequesttypedef)
- [StartOnDemandReplicationRunRequestRequestTypeDef](./type_defs.md#startondemandreplicationrunrequestrequesttypedef)
- [StopAppReplicationRequestRequestTypeDef](./type_defs.md#stopappreplicationrequestrequesttypedef)
- [TerminateAppRequestRequestTypeDef](./type_defs.md#terminateapprequestrequesttypedef)
- [AppSummaryTypeDef](./type_defs.md#appsummarytypedef)
- [CreateReplicationJobResponseTypeDef](./type_defs.md#createreplicationjobresponsetypedef)
- [GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef)
- [StartOnDemandReplicationRunResponseTypeDef](./type_defs.md#startondemandreplicationrunresponsetypedef)
- [CreateReplicationJobRequestRequestTypeDef](./type_defs.md#createreplicationjobrequestrequesttypedef)
- [ServerReplicationParametersTypeDef](./type_defs.md#serverreplicationparameterstypedef)
- [UpdateReplicationJobRequestRequestTypeDef](./type_defs.md#updatereplicationjobrequestrequesttypedef)
- [GenerateChangeSetResponseTypeDef](./type_defs.md#generatechangesetresponsetypedef)
- [GenerateTemplateResponseTypeDef](./type_defs.md#generatetemplateresponsetypedef)
- [SSMOutputTypeDef](./type_defs.md#ssmoutputtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [UserDataTypeDef](./type_defs.md#userdatatypedef)
- [GetConnectorsRequestPaginateTypeDef](./type_defs.md#getconnectorsrequestpaginatetypedef)
- [GetReplicationJobsRequestPaginateTypeDef](./type_defs.md#getreplicationjobsrequestpaginatetypedef)
- [GetReplicationRunsRequestPaginateTypeDef](./type_defs.md#getreplicationrunsrequestpaginatetypedef)
- [ListAppsRequestPaginateTypeDef](./type_defs.md#listappsrequestpaginatetypedef)
- [GetServersRequestPaginateTypeDef](./type_defs.md#getserversrequestpaginatetypedef)
- [GetServersRequestRequestTypeDef](./type_defs.md#getserversrequestrequesttypedef)
- [VmServerTypeDef](./type_defs.md#vmservertypedef)
- [NotifyAppValidationOutputRequestRequestTypeDef](./type_defs.md#notifyappvalidationoutputrequestrequesttypedef)
- [ReplicationRunTypeDef](./type_defs.md#replicationruntypedef)
- [ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef)
- [ServerReplicationParametersUnionTypeDef](./type_defs.md#serverreplicationparametersuniontypedef)
- [AppValidationOutputTypeDef](./type_defs.md#appvalidationoutputtypedef)
- [SSMValidationParametersTypeDef](./type_defs.md#ssmvalidationparameterstypedef)
- [UserDataValidationParametersTypeDef](./type_defs.md#userdatavalidationparameterstypedef)
- [ServerTypeDef](./type_defs.md#servertypedef)
- [ReplicationJobTypeDef](./type_defs.md#replicationjobtypedef)
- [AppValidationConfigurationTypeDef](./type_defs.md#appvalidationconfigurationtypedef)
- [GetServersResponseTypeDef](./type_defs.md#getserversresponsetypedef)
- [ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef)
- [ServerGroupTypeDef](./type_defs.md#servergrouptypedef)
- [ServerLaunchConfigurationTypeDef](./type_defs.md#serverlaunchconfigurationtypedef)
- [ServerReplicationConfigurationOutputTypeDef](./type_defs.md#serverreplicationconfigurationoutputtypedef)
- [ServerReplicationConfigurationTypeDef](./type_defs.md#serverreplicationconfigurationtypedef)
- [ServerValidationConfigurationTypeDef](./type_defs.md#servervalidationconfigurationtypedef)
- [ServerValidationOutputTypeDef](./type_defs.md#servervalidationoutputtypedef)
- [GetReplicationJobsResponseTypeDef](./type_defs.md#getreplicationjobsresponsetypedef)
- [GetReplicationRunsResponseTypeDef](./type_defs.md#getreplicationrunsresponsetypedef)
- [CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef)
- [GetAppResponseTypeDef](./type_defs.md#getappresponsetypedef)
- [UpdateAppResponseTypeDef](./type_defs.md#updateappresponsetypedef)
- [ServerGroupUnionTypeDef](./type_defs.md#servergroupuniontypedef)
- [UpdateAppRequestRequestTypeDef](./type_defs.md#updateapprequestrequesttypedef)
- [ServerGroupLaunchConfigurationOutputTypeDef](./type_defs.md#servergrouplaunchconfigurationoutputtypedef)
- [ServerGroupLaunchConfigurationTypeDef](./type_defs.md#servergrouplaunchconfigurationtypedef)
- [ServerGroupReplicationConfigurationOutputTypeDef](./type_defs.md#servergroupreplicationconfigurationoutputtypedef)
- [ServerReplicationConfigurationUnionTypeDef](./type_defs.md#serverreplicationconfigurationuniontypedef)
- [ServerGroupValidationConfigurationOutputTypeDef](./type_defs.md#servergroupvalidationconfigurationoutputtypedef)
- [ServerGroupValidationConfigurationTypeDef](./type_defs.md#servergroupvalidationconfigurationtypedef)
- [ValidationOutputTypeDef](./type_defs.md#validationoutputtypedef)
- [CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef)
- [GetAppLaunchConfigurationResponseTypeDef](./type_defs.md#getapplaunchconfigurationresponsetypedef)
- [ServerGroupLaunchConfigurationUnionTypeDef](./type_defs.md#servergrouplaunchconfigurationuniontypedef)
- [GetAppReplicationConfigurationResponseTypeDef](./type_defs.md#getappreplicationconfigurationresponsetypedef)
- [ServerGroupReplicationConfigurationTypeDef](./type_defs.md#servergroupreplicationconfigurationtypedef)
- [GetAppValidationConfigurationResponseTypeDef](./type_defs.md#getappvalidationconfigurationresponsetypedef)
- [ServerGroupValidationConfigurationUnionTypeDef](./type_defs.md#servergroupvalidationconfigurationuniontypedef)
- [GetAppValidationOutputResponseTypeDef](./type_defs.md#getappvalidationoutputresponsetypedef)
- [PutAppLaunchConfigurationRequestRequestTypeDef](./type_defs.md#putapplaunchconfigurationrequestrequesttypedef)
- [ServerGroupReplicationConfigurationUnionTypeDef](./type_defs.md#servergroupreplicationconfigurationuniontypedef)
- [PutAppValidationConfigurationRequestRequestTypeDef](./type_defs.md#putappvalidationconfigurationrequestrequesttypedef)
- [PutAppReplicationConfigurationRequestRequestTypeDef](./type_defs.md#putappreplicationconfigurationrequestrequesttypedef)

