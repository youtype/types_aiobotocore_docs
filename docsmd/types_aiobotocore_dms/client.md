# DatabaseMigrationServiceClient

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > DatabaseMigrationServiceClient

!!! note ""

    Auto-generated documentation for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#databasemigrationservice)
    type annotations stubs module [types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

## DatabaseMigrationServiceClient

Type annotations and code completion for `#!python session.create_client("dms")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client)

```python
# DatabaseMigrationServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_dms.client import DatabaseMigrationServiceClient

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("dms").exceptions` structure.

```python
# DatabaseMigrationServiceClient.exceptions usage example

async with session.create_client("dms") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedFault,
        client.ClientError,
        client.CollectorNotFoundFault,
        client.FailedDependencyFault,
        client.InsufficientResourceCapacityFault,
        client.InvalidCertificateFault,
        client.InvalidOperationFault,
        client.InvalidResourceStateFault,
        client.InvalidSubnet,
        client.KMSAccessDeniedFault,
        client.KMSDisabledFault,
        client.KMSFault,
        client.KMSInvalidStateFault,
        client.KMSKeyNotAccessibleFault,
        client.KMSNotFoundFault,
        client.KMSThrottlingFault,
        client.ReplicationSubnetGroupDoesNotCoverEnoughAZs,
        client.ResourceAlreadyExistsFault,
        client.ResourceNotFoundFault,
        client.ResourceQuotaExceededFault,
        client.S3AccessDeniedFault,
        client.S3ResourceNotFoundFault,
        client.SNSInvalidTopicFault,
        client.SNSNoAuthorizationFault,
        client.StorageQuotaExceededFault,
        client.SubnetAlreadyInUse,
        client.UpgradeDependencyFailureFault,
    ) as e:
        print(e)
```

```python
# DatabaseMigrationServiceClient usage type checking example

from types_aiobotocore_dms.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedFault) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("dms").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("dms").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("dms").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### add\_tags\_to\_resource

Adds metadata tags to an DMS resource, including replication instance,
endpoint, subnet group, and migration task.

Type annotations and code completion for `#!python session.create_client("dms").add_tags_to_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/add_tags_to_resource.html)

```python
# add_tags_to_resource method definition

await def add_tags_to_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# add_tags_to_resource method usage example with argument unpacking

kwargs: AddTagsToResourceMessageRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.add_tags_to_resource(**kwargs)
```

1. See [:material-code-braces: AddTagsToResourceMessageRequestTypeDef](./type_defs.md#addtagstoresourcemessagerequesttypedef) 

### apply\_pending\_maintenance\_action

Applies a pending maintenance action to a resource (for example, to a
replication instance).

Type annotations and code completion for `#!python session.create_client("dms").apply_pending_maintenance_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/apply_pending_maintenance_action.html)

```python
# apply_pending_maintenance_action method definition

await def apply_pending_maintenance_action(
    self,
    *,
    ReplicationInstanceArn: str,
    ApplyAction: str,
    OptInType: str,
) -> ApplyPendingMaintenanceActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplyPendingMaintenanceActionResponseTypeDef](./type_defs.md#applypendingmaintenanceactionresponsetypedef) 


```python
# apply_pending_maintenance_action method usage example with argument unpacking

kwargs: ApplyPendingMaintenanceActionMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceArn": ...,
    "ApplyAction": ...,
    "OptInType": ...,
}

parent.apply_pending_maintenance_action(**kwargs)
```

1. See [:material-code-braces: ApplyPendingMaintenanceActionMessageRequestTypeDef](./type_defs.md#applypendingmaintenanceactionmessagerequesttypedef) 

### batch\_start\_recommendations

Starts the analysis of up to 20 source databases to recommend target engines
for each source database.

Type annotations and code completion for `#!python session.create_client("dms").batch_start_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/batch_start_recommendations.html)

```python
# batch_start_recommendations method definition

await def batch_start_recommendations(
    self,
    *,
    Data: Sequence[StartRecommendationsRequestEntryTypeDef] = ...,  # (1)
) -> BatchStartRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartRecommendationsRequestEntryTypeDef](./type_defs.md#startrecommendationsrequestentrytypedef) 
2. See [:material-code-braces: BatchStartRecommendationsResponseTypeDef](./type_defs.md#batchstartrecommendationsresponsetypedef) 


```python
# batch_start_recommendations method usage example with argument unpacking

kwargs: BatchStartRecommendationsRequestRequestTypeDef = {  # (1)
    "Data": ...,
}

parent.batch_start_recommendations(**kwargs)
```

1. See [:material-code-braces: BatchStartRecommendationsRequestRequestTypeDef](./type_defs.md#batchstartrecommendationsrequestrequesttypedef) 

### cancel\_replication\_task\_assessment\_run

Cancels a single premigration assessment run.

Type annotations and code completion for `#!python session.create_client("dms").cancel_replication_task_assessment_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/cancel_replication_task_assessment_run.html)

```python
# cancel_replication_task_assessment_run method definition

await def cancel_replication_task_assessment_run(
    self,
    *,
    ReplicationTaskAssessmentRunArn: str,
) -> CancelReplicationTaskAssessmentRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelReplicationTaskAssessmentRunResponseTypeDef](./type_defs.md#cancelreplicationtaskassessmentrunresponsetypedef) 


```python
# cancel_replication_task_assessment_run method usage example with argument unpacking

kwargs: CancelReplicationTaskAssessmentRunMessageRequestTypeDef = {  # (1)
    "ReplicationTaskAssessmentRunArn": ...,
}

parent.cancel_replication_task_assessment_run(**kwargs)
```

1. See [:material-code-braces: CancelReplicationTaskAssessmentRunMessageRequestTypeDef](./type_defs.md#cancelreplicationtaskassessmentrunmessagerequesttypedef) 

### create\_data\_migration

Creates a data migration using the provided settings.

Type annotations and code completion for `#!python session.create_client("dms").create_data_migration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_data_migration.html)

```python
# create_data_migration method definition

await def create_data_migration(
    self,
    *,
    MigrationProjectIdentifier: str,
    DataMigrationType: MigrationTypeValueType,  # (1)
    ServiceAccessRoleArn: str,
    DataMigrationName: str = ...,
    EnableCloudwatchLogs: bool = ...,
    SourceDataSettings: Sequence[SourceDataSettingUnionTypeDef] = ...,  # (2)
    NumberOfJobs: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    SelectionRules: str = ...,
) -> CreateDataMigrationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: SourceDataSettingTypeDef](./type_defs.md#sourcedatasettingtypedef) [:material-code-braces: SourceDataSettingOutputTypeDef](./type_defs.md#sourcedatasettingoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateDataMigrationResponseTypeDef](./type_defs.md#createdatamigrationresponsetypedef) 


```python
# create_data_migration method usage example with argument unpacking

kwargs: CreateDataMigrationMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "DataMigrationType": ...,
    "ServiceAccessRoleArn": ...,
}

parent.create_data_migration(**kwargs)
```

1. See [:material-code-braces: CreateDataMigrationMessageRequestTypeDef](./type_defs.md#createdatamigrationmessagerequesttypedef) 

### create\_data\_provider

Creates a data provider using the provided settings.

Type annotations and code completion for `#!python session.create_client("dms").create_data_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_data_provider.html)

```python
# create_data_provider method definition

await def create_data_provider(
    self,
    *,
    Engine: str,
    Settings: DataProviderSettingsTypeDef,  # (1)
    DataProviderName: str = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDataProviderResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DataProviderSettingsTypeDef](./type_defs.md#dataprovidersettingstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDataProviderResponseTypeDef](./type_defs.md#createdataproviderresponsetypedef) 


```python
# create_data_provider method usage example with argument unpacking

kwargs: CreateDataProviderMessageRequestTypeDef = {  # (1)
    "Engine": ...,
    "Settings": ...,
}

parent.create_data_provider(**kwargs)
```

1. See [:material-code-braces: CreateDataProviderMessageRequestTypeDef](./type_defs.md#createdataprovidermessagerequesttypedef) 

### create\_endpoint

Creates an endpoint using the provided settings.

Type annotations and code completion for `#!python session.create_client("dms").create_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_endpoint.html)

```python
# create_endpoint method definition

await def create_endpoint(
    self,
    *,
    EndpointIdentifier: str,
    EndpointType: ReplicationEndpointTypeValueType,  # (1)
    EngineName: str,
    Username: str = ...,
    Password: str = ...,
    ServerName: str = ...,
    Port: int = ...,
    DatabaseName: str = ...,
    ExtraConnectionAttributes: str = ...,
    KmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    CertificateArn: str = ...,
    SslMode: DmsSslModeValueType = ...,  # (3)
    ServiceAccessRoleArn: str = ...,
    ExternalTableDefinition: str = ...,
    DynamoDbSettings: DynamoDbSettingsTypeDef = ...,  # (4)
    S3Settings: S3SettingsTypeDef = ...,  # (5)
    DmsTransferSettings: DmsTransferSettingsTypeDef = ...,  # (6)
    MongoDbSettings: MongoDbSettingsTypeDef = ...,  # (7)
    KinesisSettings: KinesisSettingsTypeDef = ...,  # (8)
    KafkaSettings: KafkaSettingsTypeDef = ...,  # (9)
    ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,  # (10)
    NeptuneSettings: NeptuneSettingsTypeDef = ...,  # (11)
    RedshiftSettings: RedshiftSettingsTypeDef = ...,  # (12)
    PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,  # (13)
    MySQLSettings: MySQLSettingsTypeDef = ...,  # (14)
    OracleSettings: OracleSettingsTypeDef = ...,  # (15)
    SybaseSettings: SybaseSettingsTypeDef = ...,  # (16)
    MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,  # (17)
    IBMDb2Settings: IBMDb2SettingsTypeDef = ...,  # (18)
    ResourceIdentifier: str = ...,
    DocDbSettings: DocDbSettingsTypeDef = ...,  # (19)
    RedisSettings: RedisSettingsTypeDef = ...,  # (20)
    GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,  # (21)
    TimestreamSettings: TimestreamSettingsTypeDef = ...,  # (22)
) -> CreateEndpointResponseTypeDef:  # (23)
    ...
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
23. See [:material-code-braces: CreateEndpointResponseTypeDef](./type_defs.md#createendpointresponsetypedef) 


```python
# create_endpoint method usage example with argument unpacking

kwargs: CreateEndpointMessageRequestTypeDef = {  # (1)
    "EndpointIdentifier": ...,
    "EndpointType": ...,
    "EngineName": ...,
}

