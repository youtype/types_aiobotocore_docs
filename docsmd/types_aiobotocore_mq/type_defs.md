# Type definitions

> [Index](../README.md) > [MQ](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#mq)
    type annotations stubs module [types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).



## ActionRequiredTypeDef

```python
# ActionRequiredTypeDef definition

class ActionRequiredTypeDef(TypedDict):
    ActionRequiredCode: NotRequired[str],
    ActionRequiredInfo: NotRequired[str],
```

## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## EngineVersionTypeDef

```python
# EngineVersionTypeDef definition

class EngineVersionTypeDef(TypedDict):
    Name: NotRequired[str],
```

## BrokerInstanceTypeDef

```python
# BrokerInstanceTypeDef definition

class BrokerInstanceTypeDef(TypedDict):
    ConsoleURL: NotRequired[str],
    Endpoints: NotRequired[List[str]],
    IpAddress: NotRequired[str],
```

## BrokerSummaryTypeDef

```python
# BrokerSummaryTypeDef definition

class BrokerSummaryTypeDef(TypedDict):
    DeploymentMode: DeploymentModeType,  # (2)
    EngineType: EngineTypeType,  # (3)
    BrokerArn: NotRequired[str],
    BrokerId: NotRequired[str],
    BrokerName: NotRequired[str],
    BrokerState: NotRequired[BrokerStateType],  # (1)
    Created: NotRequired[datetime],
    HostInstanceType: NotRequired[str],
```

1. See [:material-code-brackets: BrokerStateType](./literals.md#brokerstatetype) 
2. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
3. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
## ConfigurationIdTypeDef

```python
# ConfigurationIdTypeDef definition

class ConfigurationIdTypeDef(TypedDict):
    Id: str,
    Revision: NotRequired[int],
```

## ConfigurationRevisionTypeDef

```python
# ConfigurationRevisionTypeDef definition

class ConfigurationRevisionTypeDef(TypedDict):
    Created: datetime,
    Revision: int,
    Description: NotRequired[str],
```

## EncryptionOptionsTypeDef

```python
# EncryptionOptionsTypeDef definition

class EncryptionOptionsTypeDef(TypedDict):
    UseAwsOwnedKey: bool,
    KmsKeyId: NotRequired[str],
```

## LdapServerMetadataInputTypeDef

```python
# LdapServerMetadataInputTypeDef definition

class LdapServerMetadataInputTypeDef(TypedDict):
    Hosts: Sequence[str],
    RoleBase: str,
    RoleSearchMatching: str,
    ServiceAccountPassword: str,
    ServiceAccountUsername: str,
    UserBase: str,
    UserSearchMatching: str,
    RoleName: NotRequired[str],
    RoleSearchSubtree: NotRequired[bool],
    UserRoleName: NotRequired[str],
    UserSearchSubtree: NotRequired[bool],
```

## LogsTypeDef

```python
# LogsTypeDef definition

class LogsTypeDef(TypedDict):
    Audit: NotRequired[bool],
    General: NotRequired[bool],
```

## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Password: str,
    Username: str,
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[Sequence[str]],
    ReplicationUser: NotRequired[bool],
```

## WeeklyStartTimeTypeDef

```python
# WeeklyStartTimeTypeDef definition

class WeeklyStartTimeTypeDef(TypedDict):
    DayOfWeek: DayOfWeekType,  # (1)
    TimeOfDay: str,
    TimeZone: NotRequired[str],
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
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

## CreateConfigurationRequestRequestTypeDef

```python
# CreateConfigurationRequestRequestTypeDef definition

class CreateConfigurationRequestRequestTypeDef(TypedDict):
    EngineType: EngineTypeType,  # (1)
    Name: str,
    AuthenticationStrategy: NotRequired[AuthenticationStrategyType],  # (2)
    EngineVersion: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
## CreateTagsRequestRequestTypeDef

```python
# CreateTagsRequestRequestTypeDef definition

class CreateTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Password: str,
    Username: str,
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[Sequence[str]],
    ReplicationUser: NotRequired[bool],
```

## DataReplicationCounterpartTypeDef

```python
# DataReplicationCounterpartTypeDef definition

class DataReplicationCounterpartTypeDef(TypedDict):
    BrokerId: str,
    Region: str,
```

## DeleteBrokerRequestRequestTypeDef

```python
# DeleteBrokerRequestRequestTypeDef definition

class DeleteBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
```

## DeleteTagsRequestRequestTypeDef

```python
# DeleteTagsRequestRequestTypeDef definition

class DeleteTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Username: str,
```

## DescribeBrokerEngineTypesRequestRequestTypeDef

```python
# DescribeBrokerEngineTypesRequestRequestTypeDef definition

class DescribeBrokerEngineTypesRequestRequestTypeDef(TypedDict):
    EngineType: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeBrokerInstanceOptionsRequestRequestTypeDef

```python
# DescribeBrokerInstanceOptionsRequestRequestTypeDef definition

class DescribeBrokerInstanceOptionsRequestRequestTypeDef(TypedDict):
    EngineType: NotRequired[str],
    HostInstanceType: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StorageType: NotRequired[str],
```

## DescribeBrokerRequestRequestTypeDef

```python
# DescribeBrokerRequestRequestTypeDef definition

class DescribeBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
```

## LdapServerMetadataOutputTypeDef

```python
# LdapServerMetadataOutputTypeDef definition

class LdapServerMetadataOutputTypeDef(TypedDict):
    Hosts: List[str],
    RoleBase: str,
    RoleSearchMatching: str,
    ServiceAccountUsername: str,
    UserBase: str,
    UserSearchMatching: str,
    RoleName: NotRequired[str],
    RoleSearchSubtree: NotRequired[bool],
    UserRoleName: NotRequired[str],
    UserSearchSubtree: NotRequired[bool],
```

## UserSummaryTypeDef

```python
# UserSummaryTypeDef definition

class UserSummaryTypeDef(TypedDict):
    Username: str,
    PendingChange: NotRequired[ChangeTypeType],  # (1)
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## DescribeConfigurationRequestRequestTypeDef

```python
# DescribeConfigurationRequestRequestTypeDef definition

class DescribeConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
```

## DescribeConfigurationRevisionRequestRequestTypeDef

```python
# DescribeConfigurationRevisionRequestRequestTypeDef definition

class DescribeConfigurationRevisionRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
    ConfigurationRevision: str,
```

## DescribeUserRequestRequestTypeDef

```python
# DescribeUserRequestRequestTypeDef definition

class DescribeUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Username: str,
```

## UserPendingChangesTypeDef

```python
# UserPendingChangesTypeDef definition

class UserPendingChangesTypeDef(TypedDict):
    PendingChange: ChangeTypeType,  # (1)
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[List[str]],
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBrokersRequestRequestTypeDef

```python
# ListBrokersRequestRequestTypeDef definition

class ListBrokersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationRevisionsRequestRequestTypeDef

```python
# ListConfigurationRevisionsRequestRequestTypeDef definition

class ListConfigurationRevisionsRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationsRequestRequestTypeDef

```python
# ListConfigurationsRequestRequestTypeDef definition

class ListConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PendingLogsTypeDef

```python
# PendingLogsTypeDef definition

class PendingLogsTypeDef(TypedDict):
    Audit: NotRequired[bool],
    General: NotRequired[bool],
```

## PromoteRequestRequestTypeDef

```python
# PromoteRequestRequestTypeDef definition

class PromoteRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Mode: PromoteModeType,  # (1)
```

1. See [:material-code-brackets: PromoteModeType](./literals.md#promotemodetype) 
## RebootBrokerRequestRequestTypeDef

```python
# RebootBrokerRequestRequestTypeDef definition

class RebootBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
```

## SanitizationWarningTypeDef

```python
# SanitizationWarningTypeDef definition

class SanitizationWarningTypeDef(TypedDict):
    Reason: SanitizationWarningReasonType,  # (1)
    AttributeName: NotRequired[str],
    ElementName: NotRequired[str],
```

1. See [:material-code-brackets: SanitizationWarningReasonType](./literals.md#sanitizationwarningreasontype) 
## UpdateConfigurationRequestRequestTypeDef

```python
# UpdateConfigurationRequestRequestTypeDef definition

class UpdateConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
    Data: str,
    Description: NotRequired[str],
```

## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Username: str,
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[Sequence[str]],
    Password: NotRequired[str],
    ReplicationUser: NotRequired[bool],
```

## BrokerInstanceOptionTypeDef

```python
# BrokerInstanceOptionTypeDef definition

class BrokerInstanceOptionTypeDef(TypedDict):
    AvailabilityZones: NotRequired[List[AvailabilityZoneTypeDef]],  # (1)
    EngineType: NotRequired[EngineTypeType],  # (2)
    HostInstanceType: NotRequired[str],
    StorageType: NotRequired[BrokerStorageTypeType],  # (3)
    SupportedDeploymentModes: NotRequired[List[DeploymentModeType]],  # (4)
    SupportedEngineVersions: NotRequired[List[str]],
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-brackets: BrokerStorageTypeType](./literals.md#brokerstoragetypetype) 
4. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
## BrokerEngineTypeTypeDef

```python
# BrokerEngineTypeTypeDef definition

class BrokerEngineTypeTypeDef(TypedDict):
    EngineType: NotRequired[EngineTypeType],  # (1)
    EngineVersions: NotRequired[List[EngineVersionTypeDef]],  # (2)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
## ConfigurationsTypeDef

```python
# ConfigurationsTypeDef definition

class ConfigurationsTypeDef(TypedDict):
    Current: NotRequired[ConfigurationIdTypeDef],  # (1)
    History: NotRequired[List[ConfigurationIdTypeDef]],  # (2)
    Pending: NotRequired[ConfigurationIdTypeDef],  # (1)
```

1. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
2. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
3. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    Arn: str,
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    Created: datetime,
    Description: str,
    EngineType: EngineTypeType,  # (2)
    EngineVersion: str,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (3)
    Name: str,
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
## CreateBrokerRequestRequestTypeDef

```python
# CreateBrokerRequestRequestTypeDef definition

class CreateBrokerRequestRequestTypeDef(TypedDict):
    BrokerName: str,
    DeploymentMode: DeploymentModeType,  # (1)
    EngineType: EngineTypeType,  # (2)
    HostInstanceType: str,
    PubliclyAccessible: bool,
    Users: Sequence[UserTypeDef],  # (3)
    AuthenticationStrategy: NotRequired[AuthenticationStrategyType],  # (4)
    AutoMinorVersionUpgrade: NotRequired[bool],
    Configuration: NotRequired[ConfigurationIdTypeDef],  # (5)
    CreatorRequestId: NotRequired[str],
    EncryptionOptions: NotRequired[EncryptionOptionsTypeDef],  # (6)
    EngineVersion: NotRequired[str],
    LdapServerMetadata: NotRequired[LdapServerMetadataInputTypeDef],  # (7)
    Logs: NotRequired[LogsTypeDef],  # (8)
    MaintenanceWindowStartTime: NotRequired[WeeklyStartTimeTypeDef],  # (9)
    SecurityGroups: NotRequired[Sequence[str]],
    StorageType: NotRequired[BrokerStorageTypeType],  # (10)
    SubnetIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
    DataReplicationMode: NotRequired[DataReplicationModeType],  # (11)
    DataReplicationPrimaryBrokerArn: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
4. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
5. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
6. See [:material-code-braces: EncryptionOptionsTypeDef](./type_defs.md#encryptionoptionstypedef) 
7. See [:material-code-braces: LdapServerMetadataInputTypeDef](./type_defs.md#ldapservermetadatainputtypedef) 
8. See [:material-code-braces: LogsTypeDef](./type_defs.md#logstypedef) 
9. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
10. See [:material-code-brackets: BrokerStorageTypeType](./literals.md#brokerstoragetypetype) 
11. See [:material-code-brackets: DataReplicationModeType](./literals.md#datareplicationmodetype) 
## UpdateBrokerRequestRequestTypeDef

```python
# UpdateBrokerRequestRequestTypeDef definition

class UpdateBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    AuthenticationStrategy: NotRequired[AuthenticationStrategyType],  # (1)
    AutoMinorVersionUpgrade: NotRequired[bool],
    Configuration: NotRequired[ConfigurationIdTypeDef],  # (2)
    EngineVersion: NotRequired[str],
    HostInstanceType: NotRequired[str],
    LdapServerMetadata: NotRequired[LdapServerMetadataInputTypeDef],  # (3)
    Logs: NotRequired[LogsTypeDef],  # (4)
    MaintenanceWindowStartTime: NotRequired[WeeklyStartTimeTypeDef],  # (5)
    SecurityGroups: NotRequired[Sequence[str]],
    DataReplicationMode: NotRequired[DataReplicationModeType],  # (6)
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
3. See [:material-code-braces: LdapServerMetadataInputTypeDef](./type_defs.md#ldapservermetadatainputtypedef) 
4. See [:material-code-braces: LogsTypeDef](./type_defs.md#logstypedef) 
5. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
6. See [:material-code-brackets: DataReplicationModeType](./literals.md#datareplicationmodetype) 
## CreateBrokerResponseTypeDef

```python
# CreateBrokerResponseTypeDef definition

class CreateBrokerResponseTypeDef(TypedDict):
    BrokerArn: str,
    BrokerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfigurationResponseTypeDef

```python
# CreateConfigurationResponseTypeDef definition

class CreateConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    Created: datetime,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (2)
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBrokerResponseTypeDef

```python
# DeleteBrokerResponseTypeDef definition

class DeleteBrokerResponseTypeDef(TypedDict):
    BrokerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationResponseTypeDef

```python
# DescribeConfigurationResponseTypeDef definition

class DescribeConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    Created: datetime,
    Description: str,
    EngineType: EngineTypeType,  # (2)
    EngineVersion: str,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (3)
    Name: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationRevisionResponseTypeDef

```python
# DescribeConfigurationRevisionResponseTypeDef definition

class DescribeConfigurationRevisionResponseTypeDef(TypedDict):
    ConfigurationId: str,
    Created: datetime,
    Data: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBrokersResponseTypeDef

```python
# ListBrokersResponseTypeDef definition

class ListBrokersResponseTypeDef(TypedDict):
    BrokerSummaries: List[BrokerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BrokerSummaryTypeDef](./type_defs.md#brokersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationRevisionsResponseTypeDef

```python
# ListConfigurationRevisionsResponseTypeDef definition

class ListConfigurationRevisionsResponseTypeDef(TypedDict):
    ConfigurationId: str,
    MaxResults: int,
    Revisions: List[ConfigurationRevisionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromoteResponseTypeDef

```python
# PromoteResponseTypeDef definition

class PromoteResponseTypeDef(TypedDict):
    BrokerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataReplicationMetadataOutputTypeDef

```python
# DataReplicationMetadataOutputTypeDef definition

class DataReplicationMetadataOutputTypeDef(TypedDict):
    DataReplicationRole: str,
    DataReplicationCounterpart: NotRequired[DataReplicationCounterpartTypeDef],  # (1)
```

1. See [:material-code-braces: DataReplicationCounterpartTypeDef](./type_defs.md#datareplicationcounterparttypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    BrokerId: str,
    MaxResults: int,
    Users: List[UserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserSummaryTypeDef](./type_defs.md#usersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserResponseTypeDef

```python
# DescribeUserResponseTypeDef definition

class DescribeUserResponseTypeDef(TypedDict):
    BrokerId: str,
    ConsoleAccess: bool,
    Groups: List[str],
    Pending: UserPendingChangesTypeDef,  # (1)
    Username: str,
    ReplicationUser: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserPendingChangesTypeDef](./type_defs.md#userpendingchangestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBrokersRequestPaginateTypeDef

```python
# ListBrokersRequestPaginateTypeDef definition

class ListBrokersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LogsSummaryTypeDef

```python
# LogsSummaryTypeDef definition

class LogsSummaryTypeDef(TypedDict):
    General: bool,
    GeneralLogGroup: str,
    Audit: NotRequired[bool],
    AuditLogGroup: NotRequired[str],
    Pending: NotRequired[PendingLogsTypeDef],  # (1)
```

1. See [:material-code-braces: PendingLogsTypeDef](./type_defs.md#pendinglogstypedef) 
## UpdateConfigurationResponseTypeDef

```python
# UpdateConfigurationResponseTypeDef definition

class UpdateConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    Created: datetime,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (1)
    Name: str,
    Warnings: List[SanitizationWarningTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-braces: SanitizationWarningTypeDef](./type_defs.md#sanitizationwarningtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBrokerInstanceOptionsResponseTypeDef

```python
# DescribeBrokerInstanceOptionsResponseTypeDef definition

class DescribeBrokerInstanceOptionsResponseTypeDef(TypedDict):
    BrokerInstanceOptions: List[BrokerInstanceOptionTypeDef],  # (1)
    MaxResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BrokerInstanceOptionTypeDef](./type_defs.md#brokerinstanceoptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBrokerEngineTypesResponseTypeDef

```python
# DescribeBrokerEngineTypesResponseTypeDef definition

class DescribeBrokerEngineTypesResponseTypeDef(TypedDict):
    BrokerEngineTypes: List[BrokerEngineTypeTypeDef],  # (1)
    MaxResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BrokerEngineTypeTypeDef](./type_defs.md#brokerenginetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationsResponseTypeDef

```python
# ListConfigurationsResponseTypeDef definition

class ListConfigurationsResponseTypeDef(TypedDict):
    Configurations: List[ConfigurationTypeDef],  # (1)
    MaxResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerResponseTypeDef

```python
# UpdateBrokerResponseTypeDef definition

class UpdateBrokerResponseTypeDef(TypedDict):
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    AutoMinorVersionUpgrade: bool,
    BrokerId: str,
    Configuration: ConfigurationIdTypeDef,  # (2)
    EngineVersion: str,
    HostInstanceType: str,
    LdapServerMetadata: LdapServerMetadataOutputTypeDef,  # (3)
    Logs: LogsTypeDef,  # (4)
    MaintenanceWindowStartTime: WeeklyStartTimeTypeDef,  # (5)
    SecurityGroups: List[str],
    DataReplicationMetadata: DataReplicationMetadataOutputTypeDef,  # (6)
    DataReplicationMode: DataReplicationModeType,  # (7)
    PendingDataReplicationMetadata: DataReplicationMetadataOutputTypeDef,  # (6)
    PendingDataReplicationMode: DataReplicationModeType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
3. See [:material-code-braces: LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef) 
4. See [:material-code-braces: LogsTypeDef](./type_defs.md#logstypedef) 
5. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
6. See [:material-code-braces: DataReplicationMetadataOutputTypeDef](./type_defs.md#datareplicationmetadataoutputtypedef) 
7. See [:material-code-brackets: DataReplicationModeType](./literals.md#datareplicationmodetype) 
8. See [:material-code-braces: DataReplicationMetadataOutputTypeDef](./type_defs.md#datareplicationmetadataoutputtypedef) 
9. See [:material-code-brackets: DataReplicationModeType](./literals.md#datareplicationmodetype) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBrokerResponseTypeDef

```python
# DescribeBrokerResponseTypeDef definition

class DescribeBrokerResponseTypeDef(TypedDict):
    ActionsRequired: List[ActionRequiredTypeDef],  # (1)
    AuthenticationStrategy: AuthenticationStrategyType,  # (2)
    AutoMinorVersionUpgrade: bool,
    BrokerArn: str,
    BrokerId: str,
    BrokerInstances: List[BrokerInstanceTypeDef],  # (3)
    BrokerName: str,
    BrokerState: BrokerStateType,  # (4)
    Configurations: ConfigurationsTypeDef,  # (5)
    Created: datetime,
    DeploymentMode: DeploymentModeType,  # (6)
    EncryptionOptions: EncryptionOptionsTypeDef,  # (7)
    EngineType: EngineTypeType,  # (8)
    EngineVersion: str,
    HostInstanceType: str,
    LdapServerMetadata: LdapServerMetadataOutputTypeDef,  # (9)
    Logs: LogsSummaryTypeDef,  # (10)
    MaintenanceWindowStartTime: WeeklyStartTimeTypeDef,  # (11)
    PendingAuthenticationStrategy: AuthenticationStrategyType,  # (2)
    PendingEngineVersion: str,
    PendingHostInstanceType: str,
    PendingLdapServerMetadata: LdapServerMetadataOutputTypeDef,  # (9)
    PendingSecurityGroups: List[str],
    PubliclyAccessible: bool,
    SecurityGroups: List[str],
    StorageType: BrokerStorageTypeType,  # (14)
    SubnetIds: List[str],
    Tags: Dict[str, str],
    Users: List[UserSummaryTypeDef],  # (15)
    DataReplicationMetadata: DataReplicationMetadataOutputTypeDef,  # (16)
    DataReplicationMode: DataReplicationModeType,  # (17)
    PendingDataReplicationMetadata: DataReplicationMetadataOutputTypeDef,  # (16)
    PendingDataReplicationMode: DataReplicationModeType,  # (17)
    ResponseMetadata: ResponseMetadataTypeDef,  # (20)
```

1. See [:material-code-braces: ActionRequiredTypeDef](./type_defs.md#actionrequiredtypedef) 
2. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
3. See [:material-code-braces: BrokerInstanceTypeDef](./type_defs.md#brokerinstancetypedef) 
4. See [:material-code-brackets: BrokerStateType](./literals.md#brokerstatetype) 
5. See [:material-code-braces: ConfigurationsTypeDef](./type_defs.md#configurationstypedef) 
6. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
7. See [:material-code-braces: EncryptionOptionsTypeDef](./type_defs.md#encryptionoptionstypedef) 
8. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
9. See [:material-code-braces: LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef) 
10. See [:material-code-braces: LogsSummaryTypeDef](./type_defs.md#logssummarytypedef) 
11. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
12. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
13. See [:material-code-braces: LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef) 
14. See [:material-code-brackets: BrokerStorageTypeType](./literals.md#brokerstoragetypetype) 
15. See [:material-code-braces: UserSummaryTypeDef](./type_defs.md#usersummarytypedef) 
16. See [:material-code-braces: DataReplicationMetadataOutputTypeDef](./type_defs.md#datareplicationmetadataoutputtypedef) 
17. See [:material-code-brackets: DataReplicationModeType](./literals.md#datareplicationmodetype) 
18. See [:material-code-braces: DataReplicationMetadataOutputTypeDef](./type_defs.md#datareplicationmetadataoutputtypedef) 
19. See [:material-code-brackets: DataReplicationModeType](./literals.md#datareplicationmodetype) 
20. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
