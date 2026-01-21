# OdbClient

> [Index](../README.md) > [Odb](./README.md) > OdbClient

!!! note ""

    Auto-generated documentation for [Odb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#odb)
    type annotations stubs module [types-aiobotocore-odb](https://pypi.org/project/types-aiobotocore-odb/).

## OdbClient

Type annotations and code completion for `#!python session.create_client("odb")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#Odb.Client)

```python
# OdbClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_odb.client import OdbClient

session = get_session()
async with session.create_client("odb") as client:
    client: OdbClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("odb").exceptions` structure.

```python
# OdbClient.exceptions usage example

async with session.create_client("odb") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# OdbClient usage type checking example

from types_aiobotocore_odb.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("odb").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("odb").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/generate_presigned_url.html)

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


### accept\_marketplace\_registration

Registers the Amazon Web Services Marketplace token for your Amazon Web
Services account to activate your Oracle Database@Amazon Web Services
subscription.

Type annotations and code completion for `#!python session.create_client("odb").accept_marketplace_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/accept_marketplace_registration.html)

```python
# accept_marketplace_registration method definition

await def accept_marketplace_registration(
    self,
    *,
    marketplaceRegistrationToken: str,
) -> dict[str, Any]:
    ...
```

```python
# accept_marketplace_registration method usage example with argument unpacking

kwargs: AcceptMarketplaceRegistrationInputTypeDef = {  # (1)
    "marketplaceRegistrationToken": ...,
}

parent.accept_marketplace_registration(**kwargs)
```

1. See [:material-code-braces: AcceptMarketplaceRegistrationInputTypeDef](./type_defs.md#acceptmarketplaceregistrationinputtypedef)

### associate\_iam\_role\_to\_resource

Associates an Amazon Web Services Identity and Access Management (IAM) service
role with a specified resource to enable Amazon Web Services service
integration.

Type annotations and code completion for `#!python session.create_client("odb").associate_iam_role_to_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/associate_iam_role_to_resource.html)

```python
# associate_iam_role_to_resource method definition

await def associate_iam_role_to_resource(
    self,
    *,
    iamRoleArn: str,
    awsIntegration: SupportedAwsIntegrationType,  # (1)
    resourceArn: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SupportedAwsIntegrationType](./literals.md#supportedawsintegrationtype)


```python
# associate_iam_role_to_resource method usage example with argument unpacking

kwargs: AssociateIamRoleToResourceInputTypeDef = {  # (1)
    "iamRoleArn": ...,
    "awsIntegration": ...,
    "resourceArn": ...,
}

parent.associate_iam_role_to_resource(**kwargs)
```

1. See [:material-code-braces: AssociateIamRoleToResourceInputTypeDef](./type_defs.md#associateiamroletoresourceinputtypedef)

### create\_cloud\_autonomous\_vm\_cluster

Creates a new Autonomous VM cluster in the specified Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").create_cloud_autonomous_vm_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/create_cloud_autonomous_vm_cluster.html)

```python
# create_cloud_autonomous_vm_cluster method definition

await def create_cloud_autonomous_vm_cluster(
    self,
    *,
    cloudExadataInfrastructureId: str,
    odbNetworkId: str,
    displayName: str,
    autonomousDataStorageSizeInTBs: float,
    cpuCoreCountPerNode: int,
    memoryPerOracleComputeUnitInGBs: int,
    totalContainerDatabases: int,
    clientToken: str = ...,
    dbServers: Sequence[str] = ...,
    description: str = ...,
    isMtlsEnabledVmCluster: bool = ...,
    licenseModel: LicenseModelType = ...,  # (1)
    maintenanceWindow: MaintenanceWindowUnionTypeDef = ...,  # (2)
    scanListenerPortNonTls: int = ...,
    scanListenerPortTls: int = ...,
    tags: Mapping[str, str] = ...,
    timeZone: str = ...,
) -> CreateCloudAutonomousVmClusterOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)
2. See [:material-code-braces: MaintenanceWindowUnionTypeDef](#maintenancewindowuniontypedef)
3. See [:material-code-braces: CreateCloudAutonomousVmClusterOutputTypeDef](./type_defs.md#createcloudautonomousvmclusteroutputtypedef)


```python
# create_cloud_autonomous_vm_cluster method usage example with argument unpacking

kwargs: CreateCloudAutonomousVmClusterInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
    "odbNetworkId": ...,
    "displayName": ...,
    "autonomousDataStorageSizeInTBs": ...,
    "cpuCoreCountPerNode": ...,
    "memoryPerOracleComputeUnitInGBs": ...,
    "totalContainerDatabases": ...,
}

parent.create_cloud_autonomous_vm_cluster(**kwargs)
```

1. See [:material-code-braces: CreateCloudAutonomousVmClusterInputTypeDef](./type_defs.md#createcloudautonomousvmclusterinputtypedef)

### create\_cloud\_exadata\_infrastructure

Creates an Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").create_cloud_exadata_infrastructure` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/create_cloud_exadata_infrastructure.html)

```python
# create_cloud_exadata_infrastructure method definition

await def create_cloud_exadata_infrastructure(
    self,
    *,
    displayName: str,
    shape: str,
    computeCount: int,
    storageCount: int,
    availabilityZone: str = ...,
    availabilityZoneId: str = ...,
    tags: Mapping[str, str] = ...,
    customerContactsToSendToOCI: Sequence[CustomerContactTypeDef] = ...,  # (1)
    maintenanceWindow: MaintenanceWindowUnionTypeDef = ...,  # (2)
    clientToken: str = ...,
    databaseServerType: str = ...,
    storageServerType: str = ...,
) -> CreateCloudExadataInfrastructureOutputTypeDef:  # (3)
    ...
```

1. See `Sequence[CustomerContactTypeDef]`
2. See [:material-code-braces: MaintenanceWindowUnionTypeDef](#maintenancewindowuniontypedef)
3. See [:material-code-braces: CreateCloudExadataInfrastructureOutputTypeDef](./type_defs.md#createcloudexadatainfrastructureoutputtypedef)


```python
# create_cloud_exadata_infrastructure method usage example with argument unpacking

kwargs: CreateCloudExadataInfrastructureInputTypeDef = {  # (1)
    "displayName": ...,
    "shape": ...,
    "computeCount": ...,
    "storageCount": ...,
}

parent.create_cloud_exadata_infrastructure(**kwargs)
```

1. See [:material-code-braces: CreateCloudExadataInfrastructureInputTypeDef](./type_defs.md#createcloudexadatainfrastructureinputtypedef)

### create\_cloud\_vm\_cluster

Creates a VM cluster on the specified Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").create_cloud_vm_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/create_cloud_vm_cluster.html)

```python
# create_cloud_vm_cluster method definition

await def create_cloud_vm_cluster(
    self,
    *,
    cloudExadataInfrastructureId: str,
    cpuCoreCount: int,
    displayName: str,
    giVersion: str,
    hostname: str,
    sshPublicKeys: Sequence[str],
    odbNetworkId: str,
    clusterName: str = ...,
    dataCollectionOptions: DataCollectionOptionsTypeDef = ...,  # (1)
    dataStorageSizeInTBs: float = ...,
    dbNodeStorageSizeInGBs: int = ...,
    dbServers: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
    isLocalBackupEnabled: bool = ...,
    isSparseDiskgroupEnabled: bool = ...,
    licenseModel: LicenseModelType = ...,  # (2)
    memorySizeInGBs: int = ...,
    systemVersion: str = ...,
    timeZone: str = ...,
    clientToken: str = ...,
    scanListenerPortTcp: int = ...,
) -> CreateCloudVmClusterOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DataCollectionOptionsTypeDef](./type_defs.md#datacollectionoptionstypedef)
2. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)
3. See [:material-code-braces: CreateCloudVmClusterOutputTypeDef](./type_defs.md#createcloudvmclusteroutputtypedef)


```python
# create_cloud_vm_cluster method usage example with argument unpacking

kwargs: CreateCloudVmClusterInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
    "cpuCoreCount": ...,
    "displayName": ...,
    "giVersion": ...,
    "hostname": ...,
    "sshPublicKeys": ...,
    "odbNetworkId": ...,
}

parent.create_cloud_vm_cluster(**kwargs)
```

1. See [:material-code-braces: CreateCloudVmClusterInputTypeDef](./type_defs.md#createcloudvmclusterinputtypedef)

### create\_odb\_network

Creates an ODB network.

Type annotations and code completion for `#!python session.create_client("odb").create_odb_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/create_odb_network.html)

```python
# create_odb_network method definition

await def create_odb_network(
    self,
    *,
    displayName: str,
    clientSubnetCidr: str,
    availabilityZone: str = ...,
    availabilityZoneId: str = ...,
    backupSubnetCidr: str = ...,
    customDomainName: str = ...,
    defaultDnsPrefix: str = ...,
    clientToken: str = ...,
    s3Access: AccessType = ...,  # (1)
    zeroEtlAccess: AccessType = ...,  # (1)
    stsAccess: AccessType = ...,  # (1)
    kmsAccess: AccessType = ...,  # (1)
    s3PolicyDocument: str = ...,
    stsPolicyDocument: str = ...,
    kmsPolicyDocument: str = ...,
    crossRegionS3RestoreSourcesToEnable: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
) -> CreateOdbNetworkOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: AccessType](./literals.md#accesstype)
2. See [:material-code-brackets: AccessType](./literals.md#accesstype)
3. See [:material-code-brackets: AccessType](./literals.md#accesstype)
4. See [:material-code-brackets: AccessType](./literals.md#accesstype)
5. See [:material-code-braces: CreateOdbNetworkOutputTypeDef](./type_defs.md#createodbnetworkoutputtypedef)


```python
# create_odb_network method usage example with argument unpacking

kwargs: CreateOdbNetworkInputTypeDef = {  # (1)
    "displayName": ...,
    "clientSubnetCidr": ...,
}

parent.create_odb_network(**kwargs)
```

1. See [:material-code-braces: CreateOdbNetworkInputTypeDef](./type_defs.md#createodbnetworkinputtypedef)

### create\_odb\_peering\_connection

Creates a peering connection between an ODB network and a VPC.

Type annotations and code completion for `#!python session.create_client("odb").create_odb_peering_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/create_odb_peering_connection.html)

```python
# create_odb_peering_connection method definition

await def create_odb_peering_connection(
    self,
    *,
    odbNetworkId: str,
    peerNetworkId: str,
    displayName: str = ...,
    peerNetworkCidrsToBeAdded: Sequence[str] = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateOdbPeeringConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateOdbPeeringConnectionOutputTypeDef](./type_defs.md#createodbpeeringconnectionoutputtypedef)


```python
# create_odb_peering_connection method usage example with argument unpacking

kwargs: CreateOdbPeeringConnectionInputTypeDef = {  # (1)
    "odbNetworkId": ...,
    "peerNetworkId": ...,
}

parent.create_odb_peering_connection(**kwargs)
```

1. See [:material-code-braces: CreateOdbPeeringConnectionInputTypeDef](./type_defs.md#createodbpeeringconnectioninputtypedef)

### delete\_cloud\_autonomous\_vm\_cluster

Deletes an Autonomous VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").delete_cloud_autonomous_vm_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/delete_cloud_autonomous_vm_cluster.html)

```python
# delete_cloud_autonomous_vm_cluster method definition

await def delete_cloud_autonomous_vm_cluster(
    self,
    *,
    cloudAutonomousVmClusterId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_cloud_autonomous_vm_cluster method usage example with argument unpacking

kwargs: DeleteCloudAutonomousVmClusterInputTypeDef = {  # (1)
    "cloudAutonomousVmClusterId": ...,
}

parent.delete_cloud_autonomous_vm_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteCloudAutonomousVmClusterInputTypeDef](./type_defs.md#deletecloudautonomousvmclusterinputtypedef)

### delete\_cloud\_exadata\_infrastructure

Deletes the specified Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").delete_cloud_exadata_infrastructure` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/delete_cloud_exadata_infrastructure.html)

```python
# delete_cloud_exadata_infrastructure method definition

await def delete_cloud_exadata_infrastructure(
    self,
    *,
    cloudExadataInfrastructureId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_cloud_exadata_infrastructure method usage example with argument unpacking

kwargs: DeleteCloudExadataInfrastructureInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.delete_cloud_exadata_infrastructure(**kwargs)
```

1. See [:material-code-braces: DeleteCloudExadataInfrastructureInputTypeDef](./type_defs.md#deletecloudexadatainfrastructureinputtypedef)

### delete\_cloud\_vm\_cluster

Deletes the specified VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").delete_cloud_vm_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/delete_cloud_vm_cluster.html)

```python
# delete_cloud_vm_cluster method definition

await def delete_cloud_vm_cluster(
    self,
    *,
    cloudVmClusterId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_cloud_vm_cluster method usage example with argument unpacking

kwargs: DeleteCloudVmClusterInputTypeDef = {  # (1)
    "cloudVmClusterId": ...,
}

parent.delete_cloud_vm_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteCloudVmClusterInputTypeDef](./type_defs.md#deletecloudvmclusterinputtypedef)

### delete\_odb\_network

Deletes the specified ODB network.

Type annotations and code completion for `#!python session.create_client("odb").delete_odb_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/delete_odb_network.html)

```python
# delete_odb_network method definition

await def delete_odb_network(
    self,
    *,
    odbNetworkId: str,
    deleteAssociatedResources: bool,
) -> dict[str, Any]:
    ...
```

```python
# delete_odb_network method usage example with argument unpacking

kwargs: DeleteOdbNetworkInputTypeDef = {  # (1)
    "odbNetworkId": ...,
    "deleteAssociatedResources": ...,
}

parent.delete_odb_network(**kwargs)
```

1. See [:material-code-braces: DeleteOdbNetworkInputTypeDef](./type_defs.md#deleteodbnetworkinputtypedef)

### delete\_odb\_peering\_connection

Deletes an ODB peering connection.

Type annotations and code completion for `#!python session.create_client("odb").delete_odb_peering_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/delete_odb_peering_connection.html)

```python
# delete_odb_peering_connection method definition

await def delete_odb_peering_connection(
    self,
    *,
    odbPeeringConnectionId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_odb_peering_connection method usage example with argument unpacking

kwargs: DeleteOdbPeeringConnectionInputTypeDef = {  # (1)
    "odbPeeringConnectionId": ...,
}

parent.delete_odb_peering_connection(**kwargs)
```

1. See [:material-code-braces: DeleteOdbPeeringConnectionInputTypeDef](./type_defs.md#deleteodbpeeringconnectioninputtypedef)

### disassociate\_iam\_role\_from\_resource

Disassociates an Amazon Web Services Identity and Access Management (IAM)
service role from a specified resource to disable Amazon Web Services service
integration.

Type annotations and code completion for `#!python session.create_client("odb").disassociate_iam_role_from_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/disassociate_iam_role_from_resource.html)

```python
# disassociate_iam_role_from_resource method definition

await def disassociate_iam_role_from_resource(
    self,
    *,
    iamRoleArn: str,
    awsIntegration: SupportedAwsIntegrationType,  # (1)
    resourceArn: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SupportedAwsIntegrationType](./literals.md#supportedawsintegrationtype)


```python
# disassociate_iam_role_from_resource method usage example with argument unpacking

kwargs: DisassociateIamRoleFromResourceInputTypeDef = {  # (1)
    "iamRoleArn": ...,
    "awsIntegration": ...,
    "resourceArn": ...,
}

parent.disassociate_iam_role_from_resource(**kwargs)
```

1. See [:material-code-braces: DisassociateIamRoleFromResourceInputTypeDef](./type_defs.md#disassociateiamrolefromresourceinputtypedef)

### get\_cloud\_autonomous\_vm\_cluster

Gets information about a specific Autonomous VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").get_cloud_autonomous_vm_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_cloud_autonomous_vm_cluster.html)

```python
# get_cloud_autonomous_vm_cluster method definition

await def get_cloud_autonomous_vm_cluster(
    self,
    *,
    cloudAutonomousVmClusterId: str,
) -> GetCloudAutonomousVmClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudAutonomousVmClusterOutputTypeDef](./type_defs.md#getcloudautonomousvmclusteroutputtypedef)


```python
# get_cloud_autonomous_vm_cluster method usage example with argument unpacking

kwargs: GetCloudAutonomousVmClusterInputTypeDef = {  # (1)
    "cloudAutonomousVmClusterId": ...,
}

parent.get_cloud_autonomous_vm_cluster(**kwargs)
```

1. See [:material-code-braces: GetCloudAutonomousVmClusterInputTypeDef](./type_defs.md#getcloudautonomousvmclusterinputtypedef)

### get\_cloud\_exadata\_infrastructure

Returns information about the specified Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").get_cloud_exadata_infrastructure` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_cloud_exadata_infrastructure.html)

```python
# get_cloud_exadata_infrastructure method definition

await def get_cloud_exadata_infrastructure(
    self,
    *,
    cloudExadataInfrastructureId: str,
) -> GetCloudExadataInfrastructureOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudExadataInfrastructureOutputTypeDef](./type_defs.md#getcloudexadatainfrastructureoutputtypedef)


```python
# get_cloud_exadata_infrastructure method usage example with argument unpacking

kwargs: GetCloudExadataInfrastructureInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.get_cloud_exadata_infrastructure(**kwargs)
```

1. See [:material-code-braces: GetCloudExadataInfrastructureInputTypeDef](./type_defs.md#getcloudexadatainfrastructureinputtypedef)

### get\_cloud\_exadata\_infrastructure\_unallocated\_resources

Retrieves information about unallocated resources in a specified Cloud Exadata
Infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").get_cloud_exadata_infrastructure_unallocated_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_cloud_exadata_infrastructure_unallocated_resources.html)

```python
# get_cloud_exadata_infrastructure_unallocated_resources method definition

await def get_cloud_exadata_infrastructure_unallocated_resources(
    self,
    *,
    cloudExadataInfrastructureId: str,
    dbServers: Sequence[str] = ...,
) -> GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef](./type_defs.md#getcloudexadatainfrastructureunallocatedresourcesoutputtypedef)


```python
# get_cloud_exadata_infrastructure_unallocated_resources method usage example with argument unpacking

kwargs: GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.get_cloud_exadata_infrastructure_unallocated_resources(**kwargs)
```

1. See [:material-code-braces: GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef](./type_defs.md#getcloudexadatainfrastructureunallocatedresourcesinputtypedef)

### get\_cloud\_vm\_cluster

Returns information about the specified VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").get_cloud_vm_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_cloud_vm_cluster.html)

```python
# get_cloud_vm_cluster method definition

await def get_cloud_vm_cluster(
    self,
    *,
    cloudVmClusterId: str,
) -> GetCloudVmClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudVmClusterOutputTypeDef](./type_defs.md#getcloudvmclusteroutputtypedef)


```python
# get_cloud_vm_cluster method usage example with argument unpacking

kwargs: GetCloudVmClusterInputTypeDef = {  # (1)
    "cloudVmClusterId": ...,
}

parent.get_cloud_vm_cluster(**kwargs)
```

1. See [:material-code-braces: GetCloudVmClusterInputTypeDef](./type_defs.md#getcloudvmclusterinputtypedef)

### get\_db\_node

Returns information about the specified DB node.

Type annotations and code completion for `#!python session.create_client("odb").get_db_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_db_node.html)

```python
# get_db_node method definition

await def get_db_node(
    self,
    *,
    cloudVmClusterId: str,
    dbNodeId: str,
) -> GetDbNodeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDbNodeOutputTypeDef](./type_defs.md#getdbnodeoutputtypedef)


```python
# get_db_node method usage example with argument unpacking

kwargs: GetDbNodeInputTypeDef = {  # (1)
    "cloudVmClusterId": ...,
    "dbNodeId": ...,
}

parent.get_db_node(**kwargs)
```

1. See [:material-code-braces: GetDbNodeInputTypeDef](./type_defs.md#getdbnodeinputtypedef)

### get\_db\_server

Returns information about the specified database server.

Type annotations and code completion for `#!python session.create_client("odb").get_db_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_db_server.html)

```python
# get_db_server method definition

await def get_db_server(
    self,
    *,
    cloudExadataInfrastructureId: str,
    dbServerId: str,
) -> GetDbServerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDbServerOutputTypeDef](./type_defs.md#getdbserveroutputtypedef)


```python
# get_db_server method usage example with argument unpacking

kwargs: GetDbServerInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
    "dbServerId": ...,
}

parent.get_db_server(**kwargs)
```

1. See [:material-code-braces: GetDbServerInputTypeDef](./type_defs.md#getdbserverinputtypedef)

### get\_oci\_onboarding\_status

Returns the tenancy activation link and onboarding status for your Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("odb").get_oci_onboarding_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_oci_onboarding_status.html)

```python
# get_oci_onboarding_status method definition

await def get_oci_onboarding_status(
    self,
) -> GetOciOnboardingStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOciOnboardingStatusOutputTypeDef](./type_defs.md#getocionboardingstatusoutputtypedef)



### get\_odb\_network

Returns information about the specified ODB network.

Type annotations and code completion for `#!python session.create_client("odb").get_odb_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_odb_network.html)

```python
# get_odb_network method definition

await def get_odb_network(
    self,
    *,
    odbNetworkId: str,
) -> GetOdbNetworkOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOdbNetworkOutputTypeDef](./type_defs.md#getodbnetworkoutputtypedef)


```python
# get_odb_network method usage example with argument unpacking

kwargs: GetOdbNetworkInputTypeDef = {  # (1)
    "odbNetworkId": ...,
}

parent.get_odb_network(**kwargs)
```

1. See [:material-code-braces: GetOdbNetworkInputTypeDef](./type_defs.md#getodbnetworkinputtypedef)

### get\_odb\_peering\_connection

Retrieves information about an ODB peering connection.

Type annotations and code completion for `#!python session.create_client("odb").get_odb_peering_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/get_odb_peering_connection.html)

```python
# get_odb_peering_connection method definition

await def get_odb_peering_connection(
    self,
    *,
    odbPeeringConnectionId: str,
) -> GetOdbPeeringConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOdbPeeringConnectionOutputTypeDef](./type_defs.md#getodbpeeringconnectionoutputtypedef)


```python
# get_odb_peering_connection method usage example with argument unpacking

kwargs: GetOdbPeeringConnectionInputTypeDef = {  # (1)
    "odbPeeringConnectionId": ...,
}

parent.get_odb_peering_connection(**kwargs)
```

1. See [:material-code-braces: GetOdbPeeringConnectionInputTypeDef](./type_defs.md#getodbpeeringconnectioninputtypedef)

### initialize\_service

Initializes the ODB service for the first time in an account.

Type annotations and code completion for `#!python session.create_client("odb").initialize_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/initialize_service.html)

```python
# initialize_service method definition

await def initialize_service(
    self,
    *,
    ociIdentityDomain: bool = ...,
) -> dict[str, Any]:
    ...
```

```python
# initialize_service method usage example with argument unpacking

kwargs: InitializeServiceInputTypeDef = {  # (1)
    "ociIdentityDomain": ...,
}

parent.initialize_service(**kwargs)
```

1. See [:material-code-braces: InitializeServiceInputTypeDef](./type_defs.md#initializeserviceinputtypedef)

### list\_autonomous\_virtual\_machines

Lists all Autonomous VMs in an Autonomous VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").list_autonomous_virtual_machines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_autonomous_virtual_machines.html)

```python
# list_autonomous_virtual_machines method definition

await def list_autonomous_virtual_machines(
    self,
    *,
    cloudAutonomousVmClusterId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAutonomousVirtualMachinesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAutonomousVirtualMachinesOutputTypeDef](./type_defs.md#listautonomousvirtualmachinesoutputtypedef)


```python
# list_autonomous_virtual_machines method usage example with argument unpacking

kwargs: ListAutonomousVirtualMachinesInputTypeDef = {  # (1)
    "cloudAutonomousVmClusterId": ...,
}

parent.list_autonomous_virtual_machines(**kwargs)
```

1. See [:material-code-braces: ListAutonomousVirtualMachinesInputTypeDef](./type_defs.md#listautonomousvirtualmachinesinputtypedef)

### list\_cloud\_autonomous\_vm\_clusters

Lists all Autonomous VM clusters in a specified Cloud Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").list_cloud_autonomous_vm_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_cloud_autonomous_vm_clusters.html)

```python
# list_cloud_autonomous_vm_clusters method definition

await def list_cloud_autonomous_vm_clusters(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    cloudExadataInfrastructureId: str = ...,
) -> ListCloudAutonomousVmClustersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCloudAutonomousVmClustersOutputTypeDef](./type_defs.md#listcloudautonomousvmclustersoutputtypedef)


```python
# list_cloud_autonomous_vm_clusters method usage example with argument unpacking

kwargs: ListCloudAutonomousVmClustersInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_cloud_autonomous_vm_clusters(**kwargs)
```

1. See [:material-code-braces: ListCloudAutonomousVmClustersInputTypeDef](./type_defs.md#listcloudautonomousvmclustersinputtypedef)

### list\_cloud\_exadata\_infrastructures

Returns information about the Exadata infrastructures owned by your Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("odb").list_cloud_exadata_infrastructures` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_cloud_exadata_infrastructures.html)

```python
# list_cloud_exadata_infrastructures method definition

await def list_cloud_exadata_infrastructures(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListCloudExadataInfrastructuresOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCloudExadataInfrastructuresOutputTypeDef](./type_defs.md#listcloudexadatainfrastructuresoutputtypedef)


```python
# list_cloud_exadata_infrastructures method usage example with argument unpacking

kwargs: ListCloudExadataInfrastructuresInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_cloud_exadata_infrastructures(**kwargs)
```

1. See [:material-code-braces: ListCloudExadataInfrastructuresInputTypeDef](./type_defs.md#listcloudexadatainfrastructuresinputtypedef)

### list\_cloud\_vm\_clusters

Returns information about the VM clusters owned by your Amazon Web Services
account or only the ones on the specified Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").list_cloud_vm_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_cloud_vm_clusters.html)

```python
# list_cloud_vm_clusters method definition

await def list_cloud_vm_clusters(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    cloudExadataInfrastructureId: str = ...,
) -> ListCloudVmClustersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCloudVmClustersOutputTypeDef](./type_defs.md#listcloudvmclustersoutputtypedef)


```python
# list_cloud_vm_clusters method usage example with argument unpacking

kwargs: ListCloudVmClustersInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_cloud_vm_clusters(**kwargs)
```

1. See [:material-code-braces: ListCloudVmClustersInputTypeDef](./type_defs.md#listcloudvmclustersinputtypedef)

### list\_db\_nodes

Returns information about the DB nodes for the specified VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").list_db_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_db_nodes.html)

```python
# list_db_nodes method definition

await def list_db_nodes(
    self,
    *,
    cloudVmClusterId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDbNodesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDbNodesOutputTypeDef](./type_defs.md#listdbnodesoutputtypedef)


```python
# list_db_nodes method usage example with argument unpacking

kwargs: ListDbNodesInputTypeDef = {  # (1)
    "cloudVmClusterId": ...,
}

parent.list_db_nodes(**kwargs)
```

1. See [:material-code-braces: ListDbNodesInputTypeDef](./type_defs.md#listdbnodesinputtypedef)

### list\_db\_servers

Returns information about the database servers that belong to the specified
Exadata infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").list_db_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_db_servers.html)

```python
# list_db_servers method definition

await def list_db_servers(
    self,
    *,
    cloudExadataInfrastructureId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDbServersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDbServersOutputTypeDef](./type_defs.md#listdbserversoutputtypedef)


```python
# list_db_servers method usage example with argument unpacking

kwargs: ListDbServersInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.list_db_servers(**kwargs)
```

1. See [:material-code-braces: ListDbServersInputTypeDef](./type_defs.md#listdbserversinputtypedef)

### list\_db\_system\_shapes

Returns information about the shapes that are available for an Exadata
infrastructure.

Type annotations and code completion for `#!python session.create_client("odb").list_db_system_shapes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_db_system_shapes.html)

```python
# list_db_system_shapes method definition

await def list_db_system_shapes(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    availabilityZone: str = ...,
    availabilityZoneId: str = ...,
) -> ListDbSystemShapesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDbSystemShapesOutputTypeDef](./type_defs.md#listdbsystemshapesoutputtypedef)


```python
# list_db_system_shapes method usage example with argument unpacking

kwargs: ListDbSystemShapesInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_db_system_shapes(**kwargs)
```

1. See [:material-code-braces: ListDbSystemShapesInputTypeDef](./type_defs.md#listdbsystemshapesinputtypedef)

### list\_gi\_versions

Returns information about Oracle Grid Infrastructure (GI) software versions
that are available for a VM cluster for the specified shape.

Type annotations and code completion for `#!python session.create_client("odb").list_gi_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_gi_versions.html)

```python
# list_gi_versions method definition

await def list_gi_versions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    shape: str = ...,
) -> ListGiVersionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGiVersionsOutputTypeDef](./type_defs.md#listgiversionsoutputtypedef)


```python
# list_gi_versions method usage example with argument unpacking

kwargs: ListGiVersionsInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_gi_versions(**kwargs)
```

1. See [:material-code-braces: ListGiVersionsInputTypeDef](./type_defs.md#listgiversionsinputtypedef)

### list\_odb\_networks

Returns information about the ODB networks owned by your Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("odb").list_odb_networks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_odb_networks.html)

```python
# list_odb_networks method definition

await def list_odb_networks(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListOdbNetworksOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOdbNetworksOutputTypeDef](./type_defs.md#listodbnetworksoutputtypedef)


```python
# list_odb_networks method usage example with argument unpacking

kwargs: ListOdbNetworksInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_odb_networks(**kwargs)
```

1. See [:material-code-braces: ListOdbNetworksInputTypeDef](./type_defs.md#listodbnetworksinputtypedef)

### list\_odb\_peering\_connections

Lists all ODB peering connections or those associated with a specific ODB
network.

Type annotations and code completion for `#!python session.create_client("odb").list_odb_peering_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_odb_peering_connections.html)

```python
# list_odb_peering_connections method definition

await def list_odb_peering_connections(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    odbNetworkId: str = ...,
) -> ListOdbPeeringConnectionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOdbPeeringConnectionsOutputTypeDef](./type_defs.md#listodbpeeringconnectionsoutputtypedef)


```python
# list_odb_peering_connections method usage example with argument unpacking

kwargs: ListOdbPeeringConnectionsInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_odb_peering_connections(**kwargs)
```

1. See [:material-code-braces: ListOdbPeeringConnectionsInputTypeDef](./type_defs.md#listodbpeeringconnectionsinputtypedef)

### list\_system\_versions

Returns information about the system versions that are available for a VM
cluster for the specified <code>giVersion</code> and <code>shape</code>.

Type annotations and code completion for `#!python session.create_client("odb").list_system_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_system_versions.html)

```python
# list_system_versions method definition

await def list_system_versions(
    self,
    *,
    giVersion: str,
    shape: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSystemVersionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSystemVersionsOutputTypeDef](./type_defs.md#listsystemversionsoutputtypedef)


```python
# list_system_versions method usage example with argument unpacking

kwargs: ListSystemVersionsInputTypeDef = {  # (1)
    "giVersion": ...,
    "shape": ...,
}

parent.list_system_versions(**kwargs)
```

1. See [:material-code-braces: ListSystemVersionsInputTypeDef](./type_defs.md#listsystemversionsinputtypedef)

### list\_tags\_for\_resource

Returns information about the tags applied to this resource.

Type annotations and code completion for `#!python session.create_client("odb").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### reboot\_db\_node

Reboots the specified DB node in a VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").reboot_db_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/reboot_db_node.html)

```python
# reboot_db_node method definition

await def reboot_db_node(
    self,
    *,
    cloudVmClusterId: str,
    dbNodeId: str,
) -> RebootDbNodeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RebootDbNodeOutputTypeDef](./type_defs.md#rebootdbnodeoutputtypedef)


```python
# reboot_db_node method usage example with argument unpacking

kwargs: RebootDbNodeInputTypeDef = {  # (1)
    "cloudVmClusterId": ...,
    "dbNodeId": ...,
}

parent.reboot_db_node(**kwargs)
```

1. See [:material-code-braces: RebootDbNodeInputTypeDef](./type_defs.md#rebootdbnodeinputtypedef)

### start\_db\_node

Starts the specified DB node in a VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").start_db_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/start_db_node.html)

```python
# start_db_node method definition

await def start_db_node(
    self,
    *,
    cloudVmClusterId: str,
    dbNodeId: str,
) -> StartDbNodeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDbNodeOutputTypeDef](./type_defs.md#startdbnodeoutputtypedef)


```python
# start_db_node method usage example with argument unpacking

kwargs: StartDbNodeInputTypeDef = {  # (1)
    "cloudVmClusterId": ...,
    "dbNodeId": ...,
}

parent.start_db_node(**kwargs)
```

1. See [:material-code-braces: StartDbNodeInputTypeDef](./type_defs.md#startdbnodeinputtypedef)

### stop\_db\_node

Stops the specified DB node in a VM cluster.

Type annotations and code completion for `#!python session.create_client("odb").stop_db_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/stop_db_node.html)

```python
# stop_db_node method definition

await def stop_db_node(
    self,
    *,
    cloudVmClusterId: str,
    dbNodeId: str,
) -> StopDbNodeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopDbNodeOutputTypeDef](./type_defs.md#stopdbnodeoutputtypedef)


```python
# stop_db_node method usage example with argument unpacking

kwargs: StopDbNodeInputTypeDef = {  # (1)
    "cloudVmClusterId": ...,
    "dbNodeId": ...,
}

parent.stop_db_node(**kwargs)
```

1. See [:material-code-braces: StopDbNodeInputTypeDef](./type_defs.md#stopdbnodeinputtypedef)

### tag\_resource

Applies tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("odb").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```

```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("odb").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_cloud\_exadata\_infrastructure

Updates the properties of an Exadata infrastructure resource.

Type annotations and code completion for `#!python session.create_client("odb").update_cloud_exadata_infrastructure` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/update_cloud_exadata_infrastructure.html)

```python
# update_cloud_exadata_infrastructure method definition

await def update_cloud_exadata_infrastructure(
    self,
    *,
    cloudExadataInfrastructureId: str,
    maintenanceWindow: MaintenanceWindowUnionTypeDef = ...,  # (1)
) -> UpdateCloudExadataInfrastructureOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MaintenanceWindowUnionTypeDef](#maintenancewindowuniontypedef)
2. See [:material-code-braces: UpdateCloudExadataInfrastructureOutputTypeDef](./type_defs.md#updatecloudexadatainfrastructureoutputtypedef)


```python
# update_cloud_exadata_infrastructure method usage example with argument unpacking

kwargs: UpdateCloudExadataInfrastructureInputTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.update_cloud_exadata_infrastructure(**kwargs)
```

1. See [:material-code-braces: UpdateCloudExadataInfrastructureInputTypeDef](./type_defs.md#updatecloudexadatainfrastructureinputtypedef)

### update\_odb\_network

Updates properties of a specified ODB network.

Type annotations and code completion for `#!python session.create_client("odb").update_odb_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/update_odb_network.html)

```python
# update_odb_network method definition

await def update_odb_network(
    self,
    *,
    odbNetworkId: str,
    displayName: str = ...,
    peeredCidrsToBeAdded: Sequence[str] = ...,
    peeredCidrsToBeRemoved: Sequence[str] = ...,
    s3Access: AccessType = ...,  # (1)
    zeroEtlAccess: AccessType = ...,  # (1)
    stsAccess: AccessType = ...,  # (1)
    kmsAccess: AccessType = ...,  # (1)
    s3PolicyDocument: str = ...,
    stsPolicyDocument: str = ...,
    kmsPolicyDocument: str = ...,
    crossRegionS3RestoreSourcesToEnable: Sequence[str] = ...,
    crossRegionS3RestoreSourcesToDisable: Sequence[str] = ...,
) -> UpdateOdbNetworkOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: AccessType](./literals.md#accesstype)
2. See [:material-code-brackets: AccessType](./literals.md#accesstype)
3. See [:material-code-brackets: AccessType](./literals.md#accesstype)
4. See [:material-code-brackets: AccessType](./literals.md#accesstype)
5. See [:material-code-braces: UpdateOdbNetworkOutputTypeDef](./type_defs.md#updateodbnetworkoutputtypedef)


```python
# update_odb_network method usage example with argument unpacking

kwargs: UpdateOdbNetworkInputTypeDef = {  # (1)
    "odbNetworkId": ...,
}

parent.update_odb_network(**kwargs)
```

1. See [:material-code-braces: UpdateOdbNetworkInputTypeDef](./type_defs.md#updateodbnetworkinputtypedef)

### update\_odb\_peering\_connection

Modifies the settings of an Oracle Database@Amazon Web Services peering
connection.

Type annotations and code completion for `#!python session.create_client("odb").update_odb_peering_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/client/update_odb_peering_connection.html)

```python
# update_odb_peering_connection method definition

await def update_odb_peering_connection(
    self,
    *,
    odbPeeringConnectionId: str,
    displayName: str = ...,
    peerNetworkCidrsToBeAdded: Sequence[str] = ...,
    peerNetworkCidrsToBeRemoved: Sequence[str] = ...,
) -> UpdateOdbPeeringConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateOdbPeeringConnectionOutputTypeDef](./type_defs.md#updateodbpeeringconnectionoutputtypedef)


```python
# update_odb_peering_connection method usage example with argument unpacking

kwargs: UpdateOdbPeeringConnectionInputTypeDef = {  # (1)
    "odbPeeringConnectionId": ...,
}

parent.update_odb_peering_connection(**kwargs)
```

1. See [:material-code-braces: UpdateOdbPeeringConnectionInputTypeDef](./type_defs.md#updateodbpeeringconnectioninputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("odb").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#Odb.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("odb").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#Odb.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator` method with overloads.

- `client.get_paginator("list_autonomous_virtual_machines")` -> [ListAutonomousVirtualMachinesPaginator](./paginators.md#listautonomousvirtualmachinespaginator)
- `client.get_paginator("list_cloud_autonomous_vm_clusters")` -> [ListCloudAutonomousVmClustersPaginator](./paginators.md#listcloudautonomousvmclusterspaginator)
- `client.get_paginator("list_cloud_exadata_infrastructures")` -> [ListCloudExadataInfrastructuresPaginator](./paginators.md#listcloudexadatainfrastructurespaginator)
- `client.get_paginator("list_cloud_vm_clusters")` -> [ListCloudVmClustersPaginator](./paginators.md#listcloudvmclusterspaginator)
- `client.get_paginator("list_db_nodes")` -> [ListDbNodesPaginator](./paginators.md#listdbnodespaginator)
- `client.get_paginator("list_db_servers")` -> [ListDbServersPaginator](./paginators.md#listdbserverspaginator)
- `client.get_paginator("list_db_system_shapes")` -> [ListDbSystemShapesPaginator](./paginators.md#listdbsystemshapespaginator)
- `client.get_paginator("list_gi_versions")` -> [ListGiVersionsPaginator](./paginators.md#listgiversionspaginator)
- `client.get_paginator("list_odb_networks")` -> [ListOdbNetworksPaginator](./paginators.md#listodbnetworkspaginator)
- `client.get_paginator("list_odb_peering_connections")` -> [ListOdbPeeringConnectionsPaginator](./paginators.md#listodbpeeringconnectionspaginator)
- `client.get_paginator("list_system_versions")` -> [ListSystemVersionsPaginator](./paginators.md#listsystemversionspaginator)



