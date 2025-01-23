# Type definitions

> [Index](../README.md) > [SsmSap](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SsmSap](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#ssmsap)
    type annotations stubs module [types-aiobotocore-ssm-sap](https://pypi.org/project/types-aiobotocore-ssm-sap/).



## ApplicationCredentialTypeDef

```python
# ApplicationCredentialTypeDef definition

class ApplicationCredentialTypeDef(TypedDict):
    DatabaseName: str,
    CredentialType: CredentialTypeType,  # (1)
    SecretId: str,
```

1. See [:material-code-brackets: CredentialTypeType](./literals.md#credentialtypetype) 
## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    DiscoveryStatus: NotRequired[ApplicationDiscoveryStatusType],  # (1)
    Type: NotRequired[ApplicationTypeType],  # (2)
    Arn: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ApplicationDiscoveryStatusType](./literals.md#applicationdiscoverystatustype) 
2. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[ApplicationTypeType],  # (1)
    Arn: NotRequired[str],
    AppRegistryArn: NotRequired[str],
    Status: NotRequired[ApplicationStatusType],  # (2)
    DiscoveryStatus: NotRequired[ApplicationDiscoveryStatusType],  # (3)
    Components: NotRequired[List[str]],
    LastUpdated: NotRequired[datetime],
    StatusMessage: NotRequired[str],
    AssociatedApplicationArns: NotRequired[List[str]],
```

1. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-brackets: ApplicationDiscoveryStatusType](./literals.md#applicationdiscoverystatustype) 
## IpAddressMemberTypeDef

```python
# IpAddressMemberTypeDef definition

class IpAddressMemberTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    Primary: NotRequired[bool],
    AllocationType: NotRequired[AllocationTypeType],  # (1)
```

1. See [:material-code-brackets: AllocationTypeType](./literals.md#allocationtypetype) 
## BackintConfigTypeDef

```python
# BackintConfigTypeDef definition

class BackintConfigTypeDef(TypedDict):
    BackintMode: BackintModeType,  # (1)
    EnsureNoBackupInProcess: bool,
```

1. See [:material-code-brackets: BackintModeType](./literals.md#backintmodetype) 
## ComponentInfoTypeDef

```python
# ComponentInfoTypeDef definition

class ComponentInfoTypeDef(TypedDict):
    ComponentType: ComponentTypeType,  # (1)
    Sid: str,
    Ec2InstanceId: str,
```

1. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
## ComponentSummaryTypeDef

```python
# ComponentSummaryTypeDef definition

class ComponentSummaryTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ComponentId: NotRequired[str],
    ComponentType: NotRequired[ComponentTypeType],  # (1)
    Tags: NotRequired[Dict[str, str]],
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
## DatabaseConnectionTypeDef

```python
# DatabaseConnectionTypeDef definition

class DatabaseConnectionTypeDef(TypedDict):
    DatabaseConnectionMethod: NotRequired[DatabaseConnectionMethodType],  # (1)
    DatabaseArn: NotRequired[str],
    ConnectionIp: NotRequired[str],
```

1. See [:material-code-brackets: DatabaseConnectionMethodType](./literals.md#databaseconnectionmethodtype) 
## HostTypeDef

```python
# HostTypeDef definition

class HostTypeDef(TypedDict):
    HostName: NotRequired[str],
    HostIp: NotRequired[str],
    EC2InstanceId: NotRequired[str],
    InstanceId: NotRequired[str],
    HostRole: NotRequired[HostRoleType],  # (1)
    OsVersion: NotRequired[str],
```

1. See [:material-code-brackets: HostRoleType](./literals.md#hostroletype) 
## ResilienceTypeDef

```python
# ResilienceTypeDef definition

class ResilienceTypeDef(TypedDict):
    HsrTier: NotRequired[str],
    HsrReplicationMode: NotRequired[ReplicationModeType],  # (1)
    HsrOperationMode: NotRequired[OperationModeType],  # (2)
    ClusterStatus: NotRequired[ClusterStatusType],  # (3)
    EnqueueReplication: NotRequired[bool],
```

1. See [:material-code-brackets: ReplicationModeType](./literals.md#replicationmodetype) 
2. See [:material-code-brackets: OperationModeType](./literals.md#operationmodetype) 
3. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
## DatabaseSummaryTypeDef

```python
# DatabaseSummaryTypeDef definition

class DatabaseSummaryTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ComponentId: NotRequired[str],
    DatabaseId: NotRequired[str],
    DatabaseType: NotRequired[DatabaseTypeType],  # (1)
    Arn: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DatabaseTypeType](./literals.md#databasetypetype) 
## DeleteResourcePermissionInputRequestTypeDef

```python
# DeleteResourcePermissionInputRequestTypeDef definition

class DeleteResourcePermissionInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    ActionType: NotRequired[PermissionActionTypeType],  # (1)
    SourceResourceArn: NotRequired[str],
```

1. See [:material-code-brackets: PermissionActionTypeType](./literals.md#permissionactiontypetype) 
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

## DeregisterApplicationInputRequestTypeDef

```python
# DeregisterApplicationInputRequestTypeDef definition

class DeregisterApplicationInputRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Value: str,
    Operator: FilterOperatorType,  # (1)
```

1. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
## GetApplicationInputRequestTypeDef

```python
# GetApplicationInputRequestTypeDef definition

class GetApplicationInputRequestTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ApplicationArn: NotRequired[str],
    AppRegistryArn: NotRequired[str],
```

## GetComponentInputRequestTypeDef

```python
# GetComponentInputRequestTypeDef definition

class GetComponentInputRequestTypeDef(TypedDict):
    ApplicationId: str,
    ComponentId: str,
```

## GetDatabaseInputRequestTypeDef

```python
# GetDatabaseInputRequestTypeDef definition

class GetDatabaseInputRequestTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ComponentId: NotRequired[str],
    DatabaseId: NotRequired[str],
    DatabaseArn: NotRequired[str],
```

## GetOperationInputRequestTypeDef

```python
# GetOperationInputRequestTypeDef definition

class GetOperationInputRequestTypeDef(TypedDict):
    OperationId: str,
```

## OperationTypeDef

```python
# OperationTypeDef definition

class OperationTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[str],
    Status: NotRequired[OperationStatusType],  # (1)
    StatusMessage: NotRequired[str],
    Properties: NotRequired[Dict[str, str]],
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    ResourceArn: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
## GetResourcePermissionInputRequestTypeDef

```python
# GetResourcePermissionInputRequestTypeDef definition

class GetResourcePermissionInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    ActionType: NotRequired[PermissionActionTypeType],  # (1)
```

1. See [:material-code-brackets: PermissionActionTypeType](./literals.md#permissionactiontypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListComponentsInputRequestTypeDef

```python
# ListComponentsInputRequestTypeDef definition

class ListComponentsInputRequestTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDatabasesInputRequestTypeDef

```python
# ListDatabasesInputRequestTypeDef definition

class ListDatabasesInputRequestTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ComponentId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[str],
```

## PutResourcePermissionInputRequestTypeDef

```python
# PutResourcePermissionInputRequestTypeDef definition

class PutResourcePermissionInputRequestTypeDef(TypedDict):
    ActionType: PermissionActionTypeType,  # (1)
    SourceResourceArn: str,
    ResourceArn: str,
```

1. See [:material-code-brackets: PermissionActionTypeType](./literals.md#permissionactiontypetype) 
## StartApplicationInputRequestTypeDef

```python
# StartApplicationInputRequestTypeDef definition

class StartApplicationInputRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## StartApplicationRefreshInputRequestTypeDef

```python
# StartApplicationRefreshInputRequestTypeDef definition

class StartApplicationRefreshInputRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## StopApplicationInputRequestTypeDef

```python
# StopApplicationInputRequestTypeDef definition

class StopApplicationInputRequestTypeDef(TypedDict):
    ApplicationId: str,
    StopConnectedEntity: NotRequired[ConnectedEntityTypeType],  # (1)
    IncludeEc2InstanceShutdown: NotRequired[bool],
```

1. See [:material-code-brackets: ConnectedEntityTypeType](./literals.md#connectedentitytypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## DatabaseTypeDef

```python
# DatabaseTypeDef definition

class DatabaseTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ComponentId: NotRequired[str],
    Credentials: NotRequired[List[ApplicationCredentialTypeDef]],  # (1)
    DatabaseId: NotRequired[str],
    DatabaseName: NotRequired[str],
    DatabaseType: NotRequired[DatabaseTypeType],  # (2)
    Arn: NotRequired[str],
    Status: NotRequired[DatabaseStatusType],  # (3)
    PrimaryHost: NotRequired[str],
    SQLPort: NotRequired[int],
    LastUpdated: NotRequired[datetime],
    ConnectedComponentArns: NotRequired[List[str]],
```

1. See [:material-code-braces: ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef) 
2. See [:material-code-brackets: DatabaseTypeType](./literals.md#databasetypetype) 
3. See [:material-code-brackets: DatabaseStatusType](./literals.md#databasestatustype) 
## AssociatedHostTypeDef

```python
# AssociatedHostTypeDef definition

class AssociatedHostTypeDef(TypedDict):
    Hostname: NotRequired[str],
    Ec2InstanceId: NotRequired[str],
    IpAddresses: NotRequired[List[IpAddressMemberTypeDef]],  # (1)
    OsVersion: NotRequired[str],
```

1. See [:material-code-braces: IpAddressMemberTypeDef](./type_defs.md#ipaddressmembertypedef) 
## UpdateApplicationSettingsInputRequestTypeDef

```python
# UpdateApplicationSettingsInputRequestTypeDef definition

class UpdateApplicationSettingsInputRequestTypeDef(TypedDict):
    ApplicationId: str,
    CredentialsToAddOrUpdate: NotRequired[Sequence[ApplicationCredentialTypeDef]],  # (1)
    CredentialsToRemove: NotRequired[Sequence[ApplicationCredentialTypeDef]],  # (1)
    Backint: NotRequired[BackintConfigTypeDef],  # (3)
    DatabaseArn: NotRequired[str],
```

1. See [:material-code-braces: ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef) 
2. See [:material-code-braces: ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef) 
3. See [:material-code-braces: BackintConfigTypeDef](./type_defs.md#backintconfigtypedef) 
## RegisterApplicationInputRequestTypeDef

```python
# RegisterApplicationInputRequestTypeDef definition

class RegisterApplicationInputRequestTypeDef(TypedDict):
    ApplicationId: str,
    ApplicationType: ApplicationTypeType,  # (1)
    Instances: Sequence[str],
    SapInstanceNumber: NotRequired[str],
    Sid: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    Credentials: NotRequired[Sequence[ApplicationCredentialTypeDef]],  # (2)
    DatabaseArn: NotRequired[str],
    ComponentsInfo: NotRequired[Sequence[ComponentInfoTypeDef]],  # (3)
```

1. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
2. See [:material-code-braces: ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef) 
3. See [:material-code-braces: ComponentInfoTypeDef](./type_defs.md#componentinfotypedef) 
## DeleteResourcePermissionOutputTypeDef

```python
# DeleteResourcePermissionOutputTypeDef definition

class DeleteResourcePermissionOutputTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationOutputTypeDef

```python
# GetApplicationOutputTypeDef definition

class GetApplicationOutputTypeDef(TypedDict):
    Application: ApplicationTypeDef,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePermissionOutputTypeDef

```python
# GetResourcePermissionOutputTypeDef definition

class GetResourcePermissionOutputTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsOutputTypeDef

```python
# ListApplicationsOutputTypeDef definition

class ListApplicationsOutputTypeDef(TypedDict):
    Applications: List[ApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComponentsOutputTypeDef

```python
# ListComponentsOutputTypeDef definition

class ListComponentsOutputTypeDef(TypedDict):
    Components: List[ComponentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatabasesOutputTypeDef

```python
# ListDatabasesOutputTypeDef definition

class ListDatabasesOutputTypeDef(TypedDict):
    Databases: List[DatabaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatabaseSummaryTypeDef](./type_defs.md#databasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePermissionOutputTypeDef

```python
# PutResourcePermissionOutputTypeDef definition

class PutResourcePermissionOutputTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterApplicationOutputTypeDef

```python
# RegisterApplicationOutputTypeDef definition

class RegisterApplicationOutputTypeDef(TypedDict):
    Application: ApplicationTypeDef,  # (1)
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartApplicationOutputTypeDef

```python
# StartApplicationOutputTypeDef definition

class StartApplicationOutputTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartApplicationRefreshOutputTypeDef

```python
# StartApplicationRefreshOutputTypeDef definition

class StartApplicationRefreshOutputTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopApplicationOutputTypeDef

```python
# StopApplicationOutputTypeDef definition

class StopApplicationOutputTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationSettingsOutputTypeDef

```python
# UpdateApplicationSettingsOutputTypeDef definition

class UpdateApplicationSettingsOutputTypeDef(TypedDict):
    Message: str,
    OperationIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsInputRequestTypeDef

```python
# ListApplicationsInputRequestTypeDef definition

class ListApplicationsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListOperationEventsInputRequestTypeDef

```python
# ListOperationEventsInputRequestTypeDef definition

class ListOperationEventsInputRequestTypeDef(TypedDict):
    OperationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListOperationsInputRequestTypeDef

```python
# ListOperationsInputRequestTypeDef definition

class ListOperationsInputRequestTypeDef(TypedDict):
    ApplicationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetOperationOutputTypeDef

```python
# GetOperationOutputTypeDef definition

class GetOperationOutputTypeDef(TypedDict):
    Operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOperationsOutputTypeDef

```python
# ListOperationsOutputTypeDef definition

class ListOperationsOutputTypeDef(TypedDict):
    Operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsInputPaginateTypeDef

```python
# ListApplicationsInputPaginateTypeDef definition

class ListApplicationsInputPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComponentsInputPaginateTypeDef

```python
# ListComponentsInputPaginateTypeDef definition

class ListComponentsInputPaginateTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatabasesInputPaginateTypeDef

```python
# ListDatabasesInputPaginateTypeDef definition

class ListDatabasesInputPaginateTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ComponentId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOperationEventsInputPaginateTypeDef

```python
# ListOperationEventsInputPaginateTypeDef definition

class ListOperationEventsInputPaginateTypeDef(TypedDict):
    OperationId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOperationsInputPaginateTypeDef

```python
# ListOperationsInputPaginateTypeDef definition

class ListOperationsInputPaginateTypeDef(TypedDict):
    ApplicationId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## OperationEventTypeDef

```python
# OperationEventTypeDef definition

class OperationEventTypeDef(TypedDict):
    Description: NotRequired[str],
    Resource: NotRequired[ResourceTypeDef],  # (1)
    Status: NotRequired[OperationEventStatusType],  # (2)
    StatusMessage: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-brackets: OperationEventStatusType](./literals.md#operationeventstatustype) 
## GetDatabaseOutputTypeDef

```python
# GetDatabaseOutputTypeDef definition

class GetDatabaseOutputTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ComponentTypeDef

```python
# ComponentTypeDef definition

class ComponentTypeDef(TypedDict):
    ComponentId: NotRequired[str],
    Sid: NotRequired[str],
    SystemNumber: NotRequired[str],
    ParentComponent: NotRequired[str],
    ChildComponents: NotRequired[List[str]],
    ApplicationId: NotRequired[str],
    ComponentType: NotRequired[ComponentTypeType],  # (1)
    Status: NotRequired[ComponentStatusType],  # (2)
    SapHostname: NotRequired[str],
    SapFeature: NotRequired[str],
    SapKernelVersion: NotRequired[str],
    HdbVersion: NotRequired[str],
    Resilience: NotRequired[ResilienceTypeDef],  # (3)
    AssociatedHost: NotRequired[AssociatedHostTypeDef],  # (4)
    Databases: NotRequired[List[str]],
    Hosts: NotRequired[List[HostTypeDef]],  # (5)
    PrimaryHost: NotRequired[str],
    DatabaseConnection: NotRequired[DatabaseConnectionTypeDef],  # (6)
    LastUpdated: NotRequired[datetime],
    Arn: NotRequired[str],
```

1. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
2. See [:material-code-brackets: ComponentStatusType](./literals.md#componentstatustype) 
3. See [:material-code-braces: ResilienceTypeDef](./type_defs.md#resiliencetypedef) 
4. See [:material-code-braces: AssociatedHostTypeDef](./type_defs.md#associatedhosttypedef) 
5. See [:material-code-braces: HostTypeDef](./type_defs.md#hosttypedef) 
6. See [:material-code-braces: DatabaseConnectionTypeDef](./type_defs.md#databaseconnectiontypedef) 
## ListOperationEventsOutputTypeDef

```python
# ListOperationEventsOutputTypeDef definition

class ListOperationEventsOutputTypeDef(TypedDict):
    OperationEvents: List[OperationEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OperationEventTypeDef](./type_defs.md#operationeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComponentOutputTypeDef

```python
# GetComponentOutputTypeDef definition

class GetComponentOutputTypeDef(TypedDict):
    Component: ComponentTypeDef,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
