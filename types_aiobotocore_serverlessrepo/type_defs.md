<a id="typed-dictionaries-for-aiobotocore-serverlessapplicationrepository-module"></a>

# Typed dictionaries for aiobotocore ServerlessApplicationRepository module

> [Index](..) > [ServerlessApplicationRepository](.) > Typed dictionaries

Auto-generated documentation for
[ServerlessApplicationRepository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
type annotations stubs module
[types-aiobotocore-serverlessrepo](https://pypi.org/project/types-aiobotocore-serverlessrepo/).

- [Typed dictionaries for aiobotocore ServerlessApplicationRepository module](#typed-dictionaries-for-aiobotocore-serverlessapplicationrepository-module)
  - [ApplicationDependencySummaryTypeDef](#applicationdependencysummarytypedef)
  - [ApplicationPolicyStatementTypeDef](#applicationpolicystatementtypedef)
  - [ApplicationSummaryTypeDef](#applicationsummarytypedef)
  - [CreateApplicationRequestRequestTypeDef](#createapplicationrequestrequesttypedef)
  - [CreateApplicationResponseTypeDef](#createapplicationresponsetypedef)
  - [CreateApplicationVersionRequestRequestTypeDef](#createapplicationversionrequestrequesttypedef)
  - [CreateApplicationVersionResponseTypeDef](#createapplicationversionresponsetypedef)
  - [CreateCloudFormationChangeSetRequestRequestTypeDef](#createcloudformationchangesetrequestrequesttypedef)
  - [CreateCloudFormationChangeSetResponseTypeDef](#createcloudformationchangesetresponsetypedef)
  - [CreateCloudFormationTemplateRequestRequestTypeDef](#createcloudformationtemplaterequestrequesttypedef)
  - [CreateCloudFormationTemplateResponseTypeDef](#createcloudformationtemplateresponsetypedef)
  - [DeleteApplicationRequestRequestTypeDef](#deleteapplicationrequestrequesttypedef)
  - [GetApplicationPolicyRequestRequestTypeDef](#getapplicationpolicyrequestrequesttypedef)
  - [GetApplicationPolicyResponseTypeDef](#getapplicationpolicyresponsetypedef)
  - [GetApplicationRequestRequestTypeDef](#getapplicationrequestrequesttypedef)
  - [GetApplicationResponseTypeDef](#getapplicationresponsetypedef)
  - [GetCloudFormationTemplateRequestRequestTypeDef](#getcloudformationtemplaterequestrequesttypedef)
  - [GetCloudFormationTemplateResponseTypeDef](#getcloudformationtemplateresponsetypedef)
  - [ListApplicationDependenciesRequestRequestTypeDef](#listapplicationdependenciesrequestrequesttypedef)
  - [ListApplicationDependenciesResponseTypeDef](#listapplicationdependenciesresponsetypedef)
  - [ListApplicationVersionsRequestRequestTypeDef](#listapplicationversionsrequestrequesttypedef)
  - [ListApplicationVersionsResponseTypeDef](#listapplicationversionsresponsetypedef)
  - [ListApplicationsRequestRequestTypeDef](#listapplicationsrequestrequesttypedef)
  - [ListApplicationsResponseTypeDef](#listapplicationsresponsetypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [ParameterDefinitionTypeDef](#parameterdefinitiontypedef)
  - [ParameterValueTypeDef](#parametervaluetypedef)
  - [PutApplicationPolicyRequestRequestTypeDef](#putapplicationpolicyrequestrequesttypedef)
  - [PutApplicationPolicyResponseTypeDef](#putapplicationpolicyresponsetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [RollbackConfigurationTypeDef](#rollbackconfigurationtypedef)
  - [RollbackTriggerTypeDef](#rollbacktriggertypedef)
  - [TagTypeDef](#tagtypedef)
  - [UnshareApplicationRequestRequestTypeDef](#unshareapplicationrequestrequesttypedef)
  - [UpdateApplicationRequestRequestTypeDef](#updateapplicationrequestrequesttypedef)
  - [UpdateApplicationResponseTypeDef](#updateapplicationresponsetypedef)
  - [VersionSummaryTypeDef](#versionsummarytypedef)
  - [VersionTypeDef](#versiontypedef)

<a id="applicationdependencysummarytypedef"></a>

## ApplicationDependencySummaryTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `SemanticVersion`: `str`

<a id="applicationpolicystatementtypedef"></a>

## ApplicationPolicyStatementTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ApplicationPolicyStatementTypeDef
```

Required fields:

- `Actions`: `List`\[`str`\]
- `Principals`: `List`\[`str`\]

Optional fields:

- `PrincipalOrgIDs`: `List`\[`str`\]
- `StatementId`: `str`

<a id="applicationsummarytypedef"></a>

## ApplicationSummaryTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ApplicationSummaryTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `Author`: `str`
- `Description`: `str`
- `Name`: `str`

Optional fields:

- `CreationTime`: `str`
- `HomePageUrl`: `str`
- `Labels`: `List`\[`str`\]
- `SpdxLicenseId`: `str`

<a id="createapplicationrequestrequesttypedef"></a>

## CreateApplicationRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateApplicationRequestRequestTypeDef
```

Required fields:

- `Author`: `str`
- `Description`: `str`
- `Name`: `str`

Optional fields:

- `HomePageUrl`: `str`
- `Labels`: `Sequence`\[`str`\]
- `LicenseBody`: `str`
- `LicenseUrl`: `str`
- `ReadmeBody`: `str`
- `ReadmeUrl`: `str`
- `SemanticVersion`: `str`
- `SourceCodeArchiveUrl`: `str`
- `SourceCodeUrl`: `str`
- `SpdxLicenseId`: `str`
- `TemplateBody`: `str`
- `TemplateUrl`: `str`

<a id="createapplicationresponsetypedef"></a>

## CreateApplicationResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateApplicationResponseTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `Author`: `str`
- `CreationTime`: `str`
- `Description`: `str`
- `HomePageUrl`: `str`
- `IsVerifiedAuthor`: `bool`
- `Labels`: `List`\[`str`\]
- `LicenseUrl`: `str`
- `Name`: `str`
- `ReadmeUrl`: `str`
- `SpdxLicenseId`: `str`
- `VerifiedAuthorUrl`: `str`
- `Version`: [VersionTypeDef](./type_defs.md#versiontypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createapplicationversionrequestrequesttypedef"></a>

## CreateApplicationVersionRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateApplicationVersionRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `SemanticVersion`: `str`

Optional fields:

- `SourceCodeArchiveUrl`: `str`
- `SourceCodeUrl`: `str`
- `TemplateBody`: `str`
- `TemplateUrl`: `str`

<a id="createapplicationversionresponsetypedef"></a>

## CreateApplicationVersionResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateApplicationVersionResponseTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `CreationTime`: `str`
- `ParameterDefinitions`:
  `List`\[[ParameterDefinitionTypeDef](./type_defs.md#parameterdefinitiontypedef)\]
- `RequiredCapabilities`:
  `List`\[[CapabilityType](./literals.md#capabilitytype)\]
- `ResourcesSupported`: `bool`
- `SemanticVersion`: `str`
- `SourceCodeArchiveUrl`: `str`
- `SourceCodeUrl`: `str`
- `TemplateUrl`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createcloudformationchangesetrequestrequesttypedef"></a>

## CreateCloudFormationChangeSetRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateCloudFormationChangeSetRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `StackName`: `str`

Optional fields:

- `Capabilities`: `Sequence`\[`str`\]
- `ChangeSetName`: `str`
- `ClientToken`: `str`
- `Description`: `str`
- `NotificationArns`: `Sequence`\[`str`\]
- `ParameterOverrides`:
  `Sequence`\[[ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)\]
- `ResourceTypes`: `Sequence`\[`str`\]
- `RollbackConfiguration`:
  [RollbackConfigurationTypeDef](./type_defs.md#rollbackconfigurationtypedef)
- `SemanticVersion`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `TemplateId`: `str`

<a id="createcloudformationchangesetresponsetypedef"></a>

## CreateCloudFormationChangeSetResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateCloudFormationChangeSetResponseTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `ChangeSetId`: `str`
- `SemanticVersion`: `str`
- `StackId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createcloudformationtemplaterequestrequesttypedef"></a>

## CreateCloudFormationTemplateRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateCloudFormationTemplateRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`

Optional fields:

- `SemanticVersion`: `str`

<a id="createcloudformationtemplateresponsetypedef"></a>

## CreateCloudFormationTemplateResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import CreateCloudFormationTemplateResponseTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `CreationTime`: `str`
- `ExpirationTime`: `str`
- `SemanticVersion`: `str`
- `Status`: [StatusType](./literals.md#statustype)
- `TemplateId`: `str`
- `TemplateUrl`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteapplicationrequestrequesttypedef"></a>

## DeleteApplicationRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import DeleteApplicationRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`

<a id="getapplicationpolicyrequestrequesttypedef"></a>

## GetApplicationPolicyRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import GetApplicationPolicyRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`

<a id="getapplicationpolicyresponsetypedef"></a>

## GetApplicationPolicyResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import GetApplicationPolicyResponseTypeDef
```

Required fields:

- `Statements`:
  `List`\[[ApplicationPolicyStatementTypeDef](./type_defs.md#applicationpolicystatementtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getapplicationrequestrequesttypedef"></a>

## GetApplicationRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import GetApplicationRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`

Optional fields:

- `SemanticVersion`: `str`

<a id="getapplicationresponsetypedef"></a>

## GetApplicationResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import GetApplicationResponseTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `Author`: `str`
- `CreationTime`: `str`
- `Description`: `str`
- `HomePageUrl`: `str`
- `IsVerifiedAuthor`: `bool`
- `Labels`: `List`\[`str`\]
- `LicenseUrl`: `str`
- `Name`: `str`
- `ReadmeUrl`: `str`
- `SpdxLicenseId`: `str`
- `VerifiedAuthorUrl`: `str`
- `Version`: [VersionTypeDef](./type_defs.md#versiontypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getcloudformationtemplaterequestrequesttypedef"></a>

## GetCloudFormationTemplateRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import GetCloudFormationTemplateRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `TemplateId`: `str`

<a id="getcloudformationtemplateresponsetypedef"></a>

## GetCloudFormationTemplateResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import GetCloudFormationTemplateResponseTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `CreationTime`: `str`
- `ExpirationTime`: `str`
- `SemanticVersion`: `str`
- `Status`: [StatusType](./literals.md#statustype)
- `TemplateId`: `str`
- `TemplateUrl`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listapplicationdependenciesrequestrequesttypedef"></a>

## ListApplicationDependenciesRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ListApplicationDependenciesRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`

Optional fields:

- `MaxItems`: `int`
- `NextToken`: `str`
- `SemanticVersion`: `str`

<a id="listapplicationdependenciesresponsetypedef"></a>

## ListApplicationDependenciesResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ListApplicationDependenciesResponseTypeDef
```

Required fields:

- `Dependencies`:
  `List`\[[ApplicationDependencySummaryTypeDef](./type_defs.md#applicationdependencysummarytypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listapplicationversionsrequestrequesttypedef"></a>

## ListApplicationVersionsRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ListApplicationVersionsRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`

Optional fields:

- `MaxItems`: `int`
- `NextToken`: `str`

<a id="listapplicationversionsresponsetypedef"></a>

## ListApplicationVersionsResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ListApplicationVersionsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Versions`:
  `List`\[[VersionSummaryTypeDef](./type_defs.md#versionsummarytypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listapplicationsrequestrequesttypedef"></a>

## ListApplicationsRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ListApplicationsRequestRequestTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `NextToken`: `str`

<a id="listapplicationsresponsetypedef"></a>

## ListApplicationsResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ListApplicationsResponseTypeDef
```

Required fields:

- `Applications`:
  `List`\[[ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="parameterdefinitiontypedef"></a>

## ParameterDefinitionTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ParameterDefinitionTypeDef
```

Required fields:

- `Name`: `str`
- `ReferencedByResources`: `List`\[`str`\]

Optional fields:

- `AllowedPattern`: `str`
- `AllowedValues`: `List`\[`str`\]
- `ConstraintDescription`: `str`
- `DefaultValue`: `str`
- `Description`: `str`
- `MaxLength`: `int`
- `MaxValue`: `int`
- `MinLength`: `int`
- `MinValue`: `int`
- `NoEcho`: `bool`
- `Type`: `str`

<a id="parametervaluetypedef"></a>

## ParameterValueTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ParameterValueTypeDef
```

Required fields:

- `Name`: `str`
- `Value`: `str`

<a id="putapplicationpolicyrequestrequesttypedef"></a>

## PutApplicationPolicyRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import PutApplicationPolicyRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `Statements`:
  `Sequence`\[[ApplicationPolicyStatementTypeDef](./type_defs.md#applicationpolicystatementtypedef)\]

<a id="putapplicationpolicyresponsetypedef"></a>

## PutApplicationPolicyResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import PutApplicationPolicyResponseTypeDef
```

Required fields:

- `Statements`:
  `List`\[[ApplicationPolicyStatementTypeDef](./type_defs.md#applicationpolicystatementtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="rollbackconfigurationtypedef"></a>

## RollbackConfigurationTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import RollbackConfigurationTypeDef
```

Optional fields:

- `MonitoringTimeInMinutes`: `int`
- `RollbackTriggers`:
  `Sequence`\[[RollbackTriggerTypeDef](./type_defs.md#rollbacktriggertypedef)\]

<a id="rollbacktriggertypedef"></a>

## RollbackTriggerTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import RollbackTriggerTypeDef
```

Required fields:

- `Arn`: `str`
- `Type`: `str`

<a id="tagtypedef"></a>

## TagTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import TagTypeDef
```

Required fields:

- `Key`: `str`
- `Value`: `str`

<a id="unshareapplicationrequestrequesttypedef"></a>

## UnshareApplicationRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import UnshareApplicationRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `OrganizationId`: `str`

<a id="updateapplicationrequestrequesttypedef"></a>

## UpdateApplicationRequestRequestTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import UpdateApplicationRequestRequestTypeDef
```

Required fields:

- `ApplicationId`: `str`

Optional fields:

- `Author`: `str`
- `Description`: `str`
- `HomePageUrl`: `str`
- `Labels`: `Sequence`\[`str`\]
- `ReadmeBody`: `str`
- `ReadmeUrl`: `str`

<a id="updateapplicationresponsetypedef"></a>

## UpdateApplicationResponseTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import UpdateApplicationResponseTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `Author`: `str`
- `CreationTime`: `str`
- `Description`: `str`
- `HomePageUrl`: `str`
- `IsVerifiedAuthor`: `bool`
- `Labels`: `List`\[`str`\]
- `LicenseUrl`: `str`
- `Name`: `str`
- `ReadmeUrl`: `str`
- `SpdxLicenseId`: `str`
- `VerifiedAuthorUrl`: `str`
- `Version`: [VersionTypeDef](./type_defs.md#versiontypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="versionsummarytypedef"></a>

## VersionSummaryTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import VersionSummaryTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `CreationTime`: `str`
- `SemanticVersion`: `str`

Optional fields:

- `SourceCodeUrl`: `str`

<a id="versiontypedef"></a>

## VersionTypeDef

```python
from types_aiobotocore_serverlessrepo.type_defs import VersionTypeDef
```

Required fields:

- `ApplicationId`: `str`
- `CreationTime`: `str`
- `ParameterDefinitions`:
  `List`\[[ParameterDefinitionTypeDef](./type_defs.md#parameterdefinitiontypedef)\]
- `RequiredCapabilities`:
  `List`\[[CapabilityType](./literals.md#capabilitytype)\]
- `ResourcesSupported`: `bool`
- `SemanticVersion`: `str`
- `TemplateUrl`: `str`

Optional fields:

- `SourceCodeArchiveUrl`: `str`
- `SourceCodeUrl`: `str`
