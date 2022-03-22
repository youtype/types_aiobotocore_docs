<a id="typed-dictionaries-for-aiobotocore-greengrass-module"></a>

# Typed dictionaries for aiobotocore Greengrass module

> [Index](../README.md) > [Greengrass](./README.md) > Typed dictionaries

Auto-generated documentation for
[Greengrass](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
type annotations stubs module
[types-aiobotocore-greengrass](https://pypi.org/project/types-aiobotocore-greengrass/).

- [Typed dictionaries for aiobotocore Greengrass module](#typed-dictionaries-for-aiobotocore-greengrass-module)
  - [AssociateRoleToGroupRequestRequestTypeDef](#associateroletogrouprequestrequesttypedef)
  - [AssociateRoleToGroupResponseTypeDef](#associateroletogroupresponsetypedef)
  - [AssociateServiceRoleToAccountRequestRequestTypeDef](#associateserviceroletoaccountrequestrequesttypedef)
  - [AssociateServiceRoleToAccountResponseTypeDef](#associateserviceroletoaccountresponsetypedef)
  - [BulkDeploymentMetricsTypeDef](#bulkdeploymentmetricstypedef)
  - [BulkDeploymentResultTypeDef](#bulkdeploymentresulttypedef)
  - [BulkDeploymentTypeDef](#bulkdeploymenttypedef)
  - [ConnectivityInfoTypeDef](#connectivityinfotypedef)
  - [ConnectorDefinitionVersionTypeDef](#connectordefinitionversiontypedef)
  - [ConnectorTypeDef](#connectortypedef)
  - [CoreDefinitionVersionTypeDef](#coredefinitionversiontypedef)
  - [CoreTypeDef](#coretypedef)
  - [CreateConnectorDefinitionRequestRequestTypeDef](#createconnectordefinitionrequestrequesttypedef)
  - [CreateConnectorDefinitionResponseTypeDef](#createconnectordefinitionresponsetypedef)
  - [CreateConnectorDefinitionVersionRequestRequestTypeDef](#createconnectordefinitionversionrequestrequesttypedef)
  - [CreateConnectorDefinitionVersionResponseTypeDef](#createconnectordefinitionversionresponsetypedef)
  - [CreateCoreDefinitionRequestRequestTypeDef](#createcoredefinitionrequestrequesttypedef)
  - [CreateCoreDefinitionResponseTypeDef](#createcoredefinitionresponsetypedef)
  - [CreateCoreDefinitionVersionRequestRequestTypeDef](#createcoredefinitionversionrequestrequesttypedef)
  - [CreateCoreDefinitionVersionResponseTypeDef](#createcoredefinitionversionresponsetypedef)
  - [CreateDeploymentRequestRequestTypeDef](#createdeploymentrequestrequesttypedef)
  - [CreateDeploymentResponseTypeDef](#createdeploymentresponsetypedef)
  - [CreateDeviceDefinitionRequestRequestTypeDef](#createdevicedefinitionrequestrequesttypedef)
  - [CreateDeviceDefinitionResponseTypeDef](#createdevicedefinitionresponsetypedef)
  - [CreateDeviceDefinitionVersionRequestRequestTypeDef](#createdevicedefinitionversionrequestrequesttypedef)
  - [CreateDeviceDefinitionVersionResponseTypeDef](#createdevicedefinitionversionresponsetypedef)
  - [CreateFunctionDefinitionRequestRequestTypeDef](#createfunctiondefinitionrequestrequesttypedef)
  - [CreateFunctionDefinitionResponseTypeDef](#createfunctiondefinitionresponsetypedef)
  - [CreateFunctionDefinitionVersionRequestRequestTypeDef](#createfunctiondefinitionversionrequestrequesttypedef)
  - [CreateFunctionDefinitionVersionResponseTypeDef](#createfunctiondefinitionversionresponsetypedef)
  - [CreateGroupCertificateAuthorityRequestRequestTypeDef](#creategroupcertificateauthorityrequestrequesttypedef)
  - [CreateGroupCertificateAuthorityResponseTypeDef](#creategroupcertificateauthorityresponsetypedef)
  - [CreateGroupRequestRequestTypeDef](#creategrouprequestrequesttypedef)
  - [CreateGroupResponseTypeDef](#creategroupresponsetypedef)
  - [CreateGroupVersionRequestRequestTypeDef](#creategroupversionrequestrequesttypedef)
  - [CreateGroupVersionResponseTypeDef](#creategroupversionresponsetypedef)
  - [CreateLoggerDefinitionRequestRequestTypeDef](#createloggerdefinitionrequestrequesttypedef)
  - [CreateLoggerDefinitionResponseTypeDef](#createloggerdefinitionresponsetypedef)
  - [CreateLoggerDefinitionVersionRequestRequestTypeDef](#createloggerdefinitionversionrequestrequesttypedef)
  - [CreateLoggerDefinitionVersionResponseTypeDef](#createloggerdefinitionversionresponsetypedef)
  - [CreateResourceDefinitionRequestRequestTypeDef](#createresourcedefinitionrequestrequesttypedef)
  - [CreateResourceDefinitionResponseTypeDef](#createresourcedefinitionresponsetypedef)
  - [CreateResourceDefinitionVersionRequestRequestTypeDef](#createresourcedefinitionversionrequestrequesttypedef)
  - [CreateResourceDefinitionVersionResponseTypeDef](#createresourcedefinitionversionresponsetypedef)
  - [CreateSoftwareUpdateJobRequestRequestTypeDef](#createsoftwareupdatejobrequestrequesttypedef)
  - [CreateSoftwareUpdateJobResponseTypeDef](#createsoftwareupdatejobresponsetypedef)
  - [CreateSubscriptionDefinitionRequestRequestTypeDef](#createsubscriptiondefinitionrequestrequesttypedef)
  - [CreateSubscriptionDefinitionResponseTypeDef](#createsubscriptiondefinitionresponsetypedef)
  - [CreateSubscriptionDefinitionVersionRequestRequestTypeDef](#createsubscriptiondefinitionversionrequestrequesttypedef)
  - [CreateSubscriptionDefinitionVersionResponseTypeDef](#createsubscriptiondefinitionversionresponsetypedef)
  - [DefinitionInformationTypeDef](#definitioninformationtypedef)
  - [DeleteConnectorDefinitionRequestRequestTypeDef](#deleteconnectordefinitionrequestrequesttypedef)
  - [DeleteCoreDefinitionRequestRequestTypeDef](#deletecoredefinitionrequestrequesttypedef)
  - [DeleteDeviceDefinitionRequestRequestTypeDef](#deletedevicedefinitionrequestrequesttypedef)
  - [DeleteFunctionDefinitionRequestRequestTypeDef](#deletefunctiondefinitionrequestrequesttypedef)
  - [DeleteGroupRequestRequestTypeDef](#deletegrouprequestrequesttypedef)
  - [DeleteLoggerDefinitionRequestRequestTypeDef](#deleteloggerdefinitionrequestrequesttypedef)
  - [DeleteResourceDefinitionRequestRequestTypeDef](#deleteresourcedefinitionrequestrequesttypedef)
  - [DeleteSubscriptionDefinitionRequestRequestTypeDef](#deletesubscriptiondefinitionrequestrequesttypedef)
  - [DeploymentTypeDef](#deploymenttypedef)
  - [DeviceDefinitionVersionTypeDef](#devicedefinitionversiontypedef)
  - [DeviceTypeDef](#devicetypedef)
  - [DisassociateRoleFromGroupRequestRequestTypeDef](#disassociaterolefromgrouprequestrequesttypedef)
  - [DisassociateRoleFromGroupResponseTypeDef](#disassociaterolefromgroupresponsetypedef)
  - [DisassociateServiceRoleFromAccountResponseTypeDef](#disassociateservicerolefromaccountresponsetypedef)
  - [ErrorDetailTypeDef](#errordetailtypedef)
  - [FunctionConfigurationEnvironmentTypeDef](#functionconfigurationenvironmenttypedef)
  - [FunctionConfigurationTypeDef](#functionconfigurationtypedef)
  - [FunctionDefaultConfigTypeDef](#functiondefaultconfigtypedef)
  - [FunctionDefaultExecutionConfigTypeDef](#functiondefaultexecutionconfigtypedef)
  - [FunctionDefinitionVersionTypeDef](#functiondefinitionversiontypedef)
  - [FunctionExecutionConfigTypeDef](#functionexecutionconfigtypedef)
  - [FunctionRunAsConfigTypeDef](#functionrunasconfigtypedef)
  - [FunctionTypeDef](#functiontypedef)
  - [GetAssociatedRoleRequestRequestTypeDef](#getassociatedrolerequestrequesttypedef)
  - [GetAssociatedRoleResponseTypeDef](#getassociatedroleresponsetypedef)
  - [GetBulkDeploymentStatusRequestRequestTypeDef](#getbulkdeploymentstatusrequestrequesttypedef)
  - [GetBulkDeploymentStatusResponseTypeDef](#getbulkdeploymentstatusresponsetypedef)
  - [GetConnectivityInfoRequestRequestTypeDef](#getconnectivityinforequestrequesttypedef)
  - [GetConnectivityInfoResponseTypeDef](#getconnectivityinforesponsetypedef)
  - [GetConnectorDefinitionRequestRequestTypeDef](#getconnectordefinitionrequestrequesttypedef)
  - [GetConnectorDefinitionResponseTypeDef](#getconnectordefinitionresponsetypedef)
  - [GetConnectorDefinitionVersionRequestRequestTypeDef](#getconnectordefinitionversionrequestrequesttypedef)
  - [GetConnectorDefinitionVersionResponseTypeDef](#getconnectordefinitionversionresponsetypedef)
  - [GetCoreDefinitionRequestRequestTypeDef](#getcoredefinitionrequestrequesttypedef)
  - [GetCoreDefinitionResponseTypeDef](#getcoredefinitionresponsetypedef)
  - [GetCoreDefinitionVersionRequestRequestTypeDef](#getcoredefinitionversionrequestrequesttypedef)
  - [GetCoreDefinitionVersionResponseTypeDef](#getcoredefinitionversionresponsetypedef)
  - [GetDeploymentStatusRequestRequestTypeDef](#getdeploymentstatusrequestrequesttypedef)
  - [GetDeploymentStatusResponseTypeDef](#getdeploymentstatusresponsetypedef)
  - [GetDeviceDefinitionRequestRequestTypeDef](#getdevicedefinitionrequestrequesttypedef)
  - [GetDeviceDefinitionResponseTypeDef](#getdevicedefinitionresponsetypedef)
  - [GetDeviceDefinitionVersionRequestRequestTypeDef](#getdevicedefinitionversionrequestrequesttypedef)
  - [GetDeviceDefinitionVersionResponseTypeDef](#getdevicedefinitionversionresponsetypedef)
  - [GetFunctionDefinitionRequestRequestTypeDef](#getfunctiondefinitionrequestrequesttypedef)
  - [GetFunctionDefinitionResponseTypeDef](#getfunctiondefinitionresponsetypedef)
  - [GetFunctionDefinitionVersionRequestRequestTypeDef](#getfunctiondefinitionversionrequestrequesttypedef)
  - [GetFunctionDefinitionVersionResponseTypeDef](#getfunctiondefinitionversionresponsetypedef)
  - [GetGroupCertificateAuthorityRequestRequestTypeDef](#getgroupcertificateauthorityrequestrequesttypedef)
  - [GetGroupCertificateAuthorityResponseTypeDef](#getgroupcertificateauthorityresponsetypedef)
  - [GetGroupCertificateConfigurationRequestRequestTypeDef](#getgroupcertificateconfigurationrequestrequesttypedef)
  - [GetGroupCertificateConfigurationResponseTypeDef](#getgroupcertificateconfigurationresponsetypedef)
  - [GetGroupRequestRequestTypeDef](#getgrouprequestrequesttypedef)
  - [GetGroupResponseTypeDef](#getgroupresponsetypedef)
  - [GetGroupVersionRequestRequestTypeDef](#getgroupversionrequestrequesttypedef)
  - [GetGroupVersionResponseTypeDef](#getgroupversionresponsetypedef)
  - [GetLoggerDefinitionRequestRequestTypeDef](#getloggerdefinitionrequestrequesttypedef)
  - [GetLoggerDefinitionResponseTypeDef](#getloggerdefinitionresponsetypedef)
  - [GetLoggerDefinitionVersionRequestRequestTypeDef](#getloggerdefinitionversionrequestrequesttypedef)
  - [GetLoggerDefinitionVersionResponseTypeDef](#getloggerdefinitionversionresponsetypedef)
  - [GetResourceDefinitionRequestRequestTypeDef](#getresourcedefinitionrequestrequesttypedef)
  - [GetResourceDefinitionResponseTypeDef](#getresourcedefinitionresponsetypedef)
  - [GetResourceDefinitionVersionRequestRequestTypeDef](#getresourcedefinitionversionrequestrequesttypedef)
  - [GetResourceDefinitionVersionResponseTypeDef](#getresourcedefinitionversionresponsetypedef)
  - [GetServiceRoleForAccountResponseTypeDef](#getserviceroleforaccountresponsetypedef)
  - [GetSubscriptionDefinitionRequestRequestTypeDef](#getsubscriptiondefinitionrequestrequesttypedef)
  - [GetSubscriptionDefinitionResponseTypeDef](#getsubscriptiondefinitionresponsetypedef)
  - [GetSubscriptionDefinitionVersionRequestRequestTypeDef](#getsubscriptiondefinitionversionrequestrequesttypedef)
  - [GetSubscriptionDefinitionVersionResponseTypeDef](#getsubscriptiondefinitionversionresponsetypedef)
  - [GetThingRuntimeConfigurationRequestRequestTypeDef](#getthingruntimeconfigurationrequestrequesttypedef)
  - [GetThingRuntimeConfigurationResponseTypeDef](#getthingruntimeconfigurationresponsetypedef)
  - [GroupCertificateAuthorityPropertiesTypeDef](#groupcertificateauthoritypropertiestypedef)
  - [GroupInformationTypeDef](#groupinformationtypedef)
  - [GroupOwnerSettingTypeDef](#groupownersettingtypedef)
  - [GroupVersionTypeDef](#groupversiontypedef)
  - [ListBulkDeploymentDetailedReportsRequestRequestTypeDef](#listbulkdeploymentdetailedreportsrequestrequesttypedef)
  - [ListBulkDeploymentDetailedReportsResponseTypeDef](#listbulkdeploymentdetailedreportsresponsetypedef)
  - [ListBulkDeploymentsRequestRequestTypeDef](#listbulkdeploymentsrequestrequesttypedef)
  - [ListBulkDeploymentsResponseTypeDef](#listbulkdeploymentsresponsetypedef)
  - [ListConnectorDefinitionVersionsRequestRequestTypeDef](#listconnectordefinitionversionsrequestrequesttypedef)
  - [ListConnectorDefinitionVersionsResponseTypeDef](#listconnectordefinitionversionsresponsetypedef)
  - [ListConnectorDefinitionsRequestRequestTypeDef](#listconnectordefinitionsrequestrequesttypedef)
  - [ListConnectorDefinitionsResponseTypeDef](#listconnectordefinitionsresponsetypedef)
  - [ListCoreDefinitionVersionsRequestRequestTypeDef](#listcoredefinitionversionsrequestrequesttypedef)
  - [ListCoreDefinitionVersionsResponseTypeDef](#listcoredefinitionversionsresponsetypedef)
  - [ListCoreDefinitionsRequestRequestTypeDef](#listcoredefinitionsrequestrequesttypedef)
  - [ListCoreDefinitionsResponseTypeDef](#listcoredefinitionsresponsetypedef)
  - [ListDeploymentsRequestRequestTypeDef](#listdeploymentsrequestrequesttypedef)
  - [ListDeploymentsResponseTypeDef](#listdeploymentsresponsetypedef)
  - [ListDeviceDefinitionVersionsRequestRequestTypeDef](#listdevicedefinitionversionsrequestrequesttypedef)
  - [ListDeviceDefinitionVersionsResponseTypeDef](#listdevicedefinitionversionsresponsetypedef)
  - [ListDeviceDefinitionsRequestRequestTypeDef](#listdevicedefinitionsrequestrequesttypedef)
  - [ListDeviceDefinitionsResponseTypeDef](#listdevicedefinitionsresponsetypedef)
  - [ListFunctionDefinitionVersionsRequestRequestTypeDef](#listfunctiondefinitionversionsrequestrequesttypedef)
  - [ListFunctionDefinitionVersionsResponseTypeDef](#listfunctiondefinitionversionsresponsetypedef)
  - [ListFunctionDefinitionsRequestRequestTypeDef](#listfunctiondefinitionsrequestrequesttypedef)
  - [ListFunctionDefinitionsResponseTypeDef](#listfunctiondefinitionsresponsetypedef)
  - [ListGroupCertificateAuthoritiesRequestRequestTypeDef](#listgroupcertificateauthoritiesrequestrequesttypedef)
  - [ListGroupCertificateAuthoritiesResponseTypeDef](#listgroupcertificateauthoritiesresponsetypedef)
  - [ListGroupVersionsRequestRequestTypeDef](#listgroupversionsrequestrequesttypedef)
  - [ListGroupVersionsResponseTypeDef](#listgroupversionsresponsetypedef)
  - [ListGroupsRequestRequestTypeDef](#listgroupsrequestrequesttypedef)
  - [ListGroupsResponseTypeDef](#listgroupsresponsetypedef)
  - [ListLoggerDefinitionVersionsRequestRequestTypeDef](#listloggerdefinitionversionsrequestrequesttypedef)
  - [ListLoggerDefinitionVersionsResponseTypeDef](#listloggerdefinitionversionsresponsetypedef)
  - [ListLoggerDefinitionsRequestRequestTypeDef](#listloggerdefinitionsrequestrequesttypedef)
  - [ListLoggerDefinitionsResponseTypeDef](#listloggerdefinitionsresponsetypedef)
  - [ListResourceDefinitionVersionsRequestRequestTypeDef](#listresourcedefinitionversionsrequestrequesttypedef)
  - [ListResourceDefinitionVersionsResponseTypeDef](#listresourcedefinitionversionsresponsetypedef)
  - [ListResourceDefinitionsRequestRequestTypeDef](#listresourcedefinitionsrequestrequesttypedef)
  - [ListResourceDefinitionsResponseTypeDef](#listresourcedefinitionsresponsetypedef)
  - [ListSubscriptionDefinitionVersionsRequestRequestTypeDef](#listsubscriptiondefinitionversionsrequestrequesttypedef)
  - [ListSubscriptionDefinitionVersionsResponseTypeDef](#listsubscriptiondefinitionversionsresponsetypedef)
  - [ListSubscriptionDefinitionsRequestRequestTypeDef](#listsubscriptiondefinitionsrequestrequesttypedef)
  - [ListSubscriptionDefinitionsResponseTypeDef](#listsubscriptiondefinitionsresponsetypedef)
  - [ListTagsForResourceRequestRequestTypeDef](#listtagsforresourcerequestrequesttypedef)
  - [ListTagsForResourceResponseTypeDef](#listtagsforresourceresponsetypedef)
  - [LocalDeviceResourceDataTypeDef](#localdeviceresourcedatatypedef)
  - [LocalVolumeResourceDataTypeDef](#localvolumeresourcedatatypedef)
  - [LoggerDefinitionVersionTypeDef](#loggerdefinitionversiontypedef)
  - [LoggerTypeDef](#loggertypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [ResetDeploymentsRequestRequestTypeDef](#resetdeploymentsrequestrequesttypedef)
  - [ResetDeploymentsResponseTypeDef](#resetdeploymentsresponsetypedef)
  - [ResourceAccessPolicyTypeDef](#resourceaccesspolicytypedef)
  - [ResourceDataContainerTypeDef](#resourcedatacontainertypedef)
  - [ResourceDefinitionVersionTypeDef](#resourcedefinitionversiontypedef)
  - [ResourceDownloadOwnerSettingTypeDef](#resourcedownloadownersettingtypedef)
  - [ResourceTypeDef](#resourcetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [RuntimeConfigurationTypeDef](#runtimeconfigurationtypedef)
  - [S3MachineLearningModelResourceDataTypeDef](#s3machinelearningmodelresourcedatatypedef)
  - [SageMakerMachineLearningModelResourceDataTypeDef](#sagemakermachinelearningmodelresourcedatatypedef)
  - [SecretsManagerSecretResourceDataTypeDef](#secretsmanagersecretresourcedatatypedef)
  - [StartBulkDeploymentRequestRequestTypeDef](#startbulkdeploymentrequestrequesttypedef)
  - [StartBulkDeploymentResponseTypeDef](#startbulkdeploymentresponsetypedef)
  - [StopBulkDeploymentRequestRequestTypeDef](#stopbulkdeploymentrequestrequesttypedef)
  - [SubscriptionDefinitionVersionTypeDef](#subscriptiondefinitionversiontypedef)
  - [SubscriptionTypeDef](#subscriptiontypedef)
  - [TagResourceRequestRequestTypeDef](#tagresourcerequestrequesttypedef)
  - [TelemetryConfigurationTypeDef](#telemetryconfigurationtypedef)
  - [TelemetryConfigurationUpdateTypeDef](#telemetryconfigurationupdatetypedef)
  - [UntagResourceRequestRequestTypeDef](#untagresourcerequestrequesttypedef)
  - [UpdateConnectivityInfoRequestRequestTypeDef](#updateconnectivityinforequestrequesttypedef)
  - [UpdateConnectivityInfoResponseTypeDef](#updateconnectivityinforesponsetypedef)
  - [UpdateConnectorDefinitionRequestRequestTypeDef](#updateconnectordefinitionrequestrequesttypedef)
  - [UpdateCoreDefinitionRequestRequestTypeDef](#updatecoredefinitionrequestrequesttypedef)
  - [UpdateDeviceDefinitionRequestRequestTypeDef](#updatedevicedefinitionrequestrequesttypedef)
  - [UpdateFunctionDefinitionRequestRequestTypeDef](#updatefunctiondefinitionrequestrequesttypedef)
  - [UpdateGroupCertificateConfigurationRequestRequestTypeDef](#updategroupcertificateconfigurationrequestrequesttypedef)
  - [UpdateGroupCertificateConfigurationResponseTypeDef](#updategroupcertificateconfigurationresponsetypedef)
  - [UpdateGroupRequestRequestTypeDef](#updategrouprequestrequesttypedef)
  - [UpdateLoggerDefinitionRequestRequestTypeDef](#updateloggerdefinitionrequestrequesttypedef)
  - [UpdateResourceDefinitionRequestRequestTypeDef](#updateresourcedefinitionrequestrequesttypedef)
  - [UpdateSubscriptionDefinitionRequestRequestTypeDef](#updatesubscriptiondefinitionrequestrequesttypedef)
  - [UpdateThingRuntimeConfigurationRequestRequestTypeDef](#updatethingruntimeconfigurationrequestrequesttypedef)
  - [VersionInformationTypeDef](#versioninformationtypedef)

<a id="associateroletogrouprequestrequesttypedef"></a>

## AssociateRoleToGroupRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`
- `RoleArn`: `str`

<a id="associateroletogroupresponsetypedef"></a>

## AssociateRoleToGroupResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupResponseTypeDef
```

Required fields:

- `AssociatedAt`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="associateserviceroletoaccountrequestrequesttypedef"></a>

## AssociateServiceRoleToAccountRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import AssociateServiceRoleToAccountRequestRequestTypeDef
```

Required fields:

- `RoleArn`: `str`

<a id="associateserviceroletoaccountresponsetypedef"></a>

## AssociateServiceRoleToAccountResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import AssociateServiceRoleToAccountResponseTypeDef
```

Required fields:

- `AssociatedAt`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="bulkdeploymentmetricstypedef"></a>

## BulkDeploymentMetricsTypeDef

```python
from types_aiobotocore_greengrass.type_defs import BulkDeploymentMetricsTypeDef
```

Optional fields:

- `InvalidInputRecords`: `int`
- `RecordsProcessed`: `int`
- `RetryAttempts`: `int`

<a id="bulkdeploymentresulttypedef"></a>

## BulkDeploymentResultTypeDef

```python
from types_aiobotocore_greengrass.type_defs import BulkDeploymentResultTypeDef
```

Optional fields:

- `CreatedAt`: `str`
- `DeploymentArn`: `str`
- `DeploymentId`: `str`
- `DeploymentStatus`: `str`
- `DeploymentType`: [DeploymentTypeType](./literals.md#deploymenttypetype)
- `ErrorDetails`:
  `List`\[[ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)\]
- `ErrorMessage`: `str`
- `GroupArn`: `str`

<a id="bulkdeploymenttypedef"></a>

## BulkDeploymentTypeDef

```python
from types_aiobotocore_greengrass.type_defs import BulkDeploymentTypeDef
```

Optional fields:

- `BulkDeploymentArn`: `str`
- `BulkDeploymentId`: `str`
- `CreatedAt`: `str`

<a id="connectivityinfotypedef"></a>

## ConnectivityInfoTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ConnectivityInfoTypeDef
```

Optional fields:

- `HostAddress`: `str`
- `Id`: `str`
- `Metadata`: `str`
- `PortNumber`: `int`

<a id="connectordefinitionversiontypedef"></a>

## ConnectorDefinitionVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ConnectorDefinitionVersionTypeDef
```

Optional fields:

- `Connectors`:
  `Sequence`\[[ConnectorTypeDef](./type_defs.md#connectortypedef)\]

<a id="connectortypedef"></a>

## ConnectorTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ConnectorTypeDef
```

Required fields:

- `ConnectorArn`: `str`
- `Id`: `str`

Optional fields:

- `Parameters`: `Mapping`\[`str`, `str`\]

<a id="coredefinitionversiontypedef"></a>

## CoreDefinitionVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CoreDefinitionVersionTypeDef
```

Optional fields:

- `Cores`: `Sequence`\[[CoreTypeDef](./type_defs.md#coretypedef)\]

<a id="coretypedef"></a>

## CoreTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CoreTypeDef
```

Required fields:

- `CertificateArn`: `str`
- `Id`: `str`
- `ThingArn`: `str`

Optional fields:

- `SyncShadow`: `bool`

<a id="createconnectordefinitionrequestrequesttypedef"></a>

## CreateConnectorDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateConnectorDefinitionRequestRequestTypeDef
```

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`:
  [ConnectorDefinitionVersionTypeDef](./type_defs.md#connectordefinitionversiontypedef)
- `Name`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createconnectordefinitionresponsetypedef"></a>

## CreateConnectorDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateConnectorDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createconnectordefinitionversionrequestrequesttypedef"></a>

## CreateConnectorDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateConnectorDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `ConnectorDefinitionId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `Connectors`:
  `Sequence`\[[ConnectorTypeDef](./type_defs.md#connectortypedef)\]

<a id="createconnectordefinitionversionresponsetypedef"></a>

## CreateConnectorDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateConnectorDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createcoredefinitionrequestrequesttypedef"></a>

## CreateCoreDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateCoreDefinitionRequestRequestTypeDef
```

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`:
  [CoreDefinitionVersionTypeDef](./type_defs.md#coredefinitionversiontypedef)
- `Name`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createcoredefinitionresponsetypedef"></a>

## CreateCoreDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateCoreDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createcoredefinitionversionrequestrequesttypedef"></a>

## CreateCoreDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateCoreDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `CoreDefinitionId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `Cores`: `Sequence`\[[CoreTypeDef](./type_defs.md#coretypedef)\]

<a id="createcoredefinitionversionresponsetypedef"></a>

## CreateCoreDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateCoreDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createdeploymentrequestrequesttypedef"></a>

## CreateDeploymentRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateDeploymentRequestRequestTypeDef
```

Required fields:

- `DeploymentType`: [DeploymentTypeType](./literals.md#deploymenttypetype)
- `GroupId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `DeploymentId`: `str`
- `GroupVersionId`: `str`

<a id="createdeploymentresponsetypedef"></a>

## CreateDeploymentResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateDeploymentResponseTypeDef
```

Required fields:

- `DeploymentArn`: `str`
- `DeploymentId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createdevicedefinitionrequestrequesttypedef"></a>

## CreateDeviceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateDeviceDefinitionRequestRequestTypeDef
```

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`:
  [DeviceDefinitionVersionTypeDef](./type_defs.md#devicedefinitionversiontypedef)
- `Name`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createdevicedefinitionresponsetypedef"></a>

## CreateDeviceDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateDeviceDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createdevicedefinitionversionrequestrequesttypedef"></a>

## CreateDeviceDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateDeviceDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `DeviceDefinitionId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `Devices`: `Sequence`\[[DeviceTypeDef](./type_defs.md#devicetypedef)\]

<a id="createdevicedefinitionversionresponsetypedef"></a>

## CreateDeviceDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateDeviceDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createfunctiondefinitionrequestrequesttypedef"></a>

## CreateFunctionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateFunctionDefinitionRequestRequestTypeDef
```

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`:
  [FunctionDefinitionVersionTypeDef](./type_defs.md#functiondefinitionversiontypedef)
- `Name`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createfunctiondefinitionresponsetypedef"></a>

## CreateFunctionDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateFunctionDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createfunctiondefinitionversionrequestrequesttypedef"></a>

## CreateFunctionDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateFunctionDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `FunctionDefinitionId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `DefaultConfig`:
  [FunctionDefaultConfigTypeDef](./type_defs.md#functiondefaultconfigtypedef)
- `Functions`: `Sequence`\[[FunctionTypeDef](./type_defs.md#functiontypedef)\]

<a id="createfunctiondefinitionversionresponsetypedef"></a>

## CreateFunctionDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateFunctionDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="creategroupcertificateauthorityrequestrequesttypedef"></a>

## CreateGroupCertificateAuthorityRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateGroupCertificateAuthorityRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

Optional fields:

- `AmznClientToken`: `str`

<a id="creategroupcertificateauthorityresponsetypedef"></a>

## CreateGroupCertificateAuthorityResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateGroupCertificateAuthorityResponseTypeDef
```

Required fields:

- `GroupCertificateAuthorityArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="creategrouprequestrequesttypedef"></a>

## CreateGroupRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateGroupRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`: [GroupVersionTypeDef](./type_defs.md#groupversiontypedef)
- `tags`: `Mapping`\[`str`, `str`\]

<a id="creategroupresponsetypedef"></a>

## CreateGroupResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateGroupResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="creategroupversionrequestrequesttypedef"></a>

## CreateGroupVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateGroupVersionRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `ConnectorDefinitionVersionArn`: `str`
- `CoreDefinitionVersionArn`: `str`
- `DeviceDefinitionVersionArn`: `str`
- `FunctionDefinitionVersionArn`: `str`
- `LoggerDefinitionVersionArn`: `str`
- `ResourceDefinitionVersionArn`: `str`
- `SubscriptionDefinitionVersionArn`: `str`

<a id="creategroupversionresponsetypedef"></a>

## CreateGroupVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateGroupVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createloggerdefinitionrequestrequesttypedef"></a>

## CreateLoggerDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateLoggerDefinitionRequestRequestTypeDef
```

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`:
  [LoggerDefinitionVersionTypeDef](./type_defs.md#loggerdefinitionversiontypedef)
- `Name`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createloggerdefinitionresponsetypedef"></a>

## CreateLoggerDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateLoggerDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createloggerdefinitionversionrequestrequesttypedef"></a>

## CreateLoggerDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateLoggerDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `LoggerDefinitionId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `Loggers`: `Sequence`\[[LoggerTypeDef](./type_defs.md#loggertypedef)\]

<a id="createloggerdefinitionversionresponsetypedef"></a>

## CreateLoggerDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateLoggerDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createresourcedefinitionrequestrequesttypedef"></a>

## CreateResourceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateResourceDefinitionRequestRequestTypeDef
```

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`:
  [ResourceDefinitionVersionTypeDef](./type_defs.md#resourcedefinitionversiontypedef)
- `Name`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createresourcedefinitionresponsetypedef"></a>

## CreateResourceDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateResourceDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createresourcedefinitionversionrequestrequesttypedef"></a>

## CreateResourceDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateResourceDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `ResourceDefinitionId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `Resources`: `Sequence`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]

<a id="createresourcedefinitionversionresponsetypedef"></a>

## CreateResourceDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateResourceDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createsoftwareupdatejobrequestrequesttypedef"></a>

## CreateSoftwareUpdateJobRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateSoftwareUpdateJobRequestRequestTypeDef
```

Required fields:

- `S3UrlSignerRole`: `str`
- `SoftwareToUpdate`:
  [SoftwareToUpdateType](./literals.md#softwaretoupdatetype)
- `UpdateTargets`: `Sequence`\[`str`\]
- `UpdateTargetsArchitecture`:
  [UpdateTargetsArchitectureType](./literals.md#updatetargetsarchitecturetype)
- `UpdateTargetsOperatingSystem`:
  [UpdateTargetsOperatingSystemType](./literals.md#updatetargetsoperatingsystemtype)

Optional fields:

- `AmznClientToken`: `str`
- `UpdateAgentLogLevel`:
  [UpdateAgentLogLevelType](./literals.md#updateagentlogleveltype)

<a id="createsoftwareupdatejobresponsetypedef"></a>

## CreateSoftwareUpdateJobResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateSoftwareUpdateJobResponseTypeDef
```

Required fields:

- `IotJobArn`: `str`
- `IotJobId`: `str`
- `PlatformSoftwareVersion`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createsubscriptiondefinitionrequestrequesttypedef"></a>

## CreateSubscriptionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateSubscriptionDefinitionRequestRequestTypeDef
```

Optional fields:

- `AmznClientToken`: `str`
- `InitialVersion`:
  [SubscriptionDefinitionVersionTypeDef](./type_defs.md#subscriptiondefinitionversiontypedef)
- `Name`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createsubscriptiondefinitionresponsetypedef"></a>

## CreateSubscriptionDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateSubscriptionDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createsubscriptiondefinitionversionrequestrequesttypedef"></a>

## CreateSubscriptionDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateSubscriptionDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `SubscriptionDefinitionId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `Subscriptions`:
  `Sequence`\[[SubscriptionTypeDef](./type_defs.md#subscriptiontypedef)\]

<a id="createsubscriptiondefinitionversionresponsetypedef"></a>

## CreateSubscriptionDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import CreateSubscriptionDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="definitioninformationtypedef"></a>

## DefinitionInformationTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DefinitionInformationTypeDef
```

Optional fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `Tags`: `Dict`\[`str`, `str`\]

<a id="deleteconnectordefinitionrequestrequesttypedef"></a>

## DeleteConnectorDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteConnectorDefinitionRequestRequestTypeDef
```

Required fields:

- `ConnectorDefinitionId`: `str`

<a id="deletecoredefinitionrequestrequesttypedef"></a>

## DeleteCoreDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteCoreDefinitionRequestRequestTypeDef
```

Required fields:

- `CoreDefinitionId`: `str`

<a id="deletedevicedefinitionrequestrequesttypedef"></a>

## DeleteDeviceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteDeviceDefinitionRequestRequestTypeDef
```

Required fields:

- `DeviceDefinitionId`: `str`

<a id="deletefunctiondefinitionrequestrequesttypedef"></a>

## DeleteFunctionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteFunctionDefinitionRequestRequestTypeDef
```

Required fields:

- `FunctionDefinitionId`: `str`

<a id="deletegrouprequestrequesttypedef"></a>

## DeleteGroupRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteGroupRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

<a id="deleteloggerdefinitionrequestrequesttypedef"></a>

## DeleteLoggerDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteLoggerDefinitionRequestRequestTypeDef
```

Required fields:

- `LoggerDefinitionId`: `str`

<a id="deleteresourcedefinitionrequestrequesttypedef"></a>

## DeleteResourceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteResourceDefinitionRequestRequestTypeDef
```

Required fields:

- `ResourceDefinitionId`: `str`

<a id="deletesubscriptiondefinitionrequestrequesttypedef"></a>

## DeleteSubscriptionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeleteSubscriptionDefinitionRequestRequestTypeDef
```

Required fields:

- `SubscriptionDefinitionId`: `str`

<a id="deploymenttypedef"></a>

## DeploymentTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeploymentTypeDef
```

Optional fields:

- `CreatedAt`: `str`
- `DeploymentArn`: `str`
- `DeploymentId`: `str`
- `DeploymentType`: [DeploymentTypeType](./literals.md#deploymenttypetype)
- `GroupArn`: `str`

<a id="devicedefinitionversiontypedef"></a>

## DeviceDefinitionVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeviceDefinitionVersionTypeDef
```

Optional fields:

- `Devices`: `Sequence`\[[DeviceTypeDef](./type_defs.md#devicetypedef)\]

<a id="devicetypedef"></a>

## DeviceTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DeviceTypeDef
```

Required fields:

- `CertificateArn`: `str`
- `Id`: `str`
- `ThingArn`: `str`

Optional fields:

- `SyncShadow`: `bool`

<a id="disassociaterolefromgrouprequestrequesttypedef"></a>

## DisassociateRoleFromGroupRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DisassociateRoleFromGroupRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

<a id="disassociaterolefromgroupresponsetypedef"></a>

## DisassociateRoleFromGroupResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DisassociateRoleFromGroupResponseTypeDef
```

Required fields:

- `DisassociatedAt`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="disassociateservicerolefromaccountresponsetypedef"></a>

## DisassociateServiceRoleFromAccountResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import DisassociateServiceRoleFromAccountResponseTypeDef
```

Required fields:

- `DisassociatedAt`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="errordetailtypedef"></a>

## ErrorDetailTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ErrorDetailTypeDef
```

Optional fields:

- `DetailedErrorCode`: `str`
- `DetailedErrorMessage`: `str`

<a id="functionconfigurationenvironmenttypedef"></a>

## FunctionConfigurationEnvironmentTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionConfigurationEnvironmentTypeDef
```

Optional fields:

- `AccessSysfs`: `bool`
- `Execution`:
  [FunctionExecutionConfigTypeDef](./type_defs.md#functionexecutionconfigtypedef)
- `ResourceAccessPolicies`:
  `Sequence`\[[ResourceAccessPolicyTypeDef](./type_defs.md#resourceaccesspolicytypedef)\]
- `Variables`: `Mapping`\[`str`, `str`\]

<a id="functionconfigurationtypedef"></a>

## FunctionConfigurationTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionConfigurationTypeDef
```

Optional fields:

- `EncodingType`: [EncodingTypeType](./literals.md#encodingtypetype)
- `Environment`:
  [FunctionConfigurationEnvironmentTypeDef](./type_defs.md#functionconfigurationenvironmenttypedef)
- `ExecArgs`: `str`
- `Executable`: `str`
- `MemorySize`: `int`
- `Pinned`: `bool`
- `Timeout`: `int`

<a id="functiondefaultconfigtypedef"></a>

## FunctionDefaultConfigTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionDefaultConfigTypeDef
```

Optional fields:

- `Execution`:
  [FunctionDefaultExecutionConfigTypeDef](./type_defs.md#functiondefaultexecutionconfigtypedef)

<a id="functiondefaultexecutionconfigtypedef"></a>

## FunctionDefaultExecutionConfigTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionDefaultExecutionConfigTypeDef
```

Optional fields:

- `IsolationMode`:
  [FunctionIsolationModeType](./literals.md#functionisolationmodetype)
- `RunAs`:
  [FunctionRunAsConfigTypeDef](./type_defs.md#functionrunasconfigtypedef)

<a id="functiondefinitionversiontypedef"></a>

## FunctionDefinitionVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionDefinitionVersionTypeDef
```

Optional fields:

- `DefaultConfig`:
  [FunctionDefaultConfigTypeDef](./type_defs.md#functiondefaultconfigtypedef)
- `Functions`: `Sequence`\[[FunctionTypeDef](./type_defs.md#functiontypedef)\]

<a id="functionexecutionconfigtypedef"></a>

## FunctionExecutionConfigTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionExecutionConfigTypeDef
```

Optional fields:

- `IsolationMode`:
  [FunctionIsolationModeType](./literals.md#functionisolationmodetype)
- `RunAs`:
  [FunctionRunAsConfigTypeDef](./type_defs.md#functionrunasconfigtypedef)

<a id="functionrunasconfigtypedef"></a>

## FunctionRunAsConfigTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionRunAsConfigTypeDef
```

Optional fields:

- `Gid`: `int`
- `Uid`: `int`

<a id="functiontypedef"></a>

## FunctionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import FunctionTypeDef
```

Required fields:

- `Id`: `str`

Optional fields:

- `FunctionArn`: `str`
- `FunctionConfiguration`:
  [FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef)

<a id="getassociatedrolerequestrequesttypedef"></a>

## GetAssociatedRoleRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetAssociatedRoleRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

<a id="getassociatedroleresponsetypedef"></a>

## GetAssociatedRoleResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetAssociatedRoleResponseTypeDef
```

Required fields:

- `AssociatedAt`: `str`
- `RoleArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getbulkdeploymentstatusrequestrequesttypedef"></a>

## GetBulkDeploymentStatusRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetBulkDeploymentStatusRequestRequestTypeDef
```

Required fields:

- `BulkDeploymentId`: `str`

<a id="getbulkdeploymentstatusresponsetypedef"></a>

## GetBulkDeploymentStatusResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetBulkDeploymentStatusResponseTypeDef
```

Required fields:

- `BulkDeploymentMetrics`:
  [BulkDeploymentMetricsTypeDef](./type_defs.md#bulkdeploymentmetricstypedef)
- `BulkDeploymentStatus`:
  [BulkDeploymentStatusType](./literals.md#bulkdeploymentstatustype)
- `CreatedAt`: `str`
- `ErrorDetails`:
  `List`\[[ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)\]
- `ErrorMessage`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getconnectivityinforequestrequesttypedef"></a>

## GetConnectivityInfoRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetConnectivityInfoRequestRequestTypeDef
```

Required fields:

- `ThingName`: `str`

<a id="getconnectivityinforesponsetypedef"></a>

## GetConnectivityInfoResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetConnectivityInfoResponseTypeDef
```

Required fields:

- `ConnectivityInfo`:
  `List`\[[ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef)\]
- `Message`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getconnectordefinitionrequestrequesttypedef"></a>

## GetConnectorDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetConnectorDefinitionRequestRequestTypeDef
```

Required fields:

- `ConnectorDefinitionId`: `str`

<a id="getconnectordefinitionresponsetypedef"></a>

## GetConnectorDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetConnectorDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getconnectordefinitionversionrequestrequesttypedef"></a>

## GetConnectorDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetConnectorDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `ConnectorDefinitionId`: `str`
- `ConnectorDefinitionVersionId`: `str`

Optional fields:

- `NextToken`: `str`

<a id="getconnectordefinitionversionresponsetypedef"></a>

## GetConnectorDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetConnectorDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`:
  [ConnectorDefinitionVersionTypeDef](./type_defs.md#connectordefinitionversiontypedef)
- `Id`: `str`
- `NextToken`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getcoredefinitionrequestrequesttypedef"></a>

## GetCoreDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetCoreDefinitionRequestRequestTypeDef
```

Required fields:

- `CoreDefinitionId`: `str`

<a id="getcoredefinitionresponsetypedef"></a>

## GetCoreDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetCoreDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getcoredefinitionversionrequestrequesttypedef"></a>

## GetCoreDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetCoreDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `CoreDefinitionId`: `str`
- `CoreDefinitionVersionId`: `str`

<a id="getcoredefinitionversionresponsetypedef"></a>

## GetCoreDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetCoreDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`:
  [CoreDefinitionVersionTypeDef](./type_defs.md#coredefinitionversiontypedef)
- `Id`: `str`
- `NextToken`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getdeploymentstatusrequestrequesttypedef"></a>

## GetDeploymentStatusRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetDeploymentStatusRequestRequestTypeDef
```

Required fields:

- `DeploymentId`: `str`
- `GroupId`: `str`

<a id="getdeploymentstatusresponsetypedef"></a>

## GetDeploymentStatusResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetDeploymentStatusResponseTypeDef
```

Required fields:

- `DeploymentStatus`: `str`
- `DeploymentType`: [DeploymentTypeType](./literals.md#deploymenttypetype)
- `ErrorDetails`:
  `List`\[[ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)\]
- `ErrorMessage`: `str`
- `UpdatedAt`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getdevicedefinitionrequestrequesttypedef"></a>

## GetDeviceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetDeviceDefinitionRequestRequestTypeDef
```

Required fields:

- `DeviceDefinitionId`: `str`

<a id="getdevicedefinitionresponsetypedef"></a>

## GetDeviceDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetDeviceDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getdevicedefinitionversionrequestrequesttypedef"></a>

## GetDeviceDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetDeviceDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `DeviceDefinitionId`: `str`
- `DeviceDefinitionVersionId`: `str`

Optional fields:

- `NextToken`: `str`

<a id="getdevicedefinitionversionresponsetypedef"></a>

## GetDeviceDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetDeviceDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`:
  [DeviceDefinitionVersionTypeDef](./type_defs.md#devicedefinitionversiontypedef)
- `Id`: `str`
- `NextToken`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getfunctiondefinitionrequestrequesttypedef"></a>

## GetFunctionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetFunctionDefinitionRequestRequestTypeDef
```

Required fields:

- `FunctionDefinitionId`: `str`

<a id="getfunctiondefinitionresponsetypedef"></a>

## GetFunctionDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetFunctionDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getfunctiondefinitionversionrequestrequesttypedef"></a>

## GetFunctionDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetFunctionDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `FunctionDefinitionId`: `str`
- `FunctionDefinitionVersionId`: `str`

Optional fields:

- `NextToken`: `str`

<a id="getfunctiondefinitionversionresponsetypedef"></a>

## GetFunctionDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetFunctionDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`:
  [FunctionDefinitionVersionTypeDef](./type_defs.md#functiondefinitionversiontypedef)
- `Id`: `str`
- `NextToken`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getgroupcertificateauthorityrequestrequesttypedef"></a>

## GetGroupCertificateAuthorityRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupCertificateAuthorityRequestRequestTypeDef
```

Required fields:

- `CertificateAuthorityId`: `str`
- `GroupId`: `str`

<a id="getgroupcertificateauthorityresponsetypedef"></a>

## GetGroupCertificateAuthorityResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupCertificateAuthorityResponseTypeDef
```

Required fields:

- `GroupCertificateAuthorityArn`: `str`
- `GroupCertificateAuthorityId`: `str`
- `PemEncodedCertificate`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getgroupcertificateconfigurationrequestrequesttypedef"></a>

## GetGroupCertificateConfigurationRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupCertificateConfigurationRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

<a id="getgroupcertificateconfigurationresponsetypedef"></a>

## GetGroupCertificateConfigurationResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupCertificateConfigurationResponseTypeDef
```

Required fields:

- `CertificateAuthorityExpiryInMilliseconds`: `str`
- `CertificateExpiryInMilliseconds`: `str`
- `GroupId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getgrouprequestrequesttypedef"></a>

## GetGroupRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

<a id="getgroupresponsetypedef"></a>

## GetGroupResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getgroupversionrequestrequesttypedef"></a>

## GetGroupVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupVersionRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`
- `GroupVersionId`: `str`

<a id="getgroupversionresponsetypedef"></a>

## GetGroupVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetGroupVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`: [GroupVersionTypeDef](./type_defs.md#groupversiontypedef)
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getloggerdefinitionrequestrequesttypedef"></a>

## GetLoggerDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetLoggerDefinitionRequestRequestTypeDef
```

Required fields:

- `LoggerDefinitionId`: `str`

<a id="getloggerdefinitionresponsetypedef"></a>

## GetLoggerDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetLoggerDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getloggerdefinitionversionrequestrequesttypedef"></a>

## GetLoggerDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetLoggerDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `LoggerDefinitionId`: `str`
- `LoggerDefinitionVersionId`: `str`

Optional fields:

- `NextToken`: `str`

<a id="getloggerdefinitionversionresponsetypedef"></a>

## GetLoggerDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetLoggerDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`:
  [LoggerDefinitionVersionTypeDef](./type_defs.md#loggerdefinitionversiontypedef)
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getresourcedefinitionrequestrequesttypedef"></a>

## GetResourceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetResourceDefinitionRequestRequestTypeDef
```

Required fields:

- `ResourceDefinitionId`: `str`

<a id="getresourcedefinitionresponsetypedef"></a>

## GetResourceDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetResourceDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getresourcedefinitionversionrequestrequesttypedef"></a>

## GetResourceDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetResourceDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `ResourceDefinitionId`: `str`
- `ResourceDefinitionVersionId`: `str`

<a id="getresourcedefinitionversionresponsetypedef"></a>

## GetResourceDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetResourceDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`:
  [ResourceDefinitionVersionTypeDef](./type_defs.md#resourcedefinitionversiontypedef)
- `Id`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getserviceroleforaccountresponsetypedef"></a>

## GetServiceRoleForAccountResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetServiceRoleForAccountResponseTypeDef
```

Required fields:

- `AssociatedAt`: `str`
- `RoleArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getsubscriptiondefinitionrequestrequesttypedef"></a>

## GetSubscriptionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetSubscriptionDefinitionRequestRequestTypeDef
```

Required fields:

- `SubscriptionDefinitionId`: `str`

<a id="getsubscriptiondefinitionresponsetypedef"></a>

## GetSubscriptionDefinitionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetSubscriptionDefinitionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getsubscriptiondefinitionversionrequestrequesttypedef"></a>

## GetSubscriptionDefinitionVersionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetSubscriptionDefinitionVersionRequestRequestTypeDef
```

Required fields:

- `SubscriptionDefinitionId`: `str`
- `SubscriptionDefinitionVersionId`: `str`

Optional fields:

- `NextToken`: `str`

<a id="getsubscriptiondefinitionversionresponsetypedef"></a>

## GetSubscriptionDefinitionVersionResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetSubscriptionDefinitionVersionResponseTypeDef
```

Required fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Definition`:
  [SubscriptionDefinitionVersionTypeDef](./type_defs.md#subscriptiondefinitionversiontypedef)
- `Id`: `str`
- `NextToken`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getthingruntimeconfigurationrequestrequesttypedef"></a>

## GetThingRuntimeConfigurationRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetThingRuntimeConfigurationRequestRequestTypeDef
```

Required fields:

- `ThingName`: `str`

<a id="getthingruntimeconfigurationresponsetypedef"></a>

## GetThingRuntimeConfigurationResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GetThingRuntimeConfigurationResponseTypeDef
```

Required fields:

- `RuntimeConfiguration`:
  [RuntimeConfigurationTypeDef](./type_defs.md#runtimeconfigurationtypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="groupcertificateauthoritypropertiestypedef"></a>

## GroupCertificateAuthorityPropertiesTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GroupCertificateAuthorityPropertiesTypeDef
```

Optional fields:

- `GroupCertificateAuthorityArn`: `str`
- `GroupCertificateAuthorityId`: `str`

<a id="groupinformationtypedef"></a>

## GroupInformationTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GroupInformationTypeDef
```

Optional fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `LastUpdatedTimestamp`: `str`
- `LatestVersion`: `str`
- `LatestVersionArn`: `str`
- `Name`: `str`

<a id="groupownersettingtypedef"></a>

## GroupOwnerSettingTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GroupOwnerSettingTypeDef
```

Optional fields:

- `AutoAddGroupOwner`: `bool`
- `GroupOwner`: `str`

<a id="groupversiontypedef"></a>

## GroupVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import GroupVersionTypeDef
```

Optional fields:

- `ConnectorDefinitionVersionArn`: `str`
- `CoreDefinitionVersionArn`: `str`
- `DeviceDefinitionVersionArn`: `str`
- `FunctionDefinitionVersionArn`: `str`
- `LoggerDefinitionVersionArn`: `str`
- `ResourceDefinitionVersionArn`: `str`
- `SubscriptionDefinitionVersionArn`: `str`

<a id="listbulkdeploymentdetailedreportsrequestrequesttypedef"></a>

## ListBulkDeploymentDetailedReportsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListBulkDeploymentDetailedReportsRequestRequestTypeDef
```

Required fields:

- `BulkDeploymentId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listbulkdeploymentdetailedreportsresponsetypedef"></a>

## ListBulkDeploymentDetailedReportsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListBulkDeploymentDetailedReportsResponseTypeDef
```

Required fields:

- `Deployments`:
  `List`\[[BulkDeploymentResultTypeDef](./type_defs.md#bulkdeploymentresulttypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listbulkdeploymentsrequestrequesttypedef"></a>

## ListBulkDeploymentsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListBulkDeploymentsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listbulkdeploymentsresponsetypedef"></a>

## ListBulkDeploymentsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListBulkDeploymentsResponseTypeDef
```

Required fields:

- `BulkDeployments`:
  `List`\[[BulkDeploymentTypeDef](./type_defs.md#bulkdeploymenttypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listconnectordefinitionversionsrequestrequesttypedef"></a>

## ListConnectorDefinitionVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListConnectorDefinitionVersionsRequestRequestTypeDef
```

Required fields:

- `ConnectorDefinitionId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listconnectordefinitionversionsresponsetypedef"></a>

## ListConnectorDefinitionVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListConnectorDefinitionVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listconnectordefinitionsrequestrequesttypedef"></a>

## ListConnectorDefinitionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListConnectorDefinitionsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listconnectordefinitionsresponsetypedef"></a>

## ListConnectorDefinitionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListConnectorDefinitionsResponseTypeDef
```

Required fields:

- `Definitions`:
  `List`\[[DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listcoredefinitionversionsrequestrequesttypedef"></a>

## ListCoreDefinitionVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListCoreDefinitionVersionsRequestRequestTypeDef
```

Required fields:

- `CoreDefinitionId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listcoredefinitionversionsresponsetypedef"></a>

## ListCoreDefinitionVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListCoreDefinitionVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listcoredefinitionsrequestrequesttypedef"></a>

## ListCoreDefinitionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListCoreDefinitionsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listcoredefinitionsresponsetypedef"></a>

## ListCoreDefinitionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListCoreDefinitionsResponseTypeDef
```

Required fields:

- `Definitions`:
  `List`\[[DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listdeploymentsrequestrequesttypedef"></a>

## ListDeploymentsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListDeploymentsRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listdeploymentsresponsetypedef"></a>

## ListDeploymentsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListDeploymentsResponseTypeDef
```

Required fields:

- `Deployments`:
  `List`\[[DeploymentTypeDef](./type_defs.md#deploymenttypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listdevicedefinitionversionsrequestrequesttypedef"></a>

## ListDeviceDefinitionVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListDeviceDefinitionVersionsRequestRequestTypeDef
```

Required fields:

- `DeviceDefinitionId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listdevicedefinitionversionsresponsetypedef"></a>

## ListDeviceDefinitionVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListDeviceDefinitionVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listdevicedefinitionsrequestrequesttypedef"></a>

## ListDeviceDefinitionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListDeviceDefinitionsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listdevicedefinitionsresponsetypedef"></a>

## ListDeviceDefinitionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListDeviceDefinitionsResponseTypeDef
```

Required fields:

- `Definitions`:
  `List`\[[DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listfunctiondefinitionversionsrequestrequesttypedef"></a>

## ListFunctionDefinitionVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListFunctionDefinitionVersionsRequestRequestTypeDef
```

Required fields:

- `FunctionDefinitionId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listfunctiondefinitionversionsresponsetypedef"></a>

## ListFunctionDefinitionVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListFunctionDefinitionVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listfunctiondefinitionsrequestrequesttypedef"></a>

## ListFunctionDefinitionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListFunctionDefinitionsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listfunctiondefinitionsresponsetypedef"></a>

## ListFunctionDefinitionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListFunctionDefinitionsResponseTypeDef
```

Required fields:

- `Definitions`:
  `List`\[[DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listgroupcertificateauthoritiesrequestrequesttypedef"></a>

## ListGroupCertificateAuthoritiesRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListGroupCertificateAuthoritiesRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

<a id="listgroupcertificateauthoritiesresponsetypedef"></a>

## ListGroupCertificateAuthoritiesResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListGroupCertificateAuthoritiesResponseTypeDef
```

Required fields:

- `GroupCertificateAuthorities`:
  `List`\[[GroupCertificateAuthorityPropertiesTypeDef](./type_defs.md#groupcertificateauthoritypropertiestypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listgroupversionsrequestrequesttypedef"></a>

## ListGroupVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListGroupVersionsRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listgroupversionsresponsetypedef"></a>

## ListGroupVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListGroupVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listgroupsrequestrequesttypedef"></a>

## ListGroupsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListGroupsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listgroupsresponsetypedef"></a>

## ListGroupsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListGroupsResponseTypeDef
```

Required fields:

- `Groups`:
  `List`\[[GroupInformationTypeDef](./type_defs.md#groupinformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listloggerdefinitionversionsrequestrequesttypedef"></a>

## ListLoggerDefinitionVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListLoggerDefinitionVersionsRequestRequestTypeDef
```

Required fields:

- `LoggerDefinitionId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listloggerdefinitionversionsresponsetypedef"></a>

## ListLoggerDefinitionVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListLoggerDefinitionVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listloggerdefinitionsrequestrequesttypedef"></a>

## ListLoggerDefinitionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListLoggerDefinitionsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listloggerdefinitionsresponsetypedef"></a>

## ListLoggerDefinitionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListLoggerDefinitionsResponseTypeDef
```

Required fields:

- `Definitions`:
  `List`\[[DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listresourcedefinitionversionsrequestrequesttypedef"></a>

## ListResourceDefinitionVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListResourceDefinitionVersionsRequestRequestTypeDef
```

Required fields:

- `ResourceDefinitionId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listresourcedefinitionversionsresponsetypedef"></a>

## ListResourceDefinitionVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListResourceDefinitionVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listresourcedefinitionsrequestrequesttypedef"></a>

## ListResourceDefinitionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListResourceDefinitionsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listresourcedefinitionsresponsetypedef"></a>

## ListResourceDefinitionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListResourceDefinitionsResponseTypeDef
```

Required fields:

- `Definitions`:
  `List`\[[DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listsubscriptiondefinitionversionsrequestrequesttypedef"></a>

## ListSubscriptionDefinitionVersionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListSubscriptionDefinitionVersionsRequestRequestTypeDef
```

Required fields:

- `SubscriptionDefinitionId`: `str`

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listsubscriptiondefinitionversionsresponsetypedef"></a>

## ListSubscriptionDefinitionVersionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListSubscriptionDefinitionVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionInformationTypeDef](./type_defs.md#versioninformationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listsubscriptiondefinitionsrequestrequesttypedef"></a>

## ListSubscriptionDefinitionsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListSubscriptionDefinitionsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `str`
- `NextToken`: `str`

<a id="listsubscriptiondefinitionsresponsetypedef"></a>

## ListSubscriptionDefinitionsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListSubscriptionDefinitionsResponseTypeDef
```

Required fields:

- `Definitions`:
  `List`\[[DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourcerequestrequesttypedef"></a>

## ListTagsForResourceRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListTagsForResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`

<a id="listtagsforresourceresponsetypedef"></a>

## ListTagsForResourceResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ListTagsForResourceResponseTypeDef
```

Required fields:

- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="localdeviceresourcedatatypedef"></a>

## LocalDeviceResourceDataTypeDef

```python
from types_aiobotocore_greengrass.type_defs import LocalDeviceResourceDataTypeDef
```

Optional fields:

- `GroupOwnerSetting`:
  [GroupOwnerSettingTypeDef](./type_defs.md#groupownersettingtypedef)
- `SourcePath`: `str`

<a id="localvolumeresourcedatatypedef"></a>

## LocalVolumeResourceDataTypeDef

```python
from types_aiobotocore_greengrass.type_defs import LocalVolumeResourceDataTypeDef
```

Optional fields:

- `DestinationPath`: `str`
- `GroupOwnerSetting`:
  [GroupOwnerSettingTypeDef](./type_defs.md#groupownersettingtypedef)
- `SourcePath`: `str`

<a id="loggerdefinitionversiontypedef"></a>

## LoggerDefinitionVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import LoggerDefinitionVersionTypeDef
```

Optional fields:

- `Loggers`: `Sequence`\[[LoggerTypeDef](./type_defs.md#loggertypedef)\]

<a id="loggertypedef"></a>

## LoggerTypeDef

```python
from types_aiobotocore_greengrass.type_defs import LoggerTypeDef
```

Required fields:

- `Component`: [LoggerComponentType](./literals.md#loggercomponenttype)
- `Id`: `str`
- `Level`: [LoggerLevelType](./literals.md#loggerleveltype)
- `Type`: [LoggerTypeType](./literals.md#loggertypetype)

Optional fields:

- `Space`: `int`

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_greengrass.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="resetdeploymentsrequestrequesttypedef"></a>

## ResetDeploymentsRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResetDeploymentsRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `Force`: `bool`

<a id="resetdeploymentsresponsetypedef"></a>

## ResetDeploymentsResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResetDeploymentsResponseTypeDef
```

Required fields:

- `DeploymentArn`: `str`
- `DeploymentId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="resourceaccesspolicytypedef"></a>

## ResourceAccessPolicyTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResourceAccessPolicyTypeDef
```

Required fields:

- `ResourceId`: `str`

Optional fields:

- `Permission`: [PermissionType](./literals.md#permissiontype)

<a id="resourcedatacontainertypedef"></a>

## ResourceDataContainerTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResourceDataContainerTypeDef
```

Optional fields:

- `LocalDeviceResourceData`:
  [LocalDeviceResourceDataTypeDef](./type_defs.md#localdeviceresourcedatatypedef)
- `LocalVolumeResourceData`:
  [LocalVolumeResourceDataTypeDef](./type_defs.md#localvolumeresourcedatatypedef)
- `S3MachineLearningModelResourceData`:
  [S3MachineLearningModelResourceDataTypeDef](./type_defs.md#s3machinelearningmodelresourcedatatypedef)
- `SageMakerMachineLearningModelResourceData`:
  [SageMakerMachineLearningModelResourceDataTypeDef](./type_defs.md#sagemakermachinelearningmodelresourcedatatypedef)
- `SecretsManagerSecretResourceData`:
  [SecretsManagerSecretResourceDataTypeDef](./type_defs.md#secretsmanagersecretresourcedatatypedef)

<a id="resourcedefinitionversiontypedef"></a>

## ResourceDefinitionVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResourceDefinitionVersionTypeDef
```

Optional fields:

- `Resources`: `Sequence`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]

<a id="resourcedownloadownersettingtypedef"></a>

## ResourceDownloadOwnerSettingTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResourceDownloadOwnerSettingTypeDef
```

Required fields:

- `GroupOwner`: `str`
- `GroupPermission`: [PermissionType](./literals.md#permissiontype)

<a id="resourcetypedef"></a>

## ResourceTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResourceTypeDef
```

Required fields:

- `Id`: `str`
- `Name`: `str`
- `ResourceDataContainer`:
  [ResourceDataContainerTypeDef](./type_defs.md#resourcedatacontainertypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_greengrass.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="runtimeconfigurationtypedef"></a>

## RuntimeConfigurationTypeDef

```python
from types_aiobotocore_greengrass.type_defs import RuntimeConfigurationTypeDef
```

Optional fields:

- `TelemetryConfiguration`:
  [TelemetryConfigurationTypeDef](./type_defs.md#telemetryconfigurationtypedef)

<a id="s3machinelearningmodelresourcedatatypedef"></a>

## S3MachineLearningModelResourceDataTypeDef

```python
from types_aiobotocore_greengrass.type_defs import S3MachineLearningModelResourceDataTypeDef
```

Optional fields:

- `DestinationPath`: `str`
- `OwnerSetting`:
  [ResourceDownloadOwnerSettingTypeDef](./type_defs.md#resourcedownloadownersettingtypedef)
- `S3Uri`: `str`

<a id="sagemakermachinelearningmodelresourcedatatypedef"></a>

## SageMakerMachineLearningModelResourceDataTypeDef

```python
from types_aiobotocore_greengrass.type_defs import SageMakerMachineLearningModelResourceDataTypeDef
```

Optional fields:

- `DestinationPath`: `str`
- `OwnerSetting`:
  [ResourceDownloadOwnerSettingTypeDef](./type_defs.md#resourcedownloadownersettingtypedef)
- `SageMakerJobArn`: `str`

<a id="secretsmanagersecretresourcedatatypedef"></a>

## SecretsManagerSecretResourceDataTypeDef

```python
from types_aiobotocore_greengrass.type_defs import SecretsManagerSecretResourceDataTypeDef
```

Optional fields:

- `ARN`: `str`
- `AdditionalStagingLabelsToDownload`: `Sequence`\[`str`\]

<a id="startbulkdeploymentrequestrequesttypedef"></a>

## StartBulkDeploymentRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import StartBulkDeploymentRequestRequestTypeDef
```

Required fields:

- `ExecutionRoleArn`: `str`
- `InputFileUri`: `str`

Optional fields:

- `AmznClientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="startbulkdeploymentresponsetypedef"></a>

## StartBulkDeploymentResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import StartBulkDeploymentResponseTypeDef
```

Required fields:

- `BulkDeploymentArn`: `str`
- `BulkDeploymentId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="stopbulkdeploymentrequestrequesttypedef"></a>

## StopBulkDeploymentRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import StopBulkDeploymentRequestRequestTypeDef
```

Required fields:

- `BulkDeploymentId`: `str`

<a id="subscriptiondefinitionversiontypedef"></a>

## SubscriptionDefinitionVersionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import SubscriptionDefinitionVersionTypeDef
```

Optional fields:

- `Subscriptions`:
  `Sequence`\[[SubscriptionTypeDef](./type_defs.md#subscriptiontypedef)\]

<a id="subscriptiontypedef"></a>

## SubscriptionTypeDef

```python
from types_aiobotocore_greengrass.type_defs import SubscriptionTypeDef
```

Required fields:

- `Id`: `str`
- `Source`: `str`
- `Subject`: `str`
- `Target`: `str`

<a id="tagresourcerequestrequesttypedef"></a>

## TagResourceRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import TagResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`

Optional fields:

- `tags`: `Mapping`\[`str`, `str`\]

<a id="telemetryconfigurationtypedef"></a>

## TelemetryConfigurationTypeDef

```python
from types_aiobotocore_greengrass.type_defs import TelemetryConfigurationTypeDef
```

Required fields:

- `Telemetry`: [TelemetryType](./literals.md#telemetrytype)

Optional fields:

- `ConfigurationSyncStatus`:
  [ConfigurationSyncStatusType](./literals.md#configurationsyncstatustype)

<a id="telemetryconfigurationupdatetypedef"></a>

## TelemetryConfigurationUpdateTypeDef

```python
from types_aiobotocore_greengrass.type_defs import TelemetryConfigurationUpdateTypeDef
```

Required fields:

- `Telemetry`: [TelemetryType](./literals.md#telemetrytype)

<a id="untagresourcerequestrequesttypedef"></a>

## UntagResourceRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UntagResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`
- `TagKeys`: `Sequence`\[`str`\]

<a id="updateconnectivityinforequestrequesttypedef"></a>

## UpdateConnectivityInfoRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateConnectivityInfoRequestRequestTypeDef
```

Required fields:

- `ThingName`: `str`

Optional fields:

- `ConnectivityInfo`:
  `Sequence`\[[ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef)\]

<a id="updateconnectivityinforesponsetypedef"></a>

## UpdateConnectivityInfoResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateConnectivityInfoResponseTypeDef
```

Required fields:

- `Message`: `str`
- `Version`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updateconnectordefinitionrequestrequesttypedef"></a>

## UpdateConnectorDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateConnectorDefinitionRequestRequestTypeDef
```

Required fields:

- `ConnectorDefinitionId`: `str`

Optional fields:

- `Name`: `str`

<a id="updatecoredefinitionrequestrequesttypedef"></a>

## UpdateCoreDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateCoreDefinitionRequestRequestTypeDef
```

Required fields:

- `CoreDefinitionId`: `str`

Optional fields:

- `Name`: `str`

<a id="updatedevicedefinitionrequestrequesttypedef"></a>

## UpdateDeviceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateDeviceDefinitionRequestRequestTypeDef
```

Required fields:

- `DeviceDefinitionId`: `str`

Optional fields:

- `Name`: `str`

<a id="updatefunctiondefinitionrequestrequesttypedef"></a>

## UpdateFunctionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateFunctionDefinitionRequestRequestTypeDef
```

Required fields:

- `FunctionDefinitionId`: `str`

Optional fields:

- `Name`: `str`

<a id="updategroupcertificateconfigurationrequestrequesttypedef"></a>

## UpdateGroupCertificateConfigurationRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateGroupCertificateConfigurationRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

Optional fields:

- `CertificateExpiryInMilliseconds`: `str`

<a id="updategroupcertificateconfigurationresponsetypedef"></a>

## UpdateGroupCertificateConfigurationResponseTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateGroupCertificateConfigurationResponseTypeDef
```

Required fields:

- `CertificateAuthorityExpiryInMilliseconds`: `str`
- `CertificateExpiryInMilliseconds`: `str`
- `GroupId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updategrouprequestrequesttypedef"></a>

## UpdateGroupRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateGroupRequestRequestTypeDef
```

Required fields:

- `GroupId`: `str`

Optional fields:

- `Name`: `str`

<a id="updateloggerdefinitionrequestrequesttypedef"></a>

## UpdateLoggerDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateLoggerDefinitionRequestRequestTypeDef
```

Required fields:

- `LoggerDefinitionId`: `str`

Optional fields:

- `Name`: `str`

<a id="updateresourcedefinitionrequestrequesttypedef"></a>

## UpdateResourceDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateResourceDefinitionRequestRequestTypeDef
```

Required fields:

- `ResourceDefinitionId`: `str`

Optional fields:

- `Name`: `str`

<a id="updatesubscriptiondefinitionrequestrequesttypedef"></a>

## UpdateSubscriptionDefinitionRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateSubscriptionDefinitionRequestRequestTypeDef
```

Required fields:

- `SubscriptionDefinitionId`: `str`

Optional fields:

- `Name`: `str`

<a id="updatethingruntimeconfigurationrequestrequesttypedef"></a>

## UpdateThingRuntimeConfigurationRequestRequestTypeDef

```python
from types_aiobotocore_greengrass.type_defs import UpdateThingRuntimeConfigurationRequestRequestTypeDef
```

Required fields:

- `ThingName`: `str`

Optional fields:

- `TelemetryConfiguration`:
  [TelemetryConfigurationUpdateTypeDef](./type_defs.md#telemetryconfigurationupdatetypedef)

<a id="versioninformationtypedef"></a>

## VersionInformationTypeDef

```python
from types_aiobotocore_greengrass.type_defs import VersionInformationTypeDef
```

Optional fields:

- `Arn`: `str`
- `CreationTimestamp`: `str`
- `Id`: `str`
- `Version`: `str`
