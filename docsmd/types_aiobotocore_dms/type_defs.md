# Type definitions

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#databasemigrationservice)
    type annotations stubs module [types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SourceDataSettingUnionTypeDef

```python
# SourceDataSettingUnionTypeDef definition

SourceDataSettingUnionTypeDef = Union[
    SourceDataSettingTypeDef,  # (1)
    SourceDataSettingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SourceDataSettingTypeDef](./type_defs.md#sourcedatasettingtypedef) 
2. See [:material-code-braces: SourceDataSettingOutputTypeDef](./type_defs.md#sourcedatasettingoutputtypedef) 



## AccountQuotaTypeDef

```python
# AccountQuotaTypeDef definition

class AccountQuotaTypeDef(TypedDict):
    AccountQuotaName: NotRequired[str],
    Used: NotRequired[int],
    Max: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    ResourceArn: NotRequired[str],
```

## ApplyPendingMaintenanceActionMessageRequestTypeDef

```python
# ApplyPendingMaintenanceActionMessageRequestTypeDef definition

class ApplyPendingMaintenanceActionMessageRequestTypeDef(TypedDict):
    ReplicationInstanceArn: str,
    ApplyAction: str,
    OptInType: str,
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

## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## BatchStartRecommendationsErrorEntryTypeDef

```python
# BatchStartRecommendationsErrorEntryTypeDef definition

class BatchStartRecommendationsErrorEntryTypeDef(TypedDict):
    DatabaseId: NotRequired[str],
    Message: NotRequired[str],
    Code: NotRequired[str],
```

## CancelReplicationTaskAssessmentRunMessageRequestTypeDef

```python
# CancelReplicationTaskAssessmentRunMessageRequestTypeDef definition

class CancelReplicationTaskAssessmentRunMessageRequestTypeDef(TypedDict):
    ReplicationTaskAssessmentRunArn: str,
```

## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    CertificateIdentifier: NotRequired[str],
    CertificateCreationDate: NotRequired[datetime],
    CertificatePem: NotRequired[str],
    CertificateWallet: NotRequired[bytes],
    CertificateArn: NotRequired[str],
    CertificateOwner: NotRequired[str],
    ValidFromDate: NotRequired[datetime],
    ValidToDate: NotRequired[datetime],
    SigningAlgorithm: NotRequired[str],
    KeyLength: NotRequired[int],
```

## CollectorHealthCheckTypeDef

```python
# CollectorHealthCheckTypeDef definition

class CollectorHealthCheckTypeDef(TypedDict):
    CollectorStatus: NotRequired[CollectorStatusType],  # (1)
    LocalCollectorS3Access: NotRequired[bool],
    WebCollectorS3Access: NotRequired[bool],
    WebCollectorGrantedRoleBasedAccess: NotRequired[bool],
```

1. See [:material-code-brackets: CollectorStatusType](./literals.md#collectorstatustype) 
## InventoryDataTypeDef

```python
# InventoryDataTypeDef definition

class InventoryDataTypeDef(TypedDict):
    NumberOfDatabases: NotRequired[int],
    NumberOfSchemas: NotRequired[int],
```

## CollectorShortInfoResponseTypeDef

```python
# CollectorShortInfoResponseTypeDef definition

class CollectorShortInfoResponseTypeDef(TypedDict):
    CollectorReferencedId: NotRequired[str],
    CollectorName: NotRequired[str],
```

## ComputeConfigOutputTypeDef

```python
# ComputeConfigOutputTypeDef definition

class ComputeConfigOutputTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    DnsNameServers: NotRequired[str],
    KmsKeyId: NotRequired[str],
    MaxCapacityUnits: NotRequired[int],
    MinCapacityUnits: NotRequired[int],
    MultiAZ: NotRequired[bool],
    PreferredMaintenanceWindow: NotRequired[str],
    ReplicationSubnetGroupId: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[List[str]],
```

## ComputeConfigTypeDef

```python
# ComputeConfigTypeDef definition

class ComputeConfigTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    DnsNameServers: NotRequired[str],
    KmsKeyId: NotRequired[str],
    MaxCapacityUnits: NotRequired[int],
    MinCapacityUnits: NotRequired[int],
    MultiAZ: NotRequired[bool],
    PreferredMaintenanceWindow: NotRequired[str],
    ReplicationSubnetGroupId: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## ConnectionTypeDef

```python
# ConnectionTypeDef definition

class ConnectionTypeDef(TypedDict):
    ReplicationInstanceArn: NotRequired[str],
    EndpointArn: NotRequired[str],
    Status: NotRequired[str],
    LastFailureMessage: NotRequired[str],
    EndpointIdentifier: NotRequired[str],
    ReplicationInstanceIdentifier: NotRequired[str],
```

## DmsTransferSettingsTypeDef

```python
# DmsTransferSettingsTypeDef definition

class DmsTransferSettingsTypeDef(TypedDict):
    ServiceAccessRoleArn: NotRequired[str],
    BucketName: NotRequired[str],
```

## DocDbSettingsTypeDef

```python
# DocDbSettingsTypeDef definition

class DocDbSettingsTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    NestingLevel: NotRequired[NestingLevelValueType],  # (1)
    ExtractDocId: NotRequired[bool],
    DocsToInvestigate: NotRequired[int],
    KmsKeyId: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    UseUpdateLookUp: NotRequired[bool],
    ReplicateShardCollections: NotRequired[bool],
```

1. See [:material-code-brackets: NestingLevelValueType](./literals.md#nestinglevelvaluetype) 
## DynamoDbSettingsTypeDef

```python
# DynamoDbSettingsTypeDef definition

class DynamoDbSettingsTypeDef(TypedDict):
    ServiceAccessRoleArn: str,
```

## ElasticsearchSettingsTypeDef

```python
# ElasticsearchSettingsTypeDef definition

class ElasticsearchSettingsTypeDef(TypedDict):
    ServiceAccessRoleArn: str,
    EndpointUri: str,
    FullLoadErrorPercentage: NotRequired[int],
    ErrorRetryDuration: NotRequired[int],
    UseNewMappingType: NotRequired[bool],
```

## GcpMySQLSettingsTypeDef

```python
# GcpMySQLSettingsTypeDef definition

class GcpMySQLSettingsTypeDef(TypedDict):
    AfterConnectScript: NotRequired[str],
    CleanSourceMetadataOnMismatch: NotRequired[bool],
    DatabaseName: NotRequired[str],
    EventsPollInterval: NotRequired[int],
    TargetDbType: NotRequired[TargetDbTypeType],  # (1)
    MaxFileSize: NotRequired[int],
    ParallelLoadThreads: NotRequired[int],
    Password: NotRequired[str],
    Port: NotRequired[int],
    ServerName: NotRequired[str],
    ServerTimezone: NotRequired[str],
    Username: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
```

1. See [:material-code-brackets: TargetDbTypeType](./literals.md#targetdbtypetype) 
## IBMDb2SettingsTypeDef

```python
# IBMDb2SettingsTypeDef definition

class IBMDb2SettingsTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    Password: NotRequired[str],
    Port: NotRequired[int],
    ServerName: NotRequired[str],
    SetDataCaptureChanges: NotRequired[bool],
    CurrentLsn: NotRequired[str],
    MaxKBytesPerRead: NotRequired[int],
    Username: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    LoadTimeout: NotRequired[int],
    WriteBufferSize: NotRequired[int],
    MaxFileSize: NotRequired[int],
    KeepCsvFiles: NotRequired[bool],
```

## KafkaSettingsTypeDef

```python
# KafkaSettingsTypeDef definition

class KafkaSettingsTypeDef(TypedDict):
    Broker: NotRequired[str],
    Topic: NotRequired[str],
    MessageFormat: NotRequired[MessageFormatValueType],  # (1)
    IncludeTransactionDetails: NotRequired[bool],
    IncludePartitionValue: NotRequired[bool],
    PartitionIncludeSchemaTable: NotRequired[bool],
    IncludeTableAlterOperations: NotRequired[bool],
    IncludeControlDetails: NotRequired[bool],
    MessageMaxBytes: NotRequired[int],
    IncludeNullAndEmpty: NotRequired[bool],
    SecurityProtocol: NotRequired[KafkaSecurityProtocolType],  # (2)
    SslClientCertificateArn: NotRequired[str],
    SslClientKeyArn: NotRequired[str],
    SslClientKeyPassword: NotRequired[str],
    SslCaCertificateArn: NotRequired[str],
    SaslUsername: NotRequired[str],
    SaslPassword: NotRequired[str],
    NoHexPrefix: NotRequired[bool],
    SaslMechanism: NotRequired[KafkaSaslMechanismType],  # (3)
    SslEndpointIdentificationAlgorithm: NotRequired[KafkaSslEndpointIdentificationAlgorithmType],  # (4)
    UseLargeIntegerValue: NotRequired[bool],
```

1. See [:material-code-brackets: MessageFormatValueType](./literals.md#messageformatvaluetype) 
2. See [:material-code-brackets: KafkaSecurityProtocolType](./literals.md#kafkasecurityprotocoltype) 
3. See [:material-code-brackets: KafkaSaslMechanismType](./literals.md#kafkasaslmechanismtype) 
4. See [:material-code-brackets: KafkaSslEndpointIdentificationAlgorithmType](./literals.md#kafkasslendpointidentificationalgorithmtype) 
## KinesisSettingsTypeDef

```python
# KinesisSettingsTypeDef definition

class KinesisSettingsTypeDef(TypedDict):
    StreamArn: NotRequired[str],
    MessageFormat: NotRequired[MessageFormatValueType],  # (1)
    ServiceAccessRoleArn: NotRequired[str],
    IncludeTransactionDetails: NotRequired[bool],
    IncludePartitionValue: NotRequired[bool],
    PartitionIncludeSchemaTable: NotRequired[bool],
    IncludeTableAlterOperations: NotRequired[bool],
    IncludeControlDetails: NotRequired[bool],
    IncludeNullAndEmpty: NotRequired[bool],
    NoHexPrefix: NotRequired[bool],
    UseLargeIntegerValue: NotRequired[bool],
```

1. See [:material-code-brackets: MessageFormatValueType](./literals.md#messageformatvaluetype) 
## MicrosoftSQLServerSettingsTypeDef

```python
# MicrosoftSQLServerSettingsTypeDef definition

class MicrosoftSQLServerSettingsTypeDef(TypedDict):
    Port: NotRequired[int],
    BcpPacketSize: NotRequired[int],
    DatabaseName: NotRequired[str],
    ControlTablesFileGroup: NotRequired[str],
    Password: NotRequired[str],
    QuerySingleAlwaysOnNode: NotRequired[bool],
    ReadBackupOnly: NotRequired[bool],
    SafeguardPolicy: NotRequired[SafeguardPolicyType],  # (1)
    ServerName: NotRequired[str],
    Username: NotRequired[str],
    UseBcpFullLoad: NotRequired[bool],
    UseThirdPartyBackupDevice: NotRequired[bool],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    TrimSpaceInChar: NotRequired[bool],
    TlogAccessMode: NotRequired[TlogAccessModeType],  # (2)
    ForceLobLookup: NotRequired[bool],
    AuthenticationMethod: NotRequired[SqlServerAuthenticationMethodType],  # (3)
```

1. See [:material-code-brackets: SafeguardPolicyType](./literals.md#safeguardpolicytype) 
2. See [:material-code-brackets: TlogAccessModeType](./literals.md#tlogaccessmodetype) 
3. See [:material-code-brackets: SqlServerAuthenticationMethodType](./literals.md#sqlserverauthenticationmethodtype) 
## MongoDbSettingsTypeDef

```python
# MongoDbSettingsTypeDef definition

class MongoDbSettingsTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    AuthType: NotRequired[AuthTypeValueType],  # (1)
    AuthMechanism: NotRequired[AuthMechanismValueType],  # (2)
    NestingLevel: NotRequired[NestingLevelValueType],  # (3)
    ExtractDocId: NotRequired[str],
    DocsToInvestigate: NotRequired[str],
    AuthSource: NotRequired[str],
    KmsKeyId: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    UseUpdateLookUp: NotRequired[bool],
    ReplicateShardCollections: NotRequired[bool],
```

1. See [:material-code-brackets: AuthTypeValueType](./literals.md#authtypevaluetype) 
2. See [:material-code-brackets: AuthMechanismValueType](./literals.md#authmechanismvaluetype) 
3. See [:material-code-brackets: NestingLevelValueType](./literals.md#nestinglevelvaluetype) 
## MySQLSettingsTypeDef

```python
# MySQLSettingsTypeDef definition

class MySQLSettingsTypeDef(TypedDict):
    AfterConnectScript: NotRequired[str],
    CleanSourceMetadataOnMismatch: NotRequired[bool],
    DatabaseName: NotRequired[str],
    EventsPollInterval: NotRequired[int],
    TargetDbType: NotRequired[TargetDbTypeType],  # (1)
    MaxFileSize: NotRequired[int],
    ParallelLoadThreads: NotRequired[int],
    Password: NotRequired[str],
    Port: NotRequired[int],
    ServerName: NotRequired[str],
    ServerTimezone: NotRequired[str],
    Username: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    ExecuteTimeout: NotRequired[int],
```

1. See [:material-code-brackets: TargetDbTypeType](./literals.md#targetdbtypetype) 
## NeptuneSettingsTypeDef

```python
# NeptuneSettingsTypeDef definition

class NeptuneSettingsTypeDef(TypedDict):
    S3BucketName: str,
    S3BucketFolder: str,
    ServiceAccessRoleArn: NotRequired[str],
    ErrorRetryDuration: NotRequired[int],
    MaxFileSize: NotRequired[int],
    MaxRetryCount: NotRequired[int],
    IamAuthEnabled: NotRequired[bool],
```

## OracleSettingsTypeDef

```python
# OracleSettingsTypeDef definition

class OracleSettingsTypeDef(TypedDict):
    AddSupplementalLogging: NotRequired[bool],
    ArchivedLogDestId: NotRequired[int],
    AdditionalArchivedLogDestId: NotRequired[int],
    ExtraArchivedLogDestIds: NotRequired[Sequence[int]],
    AllowSelectNestedTables: NotRequired[bool],
    ParallelAsmReadThreads: NotRequired[int],
    ReadAheadBlocks: NotRequired[int],
    AccessAlternateDirectly: NotRequired[bool],
    UseAlternateFolderForOnline: NotRequired[bool],
    OraclePathPrefix: NotRequired[str],
    UsePathPrefix: NotRequired[str],
    ReplacePathPrefix: NotRequired[bool],
    EnableHomogenousTablespace: NotRequired[bool],
    DirectPathNoLog: NotRequired[bool],
    ArchivedLogsOnly: NotRequired[bool],
    AsmPassword: NotRequired[str],
    AsmServer: NotRequired[str],
    AsmUser: NotRequired[str],
    CharLengthSemantics: NotRequired[CharLengthSemanticsType],  # (1)
    DatabaseName: NotRequired[str],
    DirectPathParallelLoad: NotRequired[bool],
    FailTasksOnLobTruncation: NotRequired[bool],
    NumberDatatypeScale: NotRequired[int],
    Password: NotRequired[str],
    Port: NotRequired[int],
    ReadTableSpaceName: NotRequired[bool],
    RetryInterval: NotRequired[int],
    SecurityDbEncryption: NotRequired[str],
    SecurityDbEncryptionName: NotRequired[str],
    ServerName: NotRequired[str],
    SpatialDataOptionToGeoJsonFunctionName: NotRequired[str],
    StandbyDelayTime: NotRequired[int],
    Username: NotRequired[str],
    UseBFile: NotRequired[bool],
    UseDirectPathFullLoad: NotRequired[bool],
    UseLogminerReader: NotRequired[bool],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    SecretsManagerOracleAsmAccessRoleArn: NotRequired[str],
    SecretsManagerOracleAsmSecretId: NotRequired[str],
    TrimSpaceInChar: NotRequired[bool],
    ConvertTimestampWithZoneToUTC: NotRequired[bool],
    OpenTransactionWindow: NotRequired[int],
    AuthenticationMethod: NotRequired[OracleAuthenticationMethodType],  # (2)
```

1. See [:material-code-brackets: CharLengthSemanticsType](./literals.md#charlengthsemanticstype) 
2. See [:material-code-brackets: OracleAuthenticationMethodType](./literals.md#oracleauthenticationmethodtype) 
## PostgreSQLSettingsTypeDef

```python
# PostgreSQLSettingsTypeDef definition

class PostgreSQLSettingsTypeDef(TypedDict):
    AfterConnectScript: NotRequired[str],
    CaptureDdls: NotRequired[bool],
    MaxFileSize: NotRequired[int],
    DatabaseName: NotRequired[str],
    DdlArtifactsSchema: NotRequired[str],
    ExecuteTimeout: NotRequired[int],
    FailTasksOnLobTruncation: NotRequired[bool],
    HeartbeatEnable: NotRequired[bool],
    HeartbeatSchema: NotRequired[str],
    HeartbeatFrequency: NotRequired[int],
    Password: NotRequired[str],
    Port: NotRequired[int],
    ServerName: NotRequired[str],
    Username: NotRequired[str],
    SlotName: NotRequired[str],
    PluginName: NotRequired[PluginNameValueType],  # (1)
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    TrimSpaceInChar: NotRequired[bool],
    MapBooleanAsBoolean: NotRequired[bool],
    MapJsonbAsClob: NotRequired[bool],
    MapLongVarcharAs: NotRequired[LongVarcharMappingTypeType],  # (2)
    DatabaseMode: NotRequired[DatabaseModeType],  # (3)
    BabelfishDatabaseName: NotRequired[str],
    DisableUnicodeSourceFilter: NotRequired[bool],
```

1. See [:material-code-brackets: PluginNameValueType](./literals.md#pluginnamevaluetype) 
2. See [:material-code-brackets: LongVarcharMappingTypeType](./literals.md#longvarcharmappingtypetype) 
3. See [:material-code-brackets: DatabaseModeType](./literals.md#databasemodetype) 
## RedisSettingsTypeDef

```python
# RedisSettingsTypeDef definition

class RedisSettingsTypeDef(TypedDict):
    ServerName: str,
    Port: int,
    SslSecurityProtocol: NotRequired[SslSecurityProtocolValueType],  # (1)
    AuthType: NotRequired[RedisAuthTypeValueType],  # (2)
    AuthUserName: NotRequired[str],
    AuthPassword: NotRequired[str],
    SslCaCertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: SslSecurityProtocolValueType](./literals.md#sslsecurityprotocolvaluetype) 
2. See [:material-code-brackets: RedisAuthTypeValueType](./literals.md#redisauthtypevaluetype) 
## RedshiftSettingsTypeDef

```python
# RedshiftSettingsTypeDef definition

class RedshiftSettingsTypeDef(TypedDict):
    AcceptAnyDate: NotRequired[bool],
    AfterConnectScript: NotRequired[str],
    BucketFolder: NotRequired[str],
    BucketName: NotRequired[str],
    CaseSensitiveNames: NotRequired[bool],
    CompUpdate: NotRequired[bool],
    ConnectionTimeout: NotRequired[int],
    DatabaseName: NotRequired[str],
    DateFormat: NotRequired[str],
    EmptyAsNull: NotRequired[bool],
    EncryptionMode: NotRequired[EncryptionModeValueType],  # (1)
    ExplicitIds: NotRequired[bool],
    FileTransferUploadStreams: NotRequired[int],
    LoadTimeout: NotRequired[int],
    MaxFileSize: NotRequired[int],
    Password: NotRequired[str],
    Port: NotRequired[int],
    RemoveQuotes: NotRequired[bool],
    ReplaceInvalidChars: NotRequired[str],
    ReplaceChars: NotRequired[str],
    ServerName: NotRequired[str],
    ServiceAccessRoleArn: NotRequired[str],
    ServerSideEncryptionKmsKeyId: NotRequired[str],
    TimeFormat: NotRequired[str],
    TrimBlanks: NotRequired[bool],
    TruncateColumns: NotRequired[bool],
    Username: NotRequired[str],
    WriteBufferSize: NotRequired[int],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    MapBooleanAsBoolean: NotRequired[bool],
```

1. See [:material-code-brackets: EncryptionModeValueType](./literals.md#encryptionmodevaluetype) 
## S3SettingsTypeDef

```python
# S3SettingsTypeDef definition

class S3SettingsTypeDef(TypedDict):
    ServiceAccessRoleArn: NotRequired[str],
    ExternalTableDefinition: NotRequired[str],
    CsvRowDelimiter: NotRequired[str],
    CsvDelimiter: NotRequired[str],
    BucketFolder: NotRequired[str],
    BucketName: NotRequired[str],
    CompressionType: NotRequired[CompressionTypeValueType],  # (1)
    EncryptionMode: NotRequired[EncryptionModeValueType],  # (2)
    ServerSideEncryptionKmsKeyId: NotRequired[str],
    DataFormat: NotRequired[DataFormatValueType],  # (3)
    EncodingType: NotRequired[EncodingTypeValueType],  # (4)
    DictPageSizeLimit: NotRequired[int],
    RowGroupLength: NotRequired[int],
    DataPageSize: NotRequired[int],
    ParquetVersion: NotRequired[ParquetVersionValueType],  # (5)
    EnableStatistics: NotRequired[bool],
    IncludeOpForFullLoad: NotRequired[bool],
    CdcInsertsOnly: NotRequired[bool],
    TimestampColumnName: NotRequired[str],
    ParquetTimestampInMillisecond: NotRequired[bool],
    CdcInsertsAndUpdates: NotRequired[bool],
    DatePartitionEnabled: NotRequired[bool],
    DatePartitionSequence: NotRequired[DatePartitionSequenceValueType],  # (6)
    DatePartitionDelimiter: NotRequired[DatePartitionDelimiterValueType],  # (7)
    UseCsvNoSupValue: NotRequired[bool],
    CsvNoSupValue: NotRequired[str],
    PreserveTransactions: NotRequired[bool],
    CdcPath: NotRequired[str],
    UseTaskStartTimeForFullLoadTimestamp: NotRequired[bool],
    CannedAclForObjects: NotRequired[CannedAclForObjectsValueType],  # (8)
    AddColumnName: NotRequired[bool],
    CdcMaxBatchInterval: NotRequired[int],
    CdcMinFileSize: NotRequired[int],
    CsvNullValue: NotRequired[str],
    IgnoreHeaderRows: NotRequired[int],
    MaxFileSize: NotRequired[int],
    Rfc4180: NotRequired[bool],
    DatePartitionTimezone: NotRequired[str],
    AddTrailingPaddingCharacter: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
    GlueCatalogGeneration: NotRequired[bool],
```

1. See [:material-code-brackets: CompressionTypeValueType](./literals.md#compressiontypevaluetype) 
2. See [:material-code-brackets: EncryptionModeValueType](./literals.md#encryptionmodevaluetype) 
3. See [:material-code-brackets: DataFormatValueType](./literals.md#dataformatvaluetype) 
4. See [:material-code-brackets: EncodingTypeValueType](./literals.md#encodingtypevaluetype) 
5. See [:material-code-brackets: ParquetVersionValueType](./literals.md#parquetversionvaluetype) 
6. See [:material-code-brackets: DatePartitionSequenceValueType](./literals.md#datepartitionsequencevaluetype) 
7. See [:material-code-brackets: DatePartitionDelimiterValueType](./literals.md#datepartitiondelimitervaluetype) 
8. See [:material-code-brackets: CannedAclForObjectsValueType](./literals.md#cannedaclforobjectsvaluetype) 
## SybaseSettingsTypeDef

```python
# SybaseSettingsTypeDef definition

class SybaseSettingsTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    Password: NotRequired[str],
    Port: NotRequired[int],
    ServerName: NotRequired[str],
    Username: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
```

## TimestreamSettingsTypeDef

```python
# TimestreamSettingsTypeDef definition

class TimestreamSettingsTypeDef(TypedDict):
    DatabaseName: str,
    MemoryDuration: int,
    MagneticDuration: int,
    CdcInsertsAndUpdates: NotRequired[bool],
    EnableMagneticStoreWrites: NotRequired[bool],
```

## EventSubscriptionTypeDef

```python
# EventSubscriptionTypeDef definition

class EventSubscriptionTypeDef(TypedDict):
    CustomerAwsId: NotRequired[str],
    CustSubscriptionId: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    Status: NotRequired[str],
    SubscriptionCreationTime: NotRequired[str],
    SourceType: NotRequired[str],
    SourceIdsList: NotRequired[List[str]],
    EventCategoriesList: NotRequired[List[str]],
    Enabled: NotRequired[bool],
```

## CreateFleetAdvisorCollectorRequestRequestTypeDef

```python
# CreateFleetAdvisorCollectorRequestRequestTypeDef definition

class CreateFleetAdvisorCollectorRequestRequestTypeDef(TypedDict):
    CollectorName: str,
    ServiceAccessRoleArn: str,
    S3BucketName: str,
    Description: NotRequired[str],
```

## InstanceProfileTypeDef

```python
# InstanceProfileTypeDef definition

class InstanceProfileTypeDef(TypedDict):
    InstanceProfileArn: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    NetworkType: NotRequired[str],
    InstanceProfileName: NotRequired[str],
    Description: NotRequired[str],
    InstanceProfileCreationTime: NotRequired[datetime],
    SubnetGroupIdentifier: NotRequired[str],
    VpcSecurityGroups: NotRequired[List[str]],
```

## DataProviderDescriptorDefinitionTypeDef

```python
# DataProviderDescriptorDefinitionTypeDef definition

class DataProviderDescriptorDefinitionTypeDef(TypedDict):
    DataProviderIdentifier: str,
    SecretsManagerSecretId: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
```

## SCApplicationAttributesTypeDef

```python
# SCApplicationAttributesTypeDef definition

class SCApplicationAttributesTypeDef(TypedDict):
    S3BucketPath: NotRequired[str],
    S3BucketRoleArn: NotRequired[str],
```

## KerberosAuthenticationSettingsTypeDef

```python
# KerberosAuthenticationSettingsTypeDef definition

class KerberosAuthenticationSettingsTypeDef(TypedDict):
    KeyCacheSecretId: NotRequired[str],
    KeyCacheSecretIamArn: NotRequired[str],
    Krb5FileContents: NotRequired[str],
```

## DataMigrationSettingsTypeDef

```python
# DataMigrationSettingsTypeDef definition

class DataMigrationSettingsTypeDef(TypedDict):
    NumberOfJobs: NotRequired[int],
    CloudwatchLogsEnabled: NotRequired[bool],
    SelectionRules: NotRequired[str],
```

## DataMigrationStatisticsTypeDef

```python
# DataMigrationStatisticsTypeDef definition

class DataMigrationStatisticsTypeDef(TypedDict):
    TablesLoaded: NotRequired[int],
    ElapsedTimeMillis: NotRequired[int],
    TablesLoading: NotRequired[int],
    FullLoadPercentage: NotRequired[int],
    CDCLatency: NotRequired[int],
    TablesQueued: NotRequired[int],
    TablesErrored: NotRequired[int],
    StartTime: NotRequired[datetime],
    StopTime: NotRequired[datetime],
```

## SourceDataSettingOutputTypeDef

```python
# SourceDataSettingOutputTypeDef definition

class SourceDataSettingOutputTypeDef(TypedDict):
    CDCStartPosition: NotRequired[str],
    CDCStartTime: NotRequired[datetime],
    CDCStopTime: NotRequired[datetime],
    SlotName: NotRequired[str],
```

## DataProviderDescriptorTypeDef

```python
# DataProviderDescriptorTypeDef definition

class DataProviderDescriptorTypeDef(TypedDict):
    SecretsManagerSecretId: NotRequired[str],
    SecretsManagerAccessRoleArn: NotRequired[str],
    DataProviderName: NotRequired[str],
    DataProviderArn: NotRequired[str],
```

## DocDbDataProviderSettingsTypeDef

```python
# DocDbDataProviderSettingsTypeDef definition

class DocDbDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (1)
    CertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
## MariaDbDataProviderSettingsTypeDef

```python
# MariaDbDataProviderSettingsTypeDef definition

class MariaDbDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    SslMode: NotRequired[DmsSslModeValueType],  # (1)
    CertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
## MicrosoftSqlServerDataProviderSettingsTypeDef

```python
# MicrosoftSqlServerDataProviderSettingsTypeDef definition

class MicrosoftSqlServerDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (1)
    CertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
## MongoDbDataProviderSettingsTypeDef

```python
# MongoDbDataProviderSettingsTypeDef definition

class MongoDbDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (1)
    CertificateArn: NotRequired[str],
    AuthType: NotRequired[AuthTypeValueType],  # (2)
    AuthSource: NotRequired[str],
    AuthMechanism: NotRequired[AuthMechanismValueType],  # (3)
```

1. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
2. See [:material-code-brackets: AuthTypeValueType](./literals.md#authtypevaluetype) 
3. See [:material-code-brackets: AuthMechanismValueType](./literals.md#authmechanismvaluetype) 
## MySqlDataProviderSettingsTypeDef

```python
# MySqlDataProviderSettingsTypeDef definition

class MySqlDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    SslMode: NotRequired[DmsSslModeValueType],  # (1)
    CertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
## OracleDataProviderSettingsTypeDef

```python
# OracleDataProviderSettingsTypeDef definition

class OracleDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (1)
    CertificateArn: NotRequired[str],
    AsmServer: NotRequired[str],
    SecretsManagerOracleAsmSecretId: NotRequired[str],
    SecretsManagerOracleAsmAccessRoleArn: NotRequired[str],
    SecretsManagerSecurityDbEncryptionSecretId: NotRequired[str],
    SecretsManagerSecurityDbEncryptionAccessRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
## PostgreSqlDataProviderSettingsTypeDef

```python
# PostgreSqlDataProviderSettingsTypeDef definition

class PostgreSqlDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (1)
    CertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
## RedshiftDataProviderSettingsTypeDef

```python
# RedshiftDataProviderSettingsTypeDef definition

class RedshiftDataProviderSettingsTypeDef(TypedDict):
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
```

## DatabaseInstanceSoftwareDetailsResponseTypeDef

```python
# DatabaseInstanceSoftwareDetailsResponseTypeDef definition

class DatabaseInstanceSoftwareDetailsResponseTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    EngineEdition: NotRequired[str],
    ServicePack: NotRequired[str],
    SupportLevel: NotRequired[str],
    OsArchitecture: NotRequired[int],
    Tooltip: NotRequired[str],
```

## ServerShortInfoResponseTypeDef

```python
# ServerShortInfoResponseTypeDef definition

class ServerShortInfoResponseTypeDef(TypedDict):
    ServerId: NotRequired[str],
    IpAddress: NotRequired[str],
    ServerName: NotRequired[str],
```

## DatabaseShortInfoResponseTypeDef

```python
# DatabaseShortInfoResponseTypeDef definition

class DatabaseShortInfoResponseTypeDef(TypedDict):
    DatabaseId: NotRequired[str],
    DatabaseName: NotRequired[str],
    DatabaseIpAddress: NotRequired[str],
    DatabaseEngine: NotRequired[str],
```

## DefaultErrorDetailsTypeDef

```python
# DefaultErrorDetailsTypeDef definition

class DefaultErrorDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
```

## DeleteCertificateMessageRequestTypeDef

```python
# DeleteCertificateMessageRequestTypeDef definition

class DeleteCertificateMessageRequestTypeDef(TypedDict):
    CertificateArn: str,
```

## DeleteCollectorRequestRequestTypeDef

```python
# DeleteCollectorRequestRequestTypeDef definition

class DeleteCollectorRequestRequestTypeDef(TypedDict):
    CollectorReferencedId: str,
```

## DeleteConnectionMessageRequestTypeDef

```python
# DeleteConnectionMessageRequestTypeDef definition

class DeleteConnectionMessageRequestTypeDef(TypedDict):
    EndpointArn: str,
    ReplicationInstanceArn: str,
```

## DeleteDataMigrationMessageRequestTypeDef

```python
# DeleteDataMigrationMessageRequestTypeDef definition

class DeleteDataMigrationMessageRequestTypeDef(TypedDict):
    DataMigrationIdentifier: str,
```

## DeleteDataProviderMessageRequestTypeDef

```python
# DeleteDataProviderMessageRequestTypeDef definition

class DeleteDataProviderMessageRequestTypeDef(TypedDict):
    DataProviderIdentifier: str,
```

## DeleteEndpointMessageRequestTypeDef

```python
# DeleteEndpointMessageRequestTypeDef definition

class DeleteEndpointMessageRequestTypeDef(TypedDict):
    EndpointArn: str,
```

## DeleteEventSubscriptionMessageRequestTypeDef

```python
# DeleteEventSubscriptionMessageRequestTypeDef definition

class DeleteEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
```

## DeleteFleetAdvisorDatabasesRequestRequestTypeDef

```python
# DeleteFleetAdvisorDatabasesRequestRequestTypeDef definition

class DeleteFleetAdvisorDatabasesRequestRequestTypeDef(TypedDict):
    DatabaseIds: Sequence[str],
```

## DeleteInstanceProfileMessageRequestTypeDef

```python
# DeleteInstanceProfileMessageRequestTypeDef definition

class DeleteInstanceProfileMessageRequestTypeDef(TypedDict):
    InstanceProfileIdentifier: str,
```

## DeleteMigrationProjectMessageRequestTypeDef

```python
# DeleteMigrationProjectMessageRequestTypeDef definition

class DeleteMigrationProjectMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
```

## DeleteReplicationConfigMessageRequestTypeDef

```python
# DeleteReplicationConfigMessageRequestTypeDef definition

class DeleteReplicationConfigMessageRequestTypeDef(TypedDict):
    ReplicationConfigArn: str,
```

## DeleteReplicationInstanceMessageRequestTypeDef

```python
# DeleteReplicationInstanceMessageRequestTypeDef definition

class DeleteReplicationInstanceMessageRequestTypeDef(TypedDict):
    ReplicationInstanceArn: str,
```

## DeleteReplicationSubnetGroupMessageRequestTypeDef

```python
# DeleteReplicationSubnetGroupMessageRequestTypeDef definition

class DeleteReplicationSubnetGroupMessageRequestTypeDef(TypedDict):
    ReplicationSubnetGroupIdentifier: str,
```

## DeleteReplicationTaskAssessmentRunMessageRequestTypeDef

```python
# DeleteReplicationTaskAssessmentRunMessageRequestTypeDef definition

class DeleteReplicationTaskAssessmentRunMessageRequestTypeDef(TypedDict):
    ReplicationTaskAssessmentRunArn: str,
```

## DeleteReplicationTaskMessageRequestTypeDef

```python
# DeleteReplicationTaskMessageRequestTypeDef definition

class DeleteReplicationTaskMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
```

## DescribeApplicableIndividualAssessmentsMessageRequestTypeDef

```python
# DescribeApplicableIndividualAssessmentsMessageRequestTypeDef definition

class DescribeApplicableIndividualAssessmentsMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: NotRequired[str],
    ReplicationInstanceArn: NotRequired[str],
    SourceEngineName: NotRequired[str],
    TargetEngineName: NotRequired[str],
    MigrationType: NotRequired[MigrationTypeValueType],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeConversionConfigurationMessageRequestTypeDef

```python
# DescribeConversionConfigurationMessageRequestTypeDef definition

class DescribeConversionConfigurationMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
```

## DescribeEndpointSettingsMessageRequestTypeDef

```python
# DescribeEndpointSettingsMessageRequestTypeDef definition

class DescribeEndpointSettingsMessageRequestTypeDef(TypedDict):
    EngineName: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## EndpointSettingTypeDef

```python
# EndpointSettingTypeDef definition

class EndpointSettingTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[EndpointSettingTypeValueType],  # (1)
    EnumValues: NotRequired[List[str]],
    Sensitive: NotRequired[bool],
    Units: NotRequired[str],
    Applicability: NotRequired[str],
    IntValueMin: NotRequired[int],
    IntValueMax: NotRequired[int],
    DefaultValue: NotRequired[str],
```

1. See [:material-code-brackets: EndpointSettingTypeValueType](./literals.md#endpointsettingtypevaluetype) 
## SupportedEndpointTypeTypeDef

```python
# SupportedEndpointTypeTypeDef definition

class SupportedEndpointTypeTypeDef(TypedDict):
    EngineName: NotRequired[str],
    SupportsCDC: NotRequired[bool],
    EndpointType: NotRequired[ReplicationEndpointTypeValueType],  # (1)
    ReplicationInstanceEngineMinimumVersion: NotRequired[str],
    EngineDisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ReplicationEndpointTypeValueType](./literals.md#replicationendpointtypevaluetype) 
## DescribeEngineVersionsMessageRequestTypeDef

```python
# DescribeEngineVersionsMessageRequestTypeDef definition

class DescribeEngineVersionsMessageRequestTypeDef(TypedDict):
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## EngineVersionTypeDef

```python
# EngineVersionTypeDef definition

class EngineVersionTypeDef(TypedDict):
    Version: NotRequired[str],
    Lifecycle: NotRequired[str],
    ReleaseStatus: NotRequired[ReleaseStatusValuesType],  # (1)
    LaunchDate: NotRequired[datetime],
    AutoUpgradeDate: NotRequired[datetime],
    DeprecationDate: NotRequired[datetime],
    ForceUpgradeDate: NotRequired[datetime],
    AvailableUpgrades: NotRequired[List[str]],
```

1. See [:material-code-brackets: ReleaseStatusValuesType](./literals.md#releasestatusvaluestype) 
## EventCategoryGroupTypeDef

```python
# EventCategoryGroupTypeDef definition

class EventCategoryGroupTypeDef(TypedDict):
    SourceType: NotRequired[str],
    EventCategories: NotRequired[List[str]],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    Message: NotRequired[str],
    EventCategories: NotRequired[List[str]],
    Date: NotRequired[datetime],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef

```python
# DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef definition

class DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef(TypedDict):
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

## FleetAdvisorLsaAnalysisResponseTypeDef

```python
# FleetAdvisorLsaAnalysisResponseTypeDef definition

class FleetAdvisorLsaAnalysisResponseTypeDef(TypedDict):
    LsaAnalysisId: NotRequired[str],
    Status: NotRequired[str],
```

## FleetAdvisorSchemaObjectResponseTypeDef

```python
# FleetAdvisorSchemaObjectResponseTypeDef definition

class FleetAdvisorSchemaObjectResponseTypeDef(TypedDict):
    SchemaId: NotRequired[str],
    ObjectType: NotRequired[str],
    NumberOfObjects: NotRequired[int],
    CodeLineCount: NotRequired[int],
    CodeSize: NotRequired[int],
```

## DescribeOrderableReplicationInstancesMessageRequestTypeDef

```python
# DescribeOrderableReplicationInstancesMessageRequestTypeDef definition

class DescribeOrderableReplicationInstancesMessageRequestTypeDef(TypedDict):
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## OrderableReplicationInstanceTypeDef

```python
# OrderableReplicationInstanceTypeDef definition

class OrderableReplicationInstanceTypeDef(TypedDict):
    EngineVersion: NotRequired[str],
    ReplicationInstanceClass: NotRequired[str],
    StorageType: NotRequired[str],
    MinAllocatedStorage: NotRequired[int],
    MaxAllocatedStorage: NotRequired[int],
    DefaultAllocatedStorage: NotRequired[int],
    IncludedAllocatedStorage: NotRequired[int],
    AvailabilityZones: NotRequired[List[str]],
    ReleaseStatus: NotRequired[ReleaseStatusValuesType],  # (1)
```

1. See [:material-code-brackets: ReleaseStatusValuesType](./literals.md#releasestatusvaluestype) 
## LimitationTypeDef

```python
# LimitationTypeDef definition

class LimitationTypeDef(TypedDict):
    DatabaseId: NotRequired[str],
    EngineName: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Impact: NotRequired[str],
    Type: NotRequired[str],
```

## DescribeRefreshSchemasStatusMessageRequestTypeDef

```python
# DescribeRefreshSchemasStatusMessageRequestTypeDef definition

class DescribeRefreshSchemasStatusMessageRequestTypeDef(TypedDict):
    EndpointArn: str,
```

## RefreshSchemasStatusTypeDef

```python
# RefreshSchemasStatusTypeDef definition

class RefreshSchemasStatusTypeDef(TypedDict):
    EndpointArn: NotRequired[str],
    ReplicationInstanceArn: NotRequired[str],
    Status: NotRequired[RefreshSchemasStatusTypeValueType],  # (1)
    LastRefreshDate: NotRequired[datetime],
    LastFailureMessage: NotRequired[str],
```

1. See [:material-code-brackets: RefreshSchemasStatusTypeValueType](./literals.md#refreshschemasstatustypevaluetype) 
## DescribeReplicationInstanceTaskLogsMessageRequestTypeDef

```python
# DescribeReplicationInstanceTaskLogsMessageRequestTypeDef definition

class DescribeReplicationInstanceTaskLogsMessageRequestTypeDef(TypedDict):
    ReplicationInstanceArn: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## ReplicationInstanceTaskLogTypeDef

```python
# ReplicationInstanceTaskLogTypeDef definition

class ReplicationInstanceTaskLogTypeDef(TypedDict):
    ReplicationTaskName: NotRequired[str],
    ReplicationTaskArn: NotRequired[str],
    ReplicationInstanceTaskLogSize: NotRequired[int],
```

## TableStatisticsTypeDef

```python
# TableStatisticsTypeDef definition

class TableStatisticsTypeDef(TypedDict):
    SchemaName: NotRequired[str],
    TableName: NotRequired[str],
    Inserts: NotRequired[int],
    Deletes: NotRequired[int],
    Updates: NotRequired[int],
    Ddls: NotRequired[int],
    AppliedInserts: NotRequired[int],
    AppliedDeletes: NotRequired[int],
    AppliedUpdates: NotRequired[int],
    AppliedDdls: NotRequired[int],
    FullLoadRows: NotRequired[int],
    FullLoadCondtnlChkFailedRows: NotRequired[int],
    FullLoadErrorRows: NotRequired[int],
    FullLoadStartTime: NotRequired[datetime],
    FullLoadEndTime: NotRequired[datetime],
    FullLoadReloaded: NotRequired[bool],
    LastUpdateTime: NotRequired[datetime],
    TableState: NotRequired[str],
    ValidationPendingRecords: NotRequired[int],
    ValidationFailedRecords: NotRequired[int],
    ValidationSuspendedRecords: NotRequired[int],
    ValidationState: NotRequired[str],
    ValidationStateDetails: NotRequired[str],
```

## DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef

```python
# DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef definition

class DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## ReplicationTaskAssessmentResultTypeDef

```python
# ReplicationTaskAssessmentResultTypeDef definition

class ReplicationTaskAssessmentResultTypeDef(TypedDict):
    ReplicationTaskIdentifier: NotRequired[str],
    ReplicationTaskArn: NotRequired[str],
    ReplicationTaskLastAssessmentDate: NotRequired[datetime],
    AssessmentStatus: NotRequired[str],
    AssessmentResultsFile: NotRequired[str],
    AssessmentResults: NotRequired[str],
    S3ObjectUrl: NotRequired[str],
```

## ReplicationTaskIndividualAssessmentTypeDef

```python
# ReplicationTaskIndividualAssessmentTypeDef definition

class ReplicationTaskIndividualAssessmentTypeDef(TypedDict):
    ReplicationTaskIndividualAssessmentArn: NotRequired[str],
    ReplicationTaskAssessmentRunArn: NotRequired[str],
    IndividualAssessmentName: NotRequired[str],
    Status: NotRequired[str],
    ReplicationTaskIndividualAssessmentStartDate: NotRequired[datetime],
```

## DescribeSchemasMessageRequestTypeDef

```python
# DescribeSchemasMessageRequestTypeDef definition

class DescribeSchemasMessageRequestTypeDef(TypedDict):
    EndpointArn: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## OracleSettingsOutputTypeDef

```python
# OracleSettingsOutputTypeDef definition

class OracleSettingsOutputTypeDef(TypedDict):
    AddSupplementalLogging: NotRequired[bool],
    ArchivedLogDestId: NotRequired[int],
    AdditionalArchivedLogDestId: NotRequired[int],
    ExtraArchivedLogDestIds: NotRequired[List[int]],
    AllowSelectNestedTables: NotRequired[bool],
    ParallelAsmReadThreads: NotRequired[int],
    ReadAheadBlocks: NotRequired[int],
    AccessAlternateDirectly: NotRequired[bool],
    UseAlternateFolderForOnline: NotRequired[bool],
    OraclePathPrefix: NotRequired[str],
    UsePathPrefix: NotRequired[str],
    ReplacePathPrefix: NotRequired[bool],
    EnableHomogenousTablespace: NotRequired[bool],
    DirectPathNoLog: NotRequired[bool],
    ArchivedLogsOnly: NotRequired[bool],
    AsmPassword: NotRequired[str],
    AsmServer: NotRequired[str],
    AsmUser: NotRequired[str],
    CharLengthSemantics: NotRequired[CharLengthSemanticsType],  # (1)
    DatabaseName: NotRequired[str],
    DirectPathParallelLoad: NotRequired[bool],
    FailTasksOnLobTruncation: NotRequired[bool],
    NumberDatatypeScale: NotRequired[int],
    Password: NotRequired[str],
    Port: NotRequired[int],
    ReadTableSpaceName: NotRequired[bool],
    RetryInterval: NotRequired[int],
    SecurityDbEncryption: NotRequired[str],
    SecurityDbEncryptionName: NotRequired[str],
    ServerName: NotRequired[str],
    SpatialDataOptionToGeoJsonFunctionName: NotRequired[str],
    StandbyDelayTime: NotRequired[int],
    Username: NotRequired[str],
    UseBFile: NotRequired[bool],
    UseDirectPathFullLoad: NotRequired[bool],
    UseLogminerReader: NotRequired[bool],
    SecretsManagerAccessRoleArn: NotRequired[str],
    SecretsManagerSecretId: NotRequired[str],
    SecretsManagerOracleAsmAccessRoleArn: NotRequired[str],
    SecretsManagerOracleAsmSecretId: NotRequired[str],
    TrimSpaceInChar: NotRequired[bool],
    ConvertTimestampWithZoneToUTC: NotRequired[bool],
    OpenTransactionWindow: NotRequired[int],
    AuthenticationMethod: NotRequired[OracleAuthenticationMethodType],  # (2)
```

1. See [:material-code-brackets: CharLengthSemanticsType](./literals.md#charlengthsemanticstype) 
2. See [:material-code-brackets: OracleAuthenticationMethodType](./literals.md#oracleauthenticationmethodtype) 
## ExportMetadataModelAssessmentMessageRequestTypeDef

```python
# ExportMetadataModelAssessmentMessageRequestTypeDef definition

class ExportMetadataModelAssessmentMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    FileName: NotRequired[str],
    AssessmentReportTypes: NotRequired[Sequence[AssessmentReportTypeType]],  # (1)
```

1. See [:material-code-brackets: AssessmentReportTypeType](./literals.md#assessmentreporttypetype) 
## ExportMetadataModelAssessmentResultEntryTypeDef

```python
# ExportMetadataModelAssessmentResultEntryTypeDef definition

class ExportMetadataModelAssessmentResultEntryTypeDef(TypedDict):
    S3ObjectKey: NotRequired[str],
    ObjectURL: NotRequired[str],
```

## ExportSqlDetailsTypeDef

```python
# ExportSqlDetailsTypeDef definition

class ExportSqlDetailsTypeDef(TypedDict):
    S3ObjectKey: NotRequired[str],
    ObjectURL: NotRequired[str],
```

## ListTagsForResourceMessageRequestTypeDef

```python
# ListTagsForResourceMessageRequestTypeDef definition

class ListTagsForResourceMessageRequestTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ResourceArnList: NotRequired[Sequence[str]],
```

## ModifyConversionConfigurationMessageRequestTypeDef

```python
# ModifyConversionConfigurationMessageRequestTypeDef definition

class ModifyConversionConfigurationMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    ConversionConfiguration: str,
```

## ModifyEventSubscriptionMessageRequestTypeDef

```python
# ModifyEventSubscriptionMessageRequestTypeDef definition

class ModifyEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
    SnsTopicArn: NotRequired[str],
    SourceType: NotRequired[str],
    EventCategories: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
```

## ModifyInstanceProfileMessageRequestTypeDef

```python
# ModifyInstanceProfileMessageRequestTypeDef definition

class ModifyInstanceProfileMessageRequestTypeDef(TypedDict):
    InstanceProfileIdentifier: str,
    AvailabilityZone: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    NetworkType: NotRequired[str],
    InstanceProfileName: NotRequired[str],
    Description: NotRequired[str],
    SubnetGroupIdentifier: NotRequired[str],
    VpcSecurityGroups: NotRequired[Sequence[str]],
```

## ModifyReplicationSubnetGroupMessageRequestTypeDef

```python
# ModifyReplicationSubnetGroupMessageRequestTypeDef definition

class ModifyReplicationSubnetGroupMessageRequestTypeDef(TypedDict):
    ReplicationSubnetGroupIdentifier: str,
    SubnetIds: Sequence[str],
    ReplicationSubnetGroupDescription: NotRequired[str],
```

## MoveReplicationTaskMessageRequestTypeDef

```python
# MoveReplicationTaskMessageRequestTypeDef definition

class MoveReplicationTaskMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
    TargetReplicationInstanceArn: str,
```

## PendingMaintenanceActionTypeDef

```python
# PendingMaintenanceActionTypeDef definition

class PendingMaintenanceActionTypeDef(TypedDict):
    Action: NotRequired[str],
    AutoAppliedAfterDate: NotRequired[datetime],
    ForcedApplyDate: NotRequired[datetime],
    OptInStatus: NotRequired[str],
    CurrentApplyDate: NotRequired[datetime],
    Description: NotRequired[str],
```

## ProvisionDataTypeDef

```python
# ProvisionDataTypeDef definition

class ProvisionDataTypeDef(TypedDict):
    ProvisionState: NotRequired[str],
    ProvisionedCapacityUnits: NotRequired[int],
    DateProvisioned: NotRequired[datetime],
    IsNewProvisioningAvailable: NotRequired[bool],
    DateNewProvisioningDataAvailable: NotRequired[datetime],
    ReasonForNewProvisioningData: NotRequired[str],
```

## RdsConfigurationTypeDef

```python
# RdsConfigurationTypeDef definition

class RdsConfigurationTypeDef(TypedDict):
    EngineEdition: NotRequired[str],
    InstanceType: NotRequired[str],
    InstanceVcpu: NotRequired[float],
    InstanceMemory: NotRequired[float],
    StorageType: NotRequired[str],
    StorageSize: NotRequired[int],
    StorageIops: NotRequired[int],
    DeploymentOption: NotRequired[str],
    EngineVersion: NotRequired[str],
```

## RdsRequirementsTypeDef

```python
# RdsRequirementsTypeDef definition

class RdsRequirementsTypeDef(TypedDict):
    EngineEdition: NotRequired[str],
    InstanceVcpu: NotRequired[float],
    InstanceMemory: NotRequired[float],
    StorageSize: NotRequired[int],
    StorageIops: NotRequired[int],
    DeploymentOption: NotRequired[str],
    EngineVersion: NotRequired[str],
```

## RebootReplicationInstanceMessageRequestTypeDef

```python
# RebootReplicationInstanceMessageRequestTypeDef definition

class RebootReplicationInstanceMessageRequestTypeDef(TypedDict):
    ReplicationInstanceArn: str,
    ForceFailover: NotRequired[bool],
    ForcePlannedFailover: NotRequired[bool],
```

## RecommendationSettingsTypeDef

```python
# RecommendationSettingsTypeDef definition

class RecommendationSettingsTypeDef(TypedDict):
    InstanceSizingType: str,
    WorkloadType: str,
```

## RefreshSchemasMessageRequestTypeDef

```python
# RefreshSchemasMessageRequestTypeDef definition

class RefreshSchemasMessageRequestTypeDef(TypedDict):
    EndpointArn: str,
    ReplicationInstanceArn: str,
```

## TableToReloadTypeDef

```python
# TableToReloadTypeDef definition

class TableToReloadTypeDef(TypedDict):
    SchemaName: str,
    TableName: str,
```

## RemoveTagsFromResourceMessageRequestTypeDef

```python
# RemoveTagsFromResourceMessageRequestTypeDef definition

class RemoveTagsFromResourceMessageRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ReplicationPendingModifiedValuesTypeDef

```python
# ReplicationPendingModifiedValuesTypeDef definition

class ReplicationPendingModifiedValuesTypeDef(TypedDict):
    ReplicationInstanceClass: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    NetworkType: NotRequired[str],
```

## VpcSecurityGroupMembershipTypeDef

```python
# VpcSecurityGroupMembershipTypeDef definition

class VpcSecurityGroupMembershipTypeDef(TypedDict):
    VpcSecurityGroupId: NotRequired[str],
    Status: NotRequired[str],
```

## ReplicationStatsTypeDef

```python
# ReplicationStatsTypeDef definition

class ReplicationStatsTypeDef(TypedDict):
    FullLoadProgressPercent: NotRequired[int],
    ElapsedTimeMillis: NotRequired[int],
    TablesLoaded: NotRequired[int],
    TablesLoading: NotRequired[int],
    TablesQueued: NotRequired[int],
    TablesErrored: NotRequired[int],
    FreshStartDate: NotRequired[datetime],
    StartDate: NotRequired[datetime],
    StopDate: NotRequired[datetime],
    FullLoadStartDate: NotRequired[datetime],
    FullLoadFinishDate: NotRequired[datetime],
```

## ReplicationTaskAssessmentRunProgressTypeDef

```python
# ReplicationTaskAssessmentRunProgressTypeDef definition

class ReplicationTaskAssessmentRunProgressTypeDef(TypedDict):
    IndividualAssessmentCount: NotRequired[int],
    IndividualAssessmentCompletedCount: NotRequired[int],
```

## ReplicationTaskAssessmentRunResultStatisticTypeDef

```python
# ReplicationTaskAssessmentRunResultStatisticTypeDef definition

class ReplicationTaskAssessmentRunResultStatisticTypeDef(TypedDict):
    Passed: NotRequired[int],
    Failed: NotRequired[int],
    Error: NotRequired[int],
    Warning: NotRequired[int],
    Cancelled: NotRequired[int],
```

## ReplicationTaskStatsTypeDef

```python
# ReplicationTaskStatsTypeDef definition

class ReplicationTaskStatsTypeDef(TypedDict):
    FullLoadProgressPercent: NotRequired[int],
    ElapsedTimeMillis: NotRequired[int],
    TablesLoaded: NotRequired[int],
    TablesLoading: NotRequired[int],
    TablesQueued: NotRequired[int],
    TablesErrored: NotRequired[int],
    FreshStartDate: NotRequired[datetime],
    StartDate: NotRequired[datetime],
    StopDate: NotRequired[datetime],
    FullLoadStartDate: NotRequired[datetime],
    FullLoadFinishDate: NotRequired[datetime],
```

## SchemaShortInfoResponseTypeDef

```python
# SchemaShortInfoResponseTypeDef definition

class SchemaShortInfoResponseTypeDef(TypedDict):
    SchemaId: NotRequired[str],
    SchemaName: NotRequired[str],
    DatabaseId: NotRequired[str],
    DatabaseName: NotRequired[str],
    DatabaseIpAddress: NotRequired[str],
```

## StartDataMigrationMessageRequestTypeDef

```python
# StartDataMigrationMessageRequestTypeDef definition

class StartDataMigrationMessageRequestTypeDef(TypedDict):
    DataMigrationIdentifier: str,
    StartType: StartReplicationMigrationTypeValueType,  # (1)
```

1. See [:material-code-brackets: StartReplicationMigrationTypeValueType](./literals.md#startreplicationmigrationtypevaluetype) 
## StartExtensionPackAssociationMessageRequestTypeDef

```python
# StartExtensionPackAssociationMessageRequestTypeDef definition

class StartExtensionPackAssociationMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
```

## StartMetadataModelAssessmentMessageRequestTypeDef

```python
# StartMetadataModelAssessmentMessageRequestTypeDef definition

class StartMetadataModelAssessmentMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    SelectionRules: str,
```

## StartMetadataModelConversionMessageRequestTypeDef

```python
# StartMetadataModelConversionMessageRequestTypeDef definition

class StartMetadataModelConversionMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    SelectionRules: str,
```

## StartMetadataModelExportAsScriptMessageRequestTypeDef

```python
# StartMetadataModelExportAsScriptMessageRequestTypeDef definition

class StartMetadataModelExportAsScriptMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    Origin: OriginTypeValueType,  # (1)
    FileName: NotRequired[str],
```

1. See [:material-code-brackets: OriginTypeValueType](./literals.md#origintypevaluetype) 
## StartMetadataModelExportToTargetMessageRequestTypeDef

```python
# StartMetadataModelExportToTargetMessageRequestTypeDef definition

class StartMetadataModelExportToTargetMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    OverwriteExtensionPack: NotRequired[bool],
```

## StartMetadataModelImportMessageRequestTypeDef

```python
# StartMetadataModelImportMessageRequestTypeDef definition

class StartMetadataModelImportMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    Origin: OriginTypeValueType,  # (1)
    Refresh: NotRequired[bool],
```

1. See [:material-code-brackets: OriginTypeValueType](./literals.md#origintypevaluetype) 
## StartReplicationTaskAssessmentMessageRequestTypeDef

```python
# StartReplicationTaskAssessmentMessageRequestTypeDef definition

class StartReplicationTaskAssessmentMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
```

## StopDataMigrationMessageRequestTypeDef

```python
# StopDataMigrationMessageRequestTypeDef definition

class StopDataMigrationMessageRequestTypeDef(TypedDict):
    DataMigrationIdentifier: str,
```

## StopReplicationMessageRequestTypeDef

```python
# StopReplicationMessageRequestTypeDef definition

class StopReplicationMessageRequestTypeDef(TypedDict):
    ReplicationConfigArn: str,
```

## StopReplicationTaskMessageRequestTypeDef

```python
# StopReplicationTaskMessageRequestTypeDef definition

class StopReplicationTaskMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
```

## TestConnectionMessageRequestTypeDef

```python
# TestConnectionMessageRequestTypeDef definition

class TestConnectionMessageRequestTypeDef(TypedDict):
    ReplicationInstanceArn: str,
    EndpointArn: str,
```

## UpdateSubscriptionsToEventBridgeMessageRequestTypeDef

```python
# UpdateSubscriptionsToEventBridgeMessageRequestTypeDef definition

class UpdateSubscriptionsToEventBridgeMessageRequestTypeDef(TypedDict):
    ForceMove: NotRequired[bool],
```

## AddTagsToResourceMessageRequestTypeDef

```python
# AddTagsToResourceMessageRequestTypeDef definition

class AddTagsToResourceMessageRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEventSubscriptionMessageRequestTypeDef

```python
# CreateEventSubscriptionMessageRequestTypeDef definition

class CreateEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
    SnsTopicArn: str,
    SourceType: NotRequired[str],
    EventCategories: NotRequired[Sequence[str]],
    SourceIds: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateInstanceProfileMessageRequestTypeDef

```python
# CreateInstanceProfileMessageRequestTypeDef definition

class CreateInstanceProfileMessageRequestTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    NetworkType: NotRequired[str],
    InstanceProfileName: NotRequired[str],
    Description: NotRequired[str],
    SubnetGroupIdentifier: NotRequired[str],
    VpcSecurityGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateReplicationSubnetGroupMessageRequestTypeDef

```python
# CreateReplicationSubnetGroupMessageRequestTypeDef definition

class CreateReplicationSubnetGroupMessageRequestTypeDef(TypedDict):
    ReplicationSubnetGroupIdentifier: str,
    ReplicationSubnetGroupDescription: str,
    SubnetIds: Sequence[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartReplicationTaskAssessmentRunMessageRequestTypeDef

```python
# StartReplicationTaskAssessmentRunMessageRequestTypeDef definition

class StartReplicationTaskAssessmentRunMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
    ServiceAccessRoleArn: str,
    ResultLocationBucket: str,
    AssessmentRunName: str,
    ResultLocationFolder: NotRequired[str],
    ResultEncryptionMode: NotRequired[str],
    ResultKmsKeyArn: NotRequired[str],
    IncludeOnly: NotRequired[Sequence[str]],
    Exclude: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFleetAdvisorCollectorResponseTypeDef

```python
# CreateFleetAdvisorCollectorResponseTypeDef definition

class CreateFleetAdvisorCollectorResponseTypeDef(TypedDict):
    CollectorReferencedId: str,
    CollectorName: str,
    Description: str,
    ServiceAccessRoleArn: str,
    S3BucketName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFleetAdvisorDatabasesResponseTypeDef

```python
# DeleteFleetAdvisorDatabasesResponseTypeDef definition

class DeleteFleetAdvisorDatabasesResponseTypeDef(TypedDict):
    DatabaseIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAttributesResponseTypeDef

```python
# DescribeAccountAttributesResponseTypeDef definition

class DescribeAccountAttributesResponseTypeDef(TypedDict):
    AccountQuotas: List[AccountQuotaTypeDef],  # (1)
    UniqueAccountIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountQuotaTypeDef](./type_defs.md#accountquotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicableIndividualAssessmentsResponseTypeDef

```python
# DescribeApplicableIndividualAssessmentsResponseTypeDef definition

class DescribeApplicableIndividualAssessmentsResponseTypeDef(TypedDict):
    IndividualAssessmentNames: List[str],
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConversionConfigurationResponseTypeDef

```python
# DescribeConversionConfigurationResponseTypeDef definition

class DescribeConversionConfigurationResponseTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    ConversionConfiguration: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSchemasResponseTypeDef

```python
# DescribeSchemasResponseTypeDef definition

class DescribeSchemasResponseTypeDef(TypedDict):
    Marker: str,
    Schemas: List[str],
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
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyConversionConfigurationResponseTypeDef

```python
# ModifyConversionConfigurationResponseTypeDef definition

class ModifyConversionConfigurationResponseTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReloadReplicationTablesResponseTypeDef

```python
# ReloadReplicationTablesResponseTypeDef definition

class ReloadReplicationTablesResponseTypeDef(TypedDict):
    ReplicationConfigArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReloadTablesResponseTypeDef

```python
# ReloadTablesResponseTypeDef definition

class ReloadTablesResponseTypeDef(TypedDict):
    ReplicationTaskArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunFleetAdvisorLsaAnalysisResponseTypeDef

```python
# RunFleetAdvisorLsaAnalysisResponseTypeDef definition

class RunFleetAdvisorLsaAnalysisResponseTypeDef(TypedDict):
    LsaAnalysisId: str,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExtensionPackAssociationResponseTypeDef

```python
# StartExtensionPackAssociationResponseTypeDef definition

class StartExtensionPackAssociationResponseTypeDef(TypedDict):
    RequestIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMetadataModelAssessmentResponseTypeDef

```python
# StartMetadataModelAssessmentResponseTypeDef definition

class StartMetadataModelAssessmentResponseTypeDef(TypedDict):
    RequestIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMetadataModelConversionResponseTypeDef

```python
# StartMetadataModelConversionResponseTypeDef definition

class StartMetadataModelConversionResponseTypeDef(TypedDict):
    RequestIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMetadataModelExportAsScriptResponseTypeDef

```python
# StartMetadataModelExportAsScriptResponseTypeDef definition

class StartMetadataModelExportAsScriptResponseTypeDef(TypedDict):
    RequestIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMetadataModelExportToTargetResponseTypeDef

```python
# StartMetadataModelExportToTargetResponseTypeDef definition

class StartMetadataModelExportToTargetResponseTypeDef(TypedDict):
    RequestIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMetadataModelImportResponseTypeDef

```python
# StartMetadataModelImportResponseTypeDef definition

class StartMetadataModelImportResponseTypeDef(TypedDict):
    RequestIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSubscriptionsToEventBridgeResponseTypeDef

```python
# UpdateSubscriptionsToEventBridgeResponseTypeDef definition

class UpdateSubscriptionsToEventBridgeResponseTypeDef(TypedDict):
    Result: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubnetTypeDef

```python
# SubnetTypeDef definition

class SubnetTypeDef(TypedDict):
    SubnetIdentifier: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[AvailabilityZoneTypeDef],  # (1)
    SubnetStatus: NotRequired[str],
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
## BatchStartRecommendationsResponseTypeDef

```python
# BatchStartRecommendationsResponseTypeDef definition

class BatchStartRecommendationsResponseTypeDef(TypedDict):
    ErrorEntries: List[BatchStartRecommendationsErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchStartRecommendationsErrorEntryTypeDef](./type_defs.md#batchstartrecommendationserrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportCertificateMessageRequestTypeDef

```python
# ImportCertificateMessageRequestTypeDef definition

class ImportCertificateMessageRequestTypeDef(TypedDict):
    CertificateIdentifier: str,
    CertificatePem: NotRequired[str],
    CertificateWallet: NotRequired[BlobTypeDef],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteCertificateResponseTypeDef

```python
# DeleteCertificateResponseTypeDef definition

class DeleteCertificateResponseTypeDef(TypedDict):
    Certificate: CertificateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCertificatesResponseTypeDef

```python
# DescribeCertificatesResponseTypeDef definition

class DescribeCertificatesResponseTypeDef(TypedDict):
    Marker: str,
    Certificates: List[CertificateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportCertificateResponseTypeDef

```python
# ImportCertificateResponseTypeDef definition

class ImportCertificateResponseTypeDef(TypedDict):
    Certificate: CertificateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CollectorResponseTypeDef

```python
# CollectorResponseTypeDef definition

class CollectorResponseTypeDef(TypedDict):
    CollectorReferencedId: NotRequired[str],
    CollectorName: NotRequired[str],
    CollectorVersion: NotRequired[str],
    VersionStatus: NotRequired[VersionStatusType],  # (1)
    Description: NotRequired[str],
    S3BucketName: NotRequired[str],
    ServiceAccessRoleArn: NotRequired[str],
    CollectorHealthCheck: NotRequired[CollectorHealthCheckTypeDef],  # (2)
    LastDataReceived: NotRequired[str],
    RegisteredDate: NotRequired[str],
    CreatedDate: NotRequired[str],
    ModifiedDate: NotRequired[str],
    InventoryData: NotRequired[InventoryDataTypeDef],  # (3)
```

1. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
2. See [:material-code-braces: CollectorHealthCheckTypeDef](./type_defs.md#collectorhealthchecktypedef) 
3. See [:material-code-braces: InventoryDataTypeDef](./type_defs.md#inventorydatatypedef) 
## ReplicationConfigTypeDef

```python
# ReplicationConfigTypeDef definition

class ReplicationConfigTypeDef(TypedDict):
    ReplicationConfigIdentifier: NotRequired[str],
    ReplicationConfigArn: NotRequired[str],
    SourceEndpointArn: NotRequired[str],
    TargetEndpointArn: NotRequired[str],
    ReplicationType: NotRequired[MigrationTypeValueType],  # (1)
    ComputeConfig: NotRequired[ComputeConfigOutputTypeDef],  # (2)
    ReplicationSettings: NotRequired[str],
    SupplementalSettings: NotRequired[str],
    TableMappings: NotRequired[str],
    ReplicationConfigCreateTime: NotRequired[datetime],
    ReplicationConfigUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: ComputeConfigOutputTypeDef](./type_defs.md#computeconfigoutputtypedef) 
## CreateReplicationConfigMessageRequestTypeDef

```python
# CreateReplicationConfigMessageRequestTypeDef definition

class CreateReplicationConfigMessageRequestTypeDef(TypedDict):
    ReplicationConfigIdentifier: str,
    SourceEndpointArn: str,
    TargetEndpointArn: str,
    ComputeConfig: ComputeConfigTypeDef,  # (1)
    ReplicationType: MigrationTypeValueType,  # (2)
    TableMappings: str,
    ReplicationSettings: NotRequired[str],
    SupplementalSettings: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ComputeConfigTypeDef](./type_defs.md#computeconfigtypedef) 
2. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModifyReplicationConfigMessageRequestTypeDef

```python
# ModifyReplicationConfigMessageRequestTypeDef definition

class ModifyReplicationConfigMessageRequestTypeDef(TypedDict):
    ReplicationConfigArn: str,
    ReplicationConfigIdentifier: NotRequired[str],
    ReplicationType: NotRequired[MigrationTypeValueType],  # (1)
    TableMappings: NotRequired[str],
    ReplicationSettings: NotRequired[str],
    SupplementalSettings: NotRequired[str],
    ComputeConfig: NotRequired[ComputeConfigTypeDef],  # (2)
    SourceEndpointArn: NotRequired[str],
    TargetEndpointArn: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: ComputeConfigTypeDef](./type_defs.md#computeconfigtypedef) 
## DeleteConnectionResponseTypeDef

```python
# DeleteConnectionResponseTypeDef definition

class DeleteConnectionResponseTypeDef(TypedDict):
    Connection: ConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConnectionsResponseTypeDef

```python
# DescribeConnectionsResponseTypeDef definition

class DescribeConnectionsResponseTypeDef(TypedDict):
    Marker: str,
    Connections: List[ConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestConnectionResponseTypeDef

```python
# TestConnectionResponseTypeDef definition

class TestConnectionResponseTypeDef(TypedDict):
    Connection: ConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointMessageRequestTypeDef

```python
# CreateEndpointMessageRequestTypeDef definition

class CreateEndpointMessageRequestTypeDef(TypedDict):
    EndpointIdentifier: str,
    EndpointType: ReplicationEndpointTypeValueType,  # (1)
    EngineName: str,
    Username: NotRequired[str],
    Password: NotRequired[str],
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    ExtraConnectionAttributes: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    CertificateArn: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (3)
    ServiceAccessRoleArn: NotRequired[str],
    ExternalTableDefinition: NotRequired[str],
    DynamoDbSettings: NotRequired[DynamoDbSettingsTypeDef],  # (4)
    S3Settings: NotRequired[S3SettingsTypeDef],  # (5)
    DmsTransferSettings: NotRequired[DmsTransferSettingsTypeDef],  # (6)
    MongoDbSettings: NotRequired[MongoDbSettingsTypeDef],  # (7)
    KinesisSettings: NotRequired[KinesisSettingsTypeDef],  # (8)
    KafkaSettings: NotRequired[KafkaSettingsTypeDef],  # (9)
    ElasticsearchSettings: NotRequired[ElasticsearchSettingsTypeDef],  # (10)
    NeptuneSettings: NotRequired[NeptuneSettingsTypeDef],  # (11)
    RedshiftSettings: NotRequired[RedshiftSettingsTypeDef],  # (12)
    PostgreSQLSettings: NotRequired[PostgreSQLSettingsTypeDef],  # (13)
    MySQLSettings: NotRequired[MySQLSettingsTypeDef],  # (14)
    OracleSettings: NotRequired[OracleSettingsTypeDef],  # (15)
    SybaseSettings: NotRequired[SybaseSettingsTypeDef],  # (16)
    MicrosoftSQLServerSettings: NotRequired[MicrosoftSQLServerSettingsTypeDef],  # (17)
    IBMDb2Settings: NotRequired[IBMDb2SettingsTypeDef],  # (18)
    ResourceIdentifier: NotRequired[str],
    DocDbSettings: NotRequired[DocDbSettingsTypeDef],  # (19)
    RedisSettings: NotRequired[RedisSettingsTypeDef],  # (20)
    GcpMySQLSettings: NotRequired[GcpMySQLSettingsTypeDef],  # (21)
    TimestreamSettings: NotRequired[TimestreamSettingsTypeDef],  # (22)
```

1. See [:material-code-brackets: ReplicationEndpointTypeValueType](./literals.md#replicationendpointtypevaluetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
4. See [:material-code-braces: DynamoDbSettingsTypeDef](./type_defs.md#dynamodbsettingstypedef) 
5. See [:material-code-braces: S3SettingsTypeDef](./type_defs.md#s3settingstypedef) 
6. See [:material-code-braces: DmsTransferSettingsTypeDef](./type_defs.md#dmstransfersettingstypedef) 
7. See [:material-code-braces: MongoDbSettingsTypeDef](./type_defs.md#mongodbsettingstypedef) 
8. See [:material-code-braces: KinesisSettingsTypeDef](./type_defs.md#kinesissettingstypedef) 
9. See [:material-code-braces: KafkaSettingsTypeDef](./type_defs.md#kafkasettingstypedef) 
10. See [:material-code-braces: ElasticsearchSettingsTypeDef](./type_defs.md#elasticsearchsettingstypedef) 
11. See [:material-code-braces: NeptuneSettingsTypeDef](./type_defs.md#neptunesettingstypedef) 
12. See [:material-code-braces: RedshiftSettingsTypeDef](./type_defs.md#redshiftsettingstypedef) 
13. See [:material-code-braces: PostgreSQLSettingsTypeDef](./type_defs.md#postgresqlsettingstypedef) 
14. See [:material-code-braces: MySQLSettingsTypeDef](./type_defs.md#mysqlsettingstypedef) 
15. See [:material-code-braces: OracleSettingsTypeDef](./type_defs.md#oraclesettingstypedef) 
16. See [:material-code-braces: SybaseSettingsTypeDef](./type_defs.md#sybasesettingstypedef) 
17. See [:material-code-braces: MicrosoftSQLServerSettingsTypeDef](./type_defs.md#microsoftsqlserversettingstypedef) 
18. See [:material-code-braces: IBMDb2SettingsTypeDef](./type_defs.md#ibmdb2settingstypedef) 
19. See [:material-code-braces: DocDbSettingsTypeDef](./type_defs.md#docdbsettingstypedef) 
20. See [:material-code-braces: RedisSettingsTypeDef](./type_defs.md#redissettingstypedef) 
21. See [:material-code-braces: GcpMySQLSettingsTypeDef](./type_defs.md#gcpmysqlsettingstypedef) 
22. See [:material-code-braces: TimestreamSettingsTypeDef](./type_defs.md#timestreamsettingstypedef) 
## ModifyEndpointMessageRequestTypeDef

```python
# ModifyEndpointMessageRequestTypeDef definition

class ModifyEndpointMessageRequestTypeDef(TypedDict):
    EndpointArn: str,
    EndpointIdentifier: NotRequired[str],
    EndpointType: NotRequired[ReplicationEndpointTypeValueType],  # (1)
    EngineName: NotRequired[str],
    Username: NotRequired[str],
    Password: NotRequired[str],
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    ExtraConnectionAttributes: NotRequired[str],
    CertificateArn: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (2)
    ServiceAccessRoleArn: NotRequired[str],
    ExternalTableDefinition: NotRequired[str],
    DynamoDbSettings: NotRequired[DynamoDbSettingsTypeDef],  # (3)
    S3Settings: NotRequired[S3SettingsTypeDef],  # (4)
    DmsTransferSettings: NotRequired[DmsTransferSettingsTypeDef],  # (5)
    MongoDbSettings: NotRequired[MongoDbSettingsTypeDef],  # (6)
    KinesisSettings: NotRequired[KinesisSettingsTypeDef],  # (7)
    KafkaSettings: NotRequired[KafkaSettingsTypeDef],  # (8)
    ElasticsearchSettings: NotRequired[ElasticsearchSettingsTypeDef],  # (9)
    NeptuneSettings: NotRequired[NeptuneSettingsTypeDef],  # (10)
    RedshiftSettings: NotRequired[RedshiftSettingsTypeDef],  # (11)
    PostgreSQLSettings: NotRequired[PostgreSQLSettingsTypeDef],  # (12)
    MySQLSettings: NotRequired[MySQLSettingsTypeDef],  # (13)
    OracleSettings: NotRequired[OracleSettingsTypeDef],  # (14)
    SybaseSettings: NotRequired[SybaseSettingsTypeDef],  # (15)
    MicrosoftSQLServerSettings: NotRequired[MicrosoftSQLServerSettingsTypeDef],  # (16)
    IBMDb2Settings: NotRequired[IBMDb2SettingsTypeDef],  # (17)
    DocDbSettings: NotRequired[DocDbSettingsTypeDef],  # (18)
    RedisSettings: NotRequired[RedisSettingsTypeDef],  # (19)
    ExactSettings: NotRequired[bool],
    GcpMySQLSettings: NotRequired[GcpMySQLSettingsTypeDef],  # (20)
    TimestreamSettings: NotRequired[TimestreamSettingsTypeDef],  # (21)
```

1. See [:material-code-brackets: ReplicationEndpointTypeValueType](./literals.md#replicationendpointtypevaluetype) 
2. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
3. See [:material-code-braces: DynamoDbSettingsTypeDef](./type_defs.md#dynamodbsettingstypedef) 
4. See [:material-code-braces: S3SettingsTypeDef](./type_defs.md#s3settingstypedef) 
5. See [:material-code-braces: DmsTransferSettingsTypeDef](./type_defs.md#dmstransfersettingstypedef) 
6. See [:material-code-braces: MongoDbSettingsTypeDef](./type_defs.md#mongodbsettingstypedef) 
7. See [:material-code-braces: KinesisSettingsTypeDef](./type_defs.md#kinesissettingstypedef) 
8. See [:material-code-braces: KafkaSettingsTypeDef](./type_defs.md#kafkasettingstypedef) 
9. See [:material-code-braces: ElasticsearchSettingsTypeDef](./type_defs.md#elasticsearchsettingstypedef) 
10. See [:material-code-braces: NeptuneSettingsTypeDef](./type_defs.md#neptunesettingstypedef) 
11. See [:material-code-braces: RedshiftSettingsTypeDef](./type_defs.md#redshiftsettingstypedef) 
12. See [:material-code-braces: PostgreSQLSettingsTypeDef](./type_defs.md#postgresqlsettingstypedef) 
13. See [:material-code-braces: MySQLSettingsTypeDef](./type_defs.md#mysqlsettingstypedef) 
14. See [:material-code-braces: OracleSettingsTypeDef](./type_defs.md#oraclesettingstypedef) 
15. See [:material-code-braces: SybaseSettingsTypeDef](./type_defs.md#sybasesettingstypedef) 
16. See [:material-code-braces: MicrosoftSQLServerSettingsTypeDef](./type_defs.md#microsoftsqlserversettingstypedef) 
17. See [:material-code-braces: IBMDb2SettingsTypeDef](./type_defs.md#ibmdb2settingstypedef) 
18. See [:material-code-braces: DocDbSettingsTypeDef](./type_defs.md#docdbsettingstypedef) 
19. See [:material-code-braces: RedisSettingsTypeDef](./type_defs.md#redissettingstypedef) 
20. See [:material-code-braces: GcpMySQLSettingsTypeDef](./type_defs.md#gcpmysqlsettingstypedef) 
21. See [:material-code-braces: TimestreamSettingsTypeDef](./type_defs.md#timestreamsettingstypedef) 
## CreateEventSubscriptionResponseTypeDef

```python
# CreateEventSubscriptionResponseTypeDef definition

class CreateEventSubscriptionResponseTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEventSubscriptionResponseTypeDef

```python
# DeleteEventSubscriptionResponseTypeDef definition

class DeleteEventSubscriptionResponseTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventSubscriptionsResponseTypeDef

```python
# DescribeEventSubscriptionsResponseTypeDef definition

class DescribeEventSubscriptionsResponseTypeDef(TypedDict):
    Marker: str,
    EventSubscriptionsList: List[EventSubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyEventSubscriptionResponseTypeDef

```python
# ModifyEventSubscriptionResponseTypeDef definition

class ModifyEventSubscriptionResponseTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceProfileResponseTypeDef

```python
# CreateInstanceProfileResponseTypeDef definition

class CreateInstanceProfileResponseTypeDef(TypedDict):
    InstanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInstanceProfileResponseTypeDef

```python
# DeleteInstanceProfileResponseTypeDef definition

class DeleteInstanceProfileResponseTypeDef(TypedDict):
    InstanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstanceProfilesResponseTypeDef

```python
# DescribeInstanceProfilesResponseTypeDef definition

class DescribeInstanceProfilesResponseTypeDef(TypedDict):
    Marker: str,
    InstanceProfiles: List[InstanceProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyInstanceProfileResponseTypeDef

```python
# ModifyInstanceProfileResponseTypeDef definition

class ModifyInstanceProfileResponseTypeDef(TypedDict):
    InstanceProfile: InstanceProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMigrationProjectMessageRequestTypeDef

```python
# CreateMigrationProjectMessageRequestTypeDef definition

class CreateMigrationProjectMessageRequestTypeDef(TypedDict):
    SourceDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],  # (1)
    TargetDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],  # (1)
    InstanceProfileIdentifier: str,
    MigrationProjectName: NotRequired[str],
    TransformationRules: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    SchemaConversionApplicationAttributes: NotRequired[SCApplicationAttributesTypeDef],  # (4)
```

1. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
2. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: SCApplicationAttributesTypeDef](./type_defs.md#scapplicationattributestypedef) 
## ModifyMigrationProjectMessageRequestTypeDef

```python
# ModifyMigrationProjectMessageRequestTypeDef definition

class ModifyMigrationProjectMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    MigrationProjectName: NotRequired[str],
    SourceDataProviderDescriptors: NotRequired[Sequence[DataProviderDescriptorDefinitionTypeDef]],  # (1)
    TargetDataProviderDescriptors: NotRequired[Sequence[DataProviderDescriptorDefinitionTypeDef]],  # (1)
    InstanceProfileIdentifier: NotRequired[str],
    TransformationRules: NotRequired[str],
    Description: NotRequired[str],
    SchemaConversionApplicationAttributes: NotRequired[SCApplicationAttributesTypeDef],  # (3)
```

1. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
2. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
3. See [:material-code-braces: SCApplicationAttributesTypeDef](./type_defs.md#scapplicationattributestypedef) 
## CreateReplicationInstanceMessageRequestTypeDef

```python
# CreateReplicationInstanceMessageRequestTypeDef definition

class CreateReplicationInstanceMessageRequestTypeDef(TypedDict):
    ReplicationInstanceIdentifier: str,
    ReplicationInstanceClass: str,
    AllocatedStorage: NotRequired[int],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    AvailabilityZone: NotRequired[str],
    ReplicationSubnetGroupIdentifier: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    KmsKeyId: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    DnsNameServers: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
    NetworkType: NotRequired[str],
    KerberosAuthenticationSettings: NotRequired[KerberosAuthenticationSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: KerberosAuthenticationSettingsTypeDef](./type_defs.md#kerberosauthenticationsettingstypedef) 
## ModifyReplicationInstanceMessageRequestTypeDef

```python
# ModifyReplicationInstanceMessageRequestTypeDef definition

class ModifyReplicationInstanceMessageRequestTypeDef(TypedDict):
    ReplicationInstanceArn: str,
    AllocatedStorage: NotRequired[int],
    ApplyImmediately: NotRequired[bool],
    ReplicationInstanceClass: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    PreferredMaintenanceWindow: NotRequired[str],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AllowMajorVersionUpgrade: NotRequired[bool],
    AutoMinorVersionUpgrade: NotRequired[bool],
    ReplicationInstanceIdentifier: NotRequired[str],
    NetworkType: NotRequired[str],
    KerberosAuthenticationSettings: NotRequired[KerberosAuthenticationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: KerberosAuthenticationSettingsTypeDef](./type_defs.md#kerberosauthenticationsettingstypedef) 
## CreateReplicationTaskMessageRequestTypeDef

```python
# CreateReplicationTaskMessageRequestTypeDef definition

class CreateReplicationTaskMessageRequestTypeDef(TypedDict):
    ReplicationTaskIdentifier: str,
    SourceEndpointArn: str,
    TargetEndpointArn: str,
    ReplicationInstanceArn: str,
    MigrationType: MigrationTypeValueType,  # (1)
    TableMappings: str,
    ReplicationTaskSettings: NotRequired[str],
    CdcStartTime: NotRequired[TimestampTypeDef],
    CdcStartPosition: NotRequired[str],
    CdcStopPosition: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    TaskData: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModifyReplicationTaskMessageRequestTypeDef

```python
# ModifyReplicationTaskMessageRequestTypeDef definition

class ModifyReplicationTaskMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
    ReplicationTaskIdentifier: NotRequired[str],
    MigrationType: NotRequired[MigrationTypeValueType],  # (1)
    TableMappings: NotRequired[str],
    ReplicationTaskSettings: NotRequired[str],
    CdcStartTime: NotRequired[TimestampTypeDef],
    CdcStartPosition: NotRequired[str],
    CdcStopPosition: NotRequired[str],
    TaskData: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
## SourceDataSettingTypeDef

```python
# SourceDataSettingTypeDef definition

class SourceDataSettingTypeDef(TypedDict):
    CDCStartPosition: NotRequired[str],
    CDCStartTime: NotRequired[TimestampTypeDef],
    CDCStopTime: NotRequired[TimestampTypeDef],
    SlotName: NotRequired[str],
```

## StartReplicationMessageRequestTypeDef

```python
# StartReplicationMessageRequestTypeDef definition

class StartReplicationMessageRequestTypeDef(TypedDict):
    ReplicationConfigArn: str,
    StartReplicationType: str,
    CdcStartTime: NotRequired[TimestampTypeDef],
    CdcStartPosition: NotRequired[str],
    CdcStopPosition: NotRequired[str],
```

## StartReplicationTaskMessageRequestTypeDef

```python
# StartReplicationTaskMessageRequestTypeDef definition

class StartReplicationTaskMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
    StartReplicationTaskType: StartReplicationTaskTypeValueType,  # (1)
    CdcStartTime: NotRequired[TimestampTypeDef],
    CdcStartPosition: NotRequired[str],
    CdcStopPosition: NotRequired[str],
```

1. See [:material-code-brackets: StartReplicationTaskTypeValueType](./literals.md#startreplicationtasktypevaluetype) 
## DataMigrationTypeDef

```python
# DataMigrationTypeDef definition

class DataMigrationTypeDef(TypedDict):
    DataMigrationName: NotRequired[str],
    DataMigrationArn: NotRequired[str],
    DataMigrationCreateTime: NotRequired[datetime],
    DataMigrationStartTime: NotRequired[datetime],
    DataMigrationEndTime: NotRequired[datetime],
    ServiceAccessRoleArn: NotRequired[str],
    MigrationProjectArn: NotRequired[str],
    DataMigrationType: NotRequired[MigrationTypeValueType],  # (1)
    DataMigrationSettings: NotRequired[DataMigrationSettingsTypeDef],  # (2)
    SourceDataSettings: NotRequired[List[SourceDataSettingOutputTypeDef]],  # (3)
    DataMigrationStatistics: NotRequired[DataMigrationStatisticsTypeDef],  # (4)
    DataMigrationStatus: NotRequired[str],
    PublicIpAddresses: NotRequired[List[str]],
    DataMigrationCidrBlocks: NotRequired[List[str]],
    LastFailureMessage: NotRequired[str],
    StopReason: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: DataMigrationSettingsTypeDef](./type_defs.md#datamigrationsettingstypedef) 
3. See [:material-code-braces: SourceDataSettingOutputTypeDef](./type_defs.md#sourcedatasettingoutputtypedef) 
4. See [:material-code-braces: DataMigrationStatisticsTypeDef](./type_defs.md#datamigrationstatisticstypedef) 
## MigrationProjectTypeDef

```python
# MigrationProjectTypeDef definition

class MigrationProjectTypeDef(TypedDict):
    MigrationProjectName: NotRequired[str],
    MigrationProjectArn: NotRequired[str],
    MigrationProjectCreationTime: NotRequired[datetime],
    SourceDataProviderDescriptors: NotRequired[List[DataProviderDescriptorTypeDef]],  # (1)
    TargetDataProviderDescriptors: NotRequired[List[DataProviderDescriptorTypeDef]],  # (1)
    InstanceProfileArn: NotRequired[str],
    InstanceProfileName: NotRequired[str],
    TransformationRules: NotRequired[str],
    Description: NotRequired[str],
    SchemaConversionApplicationAttributes: NotRequired[SCApplicationAttributesTypeDef],  # (3)
```

1. See [:material-code-braces: DataProviderDescriptorTypeDef](./type_defs.md#dataproviderdescriptortypedef) 
2. See [:material-code-braces: DataProviderDescriptorTypeDef](./type_defs.md#dataproviderdescriptortypedef) 
3. See [:material-code-braces: SCApplicationAttributesTypeDef](./type_defs.md#scapplicationattributestypedef) 
## DataProviderSettingsTypeDef

```python
# DataProviderSettingsTypeDef definition

class DataProviderSettingsTypeDef(TypedDict):
    RedshiftSettings: NotRequired[RedshiftDataProviderSettingsTypeDef],  # (1)
    PostgreSqlSettings: NotRequired[PostgreSqlDataProviderSettingsTypeDef],  # (2)
    MySqlSettings: NotRequired[MySqlDataProviderSettingsTypeDef],  # (3)
    OracleSettings: NotRequired[OracleDataProviderSettingsTypeDef],  # (4)
    MicrosoftSqlServerSettings: NotRequired[MicrosoftSqlServerDataProviderSettingsTypeDef],  # (5)
    DocDbSettings: NotRequired[DocDbDataProviderSettingsTypeDef],  # (6)
    MariaDbSettings: NotRequired[MariaDbDataProviderSettingsTypeDef],  # (7)
    MongoDbSettings: NotRequired[MongoDbDataProviderSettingsTypeDef],  # (8)
```

1. See [:material-code-braces: RedshiftDataProviderSettingsTypeDef](./type_defs.md#redshiftdataprovidersettingstypedef) 
2. See [:material-code-braces: PostgreSqlDataProviderSettingsTypeDef](./type_defs.md#postgresqldataprovidersettingstypedef) 
3. See [:material-code-braces: MySqlDataProviderSettingsTypeDef](./type_defs.md#mysqldataprovidersettingstypedef) 
4. See [:material-code-braces: OracleDataProviderSettingsTypeDef](./type_defs.md#oracledataprovidersettingstypedef) 
5. See [:material-code-braces: MicrosoftSqlServerDataProviderSettingsTypeDef](./type_defs.md#microsoftsqlserverdataprovidersettingstypedef) 
6. See [:material-code-braces: DocDbDataProviderSettingsTypeDef](./type_defs.md#docdbdataprovidersettingstypedef) 
7. See [:material-code-braces: MariaDbDataProviderSettingsTypeDef](./type_defs.md#mariadbdataprovidersettingstypedef) 
8. See [:material-code-braces: MongoDbDataProviderSettingsTypeDef](./type_defs.md#mongodbdataprovidersettingstypedef) 
## DatabaseResponseTypeDef

```python
# DatabaseResponseTypeDef definition

class DatabaseResponseTypeDef(TypedDict):
    DatabaseId: NotRequired[str],
    DatabaseName: NotRequired[str],
    IpAddress: NotRequired[str],
    NumberOfSchemas: NotRequired[int],
    Server: NotRequired[ServerShortInfoResponseTypeDef],  # (1)
    SoftwareDetails: NotRequired[DatabaseInstanceSoftwareDetailsResponseTypeDef],  # (2)
    Collectors: NotRequired[List[CollectorShortInfoResponseTypeDef]],  # (3)
```

1. See [:material-code-braces: ServerShortInfoResponseTypeDef](./type_defs.md#servershortinforesponsetypedef) 
2. See [:material-code-braces: DatabaseInstanceSoftwareDetailsResponseTypeDef](./type_defs.md#databaseinstancesoftwaredetailsresponsetypedef) 
3. See [:material-code-braces: CollectorShortInfoResponseTypeDef](./type_defs.md#collectorshortinforesponsetypedef) 
## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    defaultErrorDetails: NotRequired[DefaultErrorDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: DefaultErrorDetailsTypeDef](./type_defs.md#defaulterrordetailstypedef) 
## DescribeCertificatesMessageRequestTypeDef

```python
# DescribeCertificatesMessageRequestTypeDef definition

class DescribeCertificatesMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeConnectionsMessageRequestTypeDef

```python
# DescribeConnectionsMessageRequestTypeDef definition

class DescribeConnectionsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDataMigrationsMessageRequestTypeDef

```python
# DescribeDataMigrationsMessageRequestTypeDef definition

class DescribeDataMigrationsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WithoutSettings: NotRequired[bool],
    WithoutStatistics: NotRequired[bool],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDataProvidersMessageRequestTypeDef

```python
# DescribeDataProvidersMessageRequestTypeDef definition

class DescribeDataProvidersMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEndpointTypesMessageRequestTypeDef

```python
# DescribeEndpointTypesMessageRequestTypeDef definition

class DescribeEndpointTypesMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEndpointsMessageRequestTypeDef

```python
# DescribeEndpointsMessageRequestTypeDef definition

class DescribeEndpointsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEventCategoriesMessageRequestTypeDef

```python
# DescribeEventCategoriesMessageRequestTypeDef definition

class DescribeEventCategoriesMessageRequestTypeDef(TypedDict):
    SourceType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEventSubscriptionsMessageRequestTypeDef

```python
# DescribeEventSubscriptionsMessageRequestTypeDef definition

class DescribeEventSubscriptionsMessageRequestTypeDef(TypedDict):
    SubscriptionName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEventsMessageRequestTypeDef

```python
# DescribeEventsMessageRequestTypeDef definition

class DescribeEventsMessageRequestTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    EventCategories: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeExtensionPackAssociationsMessageRequestTypeDef

```python
# DescribeExtensionPackAssociationsMessageRequestTypeDef definition

class DescribeExtensionPackAssociationsMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeFleetAdvisorCollectorsRequestRequestTypeDef

```python
# DescribeFleetAdvisorCollectorsRequestRequestTypeDef definition

class DescribeFleetAdvisorCollectorsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeFleetAdvisorDatabasesRequestRequestTypeDef

```python
# DescribeFleetAdvisorDatabasesRequestRequestTypeDef definition

class DescribeFleetAdvisorDatabasesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef

```python
# DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef definition

class DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeFleetAdvisorSchemasRequestRequestTypeDef

```python
# DescribeFleetAdvisorSchemasRequestRequestTypeDef definition

class DescribeFleetAdvisorSchemasRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeInstanceProfilesMessageRequestTypeDef

```python
# DescribeInstanceProfilesMessageRequestTypeDef definition

class DescribeInstanceProfilesMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeMetadataModelAssessmentsMessageRequestTypeDef

```python
# DescribeMetadataModelAssessmentsMessageRequestTypeDef definition

class DescribeMetadataModelAssessmentsMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeMetadataModelConversionsMessageRequestTypeDef

```python
# DescribeMetadataModelConversionsMessageRequestTypeDef definition

class DescribeMetadataModelConversionsMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeMetadataModelExportsAsScriptMessageRequestTypeDef

```python
# DescribeMetadataModelExportsAsScriptMessageRequestTypeDef definition

class DescribeMetadataModelExportsAsScriptMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeMetadataModelExportsToTargetMessageRequestTypeDef

```python
# DescribeMetadataModelExportsToTargetMessageRequestTypeDef definition

class DescribeMetadataModelExportsToTargetMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeMetadataModelImportsMessageRequestTypeDef

```python
# DescribeMetadataModelImportsMessageRequestTypeDef definition

class DescribeMetadataModelImportsMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeMigrationProjectsMessageRequestTypeDef

```python
# DescribeMigrationProjectsMessageRequestTypeDef definition

class DescribeMigrationProjectsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribePendingMaintenanceActionsMessageRequestTypeDef

```python
# DescribePendingMaintenanceActionsMessageRequestTypeDef definition

class DescribePendingMaintenanceActionsMessageRequestTypeDef(TypedDict):
    ReplicationInstanceArn: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeRecommendationLimitationsRequestRequestTypeDef

```python
# DescribeRecommendationLimitationsRequestRequestTypeDef definition

class DescribeRecommendationLimitationsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeRecommendationsRequestRequestTypeDef

```python
# DescribeRecommendationsRequestRequestTypeDef definition

class DescribeRecommendationsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationConfigsMessageRequestTypeDef

```python
# DescribeReplicationConfigsMessageRequestTypeDef definition

class DescribeReplicationConfigsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationInstancesMessageRequestTypeDef

```python
# DescribeReplicationInstancesMessageRequestTypeDef definition

class DescribeReplicationInstancesMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationSubnetGroupsMessageRequestTypeDef

```python
# DescribeReplicationSubnetGroupsMessageRequestTypeDef definition

class DescribeReplicationSubnetGroupsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationTableStatisticsMessageRequestTypeDef

```python
# DescribeReplicationTableStatisticsMessageRequestTypeDef definition

class DescribeReplicationTableStatisticsMessageRequestTypeDef(TypedDict):
    ReplicationConfigArn: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef

```python
# DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef definition

class DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef

```python
# DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef definition

class DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationTasksMessageRequestTypeDef

```python
# DescribeReplicationTasksMessageRequestTypeDef definition

class DescribeReplicationTasksMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WithoutSettings: NotRequired[bool],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReplicationsMessageRequestTypeDef

```python
# DescribeReplicationsMessageRequestTypeDef definition

class DescribeReplicationsMessageRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeTableStatisticsMessageRequestTypeDef

```python
# DescribeTableStatisticsMessageRequestTypeDef definition

class DescribeTableStatisticsMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeCertificatesMessagePaginateTypeDef

```python
# DescribeCertificatesMessagePaginateTypeDef definition

class DescribeCertificatesMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConnectionsMessagePaginateTypeDef

```python
# DescribeConnectionsMessagePaginateTypeDef definition

class DescribeConnectionsMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDataMigrationsMessagePaginateTypeDef

```python
# DescribeDataMigrationsMessagePaginateTypeDef definition

class DescribeDataMigrationsMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    WithoutSettings: NotRequired[bool],
    WithoutStatistics: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEndpointTypesMessagePaginateTypeDef

```python
# DescribeEndpointTypesMessagePaginateTypeDef definition

class DescribeEndpointTypesMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEndpointsMessagePaginateTypeDef

```python
# DescribeEndpointsMessagePaginateTypeDef definition

class DescribeEndpointsMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventSubscriptionsMessagePaginateTypeDef

```python
# DescribeEventSubscriptionsMessagePaginateTypeDef definition

class DescribeEventSubscriptionsMessagePaginateTypeDef(TypedDict):
    SubscriptionName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsMessagePaginateTypeDef

```python
# DescribeEventsMessagePaginateTypeDef definition

class DescribeEventsMessagePaginateTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    EventCategories: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrderableReplicationInstancesMessagePaginateTypeDef

```python
# DescribeOrderableReplicationInstancesMessagePaginateTypeDef definition

class DescribeOrderableReplicationInstancesMessagePaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReplicationInstancesMessagePaginateTypeDef

```python
# DescribeReplicationInstancesMessagePaginateTypeDef definition

class DescribeReplicationInstancesMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReplicationSubnetGroupsMessagePaginateTypeDef

```python
# DescribeReplicationSubnetGroupsMessagePaginateTypeDef definition

class DescribeReplicationSubnetGroupsMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReplicationTaskAssessmentResultsMessagePaginateTypeDef

```python
# DescribeReplicationTaskAssessmentResultsMessagePaginateTypeDef definition

class DescribeReplicationTaskAssessmentResultsMessagePaginateTypeDef(TypedDict):
    ReplicationTaskArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReplicationTasksMessagePaginateTypeDef

```python
# DescribeReplicationTasksMessagePaginateTypeDef definition

class DescribeReplicationTasksMessagePaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    WithoutSettings: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSchemasMessagePaginateTypeDef

```python
# DescribeSchemasMessagePaginateTypeDef definition

class DescribeSchemasMessagePaginateTypeDef(TypedDict):
    EndpointArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTableStatisticsMessagePaginateTypeDef

```python
# DescribeTableStatisticsMessagePaginateTypeDef definition

class DescribeTableStatisticsMessagePaginateTypeDef(TypedDict):
    ReplicationTaskArn: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConnectionsMessageWaitTypeDef

```python
# DescribeConnectionsMessageWaitTypeDef definition

class DescribeConnectionsMessageWaitTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEndpointsMessageWaitTypeDef

```python
# DescribeEndpointsMessageWaitTypeDef definition

class DescribeEndpointsMessageWaitTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeReplicationInstancesMessageWaitTypeDef

```python
# DescribeReplicationInstancesMessageWaitTypeDef definition

class DescribeReplicationInstancesMessageWaitTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeReplicationTasksMessageWaitTypeDef

```python
# DescribeReplicationTasksMessageWaitTypeDef definition

class DescribeReplicationTasksMessageWaitTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WithoutSettings: NotRequired[bool],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEndpointSettingsResponseTypeDef

```python
# DescribeEndpointSettingsResponseTypeDef definition

class DescribeEndpointSettingsResponseTypeDef(TypedDict):
    Marker: str,
    EndpointSettings: List[EndpointSettingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointSettingTypeDef](./type_defs.md#endpointsettingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointTypesResponseTypeDef

```python
# DescribeEndpointTypesResponseTypeDef definition

class DescribeEndpointTypesResponseTypeDef(TypedDict):
    Marker: str,
    SupportedEndpointTypes: List[SupportedEndpointTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SupportedEndpointTypeTypeDef](./type_defs.md#supportedendpointtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEngineVersionsResponseTypeDef

```python
# DescribeEngineVersionsResponseTypeDef definition

class DescribeEngineVersionsResponseTypeDef(TypedDict):
    EngineVersions: List[EngineVersionTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventCategoriesResponseTypeDef

```python
# DescribeEventCategoriesResponseTypeDef definition

class DescribeEventCategoriesResponseTypeDef(TypedDict):
    EventCategoryGroupList: List[EventCategoryGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventCategoryGroupTypeDef](./type_defs.md#eventcategorygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventsResponseTypeDef

```python
# DescribeEventsResponseTypeDef definition

class DescribeEventsResponseTypeDef(TypedDict):
    Marker: str,
    Events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetAdvisorLsaAnalysisResponseTypeDef

```python
# DescribeFleetAdvisorLsaAnalysisResponseTypeDef definition

class DescribeFleetAdvisorLsaAnalysisResponseTypeDef(TypedDict):
    Analysis: List[FleetAdvisorLsaAnalysisResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetAdvisorLsaAnalysisResponseTypeDef](./type_defs.md#fleetadvisorlsaanalysisresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef

```python
# DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef definition

class DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef(TypedDict):
    FleetAdvisorSchemaObjects: List[FleetAdvisorSchemaObjectResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetAdvisorSchemaObjectResponseTypeDef](./type_defs.md#fleetadvisorschemaobjectresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrderableReplicationInstancesResponseTypeDef

```python
# DescribeOrderableReplicationInstancesResponseTypeDef definition

class DescribeOrderableReplicationInstancesResponseTypeDef(TypedDict):
    OrderableReplicationInstances: List[OrderableReplicationInstanceTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderableReplicationInstanceTypeDef](./type_defs.md#orderablereplicationinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRecommendationLimitationsResponseTypeDef

```python
# DescribeRecommendationLimitationsResponseTypeDef definition

class DescribeRecommendationLimitationsResponseTypeDef(TypedDict):
    Limitations: List[LimitationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LimitationTypeDef](./type_defs.md#limitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRefreshSchemasStatusResponseTypeDef

```python
# DescribeRefreshSchemasStatusResponseTypeDef definition

class DescribeRefreshSchemasStatusResponseTypeDef(TypedDict):
    RefreshSchemasStatus: RefreshSchemasStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RefreshSchemasStatusTypeDef](./type_defs.md#refreshschemasstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RefreshSchemasResponseTypeDef

```python
# RefreshSchemasResponseTypeDef definition

class RefreshSchemasResponseTypeDef(TypedDict):
    RefreshSchemasStatus: RefreshSchemasStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RefreshSchemasStatusTypeDef](./type_defs.md#refreshschemasstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationInstanceTaskLogsResponseTypeDef

```python
# DescribeReplicationInstanceTaskLogsResponseTypeDef definition

class DescribeReplicationInstanceTaskLogsResponseTypeDef(TypedDict):
    ReplicationInstanceArn: str,
    ReplicationInstanceTaskLogs: List[ReplicationInstanceTaskLogTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationInstanceTaskLogTypeDef](./type_defs.md#replicationinstancetasklogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationTableStatisticsResponseTypeDef

```python
# DescribeReplicationTableStatisticsResponseTypeDef definition

class DescribeReplicationTableStatisticsResponseTypeDef(TypedDict):
    ReplicationConfigArn: str,
    Marker: str,
    ReplicationTableStatistics: List[TableStatisticsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableStatisticsTypeDef](./type_defs.md#tablestatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableStatisticsResponseTypeDef

```python
# DescribeTableStatisticsResponseTypeDef definition

class DescribeTableStatisticsResponseTypeDef(TypedDict):
    ReplicationTaskArn: str,
    TableStatistics: List[TableStatisticsTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableStatisticsTypeDef](./type_defs.md#tablestatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationTaskAssessmentResultsResponseTypeDef

```python
# DescribeReplicationTaskAssessmentResultsResponseTypeDef definition

class DescribeReplicationTaskAssessmentResultsResponseTypeDef(TypedDict):
    Marker: str,
    BucketName: str,
    ReplicationTaskAssessmentResults: List[ReplicationTaskAssessmentResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskAssessmentResultTypeDef](./type_defs.md#replicationtaskassessmentresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationTaskIndividualAssessmentsResponseTypeDef

```python
# DescribeReplicationTaskIndividualAssessmentsResponseTypeDef definition

class DescribeReplicationTaskIndividualAssessmentsResponseTypeDef(TypedDict):
    Marker: str,
    ReplicationTaskIndividualAssessments: List[ReplicationTaskIndividualAssessmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskIndividualAssessmentTypeDef](./type_defs.md#replicationtaskindividualassessmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    EndpointIdentifier: NotRequired[str],
    EndpointType: NotRequired[ReplicationEndpointTypeValueType],  # (1)
    EngineName: NotRequired[str],
    EngineDisplayName: NotRequired[str],
    Username: NotRequired[str],
    ServerName: NotRequired[str],
    Port: NotRequired[int],
    DatabaseName: NotRequired[str],
    ExtraConnectionAttributes: NotRequired[str],
    Status: NotRequired[str],
    KmsKeyId: NotRequired[str],
    EndpointArn: NotRequired[str],
    CertificateArn: NotRequired[str],
    SslMode: NotRequired[DmsSslModeValueType],  # (2)
    ServiceAccessRoleArn: NotRequired[str],
    ExternalTableDefinition: NotRequired[str],
    ExternalId: NotRequired[str],
    DynamoDbSettings: NotRequired[DynamoDbSettingsTypeDef],  # (3)
    S3Settings: NotRequired[S3SettingsTypeDef],  # (4)
    DmsTransferSettings: NotRequired[DmsTransferSettingsTypeDef],  # (5)
    MongoDbSettings: NotRequired[MongoDbSettingsTypeDef],  # (6)
    KinesisSettings: NotRequired[KinesisSettingsTypeDef],  # (7)
    KafkaSettings: NotRequired[KafkaSettingsTypeDef],  # (8)
    ElasticsearchSettings: NotRequired[ElasticsearchSettingsTypeDef],  # (9)
    NeptuneSettings: NotRequired[NeptuneSettingsTypeDef],  # (10)
    RedshiftSettings: NotRequired[RedshiftSettingsTypeDef],  # (11)
    PostgreSQLSettings: NotRequired[PostgreSQLSettingsTypeDef],  # (12)
    MySQLSettings: NotRequired[MySQLSettingsTypeDef],  # (13)
    OracleSettings: NotRequired[OracleSettingsOutputTypeDef],  # (14)
    SybaseSettings: NotRequired[SybaseSettingsTypeDef],  # (15)
    MicrosoftSQLServerSettings: NotRequired[MicrosoftSQLServerSettingsTypeDef],  # (16)
    IBMDb2Settings: NotRequired[IBMDb2SettingsTypeDef],  # (17)
    DocDbSettings: NotRequired[DocDbSettingsTypeDef],  # (18)
    RedisSettings: NotRequired[RedisSettingsTypeDef],  # (19)
    GcpMySQLSettings: NotRequired[GcpMySQLSettingsTypeDef],  # (20)
    TimestreamSettings: NotRequired[TimestreamSettingsTypeDef],  # (21)
```

1. See [:material-code-brackets: ReplicationEndpointTypeValueType](./literals.md#replicationendpointtypevaluetype) 
2. See [:material-code-brackets: DmsSslModeValueType](./literals.md#dmssslmodevaluetype) 
3. See [:material-code-braces: DynamoDbSettingsTypeDef](./type_defs.md#dynamodbsettingstypedef) 
4. See [:material-code-braces: S3SettingsTypeDef](./type_defs.md#s3settingstypedef) 
5. See [:material-code-braces: DmsTransferSettingsTypeDef](./type_defs.md#dmstransfersettingstypedef) 
6. See [:material-code-braces: MongoDbSettingsTypeDef](./type_defs.md#mongodbsettingstypedef) 
7. See [:material-code-braces: KinesisSettingsTypeDef](./type_defs.md#kinesissettingstypedef) 
8. See [:material-code-braces: KafkaSettingsTypeDef](./type_defs.md#kafkasettingstypedef) 
9. See [:material-code-braces: ElasticsearchSettingsTypeDef](./type_defs.md#elasticsearchsettingstypedef) 
10. See [:material-code-braces: NeptuneSettingsTypeDef](./type_defs.md#neptunesettingstypedef) 
11. See [:material-code-braces: RedshiftSettingsTypeDef](./type_defs.md#redshiftsettingstypedef) 
12. See [:material-code-braces: PostgreSQLSettingsTypeDef](./type_defs.md#postgresqlsettingstypedef) 
13. See [:material-code-braces: MySQLSettingsTypeDef](./type_defs.md#mysqlsettingstypedef) 
14. See [:material-code-braces: OracleSettingsOutputTypeDef](./type_defs.md#oraclesettingsoutputtypedef) 
15. See [:material-code-braces: SybaseSettingsTypeDef](./type_defs.md#sybasesettingstypedef) 
16. See [:material-code-braces: MicrosoftSQLServerSettingsTypeDef](./type_defs.md#microsoftsqlserversettingstypedef) 
17. See [:material-code-braces: IBMDb2SettingsTypeDef](./type_defs.md#ibmdb2settingstypedef) 
18. See [:material-code-braces: DocDbSettingsTypeDef](./type_defs.md#docdbsettingstypedef) 
19. See [:material-code-braces: RedisSettingsTypeDef](./type_defs.md#redissettingstypedef) 
20. See [:material-code-braces: GcpMySQLSettingsTypeDef](./type_defs.md#gcpmysqlsettingstypedef) 
21. See [:material-code-braces: TimestreamSettingsTypeDef](./type_defs.md#timestreamsettingstypedef) 
## ExportMetadataModelAssessmentResponseTypeDef

```python
# ExportMetadataModelAssessmentResponseTypeDef definition

class ExportMetadataModelAssessmentResponseTypeDef(TypedDict):
    PdfReport: ExportMetadataModelAssessmentResultEntryTypeDef,  # (1)
    CsvReport: ExportMetadataModelAssessmentResultEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ExportMetadataModelAssessmentResultEntryTypeDef](./type_defs.md#exportmetadatamodelassessmentresultentrytypedef) 
2. See [:material-code-braces: ExportMetadataModelAssessmentResultEntryTypeDef](./type_defs.md#exportmetadatamodelassessmentresultentrytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourcePendingMaintenanceActionsTypeDef

```python
# ResourcePendingMaintenanceActionsTypeDef definition

class ResourcePendingMaintenanceActionsTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    PendingMaintenanceActionDetails: NotRequired[List[PendingMaintenanceActionTypeDef]],  # (1)
```

1. See [:material-code-braces: PendingMaintenanceActionTypeDef](./type_defs.md#pendingmaintenanceactiontypedef) 
## RdsRecommendationTypeDef

```python
# RdsRecommendationTypeDef definition

class RdsRecommendationTypeDef(TypedDict):
    RequirementsToTarget: NotRequired[RdsRequirementsTypeDef],  # (1)
    TargetConfiguration: NotRequired[RdsConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RdsRequirementsTypeDef](./type_defs.md#rdsrequirementstypedef) 
2. See [:material-code-braces: RdsConfigurationTypeDef](./type_defs.md#rdsconfigurationtypedef) 
## StartRecommendationsRequestEntryTypeDef

```python
# StartRecommendationsRequestEntryTypeDef definition

class StartRecommendationsRequestEntryTypeDef(TypedDict):
    DatabaseId: str,
    Settings: RecommendationSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: RecommendationSettingsTypeDef](./type_defs.md#recommendationsettingstypedef) 
## StartRecommendationsRequestRequestTypeDef

```python
# StartRecommendationsRequestRequestTypeDef definition

class StartRecommendationsRequestRequestTypeDef(TypedDict):
    DatabaseId: str,
    Settings: RecommendationSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: RecommendationSettingsTypeDef](./type_defs.md#recommendationsettingstypedef) 
## ReloadReplicationTablesMessageRequestTypeDef

```python
# ReloadReplicationTablesMessageRequestTypeDef definition

class ReloadReplicationTablesMessageRequestTypeDef(TypedDict):
    ReplicationConfigArn: str,
    TablesToReload: Sequence[TableToReloadTypeDef],  # (1)
    ReloadOption: NotRequired[ReloadOptionValueType],  # (2)
```

1. See [:material-code-braces: TableToReloadTypeDef](./type_defs.md#tabletoreloadtypedef) 
2. See [:material-code-brackets: ReloadOptionValueType](./literals.md#reloadoptionvaluetype) 
## ReloadTablesMessageRequestTypeDef

```python
# ReloadTablesMessageRequestTypeDef definition

class ReloadTablesMessageRequestTypeDef(TypedDict):
    ReplicationTaskArn: str,
    TablesToReload: Sequence[TableToReloadTypeDef],  # (1)
    ReloadOption: NotRequired[ReloadOptionValueType],  # (2)
```

1. See [:material-code-braces: TableToReloadTypeDef](./type_defs.md#tabletoreloadtypedef) 
2. See [:material-code-brackets: ReloadOptionValueType](./literals.md#reloadoptionvaluetype) 
## ReplicationTypeDef

```python
# ReplicationTypeDef definition

class ReplicationTypeDef(TypedDict):
    ReplicationConfigIdentifier: NotRequired[str],
    ReplicationConfigArn: NotRequired[str],
    SourceEndpointArn: NotRequired[str],
    TargetEndpointArn: NotRequired[str],
    ReplicationType: NotRequired[MigrationTypeValueType],  # (1)
    Status: NotRequired[str],
    ProvisionData: NotRequired[ProvisionDataTypeDef],  # (2)
    StopReason: NotRequired[str],
    FailureMessages: NotRequired[List[str]],
    ReplicationStats: NotRequired[ReplicationStatsTypeDef],  # (3)
    StartReplicationType: NotRequired[str],
    CdcStartTime: NotRequired[datetime],
    CdcStartPosition: NotRequired[str],
    CdcStopPosition: NotRequired[str],
    RecoveryCheckpoint: NotRequired[str],
    ReplicationCreateTime: NotRequired[datetime],
    ReplicationUpdateTime: NotRequired[datetime],
    ReplicationLastStopTime: NotRequired[datetime],
    ReplicationDeprovisionTime: NotRequired[datetime],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: ProvisionDataTypeDef](./type_defs.md#provisiondatatypedef) 
3. See [:material-code-braces: ReplicationStatsTypeDef](./type_defs.md#replicationstatstypedef) 
## ReplicationTaskAssessmentRunTypeDef

```python
# ReplicationTaskAssessmentRunTypeDef definition

class ReplicationTaskAssessmentRunTypeDef(TypedDict):
    ReplicationTaskAssessmentRunArn: NotRequired[str],
    ReplicationTaskArn: NotRequired[str],
    Status: NotRequired[str],
    ReplicationTaskAssessmentRunCreationDate: NotRequired[datetime],
    AssessmentProgress: NotRequired[ReplicationTaskAssessmentRunProgressTypeDef],  # (1)
    LastFailureMessage: NotRequired[str],
    ServiceAccessRoleArn: NotRequired[str],
    ResultLocationBucket: NotRequired[str],
    ResultLocationFolder: NotRequired[str],
    ResultEncryptionMode: NotRequired[str],
    ResultKmsKeyArn: NotRequired[str],
    AssessmentRunName: NotRequired[str],
    IsLatestTaskAssessmentRun: NotRequired[bool],
    ResultStatistic: NotRequired[ReplicationTaskAssessmentRunResultStatisticTypeDef],  # (2)
```

1. See [:material-code-braces: ReplicationTaskAssessmentRunProgressTypeDef](./type_defs.md#replicationtaskassessmentrunprogresstypedef) 
2. See [:material-code-braces: ReplicationTaskAssessmentRunResultStatisticTypeDef](./type_defs.md#replicationtaskassessmentrunresultstatistictypedef) 
## ReplicationTaskTypeDef

```python
# ReplicationTaskTypeDef definition

class ReplicationTaskTypeDef(TypedDict):
    ReplicationTaskIdentifier: NotRequired[str],
    SourceEndpointArn: NotRequired[str],
    TargetEndpointArn: NotRequired[str],
    ReplicationInstanceArn: NotRequired[str],
    MigrationType: NotRequired[MigrationTypeValueType],  # (1)
    TableMappings: NotRequired[str],
    ReplicationTaskSettings: NotRequired[str],
    Status: NotRequired[str],
    LastFailureMessage: NotRequired[str],
    StopReason: NotRequired[str],
    ReplicationTaskCreationDate: NotRequired[datetime],
    ReplicationTaskStartDate: NotRequired[datetime],
    CdcStartPosition: NotRequired[str],
    CdcStopPosition: NotRequired[str],
    RecoveryCheckpoint: NotRequired[str],
    ReplicationTaskArn: NotRequired[str],
    ReplicationTaskStats: NotRequired[ReplicationTaskStatsTypeDef],  # (2)
    TaskData: NotRequired[str],
    TargetReplicationInstanceArn: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: ReplicationTaskStatsTypeDef](./type_defs.md#replicationtaskstatstypedef) 
## SchemaResponseTypeDef

```python
# SchemaResponseTypeDef definition

class SchemaResponseTypeDef(TypedDict):
    CodeLineCount: NotRequired[int],
    CodeSize: NotRequired[int],
    Complexity: NotRequired[str],
    Server: NotRequired[ServerShortInfoResponseTypeDef],  # (1)
    DatabaseInstance: NotRequired[DatabaseShortInfoResponseTypeDef],  # (2)
    SchemaId: NotRequired[str],
    SchemaName: NotRequired[str],
    OriginalSchema: NotRequired[SchemaShortInfoResponseTypeDef],  # (3)
    Similarity: NotRequired[float],
```

1. See [:material-code-braces: ServerShortInfoResponseTypeDef](./type_defs.md#servershortinforesponsetypedef) 
2. See [:material-code-braces: DatabaseShortInfoResponseTypeDef](./type_defs.md#databaseshortinforesponsetypedef) 
3. See [:material-code-braces: SchemaShortInfoResponseTypeDef](./type_defs.md#schemashortinforesponsetypedef) 
## ReplicationSubnetGroupTypeDef

```python
# ReplicationSubnetGroupTypeDef definition

class ReplicationSubnetGroupTypeDef(TypedDict):
    ReplicationSubnetGroupIdentifier: NotRequired[str],
    ReplicationSubnetGroupDescription: NotRequired[str],
    VpcId: NotRequired[str],
    SubnetGroupStatus: NotRequired[str],
    Subnets: NotRequired[List[SubnetTypeDef]],  # (1)
    SupportedNetworkTypes: NotRequired[List[str]],
```

1. See [:material-code-braces: SubnetTypeDef](./type_defs.md#subnettypedef) 
## DescribeFleetAdvisorCollectorsResponseTypeDef

```python
# DescribeFleetAdvisorCollectorsResponseTypeDef definition

class DescribeFleetAdvisorCollectorsResponseTypeDef(TypedDict):
    Collectors: List[CollectorResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CollectorResponseTypeDef](./type_defs.md#collectorresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicationConfigResponseTypeDef

```python
# CreateReplicationConfigResponseTypeDef definition

class CreateReplicationConfigResponseTypeDef(TypedDict):
    ReplicationConfig: ReplicationConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteReplicationConfigResponseTypeDef

```python
# DeleteReplicationConfigResponseTypeDef definition

class DeleteReplicationConfigResponseTypeDef(TypedDict):
    ReplicationConfig: ReplicationConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationConfigsResponseTypeDef

```python
# DescribeReplicationConfigsResponseTypeDef definition

class DescribeReplicationConfigsResponseTypeDef(TypedDict):
    Marker: str,
    ReplicationConfigs: List[ReplicationConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyReplicationConfigResponseTypeDef

```python
# ModifyReplicationConfigResponseTypeDef definition

class ModifyReplicationConfigResponseTypeDef(TypedDict):
    ReplicationConfig: ReplicationConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDataMigrationMessageRequestTypeDef

```python
# ModifyDataMigrationMessageRequestTypeDef definition

class ModifyDataMigrationMessageRequestTypeDef(TypedDict):
    DataMigrationIdentifier: str,
    DataMigrationName: NotRequired[str],
    EnableCloudwatchLogs: NotRequired[bool],
    ServiceAccessRoleArn: NotRequired[str],
    DataMigrationType: NotRequired[MigrationTypeValueType],  # (1)
    SourceDataSettings: NotRequired[Sequence[SourceDataSettingTypeDef]],  # (2)
    NumberOfJobs: NotRequired[int],
    SelectionRules: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: SourceDataSettingTypeDef](./type_defs.md#sourcedatasettingtypedef) 
## CreateDataMigrationResponseTypeDef

```python
# CreateDataMigrationResponseTypeDef definition

class CreateDataMigrationResponseTypeDef(TypedDict):
    DataMigration: DataMigrationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataMigrationTypeDef](./type_defs.md#datamigrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataMigrationResponseTypeDef

```python
# DeleteDataMigrationResponseTypeDef definition

class DeleteDataMigrationResponseTypeDef(TypedDict):
    DataMigration: DataMigrationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataMigrationTypeDef](./type_defs.md#datamigrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataMigrationsResponseTypeDef

```python
# DescribeDataMigrationsResponseTypeDef definition

class DescribeDataMigrationsResponseTypeDef(TypedDict):
    DataMigrations: List[DataMigrationTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataMigrationTypeDef](./type_defs.md#datamigrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDataMigrationResponseTypeDef

```python
# ModifyDataMigrationResponseTypeDef definition

class ModifyDataMigrationResponseTypeDef(TypedDict):
    DataMigration: DataMigrationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataMigrationTypeDef](./type_defs.md#datamigrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataMigrationResponseTypeDef

```python
# StartDataMigrationResponseTypeDef definition

class StartDataMigrationResponseTypeDef(TypedDict):
    DataMigration: DataMigrationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataMigrationTypeDef](./type_defs.md#datamigrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDataMigrationResponseTypeDef

```python
# StopDataMigrationResponseTypeDef definition

class StopDataMigrationResponseTypeDef(TypedDict):
    DataMigration: DataMigrationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataMigrationTypeDef](./type_defs.md#datamigrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMigrationProjectResponseTypeDef

```python
# CreateMigrationProjectResponseTypeDef definition

class CreateMigrationProjectResponseTypeDef(TypedDict):
    MigrationProject: MigrationProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MigrationProjectTypeDef](./type_defs.md#migrationprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMigrationProjectResponseTypeDef

```python
# DeleteMigrationProjectResponseTypeDef definition

class DeleteMigrationProjectResponseTypeDef(TypedDict):
    MigrationProject: MigrationProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MigrationProjectTypeDef](./type_defs.md#migrationprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMigrationProjectsResponseTypeDef

```python
# DescribeMigrationProjectsResponseTypeDef definition

class DescribeMigrationProjectsResponseTypeDef(TypedDict):
    Marker: str,
    MigrationProjects: List[MigrationProjectTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MigrationProjectTypeDef](./type_defs.md#migrationprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyMigrationProjectResponseTypeDef

```python
# ModifyMigrationProjectResponseTypeDef definition

class ModifyMigrationProjectResponseTypeDef(TypedDict):
    MigrationProject: MigrationProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MigrationProjectTypeDef](./type_defs.md#migrationprojecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataProviderMessageRequestTypeDef

```python
# CreateDataProviderMessageRequestTypeDef definition

class CreateDataProviderMessageRequestTypeDef(TypedDict):
    Engine: str,
    Settings: DataProviderSettingsTypeDef,  # (1)
    DataProviderName: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DataProviderSettingsTypeDef](./type_defs.md#dataprovidersettingstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DataProviderTypeDef

```python
# DataProviderTypeDef definition

class DataProviderTypeDef(TypedDict):
    DataProviderName: NotRequired[str],
    DataProviderArn: NotRequired[str],
    DataProviderCreationTime: NotRequired[datetime],
    Description: NotRequired[str],
    Engine: NotRequired[str],
    Settings: NotRequired[DataProviderSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: DataProviderSettingsTypeDef](./type_defs.md#dataprovidersettingstypedef) 
## ModifyDataProviderMessageRequestTypeDef

```python
# ModifyDataProviderMessageRequestTypeDef definition

class ModifyDataProviderMessageRequestTypeDef(TypedDict):
    DataProviderIdentifier: str,
    DataProviderName: NotRequired[str],
    Description: NotRequired[str],
    Engine: NotRequired[str],
    ExactSettings: NotRequired[bool],
    Settings: NotRequired[DataProviderSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: DataProviderSettingsTypeDef](./type_defs.md#dataprovidersettingstypedef) 
## DescribeFleetAdvisorDatabasesResponseTypeDef

```python
# DescribeFleetAdvisorDatabasesResponseTypeDef definition

class DescribeFleetAdvisorDatabasesResponseTypeDef(TypedDict):
    Databases: List[DatabaseResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatabaseResponseTypeDef](./type_defs.md#databaseresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaConversionRequestTypeDef

```python
# SchemaConversionRequestTypeDef definition

class SchemaConversionRequestTypeDef(TypedDict):
    Status: NotRequired[str],
    RequestIdentifier: NotRequired[str],
    MigrationProjectArn: NotRequired[str],
    Error: NotRequired[ErrorDetailsTypeDef],  # (1)
    ExportSqlDetails: NotRequired[ExportSqlDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
2. See [:material-code-braces: ExportSqlDetailsTypeDef](./type_defs.md#exportsqldetailstypedef) 
## CreateEndpointResponseTypeDef

```python
# CreateEndpointResponseTypeDef definition

class CreateEndpointResponseTypeDef(TypedDict):
    Endpoint: EndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEndpointResponseTypeDef

```python
# DeleteEndpointResponseTypeDef definition

class DeleteEndpointResponseTypeDef(TypedDict):
    Endpoint: EndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointsResponseTypeDef

```python
# DescribeEndpointsResponseTypeDef definition

class DescribeEndpointsResponseTypeDef(TypedDict):
    Marker: str,
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyEndpointResponseTypeDef

```python
# ModifyEndpointResponseTypeDef definition

class ModifyEndpointResponseTypeDef(TypedDict):
    Endpoint: EndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplyPendingMaintenanceActionResponseTypeDef

```python
# ApplyPendingMaintenanceActionResponseTypeDef definition

class ApplyPendingMaintenanceActionResponseTypeDef(TypedDict):
    ResourcePendingMaintenanceActions: ResourcePendingMaintenanceActionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePendingMaintenanceActionsTypeDef](./type_defs.md#resourcependingmaintenanceactionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePendingMaintenanceActionsResponseTypeDef

```python
# DescribePendingMaintenanceActionsResponseTypeDef definition

class DescribePendingMaintenanceActionsResponseTypeDef(TypedDict):
    PendingMaintenanceActions: List[ResourcePendingMaintenanceActionsTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePendingMaintenanceActionsTypeDef](./type_defs.md#resourcependingmaintenanceactionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecommendationDataTypeDef

```python
# RecommendationDataTypeDef definition

class RecommendationDataTypeDef(TypedDict):
    RdsEngine: NotRequired[RdsRecommendationTypeDef],  # (1)
```

1. See [:material-code-braces: RdsRecommendationTypeDef](./type_defs.md#rdsrecommendationtypedef) 
## BatchStartRecommendationsRequestRequestTypeDef

```python
# BatchStartRecommendationsRequestRequestTypeDef definition

class BatchStartRecommendationsRequestRequestTypeDef(TypedDict):
    Data: NotRequired[Sequence[StartRecommendationsRequestEntryTypeDef]],  # (1)
```

1. See [:material-code-braces: StartRecommendationsRequestEntryTypeDef](./type_defs.md#startrecommendationsrequestentrytypedef) 
## DescribeReplicationsResponseTypeDef

```python
# DescribeReplicationsResponseTypeDef definition

class DescribeReplicationsResponseTypeDef(TypedDict):
    Marker: str,
    Replications: List[ReplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTypeDef](./type_defs.md#replicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReplicationResponseTypeDef

```python
# StartReplicationResponseTypeDef definition

class StartReplicationResponseTypeDef(TypedDict):
    Replication: ReplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTypeDef](./type_defs.md#replicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopReplicationResponseTypeDef

```python
# StopReplicationResponseTypeDef definition

class StopReplicationResponseTypeDef(TypedDict):
    Replication: ReplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTypeDef](./type_defs.md#replicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelReplicationTaskAssessmentRunResponseTypeDef

```python
# CancelReplicationTaskAssessmentRunResponseTypeDef definition

class CancelReplicationTaskAssessmentRunResponseTypeDef(TypedDict):
    ReplicationTaskAssessmentRun: ReplicationTaskAssessmentRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskAssessmentRunTypeDef](./type_defs.md#replicationtaskassessmentruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteReplicationTaskAssessmentRunResponseTypeDef

```python
# DeleteReplicationTaskAssessmentRunResponseTypeDef definition

class DeleteReplicationTaskAssessmentRunResponseTypeDef(TypedDict):
    ReplicationTaskAssessmentRun: ReplicationTaskAssessmentRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskAssessmentRunTypeDef](./type_defs.md#replicationtaskassessmentruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationTaskAssessmentRunsResponseTypeDef

```python
# DescribeReplicationTaskAssessmentRunsResponseTypeDef definition

class DescribeReplicationTaskAssessmentRunsResponseTypeDef(TypedDict):
    Marker: str,
    ReplicationTaskAssessmentRuns: List[ReplicationTaskAssessmentRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskAssessmentRunTypeDef](./type_defs.md#replicationtaskassessmentruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReplicationTaskAssessmentRunResponseTypeDef

```python
# StartReplicationTaskAssessmentRunResponseTypeDef definition

class StartReplicationTaskAssessmentRunResponseTypeDef(TypedDict):
    ReplicationTaskAssessmentRun: ReplicationTaskAssessmentRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskAssessmentRunTypeDef](./type_defs.md#replicationtaskassessmentruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicationTaskResponseTypeDef

```python
# CreateReplicationTaskResponseTypeDef definition

class CreateReplicationTaskResponseTypeDef(TypedDict):
    ReplicationTask: ReplicationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteReplicationTaskResponseTypeDef

```python
# DeleteReplicationTaskResponseTypeDef definition

class DeleteReplicationTaskResponseTypeDef(TypedDict):
    ReplicationTask: ReplicationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationTasksResponseTypeDef

```python
# DescribeReplicationTasksResponseTypeDef definition

class DescribeReplicationTasksResponseTypeDef(TypedDict):
    Marker: str,
    ReplicationTasks: List[ReplicationTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyReplicationTaskResponseTypeDef

```python
# ModifyReplicationTaskResponseTypeDef definition

class ModifyReplicationTaskResponseTypeDef(TypedDict):
    ReplicationTask: ReplicationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MoveReplicationTaskResponseTypeDef

```python
# MoveReplicationTaskResponseTypeDef definition

class MoveReplicationTaskResponseTypeDef(TypedDict):
    ReplicationTask: ReplicationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReplicationTaskAssessmentResponseTypeDef

```python
# StartReplicationTaskAssessmentResponseTypeDef definition

class StartReplicationTaskAssessmentResponseTypeDef(TypedDict):
    ReplicationTask: ReplicationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReplicationTaskResponseTypeDef

```python
# StartReplicationTaskResponseTypeDef definition

class StartReplicationTaskResponseTypeDef(TypedDict):
    ReplicationTask: ReplicationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopReplicationTaskResponseTypeDef

```python
# StopReplicationTaskResponseTypeDef definition

class StopReplicationTaskResponseTypeDef(TypedDict):
    ReplicationTask: ReplicationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationTaskTypeDef](./type_defs.md#replicationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetAdvisorSchemasResponseTypeDef

```python
# DescribeFleetAdvisorSchemasResponseTypeDef definition

class DescribeFleetAdvisorSchemasResponseTypeDef(TypedDict):
    FleetAdvisorSchemas: List[SchemaResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaResponseTypeDef](./type_defs.md#schemaresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicationSubnetGroupResponseTypeDef

```python
# CreateReplicationSubnetGroupResponseTypeDef definition

class CreateReplicationSubnetGroupResponseTypeDef(TypedDict):
    ReplicationSubnetGroup: ReplicationSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationSubnetGroupTypeDef](./type_defs.md#replicationsubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationSubnetGroupsResponseTypeDef

```python
# DescribeReplicationSubnetGroupsResponseTypeDef definition

class DescribeReplicationSubnetGroupsResponseTypeDef(TypedDict):
    Marker: str,
    ReplicationSubnetGroups: List[ReplicationSubnetGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationSubnetGroupTypeDef](./type_defs.md#replicationsubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyReplicationSubnetGroupResponseTypeDef

```python
# ModifyReplicationSubnetGroupResponseTypeDef definition

class ModifyReplicationSubnetGroupResponseTypeDef(TypedDict):
    ReplicationSubnetGroup: ReplicationSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationSubnetGroupTypeDef](./type_defs.md#replicationsubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationInstanceTypeDef

```python
# ReplicationInstanceTypeDef definition

class ReplicationInstanceTypeDef(TypedDict):
    ReplicationInstanceIdentifier: NotRequired[str],
    ReplicationInstanceClass: NotRequired[str],
    ReplicationInstanceStatus: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    InstanceCreateTime: NotRequired[datetime],
    VpcSecurityGroups: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (1)
    AvailabilityZone: NotRequired[str],
    ReplicationSubnetGroup: NotRequired[ReplicationSubnetGroupTypeDef],  # (2)
    PreferredMaintenanceWindow: NotRequired[str],
    PendingModifiedValues: NotRequired[ReplicationPendingModifiedValuesTypeDef],  # (3)
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    ReplicationInstanceArn: NotRequired[str],
    ReplicationInstancePublicIpAddress: NotRequired[str],
    ReplicationInstancePrivateIpAddress: NotRequired[str],
    ReplicationInstancePublicIpAddresses: NotRequired[List[str]],
    ReplicationInstancePrivateIpAddresses: NotRequired[List[str]],
    ReplicationInstanceIpv6Addresses: NotRequired[List[str]],
    PubliclyAccessible: NotRequired[bool],
    SecondaryAvailabilityZone: NotRequired[str],
    FreeUntil: NotRequired[datetime],
    DnsNameServers: NotRequired[str],
    NetworkType: NotRequired[str],
    KerberosAuthenticationSettings: NotRequired[KerberosAuthenticationSettingsTypeDef],  # (4)
```

1. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
2. See [:material-code-braces: ReplicationSubnetGroupTypeDef](./type_defs.md#replicationsubnetgrouptypedef) 
3. See [:material-code-braces: ReplicationPendingModifiedValuesTypeDef](./type_defs.md#replicationpendingmodifiedvaluestypedef) 
4. See [:material-code-braces: KerberosAuthenticationSettingsTypeDef](./type_defs.md#kerberosauthenticationsettingstypedef) 
## CreateDataMigrationMessageRequestTypeDef

```python
# CreateDataMigrationMessageRequestTypeDef definition

class CreateDataMigrationMessageRequestTypeDef(TypedDict):
    MigrationProjectIdentifier: str,
    DataMigrationType: MigrationTypeValueType,  # (1)
    ServiceAccessRoleArn: str,
    DataMigrationName: NotRequired[str],
    EnableCloudwatchLogs: NotRequired[bool],
    SourceDataSettings: NotRequired[Sequence[SourceDataSettingUnionTypeDef]],  # (2)
    NumberOfJobs: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    SelectionRules: NotRequired[str],
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: SourceDataSettingTypeDef](./type_defs.md#sourcedatasettingtypedef) [:material-code-braces: SourceDataSettingOutputTypeDef](./type_defs.md#sourcedatasettingoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDataProviderResponseTypeDef

```python
# CreateDataProviderResponseTypeDef definition

class CreateDataProviderResponseTypeDef(TypedDict):
    DataProvider: DataProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataProviderTypeDef](./type_defs.md#dataprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataProviderResponseTypeDef

```python
# DeleteDataProviderResponseTypeDef definition

class DeleteDataProviderResponseTypeDef(TypedDict):
    DataProvider: DataProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataProviderTypeDef](./type_defs.md#dataprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataProvidersResponseTypeDef

```python
# DescribeDataProvidersResponseTypeDef definition

class DescribeDataProvidersResponseTypeDef(TypedDict):
    Marker: str,
    DataProviders: List[DataProviderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataProviderTypeDef](./type_defs.md#dataprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDataProviderResponseTypeDef

```python
# ModifyDataProviderResponseTypeDef definition

class ModifyDataProviderResponseTypeDef(TypedDict):
    DataProvider: DataProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataProviderTypeDef](./type_defs.md#dataprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExtensionPackAssociationsResponseTypeDef

```python
# DescribeExtensionPackAssociationsResponseTypeDef definition

class DescribeExtensionPackAssociationsResponseTypeDef(TypedDict):
    Marker: str,
    Requests: List[SchemaConversionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaConversionRequestTypeDef](./type_defs.md#schemaconversionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMetadataModelAssessmentsResponseTypeDef

```python
# DescribeMetadataModelAssessmentsResponseTypeDef definition

class DescribeMetadataModelAssessmentsResponseTypeDef(TypedDict):
    Marker: str,
    Requests: List[SchemaConversionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaConversionRequestTypeDef](./type_defs.md#schemaconversionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMetadataModelConversionsResponseTypeDef

```python
# DescribeMetadataModelConversionsResponseTypeDef definition

class DescribeMetadataModelConversionsResponseTypeDef(TypedDict):
    Marker: str,
    Requests: List[SchemaConversionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaConversionRequestTypeDef](./type_defs.md#schemaconversionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMetadataModelExportsAsScriptResponseTypeDef

```python
# DescribeMetadataModelExportsAsScriptResponseTypeDef definition

class DescribeMetadataModelExportsAsScriptResponseTypeDef(TypedDict):
    Marker: str,
    Requests: List[SchemaConversionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaConversionRequestTypeDef](./type_defs.md#schemaconversionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMetadataModelExportsToTargetResponseTypeDef

```python
# DescribeMetadataModelExportsToTargetResponseTypeDef definition

class DescribeMetadataModelExportsToTargetResponseTypeDef(TypedDict):
    Marker: str,
    Requests: List[SchemaConversionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaConversionRequestTypeDef](./type_defs.md#schemaconversionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMetadataModelImportsResponseTypeDef

```python
# DescribeMetadataModelImportsResponseTypeDef definition

class DescribeMetadataModelImportsResponseTypeDef(TypedDict):
    Marker: str,
    Requests: List[SchemaConversionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaConversionRequestTypeDef](./type_defs.md#schemaconversionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    DatabaseId: NotRequired[str],
    EngineName: NotRequired[str],
    CreatedDate: NotRequired[str],
    Status: NotRequired[str],
    Preferred: NotRequired[bool],
    Settings: NotRequired[RecommendationSettingsTypeDef],  # (1)
    Data: NotRequired[RecommendationDataTypeDef],  # (2)
```

1. See [:material-code-braces: RecommendationSettingsTypeDef](./type_defs.md#recommendationsettingstypedef) 
2. See [:material-code-braces: RecommendationDataTypeDef](./type_defs.md#recommendationdatatypedef) 
## CreateReplicationInstanceResponseTypeDef

```python
# CreateReplicationInstanceResponseTypeDef definition

class CreateReplicationInstanceResponseTypeDef(TypedDict):
    ReplicationInstance: ReplicationInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationInstanceTypeDef](./type_defs.md#replicationinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteReplicationInstanceResponseTypeDef

```python
# DeleteReplicationInstanceResponseTypeDef definition

class DeleteReplicationInstanceResponseTypeDef(TypedDict):
    ReplicationInstance: ReplicationInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationInstanceTypeDef](./type_defs.md#replicationinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationInstancesResponseTypeDef

```python
# DescribeReplicationInstancesResponseTypeDef definition

class DescribeReplicationInstancesResponseTypeDef(TypedDict):
    Marker: str,
    ReplicationInstances: List[ReplicationInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationInstanceTypeDef](./type_defs.md#replicationinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyReplicationInstanceResponseTypeDef

```python
# ModifyReplicationInstanceResponseTypeDef definition

class ModifyReplicationInstanceResponseTypeDef(TypedDict):
    ReplicationInstance: ReplicationInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationInstanceTypeDef](./type_defs.md#replicationinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootReplicationInstanceResponseTypeDef

```python
# RebootReplicationInstanceResponseTypeDef definition

class RebootReplicationInstanceResponseTypeDef(TypedDict):
    ReplicationInstance: ReplicationInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationInstanceTypeDef](./type_defs.md#replicationinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRecommendationsResponseTypeDef

```python
# DescribeRecommendationsResponseTypeDef definition

class DescribeRecommendationsResponseTypeDef(TypedDict):
    Recommendations: List[RecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