parent.create_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateEndpointMessageRequestTypeDef](./type_defs.md#createendpointmessagerequesttypedef) 

### create\_event\_subscription

Creates an DMS event notification subscription.

Type annotations and code completion for `#!python session.create_client("dms").create_event_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_event_subscription.html)

```python
# create_event_subscription method definition

await def create_event_subscription(
    self,
    *,
    SubscriptionName: str,
    SnsTopicArn: str,
    SourceType: str = ...,
    EventCategories: Sequence[str] = ...,
    SourceIds: Sequence[str] = ...,
    Enabled: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateEventSubscriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateEventSubscriptionResponseTypeDef](./type_defs.md#createeventsubscriptionresponsetypedef) 


```python
# create_event_subscription method usage example with argument unpacking

kwargs: CreateEventSubscriptionMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
    "SnsTopicArn": ...,
}

parent.create_event_subscription(**kwargs)
```

1. See [:material-code-braces: CreateEventSubscriptionMessageRequestTypeDef](./type_defs.md#createeventsubscriptionmessagerequesttypedef) 

### create\_fleet\_advisor\_collector

Creates a Fleet Advisor collector using the specified parameters.

Type annotations and code completion for `#!python session.create_client("dms").create_fleet_advisor_collector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_fleet_advisor_collector.html)

```python
# create_fleet_advisor_collector method definition

await def create_fleet_advisor_collector(
    self,
    *,
    CollectorName: str,
    ServiceAccessRoleArn: str,
    S3BucketName: str,
    Description: str = ...,
) -> CreateFleetAdvisorCollectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateFleetAdvisorCollectorResponseTypeDef](./type_defs.md#createfleetadvisorcollectorresponsetypedef) 


```python
# create_fleet_advisor_collector method usage example with argument unpacking

kwargs: CreateFleetAdvisorCollectorRequestRequestTypeDef = {  # (1)
    "CollectorName": ...,
    "ServiceAccessRoleArn": ...,
    "S3BucketName": ...,
}

parent.create_fleet_advisor_collector(**kwargs)
```

1. See [:material-code-braces: CreateFleetAdvisorCollectorRequestRequestTypeDef](./type_defs.md#createfleetadvisorcollectorrequestrequesttypedef) 

### create\_instance\_profile

Creates the instance profile using the specified parameters.

Type annotations and code completion for `#!python session.create_client("dms").create_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_instance_profile.html)

```python
# create_instance_profile method definition

await def create_instance_profile(
    self,
    *,
    AvailabilityZone: str = ...,
    KmsKeyArn: str = ...,
    PubliclyAccessible: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    NetworkType: str = ...,
    InstanceProfileName: str = ...,
    Description: str = ...,
    SubnetGroupIdentifier: str = ...,
    VpcSecurityGroups: Sequence[str] = ...,
) -> CreateInstanceProfileResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateInstanceProfileResponseTypeDef](./type_defs.md#createinstanceprofileresponsetypedef) 


```python
# create_instance_profile method usage example with argument unpacking

kwargs: CreateInstanceProfileMessageRequestTypeDef = {  # (1)
    "AvailabilityZone": ...,
}

parent.create_instance_profile(**kwargs)
```

1. See [:material-code-braces: CreateInstanceProfileMessageRequestTypeDef](./type_defs.md#createinstanceprofilemessagerequesttypedef) 

### create\_migration\_project

Creates the migration project using the specified parameters.

Type annotations and code completion for `#!python session.create_client("dms").create_migration_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_migration_project.html)

```python
# create_migration_project method definition

await def create_migration_project(
    self,
    *,
    SourceDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],  # (1)
    TargetDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],  # (1)
    InstanceProfileIdentifier: str,
    MigrationProjectName: str = ...,
    TransformationRules: str = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...,  # (4)
) -> CreateMigrationProjectResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
2. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: SCApplicationAttributesTypeDef](./type_defs.md#scapplicationattributestypedef) 
5. See [:material-code-braces: CreateMigrationProjectResponseTypeDef](./type_defs.md#createmigrationprojectresponsetypedef) 


```python
# create_migration_project method usage example with argument unpacking

kwargs: CreateMigrationProjectMessageRequestTypeDef = {  # (1)
    "SourceDataProviderDescriptors": ...,
    "TargetDataProviderDescriptors": ...,
    "InstanceProfileIdentifier": ...,
}

parent.create_migration_project(**kwargs)
```

1. See [:material-code-braces: CreateMigrationProjectMessageRequestTypeDef](./type_defs.md#createmigrationprojectmessagerequesttypedef) 

### create\_replication\_config

Creates a configuration that you can later provide to configure and start an
DMS Serverless replication.

Type annotations and code completion for `#!python session.create_client("dms").create_replication_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_replication_config.html)

```python
# create_replication_config method definition

await def create_replication_config(
    self,
    *,
    ReplicationConfigIdentifier: str,
    SourceEndpointArn: str,
    TargetEndpointArn: str,
    ComputeConfig: ComputeConfigTypeDef,  # (1)
    ReplicationType: MigrationTypeValueType,  # (2)
    TableMappings: str,
    ReplicationSettings: str = ...,
    SupplementalSettings: str = ...,
    ResourceIdentifier: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateReplicationConfigResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ComputeConfigTypeDef](./type_defs.md#computeconfigtypedef) 
2. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateReplicationConfigResponseTypeDef](./type_defs.md#createreplicationconfigresponsetypedef) 


```python
# create_replication_config method usage example with argument unpacking

kwargs: CreateReplicationConfigMessageRequestTypeDef = {  # (1)
    "ReplicationConfigIdentifier": ...,
    "SourceEndpointArn": ...,
    "TargetEndpointArn": ...,
    "ComputeConfig": ...,
    "ReplicationType": ...,
    "TableMappings": ...,
}

parent.create_replication_config(**kwargs)
```

1. See [:material-code-braces: CreateReplicationConfigMessageRequestTypeDef](./type_defs.md#createreplicationconfigmessagerequesttypedef) 

### create\_replication\_instance

Creates the replication instance using the specified parameters.

Type annotations and code completion for `#!python session.create_client("dms").create_replication_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_replication_instance.html)

```python
# create_replication_instance method definition

await def create_replication_instance(
    self,
    *,
    ReplicationInstanceIdentifier: str,
    ReplicationInstanceClass: str,
    AllocatedStorage: int = ...,
    VpcSecurityGroupIds: Sequence[str] = ...,
    AvailabilityZone: str = ...,
    ReplicationSubnetGroupIdentifier: str = ...,
    PreferredMaintenanceWindow: str = ...,
    MultiAZ: bool = ...,
    EngineVersion: str = ...,
    AutoMinorVersionUpgrade: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    KmsKeyId: str = ...,
    PubliclyAccessible: bool = ...,
    DnsNameServers: str = ...,
    ResourceIdentifier: str = ...,
    NetworkType: str = ...,
    KerberosAuthenticationSettings: KerberosAuthenticationSettingsTypeDef = ...,  # (2)
) -> CreateReplicationInstanceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: KerberosAuthenticationSettingsTypeDef](./type_defs.md#kerberosauthenticationsettingstypedef) 
3. See [:material-code-braces: CreateReplicationInstanceResponseTypeDef](./type_defs.md#createreplicationinstanceresponsetypedef) 


```python
# create_replication_instance method usage example with argument unpacking

kwargs: CreateReplicationInstanceMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceIdentifier": ...,
    "ReplicationInstanceClass": ...,
}

parent.create_replication_instance(**kwargs)
```

1. See [:material-code-braces: CreateReplicationInstanceMessageRequestTypeDef](./type_defs.md#createreplicationinstancemessagerequesttypedef) 

### create\_replication\_subnet\_group

Creates a replication subnet group given a list of the subnet IDs in a VPC.

Type annotations and code completion for `#!python session.create_client("dms").create_replication_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_replication_subnet_group.html)

```python
# create_replication_subnet_group method definition

await def create_replication_subnet_group(
    self,
    *,
    ReplicationSubnetGroupIdentifier: str,
    ReplicationSubnetGroupDescription: str,
    SubnetIds: Sequence[str],
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateReplicationSubnetGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateReplicationSubnetGroupResponseTypeDef](./type_defs.md#createreplicationsubnetgroupresponsetypedef) 


```python
# create_replication_subnet_group method usage example with argument unpacking

kwargs: CreateReplicationSubnetGroupMessageRequestTypeDef = {  # (1)
    "ReplicationSubnetGroupIdentifier": ...,
    "ReplicationSubnetGroupDescription": ...,
    "SubnetIds": ...,
}

parent.create_replication_subnet_group(**kwargs)
```

1. See [:material-code-braces: CreateReplicationSubnetGroupMessageRequestTypeDef](./type_defs.md#createreplicationsubnetgroupmessagerequesttypedef) 

### create\_replication\_task

Creates a replication task using the specified parameters.

Type annotations and code completion for `#!python session.create_client("dms").create_replication_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/create_replication_task.html)

```python
# create_replication_task method definition

await def create_replication_task(
    self,
    *,
    ReplicationTaskIdentifier: str,
    SourceEndpointArn: str,
    TargetEndpointArn: str,
    ReplicationInstanceArn: str,
    MigrationType: MigrationTypeValueType,  # (1)
    TableMappings: str,
    ReplicationTaskSettings: str = ...,
    CdcStartTime: TimestampTypeDef = ...,
    CdcStartPosition: str = ...,
    CdcStopPosition: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    TaskData: str = ...,
    ResourceIdentifier: str = ...,
) -> CreateReplicationTaskResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateReplicationTaskResponseTypeDef](./type_defs.md#createreplicationtaskresponsetypedef) 


```python
# create_replication_task method usage example with argument unpacking

kwargs: CreateReplicationTaskMessageRequestTypeDef = {  # (1)
    "ReplicationTaskIdentifier": ...,
    "SourceEndpointArn": ...,
    "TargetEndpointArn": ...,
    "ReplicationInstanceArn": ...,
    "MigrationType": ...,
    "TableMappings": ...,
}

parent.create_replication_task(**kwargs)
```

1. See [:material-code-braces: CreateReplicationTaskMessageRequestTypeDef](./type_defs.md#createreplicationtaskmessagerequesttypedef) 

### delete\_certificate

Deletes the specified certificate.

Type annotations and code completion for `#!python session.create_client("dms").delete_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_certificate.html)

```python
# delete_certificate method definition

await def delete_certificate(
    self,
    *,
    CertificateArn: str,
) -> DeleteCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCertificateResponseTypeDef](./type_defs.md#deletecertificateresponsetypedef) 


```python
# delete_certificate method usage example with argument unpacking

kwargs: DeleteCertificateMessageRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.delete_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteCertificateMessageRequestTypeDef](./type_defs.md#deletecertificatemessagerequesttypedef) 

### delete\_connection

Deletes the connection between a replication instance and an endpoint.

Type annotations and code completion for `#!python session.create_client("dms").delete_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_connection.html)

```python
# delete_connection method definition

await def delete_connection(
    self,
    *,
    EndpointArn: str,
    ReplicationInstanceArn: str,
) -> DeleteConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteConnectionResponseTypeDef](./type_defs.md#deleteconnectionresponsetypedef) 


```python
# delete_connection method usage example with argument unpacking

kwargs: DeleteConnectionMessageRequestTypeDef = {  # (1)
    "EndpointArn": ...,
    "ReplicationInstanceArn": ...,
}

parent.delete_connection(**kwargs)
```

1. See [:material-code-braces: DeleteConnectionMessageRequestTypeDef](./type_defs.md#deleteconnectionmessagerequesttypedef) 

### delete\_data\_migration

Deletes the specified data migration.

Type annotations and code completion for `#!python session.create_client("dms").delete_data_migration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_data_migration.html)

```python
# delete_data_migration method definition

await def delete_data_migration(
    self,
    *,
    DataMigrationIdentifier: str,
) -> DeleteDataMigrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataMigrationResponseTypeDef](./type_defs.md#deletedatamigrationresponsetypedef) 


```python
# delete_data_migration method usage example with argument unpacking

kwargs: DeleteDataMigrationMessageRequestTypeDef = {  # (1)
    "DataMigrationIdentifier": ...,
}

parent.delete_data_migration(**kwargs)
```

1. See [:material-code-braces: DeleteDataMigrationMessageRequestTypeDef](./type_defs.md#deletedatamigrationmessagerequesttypedef) 

### delete\_data\_provider

Deletes the specified data provider.

Type annotations and code completion for `#!python session.create_client("dms").delete_data_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_data_provider.html)

```python
# delete_data_provider method definition

await def delete_data_provider(
    self,
    *,
    DataProviderIdentifier: str,
) -> DeleteDataProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataProviderResponseTypeDef](./type_defs.md#deletedataproviderresponsetypedef) 


```python
# delete_data_provider method usage example with argument unpacking

kwargs: DeleteDataProviderMessageRequestTypeDef = {  # (1)
    "DataProviderIdentifier": ...,
}

parent.delete_data_provider(**kwargs)
```

1. See [:material-code-braces: DeleteDataProviderMessageRequestTypeDef](./type_defs.md#deletedataprovidermessagerequesttypedef) 

### delete\_endpoint

Deletes the specified endpoint.

Type annotations and code completion for `#!python session.create_client("dms").delete_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_endpoint.html)

```python
# delete_endpoint method definition

await def delete_endpoint(
    self,
    *,
    EndpointArn: str,
) -> DeleteEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEndpointResponseTypeDef](./type_defs.md#deleteendpointresponsetypedef) 


```python
# delete_endpoint method usage example with argument unpacking

kwargs: DeleteEndpointMessageRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.delete_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointMessageRequestTypeDef](./type_defs.md#deleteendpointmessagerequesttypedef) 

### delete\_event\_subscription

Deletes an DMS event subscription.

Type annotations and code completion for `#!python session.create_client("dms").delete_event_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_event_subscription.html)

```python
# delete_event_subscription method definition

await def delete_event_subscription(
    self,
    *,
    SubscriptionName: str,
) -> DeleteEventSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEventSubscriptionResponseTypeDef](./type_defs.md#deleteeventsubscriptionresponsetypedef) 


```python
# delete_event_subscription method usage example with argument unpacking

kwargs: DeleteEventSubscriptionMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.delete_event_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteEventSubscriptionMessageRequestTypeDef](./type_defs.md#deleteeventsubscriptionmessagerequesttypedef) 

### delete\_fleet\_advisor\_collector

Deletes the specified Fleet Advisor collector.

Type annotations and code completion for `#!python session.create_client("dms").delete_fleet_advisor_collector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_fleet_advisor_collector.html)

```python
# delete_fleet_advisor_collector method definition

await def delete_fleet_advisor_collector(
    self,
    *,
    CollectorReferencedId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_fleet_advisor_collector method usage example with argument unpacking

kwargs: DeleteCollectorRequestRequestTypeDef = {  # (1)
    "CollectorReferencedId": ...,
}

parent.delete_fleet_advisor_collector(**kwargs)
```

1. See [:material-code-braces: DeleteCollectorRequestRequestTypeDef](./type_defs.md#deletecollectorrequestrequesttypedef) 

### delete\_fleet\_advisor\_databases

Deletes the specified Fleet Advisor collector databases.

Type annotations and code completion for `#!python session.create_client("dms").delete_fleet_advisor_databases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_fleet_advisor_databases.html)

```python
# delete_fleet_advisor_databases method definition

await def delete_fleet_advisor_databases(
    self,
    *,
    DatabaseIds: Sequence[str],
) -> DeleteFleetAdvisorDatabasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFleetAdvisorDatabasesResponseTypeDef](./type_defs.md#deletefleetadvisordatabasesresponsetypedef) 


```python
# delete_fleet_advisor_databases method usage example with argument unpacking

kwargs: DeleteFleetAdvisorDatabasesRequestRequestTypeDef = {  # (1)
    "DatabaseIds": ...,
}

parent.delete_fleet_advisor_databases(**kwargs)
```

1. See [:material-code-braces: DeleteFleetAdvisorDatabasesRequestRequestTypeDef](./type_defs.md#deletefleetadvisordatabasesrequestrequesttypedef) 

### delete\_instance\_profile

Deletes the specified instance profile.

Type annotations and code completion for `#!python session.create_client("dms").delete_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_instance_profile.html)

```python
# delete_instance_profile method definition

await def delete_instance_profile(
    self,
    *,
    InstanceProfileIdentifier: str,
) -> DeleteInstanceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInstanceProfileResponseTypeDef](./type_defs.md#deleteinstanceprofileresponsetypedef) 


```python
# delete_instance_profile method usage example with argument unpacking

kwargs: DeleteInstanceProfileMessageRequestTypeDef = {  # (1)
    "InstanceProfileIdentifier": ...,
}

parent.delete_instance_profile(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceProfileMessageRequestTypeDef](./type_defs.md#deleteinstanceprofilemessagerequesttypedef) 

### delete\_migration\_project

Deletes the specified migration project.

Type annotations and code completion for `#!python session.create_client("dms").delete_migration_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_migration_project.html)

```python
# delete_migration_project method definition

await def delete_migration_project(
    self,
    *,
    MigrationProjectIdentifier: str,
) -> DeleteMigrationProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMigrationProjectResponseTypeDef](./type_defs.md#deletemigrationprojectresponsetypedef) 


```python
# delete_migration_project method usage example with argument unpacking

kwargs: DeleteMigrationProjectMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.delete_migration_project(**kwargs)
```

1. See [:material-code-braces: DeleteMigrationProjectMessageRequestTypeDef](./type_defs.md#deletemigrationprojectmessagerequesttypedef) 

### delete\_replication\_config

Deletes an DMS Serverless replication configuration.

Type annotations and code completion for `#!python session.create_client("dms").delete_replication_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_replication_config.html)

```python
# delete_replication_config method definition

await def delete_replication_config(
    self,
    *,
    ReplicationConfigArn: str,
) -> DeleteReplicationConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReplicationConfigResponseTypeDef](./type_defs.md#deletereplicationconfigresponsetypedef) 


```python
# delete_replication_config method usage example with argument unpacking

kwargs: DeleteReplicationConfigMessageRequestTypeDef = {  # (1)
    "ReplicationConfigArn": ...,
}

parent.delete_replication_config(**kwargs)
```

1. See [:material-code-braces: DeleteReplicationConfigMessageRequestTypeDef](./type_defs.md#deletereplicationconfigmessagerequesttypedef) 

### delete\_replication\_instance

Deletes the specified replication instance.

Type annotations and code completion for `#!python session.create_client("dms").delete_replication_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_replication_instance.html)

```python
# delete_replication_instance method definition

await def delete_replication_instance(
    self,
    *,
    ReplicationInstanceArn: str,
) -> DeleteReplicationInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReplicationInstanceResponseTypeDef](./type_defs.md#deletereplicationinstanceresponsetypedef) 


```python
# delete_replication_instance method usage example with argument unpacking

kwargs: DeleteReplicationInstanceMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceArn": ...,
}

parent.delete_replication_instance(**kwargs)
```

1. See [:material-code-braces: DeleteReplicationInstanceMessageRequestTypeDef](./type_defs.md#deletereplicationinstancemessagerequesttypedef) 

### delete\_replication\_subnet\_group

Deletes a subnet group.

Type annotations and code completion for `#!python session.create_client("dms").delete_replication_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_replication_subnet_group.html)

```python
# delete_replication_subnet_group method definition

await def delete_replication_subnet_group(
    self,
    *,
    ReplicationSubnetGroupIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_replication_subnet_group method usage example with argument unpacking

kwargs: DeleteReplicationSubnetGroupMessageRequestTypeDef = {  # (1)
    "ReplicationSubnetGroupIdentifier": ...,
}

parent.delete_replication_subnet_group(**kwargs)
```

1. See [:material-code-braces: DeleteReplicationSubnetGroupMessageRequestTypeDef](./type_defs.md#deletereplicationsubnetgroupmessagerequesttypedef) 

### delete\_replication\_task

Deletes the specified replication task.

Type annotations and code completion for `#!python session.create_client("dms").delete_replication_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_replication_task.html)

```python
# delete_replication_task method definition

await def delete_replication_task(
    self,
    *,
    ReplicationTaskArn: str,
) -> DeleteReplicationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReplicationTaskResponseTypeDef](./type_defs.md#deletereplicationtaskresponsetypedef) 


```python
# delete_replication_task method usage example with argument unpacking

kwargs: DeleteReplicationTaskMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.delete_replication_task(**kwargs)
```

1. See [:material-code-braces: DeleteReplicationTaskMessageRequestTypeDef](./type_defs.md#deletereplicationtaskmessagerequesttypedef) 

### delete\_replication\_task\_assessment\_run

Deletes the record of a single premigration assessment run.

Type annotations and code completion for `#!python session.create_client("dms").delete_replication_task_assessment_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/delete_replication_task_assessment_run.html)

```python
# delete_replication_task_assessment_run method definition

await def delete_replication_task_assessment_run(
    self,
    *,
    ReplicationTaskAssessmentRunArn: str,
) -> DeleteReplicationTaskAssessmentRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReplicationTaskAssessmentRunResponseTypeDef](./type_defs.md#deletereplicationtaskassessmentrunresponsetypedef) 


```python
# delete_replication_task_assessment_run method usage example with argument unpacking

kwargs: DeleteReplicationTaskAssessmentRunMessageRequestTypeDef = {  # (1)
    "ReplicationTaskAssessmentRunArn": ...,
}

parent.delete_replication_task_assessment_run(**kwargs)
```

1. See [:material-code-braces: DeleteReplicationTaskAssessmentRunMessageRequestTypeDef](./type_defs.md#deletereplicationtaskassessmentrunmessagerequesttypedef) 

### describe\_account\_attributes

Lists all of the DMS attributes for a customer account.

Type annotations and code completion for `#!python session.create_client("dms").describe_account_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_account_attributes.html)

```python
# describe_account_attributes method definition

await def describe_account_attributes(
    self,
) -> DescribeAccountAttributesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountAttributesResponseTypeDef](./type_defs.md#describeaccountattributesresponsetypedef) 

### describe\_applicable\_individual\_assessments

Provides a list of individual assessments that you can specify for a new
premigration assessment run, given one or more parameters.

Type annotations and code completion for `#!python session.create_client("dms").describe_applicable_individual_assessments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_applicable_individual_assessments.html)

```python
# describe_applicable_individual_assessments method definition

await def describe_applicable_individual_assessments(
    self,
    *,
    ReplicationTaskArn: str = ...,
    ReplicationInstanceArn: str = ...,
    SourceEngineName: str = ...,
    TargetEngineName: str = ...,
    MigrationType: MigrationTypeValueType = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeApplicableIndividualAssessmentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: DescribeApplicableIndividualAssessmentsResponseTypeDef](./type_defs.md#describeapplicableindividualassessmentsresponsetypedef) 


```python
# describe_applicable_individual_assessments method usage example with argument unpacking

kwargs: DescribeApplicableIndividualAssessmentsMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.describe_applicable_individual_assessments(**kwargs)
```

1. See [:material-code-braces: DescribeApplicableIndividualAssessmentsMessageRequestTypeDef](./type_defs.md#describeapplicableindividualassessmentsmessagerequesttypedef) 

### describe\_certificates

Provides a description of the certificate.

Type annotations and code completion for `#!python session.create_client("dms").describe_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_certificates.html)

```python
# describe_certificates method definition

await def describe_certificates(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeCertificatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef) 


```python
# describe_certificates method usage example with argument unpacking

kwargs: DescribeCertificatesMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_certificates(**kwargs)
```

1. See [:material-code-braces: DescribeCertificatesMessageRequestTypeDef](./type_defs.md#describecertificatesmessagerequesttypedef) 

### describe\_connections

Describes the status of the connections that have been made between the
replication instance and an endpoint.

Type annotations and code completion for `#!python session.create_client("dms").describe_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_connections.html)

```python
# describe_connections method definition

await def describe_connections(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeConnectionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeConnectionsResponseTypeDef](./type_defs.md#describeconnectionsresponsetypedef) 


```python
# describe_connections method usage example with argument unpacking

kwargs: DescribeConnectionsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_connections(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionsMessageRequestTypeDef](./type_defs.md#describeconnectionsmessagerequesttypedef) 

### describe\_conversion\_configuration

Returns configuration parameters for a schema conversion project.

Type annotations and code completion for `#!python session.create_client("dms").describe_conversion_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_conversion_configuration.html)

```python
# describe_conversion_configuration method definition

await def describe_conversion_configuration(
    self,
    *,
    MigrationProjectIdentifier: str,
) -> DescribeConversionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConversionConfigurationResponseTypeDef](./type_defs.md#describeconversionconfigurationresponsetypedef) 


```python
# describe_conversion_configuration method usage example with argument unpacking

kwargs: DescribeConversionConfigurationMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.describe_conversion_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeConversionConfigurationMessageRequestTypeDef](./type_defs.md#describeconversionconfigurationmessagerequesttypedef) 

### describe\_data\_migrations

Returns information about data migrations.

Type annotations and code completion for `#!python session.create_client("dms").describe_data_migrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_data_migrations.html)

```python
# describe_data_migrations method definition

await def describe_data_migrations(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WithoutSettings: bool = ...,
    WithoutStatistics: bool = ...,
) -> DescribeDataMigrationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeDataMigrationsResponseTypeDef](./type_defs.md#describedatamigrationsresponsetypedef) 


```python
# describe_data_migrations method usage example with argument unpacking

kwargs: DescribeDataMigrationsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_data_migrations(**kwargs)
```

1. See [:material-code-braces: DescribeDataMigrationsMessageRequestTypeDef](./type_defs.md#describedatamigrationsmessagerequesttypedef) 

### describe\_data\_providers

Returns a paginated list of data providers for your account in the current
region.

Type annotations and code completion for `#!python session.create_client("dms").describe_data_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_data_providers.html)

```python
# describe_data_providers method definition

await def describe_data_providers(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeDataProvidersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeDataProvidersResponseTypeDef](./type_defs.md#describedataprovidersresponsetypedef) 


```python
# describe_data_providers method usage example with argument unpacking

kwargs: DescribeDataProvidersMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_data_providers(**kwargs)
```

1. See [:material-code-braces: DescribeDataProvidersMessageRequestTypeDef](./type_defs.md#describedataprovidersmessagerequesttypedef) 

### describe\_endpoint\_settings

Returns information about the possible endpoint settings available when you
create an endpoint for a specific database engine.

Type annotations and code completion for `#!python session.create_client("dms").describe_endpoint_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_endpoint_settings.html)

```python
# describe_endpoint_settings method definition

await def describe_endpoint_settings(
    self,
    *,
    EngineName: str,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeEndpointSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEndpointSettingsResponseTypeDef](./type_defs.md#describeendpointsettingsresponsetypedef) 


```python
# describe_endpoint_settings method usage example with argument unpacking

kwargs: DescribeEndpointSettingsMessageRequestTypeDef = {  # (1)
    "EngineName": ...,
}

parent.describe_endpoint_settings(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointSettingsMessageRequestTypeDef](./type_defs.md#describeendpointsettingsmessagerequesttypedef) 

### describe\_endpoint\_types

Returns information about the type of endpoints available.

Type annotations and code completion for `#!python session.create_client("dms").describe_endpoint_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_endpoint_types.html)

```python
# describe_endpoint_types method definition

await def describe_endpoint_types(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeEndpointTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeEndpointTypesResponseTypeDef](./type_defs.md#describeendpointtypesresponsetypedef) 


```python
# describe_endpoint_types method usage example with argument unpacking

kwargs: DescribeEndpointTypesMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_endpoint_types(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointTypesMessageRequestTypeDef](./type_defs.md#describeendpointtypesmessagerequesttypedef) 

### describe\_endpoints

Returns information about the endpoints for your account in the current region.

Type annotations and code completion for `#!python session.create_client("dms").describe_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_endpoints.html)

```python
# describe_endpoints method definition

await def describe_endpoints(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeEndpointsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef) 


```python
# describe_endpoints method usage example with argument unpacking

kwargs: DescribeEndpointsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_endpoints(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointsMessageRequestTypeDef](./type_defs.md#describeendpointsmessagerequesttypedef) 

### describe\_engine\_versions

Returns information about the replication instance versions used in the project.

Type annotations and code completion for `#!python session.create_client("dms").describe_engine_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_engine_versions.html)

```python
# describe_engine_versions method definition

await def describe_engine_versions(
    self,
    *,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeEngineVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEngineVersionsResponseTypeDef](./type_defs.md#describeengineversionsresponsetypedef) 


```python
# describe_engine_versions method usage example with argument unpacking

kwargs: DescribeEngineVersionsMessageRequestTypeDef = {  # (1)
    "MaxRecords": ...,
}

parent.describe_engine_versions(**kwargs)
```

1. See [:material-code-braces: DescribeEngineVersionsMessageRequestTypeDef](./type_defs.md#describeengineversionsmessagerequesttypedef) 

### describe\_event\_categories

Lists categories for all event source types, or, if specified, for a specified
source type.

Type annotations and code completion for `#!python session.create_client("dms").describe_event_categories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_event_categories.html)

```python
# describe_event_categories method definition

await def describe_event_categories(
    self,
    *,
    SourceType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> DescribeEventCategoriesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeEventCategoriesResponseTypeDef](./type_defs.md#describeeventcategoriesresponsetypedef) 


```python
# describe_event_categories method usage example with argument unpacking

kwargs: DescribeEventCategoriesMessageRequestTypeDef = {  # (1)
    "SourceType": ...,
}

parent.describe_event_categories(**kwargs)
```

1. See [:material-code-braces: DescribeEventCategoriesMessageRequestTypeDef](./type_defs.md#describeeventcategoriesmessagerequesttypedef) 

### describe\_event\_subscriptions

Lists all the event subscriptions for a customer account.

Type annotations and code completion for `#!python session.create_client("dms").describe_event_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_event_subscriptions.html)

```python
# describe_event_subscriptions method definition

await def describe_event_subscriptions(
    self,
    *,
    SubscriptionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeEventSubscriptionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeEventSubscriptionsResponseTypeDef](./type_defs.md#describeeventsubscriptionsresponsetypedef) 


```python
# describe_event_subscriptions method usage example with argument unpacking

kwargs: DescribeEventSubscriptionsMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.describe_event_subscriptions(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessageRequestTypeDef](./type_defs.md#describeeventsubscriptionsmessagerequesttypedef) 

### describe\_events

Lists events for a given source identifier and source type.

Type annotations and code completion for `#!python session.create_client("dms").describe_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_events.html)

```python
# describe_events method definition

await def describe_events(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Duration: int = ...,
    EventCategories: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeEventsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python
# describe_events method usage example with argument unpacking

kwargs: DescribeEventsMessageRequestTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.describe_events(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessageRequestTypeDef](./type_defs.md#describeeventsmessagerequesttypedef) 

### describe\_extension\_pack\_associations

Returns a paginated list of extension pack associations for the specified
migration project.

Type annotations and code completion for `#!python session.create_client("dms").describe_extension_pack_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_extension_pack_associations.html)

```python
# describe_extension_pack_associations method definition

await def describe_extension_pack_associations(
    self,
    *,
    MigrationProjectIdentifier: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribeExtensionPackAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeExtensionPackAssociationsResponseTypeDef](./type_defs.md#describeextensionpackassociationsresponsetypedef) 


```python
# describe_extension_pack_associations method usage example with argument unpacking

kwargs: DescribeExtensionPackAssociationsMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.describe_extension_pack_associations(**kwargs)
```

1. See [:material-code-braces: DescribeExtensionPackAssociationsMessageRequestTypeDef](./type_defs.md#describeextensionpackassociationsmessagerequesttypedef) 

### describe\_fleet\_advisor\_collectors

Returns a list of the Fleet Advisor collectors in your account.

Type annotations and code completion for `#!python session.create_client("dms").describe_fleet_advisor_collectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_fleet_advisor_collectors.html)

```python
# describe_fleet_advisor_collectors method definition

await def describe_fleet_advisor_collectors(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeFleetAdvisorCollectorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeFleetAdvisorCollectorsResponseTypeDef](./type_defs.md#describefleetadvisorcollectorsresponsetypedef) 


```python
# describe_fleet_advisor_collectors method usage example with argument unpacking

kwargs: DescribeFleetAdvisorCollectorsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_fleet_advisor_collectors(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAdvisorCollectorsRequestRequestTypeDef](./type_defs.md#describefleetadvisorcollectorsrequestrequesttypedef) 

### describe\_fleet\_advisor\_databases

Returns a list of Fleet Advisor databases in your account.

Type annotations and code completion for `#!python session.create_client("dms").describe_fleet_advisor_databases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_fleet_advisor_databases.html)

```python
# describe_fleet_advisor_databases method definition

await def describe_fleet_advisor_databases(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeFleetAdvisorDatabasesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeFleetAdvisorDatabasesResponseTypeDef](./type_defs.md#describefleetadvisordatabasesresponsetypedef) 


```python
# describe_fleet_advisor_databases method usage example with argument unpacking

kwargs: DescribeFleetAdvisorDatabasesRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_fleet_advisor_databases(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAdvisorDatabasesRequestRequestTypeDef](./type_defs.md#describefleetadvisordatabasesrequestrequesttypedef) 

### describe\_fleet\_advisor\_lsa\_analysis

Provides descriptions of large-scale assessment (LSA) analyses produced by your
Fleet Advisor collectors.

Type annotations and code completion for `#!python session.create_client("dms").describe_fleet_advisor_lsa_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_fleet_advisor_lsa_analysis.html)

```python
# describe_fleet_advisor_lsa_analysis method definition

await def describe_fleet_advisor_lsa_analysis(
    self,
    *,
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeFleetAdvisorLsaAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetAdvisorLsaAnalysisResponseTypeDef](./type_defs.md#describefleetadvisorlsaanalysisresponsetypedef) 


```python
# describe_fleet_advisor_lsa_analysis method usage example with argument unpacking

kwargs: DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef = {  # (1)
    "MaxRecords": ...,
}

parent.describe_fleet_advisor_lsa_analysis(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef](./type_defs.md#describefleetadvisorlsaanalysisrequestrequesttypedef) 

### describe\_fleet\_advisor\_schema\_object\_summary

Provides descriptions of the schemas discovered by your Fleet Advisor
collectors.

Type annotations and code completion for `#!python session.create_client("dms").describe_fleet_advisor_schema_object_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_fleet_advisor_schema_object_summary.html)

```python
# describe_fleet_advisor_schema_object_summary method definition

await def describe_fleet_advisor_schema_object_summary(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef](./type_defs.md#describefleetadvisorschemaobjectsummaryresponsetypedef) 


```python
# describe_fleet_advisor_schema_object_summary method usage example with argument unpacking

kwargs: DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_fleet_advisor_schema_object_summary(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef](./type_defs.md#describefleetadvisorschemaobjectsummaryrequestrequesttypedef) 

### describe\_fleet\_advisor\_schemas

Returns a list of schemas detected by Fleet Advisor Collectors in your account.

Type annotations and code completion for `#!python session.create_client("dms").describe_fleet_advisor_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_fleet_advisor_schemas.html)

```python
# describe_fleet_advisor_schemas method definition

await def describe_fleet_advisor_schemas(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeFleetAdvisorSchemasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeFleetAdvisorSchemasResponseTypeDef](./type_defs.md#describefleetadvisorschemasresponsetypedef) 


```python
# describe_fleet_advisor_schemas method usage example with argument unpacking

kwargs: DescribeFleetAdvisorSchemasRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_fleet_advisor_schemas(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAdvisorSchemasRequestRequestTypeDef](./type_defs.md#describefleetadvisorschemasrequestrequesttypedef) 

### describe\_instance\_profiles

Returns a paginated list of instance profiles for your account in the current
region.

Type annotations and code completion for `#!python session.create_client("dms").describe_instance_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_instance_profiles.html)

```python
# describe_instance_profiles method definition

await def describe_instance_profiles(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeInstanceProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeInstanceProfilesResponseTypeDef](./type_defs.md#describeinstanceprofilesresponsetypedef) 


```python
# describe_instance_profiles method usage example with argument unpacking

kwargs: DescribeInstanceProfilesMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_instance_profiles(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceProfilesMessageRequestTypeDef](./type_defs.md#describeinstanceprofilesmessagerequesttypedef) 

### describe\_metadata\_model\_assessments

Returns a paginated list of metadata model assessments for your account in the
current region.

Type annotations and code completion for `#!python session.create_client("dms").describe_metadata_model_assessments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_metadata_model_assessments.html)

```python
# describe_metadata_model_assessments method definition

await def describe_metadata_model_assessments(
    self,
    *,
    MigrationProjectIdentifier: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribeMetadataModelAssessmentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeMetadataModelAssessmentsResponseTypeDef](./type_defs.md#describemetadatamodelassessmentsresponsetypedef) 


```python
# describe_metadata_model_assessments method usage example with argument unpacking

kwargs: DescribeMetadataModelAssessmentsMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.describe_metadata_model_assessments(**kwargs)
```

1. See [:material-code-braces: DescribeMetadataModelAssessmentsMessageRequestTypeDef](./type_defs.md#describemetadatamodelassessmentsmessagerequesttypedef) 

### describe\_metadata\_model\_conversions

Returns a paginated list of metadata model conversions for a migration project.

Type annotations and code completion for `#!python session.create_client("dms").describe_metadata_model_conversions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_metadata_model_conversions.html)

```python
# describe_metadata_model_conversions method definition

await def describe_metadata_model_conversions(
    self,
    *,
    MigrationProjectIdentifier: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribeMetadataModelConversionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeMetadataModelConversionsResponseTypeDef](./type_defs.md#describemetadatamodelconversionsresponsetypedef) 


```python
# describe_metadata_model_conversions method usage example with argument unpacking

kwargs: DescribeMetadataModelConversionsMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.describe_metadata_model_conversions(**kwargs)
```

1. See [:material-code-braces: DescribeMetadataModelConversionsMessageRequestTypeDef](./type_defs.md#describemetadatamodelconversionsmessagerequesttypedef) 

### describe\_metadata\_model\_exports\_as\_script

Returns a paginated list of metadata model exports.

Type annotations and code completion for `#!python session.create_client("dms").describe_metadata_model_exports_as_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_metadata_model_exports_as_script.html)

```python
# describe_metadata_model_exports_as_script method definition

await def describe_metadata_model_exports_as_script(
    self,
    *,
    MigrationProjectIdentifier: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribeMetadataModelExportsAsScriptResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeMetadataModelExportsAsScriptResponseTypeDef](./type_defs.md#describemetadatamodelexportsasscriptresponsetypedef) 


```python
# describe_metadata_model_exports_as_script method usage example with argument unpacking

kwargs: DescribeMetadataModelExportsAsScriptMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.describe_metadata_model_exports_as_script(**kwargs)
```

1. See [:material-code-braces: DescribeMetadataModelExportsAsScriptMessageRequestTypeDef](./type_defs.md#describemetadatamodelexportsasscriptmessagerequesttypedef) 

### describe\_metadata\_model\_exports\_to\_target

Returns a paginated list of metadata model exports.

Type annotations and code completion for `#!python session.create_client("dms").describe_metadata_model_exports_to_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_metadata_model_exports_to_target.html)

```python
# describe_metadata_model_exports_to_target method definition

await def describe_metadata_model_exports_to_target(
    self,
    *,
    MigrationProjectIdentifier: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribeMetadataModelExportsToTargetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeMetadataModelExportsToTargetResponseTypeDef](./type_defs.md#describemetadatamodelexportstotargetresponsetypedef) 


```python
# describe_metadata_model_exports_to_target method usage example with argument unpacking

kwargs: DescribeMetadataModelExportsToTargetMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.describe_metadata_model_exports_to_target(**kwargs)
```

1. See [:material-code-braces: DescribeMetadataModelExportsToTargetMessageRequestTypeDef](./type_defs.md#describemetadatamodelexportstotargetmessagerequesttypedef) 

### describe\_metadata\_model\_imports

Returns a paginated list of metadata model imports.

Type annotations and code completion for `#!python session.create_client("dms").describe_metadata_model_imports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_metadata_model_imports.html)

```python
# describe_metadata_model_imports method definition

await def describe_metadata_model_imports(
    self,
    *,
    MigrationProjectIdentifier: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribeMetadataModelImportsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeMetadataModelImportsResponseTypeDef](./type_defs.md#describemetadatamodelimportsresponsetypedef) 


```python
# describe_metadata_model_imports method usage example with argument unpacking

kwargs: DescribeMetadataModelImportsMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.describe_metadata_model_imports(**kwargs)
```

1. See [:material-code-braces: DescribeMetadataModelImportsMessageRequestTypeDef](./type_defs.md#describemetadatamodelimportsmessagerequesttypedef) 

### describe\_migration\_projects

Returns a paginated list of migration projects for your account in the current
region.

Type annotations and code completion for `#!python session.create_client("dms").describe_migration_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_migration_projects.html)

```python
# describe_migration_projects method definition

await def describe_migration_projects(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeMigrationProjectsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeMigrationProjectsResponseTypeDef](./type_defs.md#describemigrationprojectsresponsetypedef) 


```python
# describe_migration_projects method usage example with argument unpacking

kwargs: DescribeMigrationProjectsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_migration_projects(**kwargs)
```

1. See [:material-code-braces: DescribeMigrationProjectsMessageRequestTypeDef](./type_defs.md#describemigrationprojectsmessagerequesttypedef) 

### describe\_orderable\_replication\_instances

Returns information about the replication instance types that can be created in
the specified region.

Type annotations and code completion for `#!python session.create_client("dms").describe_orderable_replication_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_orderable_replication_instances.html)

```python
# describe_orderable_replication_instances method definition

await def describe_orderable_replication_instances(
    self,
    *,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeOrderableReplicationInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrderableReplicationInstancesResponseTypeDef](./type_defs.md#describeorderablereplicationinstancesresponsetypedef) 


```python
# describe_orderable_replication_instances method usage example with argument unpacking

kwargs: DescribeOrderableReplicationInstancesMessageRequestTypeDef = {  # (1)
    "MaxRecords": ...,
}

parent.describe_orderable_replication_instances(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableReplicationInstancesMessageRequestTypeDef](./type_defs.md#describeorderablereplicationinstancesmessagerequesttypedef) 

### describe\_pending\_maintenance\_actions

For internal use only.

Type annotations and code completion for `#!python session.create_client("dms").describe_pending_maintenance_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_pending_maintenance_actions.html)

```python
# describe_pending_maintenance_actions method definition

await def describe_pending_maintenance_actions(
    self,
    *,
    ReplicationInstanceArn: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribePendingMaintenanceActionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribePendingMaintenanceActionsResponseTypeDef](./type_defs.md#describependingmaintenanceactionsresponsetypedef) 


```python
# describe_pending_maintenance_actions method usage example with argument unpacking

kwargs: DescribePendingMaintenanceActionsMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceArn": ...,
}

parent.describe_pending_maintenance_actions(**kwargs)
```

1. See [:material-code-braces: DescribePendingMaintenanceActionsMessageRequestTypeDef](./type_defs.md#describependingmaintenanceactionsmessagerequesttypedef) 

### describe\_recommendation\_limitations

Returns a paginated list of limitations for recommendations of target Amazon
Web Services engines.

Type annotations and code completion for `#!python session.create_client("dms").describe_recommendation_limitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_recommendation_limitations.html)

```python
# describe_recommendation_limitations method definition

await def describe_recommendation_limitations(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeRecommendationLimitationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeRecommendationLimitationsResponseTypeDef](./type_defs.md#describerecommendationlimitationsresponsetypedef) 


```python
# describe_recommendation_limitations method usage example with argument unpacking

kwargs: DescribeRecommendationLimitationsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_recommendation_limitations(**kwargs)
```

1. See [:material-code-braces: DescribeRecommendationLimitationsRequestRequestTypeDef](./type_defs.md#describerecommendationlimitationsrequestrequesttypedef) 

### describe\_recommendations

Returns a paginated list of target engine recommendations for your source
databases.

Type annotations and code completion for `#!python session.create_client("dms").describe_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_recommendations.html)

```python
# describe_recommendations method definition

await def describe_recommendations(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeRecommendationsResponseTypeDef](./type_defs.md#describerecommendationsresponsetypedef) 


```python
# describe_recommendations method usage example with argument unpacking

kwargs: DescribeRecommendationsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_recommendations(**kwargs)
```

1. See [:material-code-braces: DescribeRecommendationsRequestRequestTypeDef](./type_defs.md#describerecommendationsrequestrequesttypedef) 

### describe\_refresh\_schemas\_status

Returns the status of the RefreshSchemas operation.

Type annotations and code completion for `#!python session.create_client("dms").describe_refresh_schemas_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_refresh_schemas_status.html)

```python
# describe_refresh_schemas_status method definition

await def describe_refresh_schemas_status(
    self,
    *,
    EndpointArn: str,
) -> DescribeRefreshSchemasStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRefreshSchemasStatusResponseTypeDef](./type_defs.md#describerefreshschemasstatusresponsetypedef) 


```python
# describe_refresh_schemas_status method usage example with argument unpacking

kwargs: DescribeRefreshSchemasStatusMessageRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.describe_refresh_schemas_status(**kwargs)
```

1. See [:material-code-braces: DescribeRefreshSchemasStatusMessageRequestTypeDef](./type_defs.md#describerefreshschemasstatusmessagerequesttypedef) 

### describe\_replication\_configs

Returns one or more existing DMS Serverless replication configurations as a
list of structures.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_configs.html)

```python
# describe_replication_configs method definition

await def describe_replication_configs(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationConfigsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationConfigsResponseTypeDef](./type_defs.md#describereplicationconfigsresponsetypedef) 


```python
# describe_replication_configs method usage example with argument unpacking

kwargs: DescribeReplicationConfigsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_replication_configs(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigsMessageRequestTypeDef](./type_defs.md#describereplicationconfigsmessagerequesttypedef) 

### describe\_replication\_instance\_task\_logs

Returns information about the task logs for the specified task.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_instance_task_logs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_instance_task_logs.html)

```python
# describe_replication_instance_task_logs method definition

await def describe_replication_instance_task_logs(
    self,
    *,
    ReplicationInstanceArn: str,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationInstanceTaskLogsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReplicationInstanceTaskLogsResponseTypeDef](./type_defs.md#describereplicationinstancetasklogsresponsetypedef) 


```python
# describe_replication_instance_task_logs method usage example with argument unpacking

kwargs: DescribeReplicationInstanceTaskLogsMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceArn": ...,
}

parent.describe_replication_instance_task_logs(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationInstanceTaskLogsMessageRequestTypeDef](./type_defs.md#describereplicationinstancetasklogsmessagerequesttypedef) 

### describe\_replication\_instances

Returns information about replication instances for your account in the current
region.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_instances.html)

```python
# describe_replication_instances method definition

await def describe_replication_instances(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationInstancesResponseTypeDef](./type_defs.md#describereplicationinstancesresponsetypedef) 


```python
# describe_replication_instances method usage example with argument unpacking

kwargs: DescribeReplicationInstancesMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_replication_instances(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationInstancesMessageRequestTypeDef](./type_defs.md#describereplicationinstancesmessagerequesttypedef) 

### describe\_replication\_subnet\_groups

Returns information about the replication subnet groups.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_subnet_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_subnet_groups.html)

```python
# describe_replication_subnet_groups method definition

await def describe_replication_subnet_groups(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationSubnetGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationSubnetGroupsResponseTypeDef](./type_defs.md#describereplicationsubnetgroupsresponsetypedef) 


```python
# describe_replication_subnet_groups method usage example with argument unpacking

kwargs: DescribeReplicationSubnetGroupsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_replication_subnet_groups(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationSubnetGroupsMessageRequestTypeDef](./type_defs.md#describereplicationsubnetgroupsmessagerequesttypedef) 

### describe\_replication\_table\_statistics

Returns table and schema statistics for one or more provisioned replications
that use a given DMS Serverless replication configuration.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_table_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_table_statistics.html)

```python
# describe_replication_table_statistics method definition

await def describe_replication_table_statistics(
    self,
    *,
    ReplicationConfigArn: str,
    MaxRecords: int = ...,
    Marker: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> DescribeReplicationTableStatisticsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationTableStatisticsResponseTypeDef](./type_defs.md#describereplicationtablestatisticsresponsetypedef) 


```python
# describe_replication_table_statistics method usage example with argument unpacking

kwargs: DescribeReplicationTableStatisticsMessageRequestTypeDef = {  # (1)
    "ReplicationConfigArn": ...,
}

parent.describe_replication_table_statistics(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTableStatisticsMessageRequestTypeDef](./type_defs.md#describereplicationtablestatisticsmessagerequesttypedef) 

### describe\_replication\_task\_assessment\_results

Returns the task assessment results from the Amazon S3 bucket that DMS creates
in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_task_assessment_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_task_assessment_results.html)

```python
# describe_replication_task_assessment_results method definition

await def describe_replication_task_assessment_results(
    self,
    *,
    ReplicationTaskArn: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationTaskAssessmentResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReplicationTaskAssessmentResultsResponseTypeDef](./type_defs.md#describereplicationtaskassessmentresultsresponsetypedef) 


```python
# describe_replication_task_assessment_results method usage example with argument unpacking

kwargs: DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.describe_replication_task_assessment_results(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef](./type_defs.md#describereplicationtaskassessmentresultsmessagerequesttypedef) 

### describe\_replication\_task\_assessment\_runs

Returns a paginated list of premigration assessment runs based on filter
settings.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_task_assessment_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_task_assessment_runs.html)

```python
# describe_replication_task_assessment_runs method definition

await def describe_replication_task_assessment_runs(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationTaskAssessmentRunsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationTaskAssessmentRunsResponseTypeDef](./type_defs.md#describereplicationtaskassessmentrunsresponsetypedef) 


```python
# describe_replication_task_assessment_runs method usage example with argument unpacking

kwargs: DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_replication_task_assessment_runs(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef](./type_defs.md#describereplicationtaskassessmentrunsmessagerequesttypedef) 

### describe\_replication\_task\_individual\_assessments

Returns a paginated list of individual assessments based on filter settings.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_task_individual_assessments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_task_individual_assessments.html)

```python
# describe_replication_task_individual_assessments method definition

await def describe_replication_task_individual_assessments(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationTaskIndividualAssessmentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationTaskIndividualAssessmentsResponseTypeDef](./type_defs.md#describereplicationtaskindividualassessmentsresponsetypedef) 


```python
# describe_replication_task_individual_assessments method usage example with argument unpacking

kwargs: DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_replication_task_individual_assessments(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef](./type_defs.md#describereplicationtaskindividualassessmentsmessagerequesttypedef) 

### describe\_replication\_tasks

Returns information about replication tasks for your account in the current
region.

Type annotations and code completion for `#!python session.create_client("dms").describe_replication_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replication_tasks.html)

```python
# describe_replication_tasks method definition

await def describe_replication_tasks(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WithoutSettings: bool = ...,
) -> DescribeReplicationTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationTasksResponseTypeDef](./type_defs.md#describereplicationtasksresponsetypedef) 


```python
# describe_replication_tasks method usage example with argument unpacking

kwargs: DescribeReplicationTasksMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_replication_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTasksMessageRequestTypeDef](./type_defs.md#describereplicationtasksmessagerequesttypedef) 

### describe\_replications

Provides details on replication progress by returning status information for
one or more provisioned DMS Serverless replications.

Type annotations and code completion for `#!python session.create_client("dms").describe_replications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_replications.html)

```python
# describe_replications method definition

await def describe_replications(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReplicationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeReplicationsResponseTypeDef](./type_defs.md#describereplicationsresponsetypedef) 


```python
# describe_replications method usage example with argument unpacking

kwargs: DescribeReplicationsMessageRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_replications(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationsMessageRequestTypeDef](./type_defs.md#describereplicationsmessagerequesttypedef) 

### describe\_schemas

Returns information about the schema for the specified endpoint.

Type annotations and code completion for `#!python session.create_client("dms").describe_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_schemas.html)

```python
# describe_schemas method definition

await def describe_schemas(
    self,
    *,
    EndpointArn: str,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeSchemasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSchemasResponseTypeDef](./type_defs.md#describeschemasresponsetypedef) 


```python
# describe_schemas method usage example with argument unpacking

kwargs: DescribeSchemasMessageRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.describe_schemas(**kwargs)
```

1. See [:material-code-braces: DescribeSchemasMessageRequestTypeDef](./type_defs.md#describeschemasmessagerequesttypedef) 

### describe\_table\_statistics

Returns table statistics on the database migration task, including table name,
rows inserted, rows updated, and rows deleted.

Type annotations and code completion for `#!python session.create_client("dms").describe_table_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/describe_table_statistics.html)

```python
# describe_table_statistics method definition

await def describe_table_statistics(
    self,
    *,
    ReplicationTaskArn: str,
    MaxRecords: int = ...,
    Marker: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> DescribeTableStatisticsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeTableStatisticsResponseTypeDef](./type_defs.md#describetablestatisticsresponsetypedef) 


```python
# describe_table_statistics method usage example with argument unpacking

kwargs: DescribeTableStatisticsMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.describe_table_statistics(**kwargs)
```

1. See [:material-code-braces: DescribeTableStatisticsMessageRequestTypeDef](./type_defs.md#describetablestatisticsmessagerequesttypedef) 

### export\_metadata\_model\_assessment

Saves a copy of a database migration assessment report to your Amazon S3 bucket.

Type annotations and code completion for `#!python session.create_client("dms").export_metadata_model_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/export_metadata_model_assessment.html)

```python
# export_metadata_model_assessment method definition

await def export_metadata_model_assessment(
    self,
    *,
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    FileName: str = ...,
    AssessmentReportTypes: Sequence[AssessmentReportTypeType] = ...,  # (1)
) -> ExportMetadataModelAssessmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssessmentReportTypeType](./literals.md#assessmentreporttypetype) 
2. See [:material-code-braces: ExportMetadataModelAssessmentResponseTypeDef](./type_defs.md#exportmetadatamodelassessmentresponsetypedef) 


```python
# export_metadata_model_assessment method usage example with argument unpacking

kwargs: ExportMetadataModelAssessmentMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "SelectionRules": ...,
}

parent.export_metadata_model_assessment(**kwargs)
```

1. See [:material-code-braces: ExportMetadataModelAssessmentMessageRequestTypeDef](./type_defs.md#exportmetadatamodelassessmentmessagerequesttypedef) 

### import\_certificate

Uploads the specified certificate.

Type annotations and code completion for `#!python session.create_client("dms").import_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/import_certificate.html)

```python
# import_certificate method definition

await def import_certificate(
    self,
    *,
    CertificateIdentifier: str,
    CertificatePem: str = ...,
    CertificateWallet: BlobTypeDef = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ImportCertificateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ImportCertificateResponseTypeDef](./type_defs.md#importcertificateresponsetypedef) 


```python
# import_certificate method usage example with argument unpacking

kwargs: ImportCertificateMessageRequestTypeDef = {  # (1)
    "CertificateIdentifier": ...,
}

parent.import_certificate(**kwargs)
```

1. See [:material-code-braces: ImportCertificateMessageRequestTypeDef](./type_defs.md#importcertificatemessagerequesttypedef) 

### list\_tags\_for\_resource

Lists all metadata tags attached to an DMS resource, including replication
instance, endpoint, subnet group, and migration task.

Type annotations and code completion for `#!python session.create_client("dms").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str = ...,
    ResourceArnList: Sequence[str] = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceMessageRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceMessageRequestTypeDef](./type_defs.md#listtagsforresourcemessagerequesttypedef) 

### modify\_conversion\_configuration

Modifies the specified schema conversion configuration using the provided
parameters.

Type annotations and code completion for `#!python session.create_client("dms").modify_conversion_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_conversion_configuration.html)

```python
# modify_conversion_configuration method definition

await def modify_conversion_configuration(
    self,
    *,
    MigrationProjectIdentifier: str,
    ConversionConfiguration: str,
) -> ModifyConversionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyConversionConfigurationResponseTypeDef](./type_defs.md#modifyconversionconfigurationresponsetypedef) 


```python
# modify_conversion_configuration method usage example with argument unpacking

kwargs: ModifyConversionConfigurationMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "ConversionConfiguration": ...,
}

parent.modify_conversion_configuration(**kwargs)
```

1. See [:material-code-braces: ModifyConversionConfigurationMessageRequestTypeDef](./type_defs.md#modifyconversionconfigurationmessagerequesttypedef) 

### modify\_data\_migration

Modifies an existing DMS data migration.

Type annotations and code completion for `#!python session.create_client("dms").modify_data_migration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_data_migration.html)

```python
# modify_data_migration method definition

await def modify_data_migration(
    self,
    *,
    DataMigrationIdentifier: str,
    DataMigrationName: str = ...,
    EnableCloudwatchLogs: bool = ...,
    ServiceAccessRoleArn: str = ...,
    DataMigrationType: MigrationTypeValueType = ...,  # (1)
    SourceDataSettings: Sequence[SourceDataSettingTypeDef] = ...,  # (2)
    NumberOfJobs: int = ...,
    SelectionRules: str = ...,
) -> ModifyDataMigrationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: SourceDataSettingTypeDef](./type_defs.md#sourcedatasettingtypedef) 
3. See [:material-code-braces: ModifyDataMigrationResponseTypeDef](./type_defs.md#modifydatamigrationresponsetypedef) 


```python
# modify_data_migration method usage example with argument unpacking

kwargs: ModifyDataMigrationMessageRequestTypeDef = {  # (1)
    "DataMigrationIdentifier": ...,
}

parent.modify_data_migration(**kwargs)
```

1. See [:material-code-braces: ModifyDataMigrationMessageRequestTypeDef](./type_defs.md#modifydatamigrationmessagerequesttypedef) 

### modify\_data\_provider

Modifies the specified data provider using the provided settings.

Type annotations and code completion for `#!python session.create_client("dms").modify_data_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_data_provider.html)

```python
# modify_data_provider method definition

await def modify_data_provider(
    self,
    *,
    DataProviderIdentifier: str,
    DataProviderName: str = ...,
    Description: str = ...,
    Engine: str = ...,
    ExactSettings: bool = ...,
    Settings: DataProviderSettingsTypeDef = ...,  # (1)
) -> ModifyDataProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataProviderSettingsTypeDef](./type_defs.md#dataprovidersettingstypedef) 
2. See [:material-code-braces: ModifyDataProviderResponseTypeDef](./type_defs.md#modifydataproviderresponsetypedef) 


```python
# modify_data_provider method usage example with argument unpacking

kwargs: ModifyDataProviderMessageRequestTypeDef = {  # (1)
    "DataProviderIdentifier": ...,
}

parent.modify_data_provider(**kwargs)
```

1. See [:material-code-braces: ModifyDataProviderMessageRequestTypeDef](./type_defs.md#modifydataprovidermessagerequesttypedef) 

### modify\_endpoint

Modifies the specified endpoint.

Type annotations and code completion for `#!python session.create_client("dms").modify_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_endpoint.html)

```python
# modify_endpoint method definition

await def modify_endpoint(
    self,
    *,
    EndpointArn: str,
    EndpointIdentifier: str = ...,
    EndpointType: ReplicationEndpointTypeValueType = ...,  # (1)
    EngineName: str = ...,
    Username: str = ...,
    Password: str = ...,
    ServerName: str = ...,
    Port: int = ...,
    DatabaseName: str = ...,
    ExtraConnectionAttributes: str = ...,
    CertificateArn: str = ...,
    SslMode: DmsSslModeValueType = ...,  # (2)
    ServiceAccessRoleArn: str = ...,
    ExternalTableDefinition: str = ...,
    DynamoDbSettings: DynamoDbSettingsTypeDef = ...,  # (3)
    S3Settings: S3SettingsTypeDef = ...,  # (4)
    DmsTransferSettings: DmsTransferSettingsTypeDef = ...,  # (5)
    MongoDbSettings: MongoDbSettingsTypeDef = ...,  # (6)
    KinesisSettings: KinesisSettingsTypeDef = ...,  # (7)
    KafkaSettings: KafkaSettingsTypeDef = ...,  # (8)
    ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,  # (9)
    NeptuneSettings: NeptuneSettingsTypeDef = ...,  # (10)
    RedshiftSettings: RedshiftSettingsTypeDef = ...,  # (11)
    PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,  # (12)
    MySQLSettings: MySQLSettingsTypeDef = ...,  # (13)
    OracleSettings: OracleSettingsTypeDef = ...,  # (14)
    SybaseSettings: SybaseSettingsTypeDef = ...,  # (15)
    MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,  # (16)
    IBMDb2Settings: IBMDb2SettingsTypeDef = ...,  # (17)
    DocDbSettings: DocDbSettingsTypeDef = ...,  # (18)
    RedisSettings: RedisSettingsTypeDef = ...,  # (19)
    ExactSettings: bool = ...,
    GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,  # (20)
    TimestreamSettings: TimestreamSettingsTypeDef = ...,  # (21)
) -> ModifyEndpointResponseTypeDef:  # (22)
    ...
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
22. See [:material-code-braces: ModifyEndpointResponseTypeDef](./type_defs.md#modifyendpointresponsetypedef) 


```python
# modify_endpoint method usage example with argument unpacking

kwargs: ModifyEndpointMessageRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.modify_endpoint(**kwargs)
```

1. See [:material-code-braces: ModifyEndpointMessageRequestTypeDef](./type_defs.md#modifyendpointmessagerequesttypedef) 

### modify\_event\_subscription

Modifies an existing DMS event notification subscription.

Type annotations and code completion for `#!python session.create_client("dms").modify_event_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_event_subscription.html)

```python
# modify_event_subscription method definition

await def modify_event_subscription(
    self,
    *,
    SubscriptionName: str,
    SnsTopicArn: str = ...,
    SourceType: str = ...,
    EventCategories: Sequence[str] = ...,
    Enabled: bool = ...,
) -> ModifyEventSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyEventSubscriptionResponseTypeDef](./type_defs.md#modifyeventsubscriptionresponsetypedef) 


```python
# modify_event_subscription method usage example with argument unpacking

kwargs: ModifyEventSubscriptionMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.modify_event_subscription(**kwargs)
```

1. See [:material-code-braces: ModifyEventSubscriptionMessageRequestTypeDef](./type_defs.md#modifyeventsubscriptionmessagerequesttypedef) 

### modify\_instance\_profile

Modifies the specified instance profile using the provided parameters.

Type annotations and code completion for `#!python session.create_client("dms").modify_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_instance_profile.html)

```python
# modify_instance_profile method definition

await def modify_instance_profile(
    self,
    *,
    InstanceProfileIdentifier: str,
    AvailabilityZone: str = ...,
    KmsKeyArn: str = ...,
    PubliclyAccessible: bool = ...,
    NetworkType: str = ...,
    InstanceProfileName: str = ...,
    Description: str = ...,
    SubnetGroupIdentifier: str = ...,
    VpcSecurityGroups: Sequence[str] = ...,
) -> ModifyInstanceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyInstanceProfileResponseTypeDef](./type_defs.md#modifyinstanceprofileresponsetypedef) 


```python
# modify_instance_profile method usage example with argument unpacking

kwargs: ModifyInstanceProfileMessageRequestTypeDef = {  # (1)
    "InstanceProfileIdentifier": ...,
}

parent.modify_instance_profile(**kwargs)
```

1. See [:material-code-braces: ModifyInstanceProfileMessageRequestTypeDef](./type_defs.md#modifyinstanceprofilemessagerequesttypedef) 

### modify\_migration\_project

Modifies the specified migration project using the provided parameters.

Type annotations and code completion for `#!python session.create_client("dms").modify_migration_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_migration_project.html)

```python
# modify_migration_project method definition

await def modify_migration_project(
    self,
    *,
    MigrationProjectIdentifier: str,
    MigrationProjectName: str = ...,
    SourceDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef] = ...,  # (1)
    TargetDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef] = ...,  # (1)
    InstanceProfileIdentifier: str = ...,
    TransformationRules: str = ...,
    Description: str = ...,
    SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...,  # (3)
) -> ModifyMigrationProjectResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
2. See [:material-code-braces: DataProviderDescriptorDefinitionTypeDef](./type_defs.md#dataproviderdescriptordefinitiontypedef) 
3. See [:material-code-braces: SCApplicationAttributesTypeDef](./type_defs.md#scapplicationattributestypedef) 
4. See [:material-code-braces: ModifyMigrationProjectResponseTypeDef](./type_defs.md#modifymigrationprojectresponsetypedef) 


```python
# modify_migration_project method usage example with argument unpacking

kwargs: ModifyMigrationProjectMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.modify_migration_project(**kwargs)
```

1. See [:material-code-braces: ModifyMigrationProjectMessageRequestTypeDef](./type_defs.md#modifymigrationprojectmessagerequesttypedef) 

### modify\_replication\_config

Modifies an existing DMS Serverless replication configuration that you can use
to start a replication.

Type annotations and code completion for `#!python session.create_client("dms").modify_replication_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_replication_config.html)

```python
# modify_replication_config method definition

await def modify_replication_config(
    self,
    *,
    ReplicationConfigArn: str,
    ReplicationConfigIdentifier: str = ...,
    ReplicationType: MigrationTypeValueType = ...,  # (1)
    TableMappings: str = ...,
    ReplicationSettings: str = ...,
    SupplementalSettings: str = ...,
    ComputeConfig: ComputeConfigTypeDef = ...,  # (2)
    SourceEndpointArn: str = ...,
    TargetEndpointArn: str = ...,
) -> ModifyReplicationConfigResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: ComputeConfigTypeDef](./type_defs.md#computeconfigtypedef) 
3. See [:material-code-braces: ModifyReplicationConfigResponseTypeDef](./type_defs.md#modifyreplicationconfigresponsetypedef) 


```python
# modify_replication_config method usage example with argument unpacking

kwargs: ModifyReplicationConfigMessageRequestTypeDef = {  # (1)
    "ReplicationConfigArn": ...,
}

parent.modify_replication_config(**kwargs)
```

1. See [:material-code-braces: ModifyReplicationConfigMessageRequestTypeDef](./type_defs.md#modifyreplicationconfigmessagerequesttypedef) 

### modify\_replication\_instance

Modifies the replication instance to apply new settings.

Type annotations and code completion for `#!python session.create_client("dms").modify_replication_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_replication_instance.html)

```python
# modify_replication_instance method definition

await def modify_replication_instance(
    self,
    *,
    ReplicationInstanceArn: str,
    AllocatedStorage: int = ...,
    ApplyImmediately: bool = ...,
    ReplicationInstanceClass: str = ...,
    VpcSecurityGroupIds: Sequence[str] = ...,
    PreferredMaintenanceWindow: str = ...,
    MultiAZ: bool = ...,
    EngineVersion: str = ...,
    AllowMajorVersionUpgrade: bool = ...,
    AutoMinorVersionUpgrade: bool = ...,
    ReplicationInstanceIdentifier: str = ...,
    NetworkType: str = ...,
    KerberosAuthenticationSettings: KerberosAuthenticationSettingsTypeDef = ...,  # (1)
) -> ModifyReplicationInstanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KerberosAuthenticationSettingsTypeDef](./type_defs.md#kerberosauthenticationsettingstypedef) 
2. See [:material-code-braces: ModifyReplicationInstanceResponseTypeDef](./type_defs.md#modifyreplicationinstanceresponsetypedef) 


```python
# modify_replication_instance method usage example with argument unpacking

kwargs: ModifyReplicationInstanceMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceArn": ...,
}

parent.modify_replication_instance(**kwargs)
```

1. See [:material-code-braces: ModifyReplicationInstanceMessageRequestTypeDef](./type_defs.md#modifyreplicationinstancemessagerequesttypedef) 

### modify\_replication\_subnet\_group

Modifies the settings for the specified replication subnet group.

Type annotations and code completion for `#!python session.create_client("dms").modify_replication_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_replication_subnet_group.html)

```python
# modify_replication_subnet_group method definition

await def modify_replication_subnet_group(
    self,
    *,
    ReplicationSubnetGroupIdentifier: str,
    SubnetIds: Sequence[str],
    ReplicationSubnetGroupDescription: str = ...,
) -> ModifyReplicationSubnetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyReplicationSubnetGroupResponseTypeDef](./type_defs.md#modifyreplicationsubnetgroupresponsetypedef) 


```python
# modify_replication_subnet_group method usage example with argument unpacking

kwargs: ModifyReplicationSubnetGroupMessageRequestTypeDef = {  # (1)
    "ReplicationSubnetGroupIdentifier": ...,
    "SubnetIds": ...,
}

parent.modify_replication_subnet_group(**kwargs)
```

1. See [:material-code-braces: ModifyReplicationSubnetGroupMessageRequestTypeDef](./type_defs.md#modifyreplicationsubnetgroupmessagerequesttypedef) 

### modify\_replication\_task

Modifies the specified replication task.

Type annotations and code completion for `#!python session.create_client("dms").modify_replication_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/modify_replication_task.html)

```python
# modify_replication_task method definition

await def modify_replication_task(
    self,
    *,
    ReplicationTaskArn: str,
    ReplicationTaskIdentifier: str = ...,
    MigrationType: MigrationTypeValueType = ...,  # (1)
    TableMappings: str = ...,
    ReplicationTaskSettings: str = ...,
    CdcStartTime: TimestampTypeDef = ...,
    CdcStartPosition: str = ...,
    CdcStopPosition: str = ...,
    TaskData: str = ...,
) -> ModifyReplicationTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MigrationTypeValueType](./literals.md#migrationtypevaluetype) 
2. See [:material-code-braces: ModifyReplicationTaskResponseTypeDef](./type_defs.md#modifyreplicationtaskresponsetypedef) 


```python
# modify_replication_task method usage example with argument unpacking

kwargs: ModifyReplicationTaskMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.modify_replication_task(**kwargs)
```

1. See [:material-code-braces: ModifyReplicationTaskMessageRequestTypeDef](./type_defs.md#modifyreplicationtaskmessagerequesttypedef) 

### move\_replication\_task

Moves a replication task from its current replication instance to a different
target replication instance using the specified parameters.

Type annotations and code completion for `#!python session.create_client("dms").move_replication_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/move_replication_task.html)

```python
# move_replication_task method definition

await def move_replication_task(
    self,
    *,
    ReplicationTaskArn: str,
    TargetReplicationInstanceArn: str,
) -> MoveReplicationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MoveReplicationTaskResponseTypeDef](./type_defs.md#movereplicationtaskresponsetypedef) 


```python
# move_replication_task method usage example with argument unpacking

kwargs: MoveReplicationTaskMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
    "TargetReplicationInstanceArn": ...,
}

parent.move_replication_task(**kwargs)
```

1. See [:material-code-braces: MoveReplicationTaskMessageRequestTypeDef](./type_defs.md#movereplicationtaskmessagerequesttypedef) 

### reboot\_replication\_instance

Reboots a replication instance.

Type annotations and code completion for `#!python session.create_client("dms").reboot_replication_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/reboot_replication_instance.html)

```python
# reboot_replication_instance method definition

await def reboot_replication_instance(
    self,
    *,
    ReplicationInstanceArn: str,
    ForceFailover: bool = ...,
    ForcePlannedFailover: bool = ...,
) -> RebootReplicationInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RebootReplicationInstanceResponseTypeDef](./type_defs.md#rebootreplicationinstanceresponsetypedef) 


```python
# reboot_replication_instance method usage example with argument unpacking

kwargs: RebootReplicationInstanceMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceArn": ...,
}

parent.reboot_replication_instance(**kwargs)
```

1. See [:material-code-braces: RebootReplicationInstanceMessageRequestTypeDef](./type_defs.md#rebootreplicationinstancemessagerequesttypedef) 

### refresh\_schemas

Populates the schema for the specified endpoint.

Type annotations and code completion for `#!python session.create_client("dms").refresh_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/refresh_schemas.html)

```python
# refresh_schemas method definition

await def refresh_schemas(
    self,
    *,
    EndpointArn: str,
    ReplicationInstanceArn: str,
) -> RefreshSchemasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RefreshSchemasResponseTypeDef](./type_defs.md#refreshschemasresponsetypedef) 


```python
# refresh_schemas method usage example with argument unpacking

kwargs: RefreshSchemasMessageRequestTypeDef = {  # (1)
    "EndpointArn": ...,
    "ReplicationInstanceArn": ...,
}

parent.refresh_schemas(**kwargs)
```

1. See [:material-code-braces: RefreshSchemasMessageRequestTypeDef](./type_defs.md#refreshschemasmessagerequesttypedef) 

### reload\_replication\_tables

Reloads the target database table with the source data for a given DMS
Serverless replication configuration.

Type annotations and code completion for `#!python session.create_client("dms").reload_replication_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/reload_replication_tables.html)

```python
# reload_replication_tables method definition

await def reload_replication_tables(
    self,
    *,
    ReplicationConfigArn: str,
    TablesToReload: Sequence[TableToReloadTypeDef],  # (1)
    ReloadOption: ReloadOptionValueType = ...,  # (2)
) -> ReloadReplicationTablesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TableToReloadTypeDef](./type_defs.md#tabletoreloadtypedef) 
2. See [:material-code-brackets: ReloadOptionValueType](./literals.md#reloadoptionvaluetype) 
3. See [:material-code-braces: ReloadReplicationTablesResponseTypeDef](./type_defs.md#reloadreplicationtablesresponsetypedef) 


```python
# reload_replication_tables method usage example with argument unpacking

kwargs: ReloadReplicationTablesMessageRequestTypeDef = {  # (1)
    "ReplicationConfigArn": ...,
    "TablesToReload": ...,
}

parent.reload_replication_tables(**kwargs)
```

1. See [:material-code-braces: ReloadReplicationTablesMessageRequestTypeDef](./type_defs.md#reloadreplicationtablesmessagerequesttypedef) 

### reload\_tables

Reloads the target database table with the source data.

Type annotations and code completion for `#!python session.create_client("dms").reload_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/reload_tables.html)

```python
# reload_tables method definition

await def reload_tables(
    self,
    *,
    ReplicationTaskArn: str,
    TablesToReload: Sequence[TableToReloadTypeDef],  # (1)
    ReloadOption: ReloadOptionValueType = ...,  # (2)
) -> ReloadTablesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TableToReloadTypeDef](./type_defs.md#tabletoreloadtypedef) 
2. See [:material-code-brackets: ReloadOptionValueType](./literals.md#reloadoptionvaluetype) 
3. See [:material-code-braces: ReloadTablesResponseTypeDef](./type_defs.md#reloadtablesresponsetypedef) 


```python
# reload_tables method usage example with argument unpacking

kwargs: ReloadTablesMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
    "TablesToReload": ...,
}

parent.reload_tables(**kwargs)
```

1. See [:material-code-braces: ReloadTablesMessageRequestTypeDef](./type_defs.md#reloadtablesmessagerequesttypedef) 

### remove\_tags\_from\_resource

Removes metadata tags from an DMS resource, including replication instance,
endpoint, subnet group, and migration task.

Type annotations and code completion for `#!python session.create_client("dms").remove_tags_from_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/remove_tags_from_resource.html)

```python
# remove_tags_from_resource method definition

await def remove_tags_from_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# remove_tags_from_resource method usage example with argument unpacking

kwargs: RemoveTagsFromResourceMessageRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.remove_tags_from_resource(**kwargs)
```

1. See [:material-code-braces: RemoveTagsFromResourceMessageRequestTypeDef](./type_defs.md#removetagsfromresourcemessagerequesttypedef) 

### run\_fleet\_advisor\_lsa\_analysis

Runs large-scale assessment (LSA) analysis on every Fleet Advisor collector in
your account.

Type annotations and code completion for `#!python session.create_client("dms").run_fleet_advisor_lsa_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/run_fleet_advisor_lsa_analysis.html)

```python
# run_fleet_advisor_lsa_analysis method definition

await def run_fleet_advisor_lsa_analysis(
    self,
) -> RunFleetAdvisorLsaAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RunFleetAdvisorLsaAnalysisResponseTypeDef](./type_defs.md#runfleetadvisorlsaanalysisresponsetypedef) 

### start\_data\_migration

Starts the specified data migration.

Type annotations and code completion for `#!python session.create_client("dms").start_data_migration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_data_migration.html)

```python
# start_data_migration method definition

await def start_data_migration(
    self,
    *,
    DataMigrationIdentifier: str,
    StartType: StartReplicationMigrationTypeValueType,  # (1)
) -> StartDataMigrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StartReplicationMigrationTypeValueType](./literals.md#startreplicationmigrationtypevaluetype) 
2. See [:material-code-braces: StartDataMigrationResponseTypeDef](./type_defs.md#startdatamigrationresponsetypedef) 


```python
# start_data_migration method usage example with argument unpacking

kwargs: StartDataMigrationMessageRequestTypeDef = {  # (1)
    "DataMigrationIdentifier": ...,
    "StartType": ...,
}

parent.start_data_migration(**kwargs)
```

1. See [:material-code-braces: StartDataMigrationMessageRequestTypeDef](./type_defs.md#startdatamigrationmessagerequesttypedef) 

### start\_extension\_pack\_association

Applies the extension pack to your target database.

Type annotations and code completion for `#!python session.create_client("dms").start_extension_pack_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_extension_pack_association.html)

```python
# start_extension_pack_association method definition

await def start_extension_pack_association(
    self,
    *,
    MigrationProjectIdentifier: str,
) -> StartExtensionPackAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartExtensionPackAssociationResponseTypeDef](./type_defs.md#startextensionpackassociationresponsetypedef) 


```python
# start_extension_pack_association method usage example with argument unpacking

kwargs: StartExtensionPackAssociationMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
}

parent.start_extension_pack_association(**kwargs)
```

1. See [:material-code-braces: StartExtensionPackAssociationMessageRequestTypeDef](./type_defs.md#startextensionpackassociationmessagerequesttypedef) 

### start\_metadata\_model\_assessment

Creates a database migration assessment report by assessing the migration
complexity for your source database.

Type annotations and code completion for `#!python session.create_client("dms").start_metadata_model_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_metadata_model_assessment.html)

```python
# start_metadata_model_assessment method definition

await def start_metadata_model_assessment(
    self,
    *,
    MigrationProjectIdentifier: str,
    SelectionRules: str,
) -> StartMetadataModelAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMetadataModelAssessmentResponseTypeDef](./type_defs.md#startmetadatamodelassessmentresponsetypedef) 


```python
# start_metadata_model_assessment method usage example with argument unpacking

kwargs: StartMetadataModelAssessmentMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "SelectionRules": ...,
}

parent.start_metadata_model_assessment(**kwargs)
```

1. See [:material-code-braces: StartMetadataModelAssessmentMessageRequestTypeDef](./type_defs.md#startmetadatamodelassessmentmessagerequesttypedef) 

### start\_metadata\_model\_conversion

Converts your source database objects to a format compatible with the target
database.

Type annotations and code completion for `#!python session.create_client("dms").start_metadata_model_conversion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_metadata_model_conversion.html)

```python
# start_metadata_model_conversion method definition

await def start_metadata_model_conversion(
    self,
    *,
    MigrationProjectIdentifier: str,
    SelectionRules: str,
) -> StartMetadataModelConversionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMetadataModelConversionResponseTypeDef](./type_defs.md#startmetadatamodelconversionresponsetypedef) 


```python
# start_metadata_model_conversion method usage example with argument unpacking

kwargs: StartMetadataModelConversionMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "SelectionRules": ...,
}

parent.start_metadata_model_conversion(**kwargs)
```

1. See [:material-code-braces: StartMetadataModelConversionMessageRequestTypeDef](./type_defs.md#startmetadatamodelconversionmessagerequesttypedef) 

### start\_metadata\_model\_export\_as\_script

Saves your converted code to a file as a SQL script, and stores this file on
your Amazon S3 bucket.

Type annotations and code completion for `#!python session.create_client("dms").start_metadata_model_export_as_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_metadata_model_export_as_script.html)

```python
# start_metadata_model_export_as_script method definition

await def start_metadata_model_export_as_script(
    self,
    *,
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    Origin: OriginTypeValueType,  # (1)
    FileName: str = ...,
) -> StartMetadataModelExportAsScriptResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OriginTypeValueType](./literals.md#origintypevaluetype) 
2. See [:material-code-braces: StartMetadataModelExportAsScriptResponseTypeDef](./type_defs.md#startmetadatamodelexportasscriptresponsetypedef) 


```python
# start_metadata_model_export_as_script method usage example with argument unpacking

kwargs: StartMetadataModelExportAsScriptMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "SelectionRules": ...,
    "Origin": ...,
}

parent.start_metadata_model_export_as_script(**kwargs)
```

1. See [:material-code-braces: StartMetadataModelExportAsScriptMessageRequestTypeDef](./type_defs.md#startmetadatamodelexportasscriptmessagerequesttypedef) 

### start\_metadata\_model\_export\_to\_target

Applies converted database objects to your target database.

Type annotations and code completion for `#!python session.create_client("dms").start_metadata_model_export_to_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_metadata_model_export_to_target.html)

```python
# start_metadata_model_export_to_target method definition

await def start_metadata_model_export_to_target(
    self,
    *,
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    OverwriteExtensionPack: bool = ...,
) -> StartMetadataModelExportToTargetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMetadataModelExportToTargetResponseTypeDef](./type_defs.md#startmetadatamodelexporttotargetresponsetypedef) 


```python
# start_metadata_model_export_to_target method usage example with argument unpacking

kwargs: StartMetadataModelExportToTargetMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "SelectionRules": ...,
}

parent.start_metadata_model_export_to_target(**kwargs)
```

1. See [:material-code-braces: StartMetadataModelExportToTargetMessageRequestTypeDef](./type_defs.md#startmetadatamodelexporttotargetmessagerequesttypedef) 

### start\_metadata\_model\_import

Loads the metadata for all the dependent database objects of the parent object.

Type annotations and code completion for `#!python session.create_client("dms").start_metadata_model_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_metadata_model_import.html)

```python
# start_metadata_model_import method definition

await def start_metadata_model_import(
    self,
    *,
    MigrationProjectIdentifier: str,
    SelectionRules: str,
    Origin: OriginTypeValueType,  # (1)
    Refresh: bool = ...,
) -> StartMetadataModelImportResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OriginTypeValueType](./literals.md#origintypevaluetype) 
2. See [:material-code-braces: StartMetadataModelImportResponseTypeDef](./type_defs.md#startmetadatamodelimportresponsetypedef) 


```python
# start_metadata_model_import method usage example with argument unpacking

kwargs: StartMetadataModelImportMessageRequestTypeDef = {  # (1)
    "MigrationProjectIdentifier": ...,
    "SelectionRules": ...,
    "Origin": ...,
}

parent.start_metadata_model_import(**kwargs)
```

1. See [:material-code-braces: StartMetadataModelImportMessageRequestTypeDef](./type_defs.md#startmetadatamodelimportmessagerequesttypedef) 

### start\_recommendations

Starts the analysis of your source database to provide recommendations of
target engines.

Type annotations and code completion for `#!python session.create_client("dms").start_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_recommendations.html)

```python
# start_recommendations method definition

await def start_recommendations(
    self,
    *,
    DatabaseId: str,
    Settings: RecommendationSettingsTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RecommendationSettingsTypeDef](./type_defs.md#recommendationsettingstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_recommendations method usage example with argument unpacking

kwargs: StartRecommendationsRequestRequestTypeDef = {  # (1)
    "DatabaseId": ...,
    "Settings": ...,
}

parent.start_recommendations(**kwargs)
```

1. See [:material-code-braces: StartRecommendationsRequestRequestTypeDef](./type_defs.md#startrecommendationsrequestrequesttypedef) 

### start\_replication

For a given DMS Serverless replication configuration, DMS connects to the
source endpoint and collects the metadata to analyze the replication workload.

Type annotations and code completion for `#!python session.create_client("dms").start_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_replication.html)

```python
# start_replication method definition

await def start_replication(
    self,
    *,
    ReplicationConfigArn: str,
    StartReplicationType: str,
    CdcStartTime: TimestampTypeDef = ...,
    CdcStartPosition: str = ...,
    CdcStopPosition: str = ...,
) -> StartReplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartReplicationResponseTypeDef](./type_defs.md#startreplicationresponsetypedef) 


```python
# start_replication method usage example with argument unpacking

kwargs: StartReplicationMessageRequestTypeDef = {  # (1)
    "ReplicationConfigArn": ...,
    "StartReplicationType": ...,
}

parent.start_replication(**kwargs)
```

1. See [:material-code-braces: StartReplicationMessageRequestTypeDef](./type_defs.md#startreplicationmessagerequesttypedef) 

### start\_replication\_task

Starts the replication task.

Type annotations and code completion for `#!python session.create_client("dms").start_replication_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_replication_task.html)

```python
# start_replication_task method definition

await def start_replication_task(
    self,
    *,
    ReplicationTaskArn: str,
    StartReplicationTaskType: StartReplicationTaskTypeValueType,  # (1)
    CdcStartTime: TimestampTypeDef = ...,
    CdcStartPosition: str = ...,
    CdcStopPosition: str = ...,
) -> StartReplicationTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StartReplicationTaskTypeValueType](./literals.md#startreplicationtasktypevaluetype) 
2. See [:material-code-braces: StartReplicationTaskResponseTypeDef](./type_defs.md#startreplicationtaskresponsetypedef) 


```python
# start_replication_task method usage example with argument unpacking

kwargs: StartReplicationTaskMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
    "StartReplicationTaskType": ...,
}

parent.start_replication_task(**kwargs)
```

1. See [:material-code-braces: StartReplicationTaskMessageRequestTypeDef](./type_defs.md#startreplicationtaskmessagerequesttypedef) 

### start\_replication\_task\_assessment

Starts the replication task assessment for unsupported data types in the source
database.

Type annotations and code completion for `#!python session.create_client("dms").start_replication_task_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_replication_task_assessment.html)

```python
# start_replication_task_assessment method definition

await def start_replication_task_assessment(
    self,
    *,
    ReplicationTaskArn: str,
) -> StartReplicationTaskAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartReplicationTaskAssessmentResponseTypeDef](./type_defs.md#startreplicationtaskassessmentresponsetypedef) 


```python
# start_replication_task_assessment method usage example with argument unpacking

kwargs: StartReplicationTaskAssessmentMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.start_replication_task_assessment(**kwargs)
```

1. See [:material-code-braces: StartReplicationTaskAssessmentMessageRequestTypeDef](./type_defs.md#startreplicationtaskassessmentmessagerequesttypedef) 

### start\_replication\_task\_assessment\_run

Starts a new premigration assessment run for one or more individual assessments
of a migration task.

Type annotations and code completion for `#!python session.create_client("dms").start_replication_task_assessment_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/start_replication_task_assessment_run.html)

```python
# start_replication_task_assessment_run method definition

await def start_replication_task_assessment_run(
    self,
    *,
    ReplicationTaskArn: str,
    ServiceAccessRoleArn: str,
    ResultLocationBucket: str,
    AssessmentRunName: str,
    ResultLocationFolder: str = ...,
    ResultEncryptionMode: str = ...,
    ResultKmsKeyArn: str = ...,
    IncludeOnly: Sequence[str] = ...,
    Exclude: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> StartReplicationTaskAssessmentRunResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: StartReplicationTaskAssessmentRunResponseTypeDef](./type_defs.md#startreplicationtaskassessmentrunresponsetypedef) 


```python
# start_replication_task_assessment_run method usage example with argument unpacking

kwargs: StartReplicationTaskAssessmentRunMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
    "ServiceAccessRoleArn": ...,
    "ResultLocationBucket": ...,
    "AssessmentRunName": ...,
}

parent.start_replication_task_assessment_run(**kwargs)
```

1. See [:material-code-braces: StartReplicationTaskAssessmentRunMessageRequestTypeDef](./type_defs.md#startreplicationtaskassessmentrunmessagerequesttypedef) 

### stop\_data\_migration

Stops the specified data migration.

Type annotations and code completion for `#!python session.create_client("dms").stop_data_migration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/stop_data_migration.html)

```python
# stop_data_migration method definition

await def stop_data_migration(
    self,
    *,
    DataMigrationIdentifier: str,
) -> StopDataMigrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopDataMigrationResponseTypeDef](./type_defs.md#stopdatamigrationresponsetypedef) 


```python
# stop_data_migration method usage example with argument unpacking

kwargs: StopDataMigrationMessageRequestTypeDef = {  # (1)
    "DataMigrationIdentifier": ...,
}

parent.stop_data_migration(**kwargs)
```

1. See [:material-code-braces: StopDataMigrationMessageRequestTypeDef](./type_defs.md#stopdatamigrationmessagerequesttypedef) 

### stop\_replication

For a given DMS Serverless replication configuration, DMS stops any and all
ongoing DMS Serverless replications.

Type annotations and code completion for `#!python session.create_client("dms").stop_replication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/stop_replication.html)

```python
# stop_replication method definition

await def stop_replication(
    self,
    *,
    ReplicationConfigArn: str,
) -> StopReplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopReplicationResponseTypeDef](./type_defs.md#stopreplicationresponsetypedef) 


```python
# stop_replication method usage example with argument unpacking

kwargs: StopReplicationMessageRequestTypeDef = {  # (1)
    "ReplicationConfigArn": ...,
}

parent.stop_replication(**kwargs)
```

1. See [:material-code-braces: StopReplicationMessageRequestTypeDef](./type_defs.md#stopreplicationmessagerequesttypedef) 

### stop\_replication\_task

Stops the replication task.

Type annotations and code completion for `#!python session.create_client("dms").stop_replication_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/stop_replication_task.html)

```python
# stop_replication_task method definition

await def stop_replication_task(
    self,
    *,
    ReplicationTaskArn: str,
) -> StopReplicationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopReplicationTaskResponseTypeDef](./type_defs.md#stopreplicationtaskresponsetypedef) 


```python
# stop_replication_task method usage example with argument unpacking

kwargs: StopReplicationTaskMessageRequestTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.stop_replication_task(**kwargs)
```

1. See [:material-code-braces: StopReplicationTaskMessageRequestTypeDef](./type_defs.md#stopreplicationtaskmessagerequesttypedef) 

### test\_connection

Tests the connection between the replication instance and the endpoint.

Type annotations and code completion for `#!python session.create_client("dms").test_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/test_connection.html)

```python
# test_connection method definition

await def test_connection(
    self,
    *,
    ReplicationInstanceArn: str,
    EndpointArn: str,
) -> TestConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestConnectionResponseTypeDef](./type_defs.md#testconnectionresponsetypedef) 


```python
# test_connection method usage example with argument unpacking

kwargs: TestConnectionMessageRequestTypeDef = {  # (1)
    "ReplicationInstanceArn": ...,
    "EndpointArn": ...,
}

parent.test_connection(**kwargs)
```

1. See [:material-code-braces: TestConnectionMessageRequestTypeDef](./type_defs.md#testconnectionmessagerequesttypedef) 

### update\_subscriptions\_to\_event\_bridge

Migrates 10 active and enabled Amazon SNS subscriptions at a time and converts
them to corresponding Amazon EventBridge rules.

Type annotations and code completion for `#!python session.create_client("dms").update_subscriptions_to_event_bridge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/client/update_subscriptions_to_event_bridge.html)

```python
# update_subscriptions_to_event_bridge method definition

await def update_subscriptions_to_event_bridge(
    self,
    *,
    ForceMove: bool = ...,
) -> UpdateSubscriptionsToEventBridgeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSubscriptionsToEventBridgeResponseTypeDef](./type_defs.md#updatesubscriptionstoeventbridgeresponsetypedef) 


```python
# update_subscriptions_to_event_bridge method usage example with argument unpacking

kwargs: UpdateSubscriptionsToEventBridgeMessageRequestTypeDef = {  # (1)
    "ForceMove": ...,
}

parent.update_subscriptions_to_event_bridge(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriptionsToEventBridgeMessageRequestTypeDef](./type_defs.md#updatesubscriptionstoeventbridgemessagerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("dms").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "DatabaseMigrationServiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("dms").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator` method with overloads.

- `client.get_paginator("describe_certificates")` -> [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
- `client.get_paginator("describe_connections")` -> [DescribeConnectionsPaginator](./paginators.md#describeconnectionspaginator)
- `client.get_paginator("describe_data_migrations")` -> [DescribeDataMigrationsPaginator](./paginators.md#describedatamigrationspaginator)
- `client.get_paginator("describe_endpoint_types")` -> [DescribeEndpointTypesPaginator](./paginators.md#describeendpointtypespaginator)
- `client.get_paginator("describe_endpoints")` -> [DescribeEndpointsPaginator](./paginators.md#describeendpointspaginator)
- `client.get_paginator("describe_event_subscriptions")` -> [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
- `client.get_paginator("describe_events")` -> [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_orderable_replication_instances")` -> [DescribeOrderableReplicationInstancesPaginator](./paginators.md#describeorderablereplicationinstancespaginator)
- `client.get_paginator("describe_replication_instances")` -> [DescribeReplicationInstancesPaginator](./paginators.md#describereplicationinstancespaginator)
- `client.get_paginator("describe_replication_subnet_groups")` -> [DescribeReplicationSubnetGroupsPaginator](./paginators.md#describereplicationsubnetgroupspaginator)
- `client.get_paginator("describe_replication_task_assessment_results")` -> [DescribeReplicationTaskAssessmentResultsPaginator](./paginators.md#describereplicationtaskassessmentresultspaginator)
- `client.get_paginator("describe_replication_tasks")` -> [DescribeReplicationTasksPaginator](./paginators.md#describereplicationtaskspaginator)
- `client.get_paginator("describe_schemas")` -> [DescribeSchemasPaginator](./paginators.md#describeschemaspaginator)
- `client.get_paginator("describe_table_statistics")` -> [DescribeTableStatisticsPaginator](./paginators.md#describetablestatisticspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("dms").get_waiter` method with overloads.

- `client.get_waiter("endpoint_deleted")` -> [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)
- `client.get_waiter("replication_instance_available")` -> [ReplicationInstanceAvailableWaiter](./waiters.md#replicationinstanceavailablewaiter)
- `client.get_waiter("replication_instance_deleted")` -> [ReplicationInstanceDeletedWaiter](./waiters.md#replicationinstancedeletedwaiter)
- `client.get_waiter("replication_task_deleted")` -> [ReplicationTaskDeletedWaiter](./waiters.md#replicationtaskdeletedwaiter)
- `client.get_waiter("replication_task_ready")` -> [ReplicationTaskReadyWaiter](./waiters.md#replicationtaskreadywaiter)
- `client.get_waiter("replication_task_running")` -> [ReplicationTaskRunningWaiter](./waiters.md#replicationtaskrunningwaiter)
- `client.get_waiter("replication_task_stopped")` -> [ReplicationTaskStoppedWaiter](./waiters.md#replicationtaskstoppedwaiter)
- `client.get_waiter("test_connection_succeeds")` -> [TestConnectionSucceedsWaiter](./waiters.md#testconnectionsucceedswaiter)

