# Type definitions

> [Index](../README.md) > [ServerlessApplicationRepository](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ServerlessApplicationRepository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
    type annotations stubs module [types-aiobotocore-serverlessrepo](https://pypi.org/project/types-aiobotocore-serverlessrepo/).

## ApplicationPolicyStatementUnionTypeDef

```python
# ApplicationPolicyStatementUnionTypeDef definition

ApplicationPolicyStatementUnionTypeDef = Union[
    ApplicationPolicyStatementTypeDef,  # (1)
    ApplicationPolicyStatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApplicationPolicyStatementTypeDef](./type_defs.md#applicationpolicystatementtypedef) 
2. See [:material-code-braces: ApplicationPolicyStatementOutputTypeDef](./type_defs.md#applicationpolicystatementoutputtypedef) 



## ApplicationDependencySummaryTypeDef

```python
# ApplicationDependencySummaryTypeDef definition

class ApplicationDependencySummaryTypeDef(TypedDict):
    ApplicationId: str,
    SemanticVersion: str,
```

## ApplicationPolicyStatementOutputTypeDef

```python
# ApplicationPolicyStatementOutputTypeDef definition

class ApplicationPolicyStatementOutputTypeDef(TypedDict):
    Actions: List[str],
    Principals: List[str],
    PrincipalOrgIDs: NotRequired[List[str]],
    StatementId: NotRequired[str],
```

## ApplicationPolicyStatementTypeDef

```python
# ApplicationPolicyStatementTypeDef definition

class ApplicationPolicyStatementTypeDef(TypedDict):
    Actions: Sequence[str],
    Principals: Sequence[str],
    PrincipalOrgIDs: NotRequired[Sequence[str]],
    StatementId: NotRequired[str],
```

## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    ApplicationId: str,
    Author: str,
    Description: str,
    Name: str,
    CreationTime: NotRequired[str],
    HomePageUrl: NotRequired[str],
    Labels: NotRequired[List[str]],
    SpdxLicenseId: NotRequired[str],
```

## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    Author: str,
    Description: str,
    Name: str,
    HomePageUrl: NotRequired[str],
    Labels: NotRequired[Sequence[str]],
    LicenseBody: NotRequired[str],
    LicenseUrl: NotRequired[str],
    ReadmeBody: NotRequired[str],
    ReadmeUrl: NotRequired[str],
    SemanticVersion: NotRequired[str],
    SourceCodeArchiveUrl: NotRequired[str],
    SourceCodeUrl: NotRequired[str],
    SpdxLicenseId: NotRequired[str],
    TemplateBody: NotRequired[str],
    TemplateUrl: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CreateApplicationVersionRequestRequestTypeDef

```python
# CreateApplicationVersionRequestRequestTypeDef definition

class CreateApplicationVersionRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SemanticVersion: str,
    SourceCodeArchiveUrl: NotRequired[str],
    SourceCodeUrl: NotRequired[str],
    TemplateBody: NotRequired[str],
    TemplateUrl: NotRequired[str],
```

## ParameterDefinitionTypeDef

```python
# ParameterDefinitionTypeDef definition

class ParameterDefinitionTypeDef(TypedDict):
    Name: str,
    ReferencedByResources: List[str],
    AllowedPattern: NotRequired[str],
    AllowedValues: NotRequired[List[str]],
    ConstraintDescription: NotRequired[str],
    DefaultValue: NotRequired[str],
    Description: NotRequired[str],
    MaxLength: NotRequired[int],
    MaxValue: NotRequired[int],
    MinLength: NotRequired[int],
    MinValue: NotRequired[int],
    NoEcho: NotRequired[bool],
    Type: NotRequired[str],
```

## ParameterValueTypeDef

```python
# ParameterValueTypeDef definition

class ParameterValueTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateCloudFormationTemplateRequestRequestTypeDef

```python
# CreateCloudFormationTemplateRequestRequestTypeDef definition

class CreateCloudFormationTemplateRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SemanticVersion: NotRequired[str],
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetApplicationPolicyRequestRequestTypeDef

```python
# GetApplicationPolicyRequestRequestTypeDef definition

class GetApplicationPolicyRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SemanticVersion: NotRequired[str],
```

## GetCloudFormationTemplateRequestRequestTypeDef

```python
# GetCloudFormationTemplateRequestRequestTypeDef definition

class GetCloudFormationTemplateRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    TemplateId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationDependenciesRequestRequestTypeDef

```python
# ListApplicationDependenciesRequestRequestTypeDef definition

class ListApplicationDependenciesRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    MaxItems: NotRequired[int],
    NextToken: NotRequired[str],
    SemanticVersion: NotRequired[str],
```

## ListApplicationVersionsRequestRequestTypeDef

```python
# ListApplicationVersionsRequestRequestTypeDef definition

class ListApplicationVersionsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    MaxItems: NotRequired[int],
    NextToken: NotRequired[str],
```

## VersionSummaryTypeDef

```python
# VersionSummaryTypeDef definition

class VersionSummaryTypeDef(TypedDict):
    ApplicationId: str,
    CreationTime: str,
    SemanticVersion: str,
    SourceCodeUrl: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    NextToken: NotRequired[str],
```

## RollbackTriggerTypeDef

```python
# RollbackTriggerTypeDef definition

class RollbackTriggerTypeDef(TypedDict):
    Arn: str,
    Type: str,
```

## UnshareApplicationRequestRequestTypeDef

```python
# UnshareApplicationRequestRequestTypeDef definition

class UnshareApplicationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    OrganizationId: str,
```

## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    Author: NotRequired[str],
    Description: NotRequired[str],
    HomePageUrl: NotRequired[str],
    Labels: NotRequired[Sequence[str]],
    ReadmeBody: NotRequired[str],
    ReadmeUrl: NotRequired[str],
```

## CreateCloudFormationChangeSetResponseTypeDef

```python
# CreateCloudFormationChangeSetResponseTypeDef definition

class CreateCloudFormationChangeSetResponseTypeDef(TypedDict):
    ApplicationId: str,
    ChangeSetId: str,
    SemanticVersion: str,
    StackId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCloudFormationTemplateResponseTypeDef

```python
# CreateCloudFormationTemplateResponseTypeDef definition

class CreateCloudFormationTemplateResponseTypeDef(TypedDict):
    ApplicationId: str,
    CreationTime: str,
    ExpirationTime: str,
    SemanticVersion: str,
    Status: StatusType,  # (1)
    TemplateId: str,
    TemplateUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationPolicyResponseTypeDef

```python
# GetApplicationPolicyResponseTypeDef definition

class GetApplicationPolicyResponseTypeDef(TypedDict):
    Statements: List[ApplicationPolicyStatementOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationPolicyStatementOutputTypeDef](./type_defs.md#applicationpolicystatementoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCloudFormationTemplateResponseTypeDef

```python
# GetCloudFormationTemplateResponseTypeDef definition

class GetCloudFormationTemplateResponseTypeDef(TypedDict):
    ApplicationId: str,
    CreationTime: str,
    ExpirationTime: str,
    SemanticVersion: str,
    Status: StatusType,  # (1)
    TemplateId: str,
    TemplateUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationDependenciesResponseTypeDef

```python
# ListApplicationDependenciesResponseTypeDef definition

class ListApplicationDependenciesResponseTypeDef(TypedDict):
    Dependencies: List[ApplicationDependencySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationDependencySummaryTypeDef](./type_defs.md#applicationdependencysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    Applications: List[ApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutApplicationPolicyResponseTypeDef

```python
# PutApplicationPolicyResponseTypeDef definition

class PutApplicationPolicyResponseTypeDef(TypedDict):
    Statements: List[ApplicationPolicyStatementOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationPolicyStatementOutputTypeDef](./type_defs.md#applicationpolicystatementoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationVersionResponseTypeDef

```python
# CreateApplicationVersionResponseTypeDef definition

class CreateApplicationVersionResponseTypeDef(TypedDict):
    ApplicationId: str,
    CreationTime: str,
    ParameterDefinitions: List[ParameterDefinitionTypeDef],  # (1)
    RequiredCapabilities: List[CapabilityType],  # (2)
    ResourcesSupported: bool,
    SemanticVersion: str,
    SourceCodeArchiveUrl: str,
    SourceCodeUrl: str,
    TemplateUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ParameterDefinitionTypeDef](./type_defs.md#parameterdefinitiontypedef) 
2. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VersionTypeDef

```python
# VersionTypeDef definition

class VersionTypeDef(TypedDict):
    ApplicationId: str,
    CreationTime: str,
    ParameterDefinitions: List[ParameterDefinitionTypeDef],  # (1)
    RequiredCapabilities: List[CapabilityType],  # (2)
    ResourcesSupported: bool,
    SemanticVersion: str,
    TemplateUrl: str,
    SourceCodeArchiveUrl: NotRequired[str],
    SourceCodeUrl: NotRequired[str],
```

1. See [:material-code-braces: ParameterDefinitionTypeDef](./type_defs.md#parameterdefinitiontypedef) 
2. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
## ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef

```python
# ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef definition

class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(TypedDict):
    ApplicationId: str,
    SemanticVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef

```python
# ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef definition

class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(TypedDict):
    ApplicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestListApplicationsPaginateTypeDef

```python
# ListApplicationsRequestListApplicationsPaginateTypeDef definition

class ListApplicationsRequestListApplicationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationVersionsResponseTypeDef

```python
# ListApplicationVersionsResponseTypeDef definition

class ListApplicationVersionsResponseTypeDef(TypedDict):
    Versions: List[VersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionSummaryTypeDef](./type_defs.md#versionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RollbackConfigurationTypeDef

```python
# RollbackConfigurationTypeDef definition

class RollbackConfigurationTypeDef(TypedDict):
    MonitoringTimeInMinutes: NotRequired[int],
    RollbackTriggers: NotRequired[Sequence[RollbackTriggerTypeDef]],  # (1)
```

1. See [:material-code-braces: RollbackTriggerTypeDef](./type_defs.md#rollbacktriggertypedef) 
## PutApplicationPolicyRequestRequestTypeDef

```python
# PutApplicationPolicyRequestRequestTypeDef definition

class PutApplicationPolicyRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    Statements: Sequence[ApplicationPolicyStatementUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationPolicyStatementTypeDef](./type_defs.md#applicationpolicystatementtypedef) [:material-code-braces: ApplicationPolicyStatementOutputTypeDef](./type_defs.md#applicationpolicystatementoutputtypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    ApplicationId: str,
    Author: str,
    CreationTime: str,
    Description: str,
    HomePageUrl: str,
    IsVerifiedAuthor: bool,
    Labels: List[str],
    LicenseUrl: str,
    Name: str,
    ReadmeUrl: str,
    SpdxLicenseId: str,
    VerifiedAuthorUrl: str,
    Version: VersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VersionTypeDef](./type_defs.md#versiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    ApplicationId: str,
    Author: str,
    CreationTime: str,
    Description: str,
    HomePageUrl: str,
    IsVerifiedAuthor: bool,
    Labels: List[str],
    LicenseUrl: str,
    Name: str,
    ReadmeUrl: str,
    SpdxLicenseId: str,
    VerifiedAuthorUrl: str,
    Version: VersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VersionTypeDef](./type_defs.md#versiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationResponseTypeDef

```python
# UpdateApplicationResponseTypeDef definition

class UpdateApplicationResponseTypeDef(TypedDict):
    ApplicationId: str,
    Author: str,
    CreationTime: str,
    Description: str,
    HomePageUrl: str,
    IsVerifiedAuthor: bool,
    Labels: List[str],
    LicenseUrl: str,
    Name: str,
    ReadmeUrl: str,
    SpdxLicenseId: str,
    VerifiedAuthorUrl: str,
    Version: VersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VersionTypeDef](./type_defs.md#versiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCloudFormationChangeSetRequestRequestTypeDef

```python
# CreateCloudFormationChangeSetRequestRequestTypeDef definition

class CreateCloudFormationChangeSetRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    StackName: str,
    Capabilities: NotRequired[Sequence[str]],
    ChangeSetName: NotRequired[str],
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    NotificationArns: NotRequired[Sequence[str]],
    ParameterOverrides: NotRequired[Sequence[ParameterValueTypeDef]],  # (1)
    ResourceTypes: NotRequired[Sequence[str]],
    RollbackConfiguration: NotRequired[RollbackConfigurationTypeDef],  # (2)
    SemanticVersion: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    TemplateId: NotRequired[str],
```

1. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 
2. See [:material-code-braces: RollbackConfigurationTypeDef](./type_defs.md#rollbackconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
