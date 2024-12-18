# OpsWorksClient

> [Index](../README.md) > [OpsWorks](./README.md) > OpsWorksClient

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## OpsWorksClient

Type annotations and code completion for `#!python session.create_client("opsworks")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client)

```python
# OpsWorksClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_opsworks.client import OpsWorksClient

session = get_session()
async with session.create_client("opsworks") as client:
    client: OpsWorksClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("opsworks").exceptions` structure.

```python
# OpsWorksClient.exceptions usage example

async with session.create_client("opsworks") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# OpsWorksClient usage type checking example

from types_aiobotocore_opsworks.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("opsworks").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("opsworks").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("opsworks").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### assign\_instance

Assign a registered instance to a layer.

Type annotations and code completion for `#!python session.create_client("opsworks").assign_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/assign_instance.html)

```python
# assign_instance method definition

await def assign_instance(
    self,
    *,
    InstanceId: str,
    LayerIds: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# assign_instance method usage example with argument unpacking

kwargs: AssignInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "LayerIds": ...,
}

parent.assign_instance(**kwargs)
```

1. See [:material-code-braces: AssignInstanceRequestRequestTypeDef](./type_defs.md#assigninstancerequestrequesttypedef) 

### assign\_volume

Assigns one of the stack's registered Amazon EBS volumes to a specified
instance.

Type annotations and code completion for `#!python session.create_client("opsworks").assign_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/assign_volume.html)

```python
# assign_volume method definition

await def assign_volume(
    self,
    *,
    VolumeId: str,
    InstanceId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# assign_volume method usage example with argument unpacking

kwargs: AssignVolumeRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
}

parent.assign_volume(**kwargs)
```

1. See [:material-code-braces: AssignVolumeRequestRequestTypeDef](./type_defs.md#assignvolumerequestrequesttypedef) 

### associate\_elastic\_ip

Associates one of the stack's registered Elastic IP addresses with a specified
instance.

Type annotations and code completion for `#!python session.create_client("opsworks").associate_elastic_ip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/associate_elastic_ip.html)

```python
# associate_elastic_ip method definition

await def associate_elastic_ip(
    self,
    *,
    ElasticIp: str,
    InstanceId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_elastic_ip method usage example with argument unpacking

kwargs: AssociateElasticIpRequestRequestTypeDef = {  # (1)
    "ElasticIp": ...,
}

parent.associate_elastic_ip(**kwargs)
```

1. See [:material-code-braces: AssociateElasticIpRequestRequestTypeDef](./type_defs.md#associateelasticiprequestrequesttypedef) 

### attach\_elastic\_load\_balancer

Attaches an Elastic Load Balancing load balancer to a specified layer.

Type annotations and code completion for `#!python session.create_client("opsworks").attach_elastic_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/attach_elastic_load_balancer.html)

```python
# attach_elastic_load_balancer method definition

await def attach_elastic_load_balancer(
    self,
    *,
    ElasticLoadBalancerName: str,
    LayerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# attach_elastic_load_balancer method usage example with argument unpacking

kwargs: AttachElasticLoadBalancerRequestRequestTypeDef = {  # (1)
    "ElasticLoadBalancerName": ...,
    "LayerId": ...,
}

parent.attach_elastic_load_balancer(**kwargs)
```

1. See [:material-code-braces: AttachElasticLoadBalancerRequestRequestTypeDef](./type_defs.md#attachelasticloadbalancerrequestrequesttypedef) 

### clone\_stack

Creates a clone of a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").clone_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/clone_stack.html)

```python
# clone_stack method definition

await def clone_stack(
    self,
    *,
    SourceStackId: str,
    ServiceRoleArn: str,
    Name: str = ...,
    Region: str = ...,
    VpcId: str = ...,
    Attributes: Mapping[StackAttributesKeysType, str] = ...,  # (1)
    DefaultInstanceProfileArn: str = ...,
    DefaultOs: str = ...,
    HostnameTheme: str = ...,
    DefaultAvailabilityZone: str = ...,
    DefaultSubnetId: str = ...,
    CustomJson: str = ...,
    ConfigurationManager: StackConfigurationManagerTypeDef = ...,  # (2)
    ChefConfiguration: ChefConfigurationTypeDef = ...,  # (3)
    UseCustomCookbooks: bool = ...,
    UseOpsworksSecurityGroups: bool = ...,
    CustomCookbooksSource: SourceTypeDef = ...,  # (4)
    DefaultSshKeyName: str = ...,
    ClonePermissions: bool = ...,
    CloneAppIds: Sequence[str] = ...,
    DefaultRootDeviceType: RootDeviceTypeType = ...,  # (5)
    AgentVersion: str = ...,
) -> CloneStackResultTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
6. See [:material-code-braces: CloneStackResultTypeDef](./type_defs.md#clonestackresulttypedef) 


```python
# clone_stack method usage example with argument unpacking

kwargs: CloneStackRequestRequestTypeDef = {  # (1)
    "SourceStackId": ...,
    "ServiceRoleArn": ...,
}

parent.clone_stack(**kwargs)
```

1. See [:material-code-braces: CloneStackRequestRequestTypeDef](./type_defs.md#clonestackrequestrequesttypedef) 

### create\_app

Creates an app for a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").create_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/create_app.html)

```python
# create_app method definition

await def create_app(
    self,
    *,
    StackId: str,
    Name: str,
    Type: AppTypeType,  # (1)
    Shortname: str = ...,
    Description: str = ...,
    DataSources: Sequence[DataSourceTypeDef] = ...,  # (2)
    AppSource: SourceTypeDef = ...,  # (3)
    Domains: Sequence[str] = ...,
    EnableSsl: bool = ...,
    SslConfiguration: SslConfigurationTypeDef = ...,  # (4)
    Attributes: Mapping[AppAttributesKeysType, str] = ...,  # (5)
    Environment: Sequence[EnvironmentVariableTypeDef] = ...,  # (6)
) -> CreateAppResultTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
4. See [:material-code-braces: SslConfigurationTypeDef](./type_defs.md#sslconfigurationtypedef) 
5. See [:material-code-brackets: AppAttributesKeysType](./literals.md#appattributeskeystype) 
6. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
7. See [:material-code-braces: CreateAppResultTypeDef](./type_defs.md#createappresulttypedef) 


```python
# create_app method usage example with argument unpacking

kwargs: CreateAppRequestRequestTypeDef = {  # (1)
    "StackId": ...,
    "Name": ...,
    "Type": ...,
}

parent.create_app(**kwargs)
```

1. See [:material-code-braces: CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef) 

### create\_deployment

Runs deployment or stack commands.

Type annotations and code completion for `#!python session.create_client("opsworks").create_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/create_deployment.html)

```python
# create_deployment method definition

await def create_deployment(
    self,
    *,
    StackId: str,
    Command: DeploymentCommandTypeDef,  # (1)
    AppId: str = ...,
    InstanceIds: Sequence[str] = ...,
    LayerIds: Sequence[str] = ...,
    Comment: str = ...,
    CustomJson: str = ...,
) -> CreateDeploymentResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeploymentCommandTypeDef](./type_defs.md#deploymentcommandtypedef) 
2. See [:material-code-braces: CreateDeploymentResultTypeDef](./type_defs.md#createdeploymentresulttypedef) 


```python
# create_deployment method usage example with argument unpacking

kwargs: CreateDeploymentRequestRequestTypeDef = {  # (1)
    "StackId": ...,
    "Command": ...,
}

parent.create_deployment(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentRequestRequestTypeDef](./type_defs.md#createdeploymentrequestrequesttypedef) 

### create\_instance

Creates an instance in a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").create_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/create_instance.html)

```python
# create_instance method definition

await def create_instance(
    self,
    *,
    StackId: str,
    LayerIds: Sequence[str],
    InstanceType: str,
    AutoScalingType: AutoScalingTypeType = ...,  # (1)
    Hostname: str = ...,
    Os: str = ...,
    AmiId: str = ...,
    SshKeyName: str = ...,
    AvailabilityZone: str = ...,
    VirtualizationType: str = ...,
    SubnetId: str = ...,
    Architecture: ArchitectureType = ...,  # (2)
    RootDeviceType: RootDeviceTypeType = ...,  # (3)
    BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,  # (4)
    InstallUpdatesOnBoot: bool = ...,
    EbsOptimized: bool = ...,
    AgentVersion: str = ...,
    Tenancy: str = ...,
) -> CreateInstanceResultTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: AutoScalingTypeType](./literals.md#autoscalingtypetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
4. See [:material-code-braces: BlockDeviceMappingTypeDef](./type_defs.md#blockdevicemappingtypedef) 
5. See [:material-code-braces: CreateInstanceResultTypeDef](./type_defs.md#createinstanceresulttypedef) 


```python
# create_instance method usage example with argument unpacking

kwargs: CreateInstanceRequestRequestTypeDef = {  # (1)
    "StackId": ...,
    "LayerIds": ...,
    "InstanceType": ...,
}

parent.create_instance(**kwargs)
```

1. See [:material-code-braces: CreateInstanceRequestRequestTypeDef](./type_defs.md#createinstancerequestrequesttypedef) 

### create\_layer

Creates a layer.

Type annotations and code completion for `#!python session.create_client("opsworks").create_layer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/create_layer.html)

```python
# create_layer method definition

await def create_layer(
    self,
    *,
    StackId: str,
    Type: LayerTypeType,  # (1)
    Name: str,
    Shortname: str,
    Attributes: Mapping[LayerAttributesKeysType, str] = ...,  # (2)
    CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,  # (3)
    CustomInstanceProfileArn: str = ...,
    CustomJson: str = ...,
    CustomSecurityGroupIds: Sequence[str] = ...,
    Packages: Sequence[str] = ...,
    VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,  # (4)
    EnableAutoHealing: bool = ...,
    AutoAssignElasticIps: bool = ...,
    AutoAssignPublicIps: bool = ...,
    CustomRecipes: RecipesTypeDef = ...,  # (5)
    InstallUpdatesOnBoot: bool = ...,
    UseEbsOptimizedInstances: bool = ...,
    LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,  # (6)
) -> CreateLayerResultTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) 
6. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
7. See [:material-code-braces: CreateLayerResultTypeDef](./type_defs.md#createlayerresulttypedef) 


```python
# create_layer method usage example with argument unpacking

kwargs: CreateLayerRequestRequestTypeDef = {  # (1)
    "StackId": ...,
    "Type": ...,
    "Name": ...,
    "Shortname": ...,
}

parent.create_layer(**kwargs)
```

1. See [:material-code-braces: CreateLayerRequestRequestTypeDef](./type_defs.md#createlayerrequestrequesttypedef) 

### create\_stack

Creates a new stack.

Type annotations and code completion for `#!python session.create_client("opsworks").create_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/create_stack.html)

```python
# create_stack method definition

await def create_stack(
    self,
    *,
    Name: str,
    Region: str,
    ServiceRoleArn: str,
    DefaultInstanceProfileArn: str,
    VpcId: str = ...,
    Attributes: Mapping[StackAttributesKeysType, str] = ...,  # (1)
    DefaultOs: str = ...,
    HostnameTheme: str = ...,
    DefaultAvailabilityZone: str = ...,
    DefaultSubnetId: str = ...,
    CustomJson: str = ...,
    ConfigurationManager: StackConfigurationManagerTypeDef = ...,  # (2)
    ChefConfiguration: ChefConfigurationTypeDef = ...,  # (3)
    UseCustomCookbooks: bool = ...,
    UseOpsworksSecurityGroups: bool = ...,
    CustomCookbooksSource: SourceTypeDef = ...,  # (4)
    DefaultSshKeyName: str = ...,
    DefaultRootDeviceType: RootDeviceTypeType = ...,  # (5)
    AgentVersion: str = ...,
) -> CreateStackResultTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
6. See [:material-code-braces: CreateStackResultTypeDef](./type_defs.md#createstackresulttypedef) 


```python
# create_stack method usage example with argument unpacking

kwargs: CreateStackRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Region": ...,
    "ServiceRoleArn": ...,
    "DefaultInstanceProfileArn": ...,
}

parent.create_stack(**kwargs)
```

1. See [:material-code-braces: CreateStackRequestRequestTypeDef](./type_defs.md#createstackrequestrequesttypedef) 

### create\_user\_profile

Creates a new user profile.

Type annotations and code completion for `#!python session.create_client("opsworks").create_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/create_user_profile.html)

```python
# create_user_profile method definition

await def create_user_profile(
    self,
    *,
    IamUserArn: str,
    SshUsername: str = ...,
    SshPublicKey: str = ...,
    AllowSelfManagement: bool = ...,
) -> CreateUserProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateUserProfileResultTypeDef](./type_defs.md#createuserprofileresulttypedef) 


```python
# create_user_profile method usage example with argument unpacking

kwargs: CreateUserProfileRequestRequestTypeDef = {  # (1)
    "IamUserArn": ...,
}

parent.create_user_profile(**kwargs)
```

1. See [:material-code-braces: CreateUserProfileRequestRequestTypeDef](./type_defs.md#createuserprofilerequestrequesttypedef) 

### delete\_app

Deletes a specified app.

Type annotations and code completion for `#!python session.create_client("opsworks").delete_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/delete_app.html)

```python
# delete_app method definition

await def delete_app(
    self,
    *,
    AppId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_app method usage example with argument unpacking

kwargs: DeleteAppRequestRequestTypeDef = {  # (1)
    "AppId": ...,
}

parent.delete_app(**kwargs)
```

1. See [:material-code-braces: DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef) 

### delete\_instance

Deletes a specified instance, which terminates the associated Amazon EC2
instance.

Type annotations and code completion for `#!python session.create_client("opsworks").delete_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/delete_instance.html)

```python
# delete_instance method definition

await def delete_instance(
    self,
    *,
    InstanceId: str,
    DeleteElasticIp: bool = ...,
    DeleteVolumes: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_instance method usage example with argument unpacking

kwargs: DeleteInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.delete_instance(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceRequestRequestTypeDef](./type_defs.md#deleteinstancerequestrequesttypedef) 

### delete\_layer

Deletes a specified layer.

Type annotations and code completion for `#!python session.create_client("opsworks").delete_layer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/delete_layer.html)

```python
# delete_layer method definition

await def delete_layer(
    self,
    *,
    LayerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_layer method usage example with argument unpacking

kwargs: DeleteLayerRequestRequestTypeDef = {  # (1)
    "LayerId": ...,
}

parent.delete_layer(**kwargs)
```

1. See [:material-code-braces: DeleteLayerRequestRequestTypeDef](./type_defs.md#deletelayerrequestrequesttypedef) 

### delete\_stack

Deletes a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").delete_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/delete_stack.html)

```python
# delete_stack method definition

await def delete_stack(
    self,
    *,
    StackId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_stack method usage example with argument unpacking

kwargs: DeleteStackRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.delete_stack(**kwargs)
```

1. See [:material-code-braces: DeleteStackRequestRequestTypeDef](./type_defs.md#deletestackrequestrequesttypedef) 

### delete\_user\_profile

Deletes a user profile.

Type annotations and code completion for `#!python session.create_client("opsworks").delete_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/delete_user_profile.html)

```python
# delete_user_profile method definition

await def delete_user_profile(
    self,
    *,
    IamUserArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user_profile method usage example with argument unpacking

kwargs: DeleteUserProfileRequestRequestTypeDef = {  # (1)
    "IamUserArn": ...,
}

parent.delete_user_profile(**kwargs)
```

1. See [:material-code-braces: DeleteUserProfileRequestRequestTypeDef](./type_defs.md#deleteuserprofilerequestrequesttypedef) 

### deregister\_ecs\_cluster

Deregisters a specified Amazon ECS cluster from a stack.

Type annotations and code completion for `#!python session.create_client("opsworks").deregister_ecs_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/deregister_ecs_cluster.html)

```python
# deregister_ecs_cluster method definition

await def deregister_ecs_cluster(
    self,
    *,
    EcsClusterArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_ecs_cluster method usage example with argument unpacking

kwargs: DeregisterEcsClusterRequestRequestTypeDef = {  # (1)
    "EcsClusterArn": ...,
}

parent.deregister_ecs_cluster(**kwargs)
```

1. See [:material-code-braces: DeregisterEcsClusterRequestRequestTypeDef](./type_defs.md#deregisterecsclusterrequestrequesttypedef) 

### deregister\_elastic\_ip

Deregisters a specified Elastic IP address.

Type annotations and code completion for `#!python session.create_client("opsworks").deregister_elastic_ip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/deregister_elastic_ip.html)

```python
# deregister_elastic_ip method definition

await def deregister_elastic_ip(
    self,
    *,
    ElasticIp: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_elastic_ip method usage example with argument unpacking

kwargs: DeregisterElasticIpRequestRequestTypeDef = {  # (1)
    "ElasticIp": ...,
}

parent.deregister_elastic_ip(**kwargs)
```

1. See [:material-code-braces: DeregisterElasticIpRequestRequestTypeDef](./type_defs.md#deregisterelasticiprequestrequesttypedef) 

### deregister\_instance

Deregister an instance from OpsWorks Stacks.

Type annotations and code completion for `#!python session.create_client("opsworks").deregister_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/deregister_instance.html)

```python
# deregister_instance method definition

await def deregister_instance(
    self,
    *,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_instance method usage example with argument unpacking

kwargs: DeregisterInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.deregister_instance(**kwargs)
```

1. See [:material-code-braces: DeregisterInstanceRequestRequestTypeDef](./type_defs.md#deregisterinstancerequestrequesttypedef) 

### deregister\_rds\_db\_instance

Deregisters an Amazon RDS instance.

Type annotations and code completion for `#!python session.create_client("opsworks").deregister_rds_db_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/deregister_rds_db_instance.html)

```python
# deregister_rds_db_instance method definition

await def deregister_rds_db_instance(
    self,
    *,
    RdsDbInstanceArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_rds_db_instance method usage example with argument unpacking

kwargs: DeregisterRdsDbInstanceRequestRequestTypeDef = {  # (1)
    "RdsDbInstanceArn": ...,
}

parent.deregister_rds_db_instance(**kwargs)
```

1. See [:material-code-braces: DeregisterRdsDbInstanceRequestRequestTypeDef](./type_defs.md#deregisterrdsdbinstancerequestrequesttypedef) 

### deregister\_volume

Deregisters an Amazon EBS volume.

Type annotations and code completion for `#!python session.create_client("opsworks").deregister_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/deregister_volume.html)

```python
# deregister_volume method definition

await def deregister_volume(
    self,
    *,
    VolumeId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_volume method usage example with argument unpacking

kwargs: DeregisterVolumeRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
}

parent.deregister_volume(**kwargs)
```

1. See [:material-code-braces: DeregisterVolumeRequestRequestTypeDef](./type_defs.md#deregistervolumerequestrequesttypedef) 

### describe\_agent\_versions

Describes the available OpsWorks Stacks agent versions.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_agent_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_agent_versions.html)

```python
# describe_agent_versions method definition

await def describe_agent_versions(
    self,
    *,
    StackId: str = ...,
    ConfigurationManager: StackConfigurationManagerTypeDef = ...,  # (1)
) -> DescribeAgentVersionsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
2. See [:material-code-braces: DescribeAgentVersionsResultTypeDef](./type_defs.md#describeagentversionsresulttypedef) 


```python
# describe_agent_versions method usage example with argument unpacking

kwargs: DescribeAgentVersionsRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_agent_versions(**kwargs)
```

1. See [:material-code-braces: DescribeAgentVersionsRequestRequestTypeDef](./type_defs.md#describeagentversionsrequestrequesttypedef) 

### describe\_apps

Requests a description of a specified set of apps.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_apps.html)

```python
# describe_apps method definition

await def describe_apps(
    self,
    *,
    StackId: str = ...,
    AppIds: Sequence[str] = ...,
) -> DescribeAppsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppsResultTypeDef](./type_defs.md#describeappsresulttypedef) 


```python
# describe_apps method usage example with argument unpacking

kwargs: DescribeAppsRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_apps(**kwargs)
```

1. See [:material-code-braces: DescribeAppsRequestRequestTypeDef](./type_defs.md#describeappsrequestrequesttypedef) 

### describe\_commands

Describes the results of specified commands.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_commands` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_commands.html)

```python
# describe_commands method definition

await def describe_commands(
    self,
    *,
    DeploymentId: str = ...,
    InstanceId: str = ...,
    CommandIds: Sequence[str] = ...,
) -> DescribeCommandsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCommandsResultTypeDef](./type_defs.md#describecommandsresulttypedef) 


```python
# describe_commands method usage example with argument unpacking

kwargs: DescribeCommandsRequestRequestTypeDef = {  # (1)
    "DeploymentId": ...,
}

parent.describe_commands(**kwargs)
```

1. See [:material-code-braces: DescribeCommandsRequestRequestTypeDef](./type_defs.md#describecommandsrequestrequesttypedef) 

### describe\_deployments

Requests a description of a specified set of deployments.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_deployments.html)

```python
# describe_deployments method definition

await def describe_deployments(
    self,
    *,
    StackId: str = ...,
    AppId: str = ...,
    DeploymentIds: Sequence[str] = ...,
) -> DescribeDeploymentsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeploymentsResultTypeDef](./type_defs.md#describedeploymentsresulttypedef) 


```python
# describe_deployments method usage example with argument unpacking

kwargs: DescribeDeploymentsRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_deployments(**kwargs)
```

1. See [:material-code-braces: DescribeDeploymentsRequestRequestTypeDef](./type_defs.md#describedeploymentsrequestrequesttypedef) 

### describe\_ecs\_clusters

Describes Amazon ECS clusters that are registered with a stack.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_ecs_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_ecs_clusters.html)

```python
# describe_ecs_clusters method definition

await def describe_ecs_clusters(
    self,
    *,
    EcsClusterArns: Sequence[str] = ...,
    StackId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeEcsClustersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef) 


```python
# describe_ecs_clusters method usage example with argument unpacking

kwargs: DescribeEcsClustersRequestRequestTypeDef = {  # (1)
    "EcsClusterArns": ...,
}

parent.describe_ecs_clusters(**kwargs)
```

1. See [:material-code-braces: DescribeEcsClustersRequestRequestTypeDef](./type_defs.md#describeecsclustersrequestrequesttypedef) 

### describe\_elastic\_ips

Describes <a
href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-addresses-eip.html">Elastic
IP addresses</a>.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_elastic_ips` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_elastic_ips.html)

```python
# describe_elastic_ips method definition

await def describe_elastic_ips(
    self,
    *,
    InstanceId: str = ...,
    StackId: str = ...,
    Ips: Sequence[str] = ...,
) -> DescribeElasticIpsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeElasticIpsResultTypeDef](./type_defs.md#describeelasticipsresulttypedef) 


```python
# describe_elastic_ips method usage example with argument unpacking

kwargs: DescribeElasticIpsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_elastic_ips(**kwargs)
```

1. See [:material-code-braces: DescribeElasticIpsRequestRequestTypeDef](./type_defs.md#describeelasticipsrequestrequesttypedef) 

### describe\_elastic\_load\_balancers

Describes a stack's Elastic Load Balancing instances.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_elastic_load_balancers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_elastic_load_balancers.html)

```python
# describe_elastic_load_balancers method definition

await def describe_elastic_load_balancers(
    self,
    *,
    StackId: str = ...,
    LayerIds: Sequence[str] = ...,
) -> DescribeElasticLoadBalancersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeElasticLoadBalancersResultTypeDef](./type_defs.md#describeelasticloadbalancersresulttypedef) 


```python
# describe_elastic_load_balancers method usage example with argument unpacking

kwargs: DescribeElasticLoadBalancersRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_elastic_load_balancers(**kwargs)
```

1. See [:material-code-braces: DescribeElasticLoadBalancersRequestRequestTypeDef](./type_defs.md#describeelasticloadbalancersrequestrequesttypedef) 

### describe\_instances

Requests a description of a set of instances.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_instances.html)

```python
# describe_instances method definition

await def describe_instances(
    self,
    *,
    StackId: str = ...,
    LayerId: str = ...,
    InstanceIds: Sequence[str] = ...,
) -> DescribeInstancesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInstancesResultTypeDef](./type_defs.md#describeinstancesresulttypedef) 


```python
# describe_instances method usage example with argument unpacking

kwargs: DescribeInstancesRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_instances(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesRequestRequestTypeDef](./type_defs.md#describeinstancesrequestrequesttypedef) 

### describe\_layers

Requests a description of one or more layers in a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_layers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_layers.html)

```python
# describe_layers method definition

await def describe_layers(
    self,
    *,
    StackId: str = ...,
    LayerIds: Sequence[str] = ...,
) -> DescribeLayersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLayersResultTypeDef](./type_defs.md#describelayersresulttypedef) 


```python
# describe_layers method usage example with argument unpacking

kwargs: DescribeLayersRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_layers(**kwargs)
```

1. See [:material-code-braces: DescribeLayersRequestRequestTypeDef](./type_defs.md#describelayersrequestrequesttypedef) 

### describe\_load\_based\_auto\_scaling

Describes load-based auto scaling configurations for specified layers.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_load_based_auto_scaling` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_load_based_auto_scaling.html)

```python
# describe_load_based_auto_scaling method definition

await def describe_load_based_auto_scaling(
    self,
    *,
    LayerIds: Sequence[str],
) -> DescribeLoadBasedAutoScalingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoadBasedAutoScalingResultTypeDef](./type_defs.md#describeloadbasedautoscalingresulttypedef) 


```python
# describe_load_based_auto_scaling method usage example with argument unpacking

kwargs: DescribeLoadBasedAutoScalingRequestRequestTypeDef = {  # (1)
    "LayerIds": ...,
}

parent.describe_load_based_auto_scaling(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBasedAutoScalingRequestRequestTypeDef](./type_defs.md#describeloadbasedautoscalingrequestrequesttypedef) 

### describe\_my\_user\_profile

Describes a user's SSH information.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_my_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_my_user_profile.html)

```python
# describe_my_user_profile method definition

await def describe_my_user_profile(
    self,
) -> DescribeMyUserProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMyUserProfileResultTypeDef](./type_defs.md#describemyuserprofileresulttypedef) 

### describe\_operating\_systems

Describes the operating systems that are supported by OpsWorks Stacks.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_operating_systems` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_operating_systems.html)

```python
# describe_operating_systems method definition

await def describe_operating_systems(
    self,
) -> DescribeOperatingSystemsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOperatingSystemsResponseTypeDef](./type_defs.md#describeoperatingsystemsresponsetypedef) 

### describe\_permissions

Describes the permissions for a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_permissions.html)

```python
# describe_permissions method definition

await def describe_permissions(
    self,
    *,
    IamUserArn: str = ...,
    StackId: str = ...,
) -> DescribePermissionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePermissionsResultTypeDef](./type_defs.md#describepermissionsresulttypedef) 


```python
# describe_permissions method usage example with argument unpacking

kwargs: DescribePermissionsRequestRequestTypeDef = {  # (1)
    "IamUserArn": ...,
}

parent.describe_permissions(**kwargs)
```

1. See [:material-code-braces: DescribePermissionsRequestRequestTypeDef](./type_defs.md#describepermissionsrequestrequesttypedef) 

### describe\_raid\_arrays

Describe an instance's RAID arrays.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_raid_arrays` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_raid_arrays.html)

```python
# describe_raid_arrays method definition

await def describe_raid_arrays(
    self,
    *,
    InstanceId: str = ...,
    StackId: str = ...,
    RaidArrayIds: Sequence[str] = ...,
) -> DescribeRaidArraysResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRaidArraysResultTypeDef](./type_defs.md#describeraidarraysresulttypedef) 


```python
# describe_raid_arrays method usage example with argument unpacking

kwargs: DescribeRaidArraysRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_raid_arrays(**kwargs)
```

1. See [:material-code-braces: DescribeRaidArraysRequestRequestTypeDef](./type_defs.md#describeraidarraysrequestrequesttypedef) 

### describe\_rds\_db\_instances

Describes Amazon RDS instances.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_rds_db_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_rds_db_instances.html)

```python
# describe_rds_db_instances method definition

await def describe_rds_db_instances(
    self,
    *,
    StackId: str,
    RdsDbInstanceArns: Sequence[str] = ...,
) -> DescribeRdsDbInstancesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRdsDbInstancesResultTypeDef](./type_defs.md#describerdsdbinstancesresulttypedef) 


```python
# describe_rds_db_instances method usage example with argument unpacking

kwargs: DescribeRdsDbInstancesRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_rds_db_instances(**kwargs)
```

1. See [:material-code-braces: DescribeRdsDbInstancesRequestRequestTypeDef](./type_defs.md#describerdsdbinstancesrequestrequesttypedef) 

### describe\_service\_errors

Describes OpsWorks Stacks service errors.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_service_errors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_service_errors.html)

```python
# describe_service_errors method definition

await def describe_service_errors(
    self,
    *,
    StackId: str = ...,
    InstanceId: str = ...,
    ServiceErrorIds: Sequence[str] = ...,
) -> DescribeServiceErrorsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServiceErrorsResultTypeDef](./type_defs.md#describeserviceerrorsresulttypedef) 


```python
# describe_service_errors method usage example with argument unpacking

kwargs: DescribeServiceErrorsRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_service_errors(**kwargs)
```

1. See [:material-code-braces: DescribeServiceErrorsRequestRequestTypeDef](./type_defs.md#describeserviceerrorsrequestrequesttypedef) 

### describe\_stack\_provisioning\_parameters

Requests a description of a stack's provisioning parameters.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_stack_provisioning_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_stack_provisioning_parameters.html)

```python
# describe_stack_provisioning_parameters method definition

await def describe_stack_provisioning_parameters(
    self,
    *,
    StackId: str,
) -> DescribeStackProvisioningParametersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStackProvisioningParametersResultTypeDef](./type_defs.md#describestackprovisioningparametersresulttypedef) 


```python
# describe_stack_provisioning_parameters method usage example with argument unpacking

kwargs: DescribeStackProvisioningParametersRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_stack_provisioning_parameters(**kwargs)
```

1. See [:material-code-braces: DescribeStackProvisioningParametersRequestRequestTypeDef](./type_defs.md#describestackprovisioningparametersrequestrequesttypedef) 

### describe\_stack\_summary

Describes the number of layers and apps in a specified stack, and the number of
instances in each state, such as <code>running_setup</code> or
<code>online</code>.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_stack_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_stack_summary.html)

```python
# describe_stack_summary method definition

await def describe_stack_summary(
    self,
    *,
    StackId: str,
) -> DescribeStackSummaryResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStackSummaryResultTypeDef](./type_defs.md#describestacksummaryresulttypedef) 


```python
# describe_stack_summary method usage example with argument unpacking

kwargs: DescribeStackSummaryRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.describe_stack_summary(**kwargs)
```

1. See [:material-code-braces: DescribeStackSummaryRequestRequestTypeDef](./type_defs.md#describestacksummaryrequestrequesttypedef) 

### describe\_stacks

Requests a description of one or more stacks.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_stacks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_stacks.html)

```python
# describe_stacks method definition

await def describe_stacks(
    self,
    *,
    StackIds: Sequence[str] = ...,
) -> DescribeStacksResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStacksResultTypeDef](./type_defs.md#describestacksresulttypedef) 


```python
# describe_stacks method usage example with argument unpacking

kwargs: DescribeStacksRequestRequestTypeDef = {  # (1)
    "StackIds": ...,
}

parent.describe_stacks(**kwargs)
```

1. See [:material-code-braces: DescribeStacksRequestRequestTypeDef](./type_defs.md#describestacksrequestrequesttypedef) 

### describe\_time\_based\_auto\_scaling

Describes time-based auto scaling configurations for specified instances.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_time_based_auto_scaling` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_time_based_auto_scaling.html)

```python
# describe_time_based_auto_scaling method definition

await def describe_time_based_auto_scaling(
    self,
    *,
    InstanceIds: Sequence[str],
) -> DescribeTimeBasedAutoScalingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTimeBasedAutoScalingResultTypeDef](./type_defs.md#describetimebasedautoscalingresulttypedef) 


```python
# describe_time_based_auto_scaling method usage example with argument unpacking

kwargs: DescribeTimeBasedAutoScalingRequestRequestTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.describe_time_based_auto_scaling(**kwargs)
```

1. See [:material-code-braces: DescribeTimeBasedAutoScalingRequestRequestTypeDef](./type_defs.md#describetimebasedautoscalingrequestrequesttypedef) 

### describe\_user\_profiles

Describe specified users.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_user_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_user_profiles.html)

```python
# describe_user_profiles method definition

await def describe_user_profiles(
    self,
    *,
    IamUserArns: Sequence[str] = ...,
) -> DescribeUserProfilesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserProfilesResultTypeDef](./type_defs.md#describeuserprofilesresulttypedef) 


```python
# describe_user_profiles method usage example with argument unpacking

kwargs: DescribeUserProfilesRequestRequestTypeDef = {  # (1)
    "IamUserArns": ...,
}

parent.describe_user_profiles(**kwargs)
```

1. See [:material-code-braces: DescribeUserProfilesRequestRequestTypeDef](./type_defs.md#describeuserprofilesrequestrequesttypedef) 

### describe\_volumes

Describes an instance's Amazon EBS volumes.

Type annotations and code completion for `#!python session.create_client("opsworks").describe_volumes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/describe_volumes.html)

```python
# describe_volumes method definition

await def describe_volumes(
    self,
    *,
    InstanceId: str = ...,
    StackId: str = ...,
    RaidArrayId: str = ...,
    VolumeIds: Sequence[str] = ...,
) -> DescribeVolumesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVolumesResultTypeDef](./type_defs.md#describevolumesresulttypedef) 


```python
# describe_volumes method usage example with argument unpacking

kwargs: DescribeVolumesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_volumes(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestRequestTypeDef](./type_defs.md#describevolumesrequestrequesttypedef) 

### detach\_elastic\_load\_balancer

Detaches a specified Elastic Load Balancing instance from its layer.

Type annotations and code completion for `#!python session.create_client("opsworks").detach_elastic_load_balancer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/detach_elastic_load_balancer.html)

```python
# detach_elastic_load_balancer method definition

await def detach_elastic_load_balancer(
    self,
    *,
    ElasticLoadBalancerName: str,
    LayerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# detach_elastic_load_balancer method usage example with argument unpacking

kwargs: DetachElasticLoadBalancerRequestRequestTypeDef = {  # (1)
    "ElasticLoadBalancerName": ...,
    "LayerId": ...,
}

parent.detach_elastic_load_balancer(**kwargs)
```

1. See [:material-code-braces: DetachElasticLoadBalancerRequestRequestTypeDef](./type_defs.md#detachelasticloadbalancerrequestrequesttypedef) 

### disassociate\_elastic\_ip

Disassociates an Elastic IP address from its instance.

Type annotations and code completion for `#!python session.create_client("opsworks").disassociate_elastic_ip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/disassociate_elastic_ip.html)

```python
# disassociate_elastic_ip method definition

await def disassociate_elastic_ip(
    self,
    *,
    ElasticIp: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_elastic_ip method usage example with argument unpacking

kwargs: DisassociateElasticIpRequestRequestTypeDef = {  # (1)
    "ElasticIp": ...,
}

parent.disassociate_elastic_ip(**kwargs)
```

1. See [:material-code-braces: DisassociateElasticIpRequestRequestTypeDef](./type_defs.md#disassociateelasticiprequestrequesttypedef) 

### get\_hostname\_suggestion

Gets a generated host name for the specified layer, based on the current host
name theme.

Type annotations and code completion for `#!python session.create_client("opsworks").get_hostname_suggestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/get_hostname_suggestion.html)

```python
# get_hostname_suggestion method definition

await def get_hostname_suggestion(
    self,
    *,
    LayerId: str,
) -> GetHostnameSuggestionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHostnameSuggestionResultTypeDef](./type_defs.md#gethostnamesuggestionresulttypedef) 


```python
# get_hostname_suggestion method usage example with argument unpacking

kwargs: GetHostnameSuggestionRequestRequestTypeDef = {  # (1)
    "LayerId": ...,
}

parent.get_hostname_suggestion(**kwargs)
```

1. See [:material-code-braces: GetHostnameSuggestionRequestRequestTypeDef](./type_defs.md#gethostnamesuggestionrequestrequesttypedef) 

### grant\_access

This action can be used only with Windows stacks.

Type annotations and code completion for `#!python session.create_client("opsworks").grant_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/grant_access.html)

```python
# grant_access method definition

await def grant_access(
    self,
    *,
    InstanceId: str,
    ValidForInMinutes: int = ...,
) -> GrantAccessResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GrantAccessResultTypeDef](./type_defs.md#grantaccessresulttypedef) 


```python
# grant_access method usage example with argument unpacking

kwargs: GrantAccessRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.grant_access(**kwargs)
```

1. See [:material-code-braces: GrantAccessRequestRequestTypeDef](./type_defs.md#grantaccessrequestrequesttypedef) 

### list\_tags

Returns a list of tags that are applied to the specified stack or layer.

Type annotations and code completion for `#!python session.create_client("opsworks").list_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/list_tags.html)

```python
# list_tags method definition

await def list_tags(
    self,
    *,
    ResourceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsResultTypeDef](./type_defs.md#listtagsresulttypedef) 


```python
# list_tags method usage example with argument unpacking

kwargs: ListTagsRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef) 

### reboot\_instance

Reboots a specified instance.

Type annotations and code completion for `#!python session.create_client("opsworks").reboot_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/reboot_instance.html)

```python
# reboot_instance method definition

await def reboot_instance(
    self,
    *,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# reboot_instance method usage example with argument unpacking

kwargs: RebootInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.reboot_instance(**kwargs)
```

1. See [:material-code-braces: RebootInstanceRequestRequestTypeDef](./type_defs.md#rebootinstancerequestrequesttypedef) 

### register\_ecs\_cluster

Registers a specified Amazon ECS cluster with a stack.

Type annotations and code completion for `#!python session.create_client("opsworks").register_ecs_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/register_ecs_cluster.html)

```python
# register_ecs_cluster method definition

await def register_ecs_cluster(
    self,
    *,
    EcsClusterArn: str,
    StackId: str,
) -> RegisterEcsClusterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterEcsClusterResultTypeDef](./type_defs.md#registerecsclusterresulttypedef) 


```python
# register_ecs_cluster method usage example with argument unpacking

kwargs: RegisterEcsClusterRequestRequestTypeDef = {  # (1)
    "EcsClusterArn": ...,
    "StackId": ...,
}

parent.register_ecs_cluster(**kwargs)
```

1. See [:material-code-braces: RegisterEcsClusterRequestRequestTypeDef](./type_defs.md#registerecsclusterrequestrequesttypedef) 

### register\_elastic\_ip

Registers an Elastic IP address with a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").register_elastic_ip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/register_elastic_ip.html)

```python
# register_elastic_ip method definition

await def register_elastic_ip(
    self,
    *,
    ElasticIp: str,
    StackId: str,
) -> RegisterElasticIpResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterElasticIpResultTypeDef](./type_defs.md#registerelasticipresulttypedef) 


```python
# register_elastic_ip method usage example with argument unpacking

kwargs: RegisterElasticIpRequestRequestTypeDef = {  # (1)
    "ElasticIp": ...,
    "StackId": ...,
}

parent.register_elastic_ip(**kwargs)
```

1. See [:material-code-braces: RegisterElasticIpRequestRequestTypeDef](./type_defs.md#registerelasticiprequestrequesttypedef) 

### register\_instance

Registers instances that were created outside of OpsWorks Stacks with a
specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").register_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/register_instance.html)

```python
# register_instance method definition

await def register_instance(
    self,
    *,
    StackId: str,
    Hostname: str = ...,
    PublicIp: str = ...,
    PrivateIp: str = ...,
    RsaPublicKey: str = ...,
    RsaPublicKeyFingerprint: str = ...,
    InstanceIdentity: InstanceIdentityTypeDef = ...,  # (1)
) -> RegisterInstanceResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef) 
2. See [:material-code-braces: RegisterInstanceResultTypeDef](./type_defs.md#registerinstanceresulttypedef) 


```python
# register_instance method usage example with argument unpacking

kwargs: RegisterInstanceRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.register_instance(**kwargs)
```

1. See [:material-code-braces: RegisterInstanceRequestRequestTypeDef](./type_defs.md#registerinstancerequestrequesttypedef) 

### register\_rds\_db\_instance

Registers an Amazon RDS instance with a stack.

Type annotations and code completion for `#!python session.create_client("opsworks").register_rds_db_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/register_rds_db_instance.html)

```python
# register_rds_db_instance method definition

await def register_rds_db_instance(
    self,
    *,
    StackId: str,
    RdsDbInstanceArn: str,
    DbUser: str,
    DbPassword: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# register_rds_db_instance method usage example with argument unpacking

kwargs: RegisterRdsDbInstanceRequestRequestTypeDef = {  # (1)
    "StackId": ...,
    "RdsDbInstanceArn": ...,
    "DbUser": ...,
    "DbPassword": ...,
}

parent.register_rds_db_instance(**kwargs)
```

1. See [:material-code-braces: RegisterRdsDbInstanceRequestRequestTypeDef](./type_defs.md#registerrdsdbinstancerequestrequesttypedef) 

### register\_volume

Registers an Amazon EBS volume with a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").register_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/register_volume.html)

```python
# register_volume method definition

await def register_volume(
    self,
    *,
    StackId: str,
    Ec2VolumeId: str = ...,
) -> RegisterVolumeResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterVolumeResultTypeDef](./type_defs.md#registervolumeresulttypedef) 


```python
# register_volume method usage example with argument unpacking

kwargs: RegisterVolumeRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.register_volume(**kwargs)
```

1. See [:material-code-braces: RegisterVolumeRequestRequestTypeDef](./type_defs.md#registervolumerequestrequesttypedef) 

### set\_load\_based\_auto\_scaling

Specify the load-based auto scaling configuration for a specified layer.

Type annotations and code completion for `#!python session.create_client("opsworks").set_load_based_auto_scaling` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/set_load_based_auto_scaling.html)

```python
# set_load_based_auto_scaling method definition

await def set_load_based_auto_scaling(
    self,
    *,
    LayerId: str,
    Enable: bool = ...,
    UpScaling: AutoScalingThresholdsTypeDef = ...,  # (1)
    DownScaling: AutoScalingThresholdsTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef) 
2. See [:material-code-braces: AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_load_based_auto_scaling method usage example with argument unpacking

kwargs: SetLoadBasedAutoScalingRequestRequestTypeDef = {  # (1)
    "LayerId": ...,
}

parent.set_load_based_auto_scaling(**kwargs)
```

1. See [:material-code-braces: SetLoadBasedAutoScalingRequestRequestTypeDef](./type_defs.md#setloadbasedautoscalingrequestrequesttypedef) 

### set\_permission

Specifies a user's permissions.

Type annotations and code completion for `#!python session.create_client("opsworks").set_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/set_permission.html)

```python
# set_permission method definition

await def set_permission(
    self,
    *,
    StackId: str,
    IamUserArn: str,
    AllowSsh: bool = ...,
    AllowSudo: bool = ...,
    Level: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_permission method usage example with argument unpacking

kwargs: SetPermissionRequestRequestTypeDef = {  # (1)
    "StackId": ...,
    "IamUserArn": ...,
}

parent.set_permission(**kwargs)
```

1. See [:material-code-braces: SetPermissionRequestRequestTypeDef](./type_defs.md#setpermissionrequestrequesttypedef) 

### set\_time\_based\_auto\_scaling

Specify the time-based auto scaling configuration for a specified instance.

Type annotations and code completion for `#!python session.create_client("opsworks").set_time_based_auto_scaling` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/set_time_based_auto_scaling.html)

```python
# set_time_based_auto_scaling method definition

await def set_time_based_auto_scaling(
    self,
    *,
    InstanceId: str,
    AutoScalingSchedule: WeeklyAutoScalingScheduleTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: WeeklyAutoScalingScheduleTypeDef](./type_defs.md#weeklyautoscalingscheduletypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_time_based_auto_scaling method usage example with argument unpacking

kwargs: SetTimeBasedAutoScalingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.set_time_based_auto_scaling(**kwargs)
```

1. See [:material-code-braces: SetTimeBasedAutoScalingRequestRequestTypeDef](./type_defs.md#settimebasedautoscalingrequestrequesttypedef) 

### start\_instance

Starts a specified instance.

Type annotations and code completion for `#!python session.create_client("opsworks").start_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/start_instance.html)

```python
# start_instance method definition

await def start_instance(
    self,
    *,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_instance method usage example with argument unpacking

kwargs: StartInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.start_instance(**kwargs)
```

1. See [:material-code-braces: StartInstanceRequestRequestTypeDef](./type_defs.md#startinstancerequestrequesttypedef) 

### start\_stack

Starts a stack's instances.

Type annotations and code completion for `#!python session.create_client("opsworks").start_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/start_stack.html)

```python
# start_stack method definition

await def start_stack(
    self,
    *,
    StackId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_stack method usage example with argument unpacking

kwargs: StartStackRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.start_stack(**kwargs)
```

1. See [:material-code-braces: StartStackRequestRequestTypeDef](./type_defs.md#startstackrequestrequesttypedef) 

### stop\_instance

Stops a specified instance.

Type annotations and code completion for `#!python session.create_client("opsworks").stop_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/stop_instance.html)

```python
# stop_instance method definition

await def stop_instance(
    self,
    *,
    InstanceId: str,
    Force: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_instance method usage example with argument unpacking

kwargs: StopInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.stop_instance(**kwargs)
```

1. See [:material-code-braces: StopInstanceRequestRequestTypeDef](./type_defs.md#stopinstancerequestrequesttypedef) 

### stop\_stack

Stops a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").stop_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/stop_stack.html)

```python
# stop_stack method definition

await def stop_stack(
    self,
    *,
    StackId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_stack method usage example with argument unpacking

kwargs: StopStackRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.stop_stack(**kwargs)
```

1. See [:material-code-braces: StopStackRequestRequestTypeDef](./type_defs.md#stopstackrequestrequesttypedef) 

### tag\_resource

Apply cost-allocation tags to a specified stack or layer in OpsWorks Stacks.

Type annotations and code completion for `#!python session.create_client("opsworks").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### unassign\_instance

Unassigns a registered instance from all layers that are using the instance.

Type annotations and code completion for `#!python session.create_client("opsworks").unassign_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/unassign_instance.html)

```python
# unassign_instance method definition

await def unassign_instance(
    self,
    *,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# unassign_instance method usage example with argument unpacking

kwargs: UnassignInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.unassign_instance(**kwargs)
```

1. See [:material-code-braces: UnassignInstanceRequestRequestTypeDef](./type_defs.md#unassigninstancerequestrequesttypedef) 

### unassign\_volume

Unassigns an assigned Amazon EBS volume.

Type annotations and code completion for `#!python session.create_client("opsworks").unassign_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/unassign_volume.html)

```python
# unassign_volume method definition

await def unassign_volume(
    self,
    *,
    VolumeId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# unassign_volume method usage example with argument unpacking

kwargs: UnassignVolumeRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
}

parent.unassign_volume(**kwargs)
```

1. See [:material-code-braces: UnassignVolumeRequestRequestTypeDef](./type_defs.md#unassignvolumerequestrequesttypedef) 

### untag\_resource

Removes tags from a specified stack or layer.

Type annotations and code completion for `#!python session.create_client("opsworks").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_app

Updates a specified app.

Type annotations and code completion for `#!python session.create_client("opsworks").update_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_app.html)

```python
# update_app method definition

await def update_app(
    self,
    *,
    AppId: str,
    Name: str = ...,
    Description: str = ...,
    DataSources: Sequence[DataSourceTypeDef] = ...,  # (1)
    Type: AppTypeType = ...,  # (2)
    AppSource: SourceTypeDef = ...,  # (3)
    Domains: Sequence[str] = ...,
    EnableSsl: bool = ...,
    SslConfiguration: SslConfigurationTypeDef = ...,  # (4)
    Attributes: Mapping[AppAttributesKeysType, str] = ...,  # (5)
    Environment: Sequence[EnvironmentVariableTypeDef] = ...,  # (6)
) -> EmptyResponseMetadataTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
4. See [:material-code-braces: SslConfigurationTypeDef](./type_defs.md#sslconfigurationtypedef) 
5. See [:material-code-brackets: AppAttributesKeysType](./literals.md#appattributeskeystype) 
6. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
7. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_app method usage example with argument unpacking

kwargs: UpdateAppRequestRequestTypeDef = {  # (1)
    "AppId": ...,
}

parent.update_app(**kwargs)
```

1. See [:material-code-braces: UpdateAppRequestRequestTypeDef](./type_defs.md#updateapprequestrequesttypedef) 

### update\_elastic\_ip

Updates a registered Elastic IP address's name.

Type annotations and code completion for `#!python session.create_client("opsworks").update_elastic_ip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_elastic_ip.html)

```python
# update_elastic_ip method definition

await def update_elastic_ip(
    self,
    *,
    ElasticIp: str,
    Name: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_elastic_ip method usage example with argument unpacking

kwargs: UpdateElasticIpRequestRequestTypeDef = {  # (1)
    "ElasticIp": ...,
}

parent.update_elastic_ip(**kwargs)
```

1. See [:material-code-braces: UpdateElasticIpRequestRequestTypeDef](./type_defs.md#updateelasticiprequestrequesttypedef) 

### update\_instance

Updates a specified instance.

Type annotations and code completion for `#!python session.create_client("opsworks").update_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_instance.html)

```python
# update_instance method definition

await def update_instance(
    self,
    *,
    InstanceId: str,
    LayerIds: Sequence[str] = ...,
    InstanceType: str = ...,
    AutoScalingType: AutoScalingTypeType = ...,  # (1)
    Hostname: str = ...,
    Os: str = ...,
    AmiId: str = ...,
    SshKeyName: str = ...,
    Architecture: ArchitectureType = ...,  # (2)
    InstallUpdatesOnBoot: bool = ...,
    EbsOptimized: bool = ...,
    AgentVersion: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AutoScalingTypeType](./literals.md#autoscalingtypetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_instance method usage example with argument unpacking

kwargs: UpdateInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.update_instance(**kwargs)
```

1. See [:material-code-braces: UpdateInstanceRequestRequestTypeDef](./type_defs.md#updateinstancerequestrequesttypedef) 

### update\_layer

Updates a specified layer.

Type annotations and code completion for `#!python session.create_client("opsworks").update_layer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_layer.html)

```python
# update_layer method definition

await def update_layer(
    self,
    *,
    LayerId: str,
    Name: str = ...,
    Shortname: str = ...,
    Attributes: Mapping[LayerAttributesKeysType, str] = ...,  # (1)
    CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,  # (2)
    CustomInstanceProfileArn: str = ...,
    CustomJson: str = ...,
    CustomSecurityGroupIds: Sequence[str] = ...,
    Packages: Sequence[str] = ...,
    VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,  # (3)
    EnableAutoHealing: bool = ...,
    AutoAssignElasticIps: bool = ...,
    AutoAssignPublicIps: bool = ...,
    CustomRecipes: RecipesTypeDef = ...,  # (4)
    InstallUpdatesOnBoot: bool = ...,
    UseEbsOptimizedInstances: bool = ...,
    LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,  # (5)
) -> EmptyResponseMetadataTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
2. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) 
3. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
4. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) 
5. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
6. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_layer method usage example with argument unpacking

kwargs: UpdateLayerRequestRequestTypeDef = {  # (1)
    "LayerId": ...,
}

parent.update_layer(**kwargs)
```

1. See [:material-code-braces: UpdateLayerRequestRequestTypeDef](./type_defs.md#updatelayerrequestrequesttypedef) 

### update\_my\_user\_profile

Updates a user's SSH public key.

Type annotations and code completion for `#!python session.create_client("opsworks").update_my_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_my_user_profile.html)

```python
# update_my_user_profile method definition

await def update_my_user_profile(
    self,
    *,
    SshPublicKey: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_my_user_profile method usage example with argument unpacking

kwargs: UpdateMyUserProfileRequestRequestTypeDef = {  # (1)
    "SshPublicKey": ...,
}

parent.update_my_user_profile(**kwargs)
```

1. See [:material-code-braces: UpdateMyUserProfileRequestRequestTypeDef](./type_defs.md#updatemyuserprofilerequestrequesttypedef) 

### update\_rds\_db\_instance

Updates an Amazon RDS instance.

Type annotations and code completion for `#!python session.create_client("opsworks").update_rds_db_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_rds_db_instance.html)

```python
# update_rds_db_instance method definition

await def update_rds_db_instance(
    self,
    *,
    RdsDbInstanceArn: str,
    DbUser: str = ...,
    DbPassword: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_rds_db_instance method usage example with argument unpacking

kwargs: UpdateRdsDbInstanceRequestRequestTypeDef = {  # (1)
    "RdsDbInstanceArn": ...,
}

parent.update_rds_db_instance(**kwargs)
```

1. See [:material-code-braces: UpdateRdsDbInstanceRequestRequestTypeDef](./type_defs.md#updaterdsdbinstancerequestrequesttypedef) 

### update\_stack

Updates a specified stack.

Type annotations and code completion for `#!python session.create_client("opsworks").update_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_stack.html)

```python
# update_stack method definition

await def update_stack(
    self,
    *,
    StackId: str,
    Name: str = ...,
    Attributes: Mapping[StackAttributesKeysType, str] = ...,  # (1)
    ServiceRoleArn: str = ...,
    DefaultInstanceProfileArn: str = ...,
    DefaultOs: str = ...,
    HostnameTheme: str = ...,
    DefaultAvailabilityZone: str = ...,
    DefaultSubnetId: str = ...,
    CustomJson: str = ...,
    ConfigurationManager: StackConfigurationManagerTypeDef = ...,  # (2)
    ChefConfiguration: ChefConfigurationTypeDef = ...,  # (3)
    UseCustomCookbooks: bool = ...,
    CustomCookbooksSource: SourceTypeDef = ...,  # (4)
    DefaultSshKeyName: str = ...,
    DefaultRootDeviceType: RootDeviceTypeType = ...,  # (5)
    UseOpsworksSecurityGroups: bool = ...,
    AgentVersion: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
6. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_stack method usage example with argument unpacking

kwargs: UpdateStackRequestRequestTypeDef = {  # (1)
    "StackId": ...,
}

parent.update_stack(**kwargs)
```

1. See [:material-code-braces: UpdateStackRequestRequestTypeDef](./type_defs.md#updatestackrequestrequesttypedef) 

### update\_user\_profile

Updates a specified user profile.

Type annotations and code completion for `#!python session.create_client("opsworks").update_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_user_profile.html)

```python
# update_user_profile method definition

await def update_user_profile(
    self,
    *,
    IamUserArn: str,
    SshUsername: str = ...,
    SshPublicKey: str = ...,
    AllowSelfManagement: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_profile method usage example with argument unpacking

kwargs: UpdateUserProfileRequestRequestTypeDef = {  # (1)
    "IamUserArn": ...,
}

parent.update_user_profile(**kwargs)
```

1. See [:material-code-braces: UpdateUserProfileRequestRequestTypeDef](./type_defs.md#updateuserprofilerequestrequesttypedef) 

### update\_volume

Updates an Amazon EBS volume's name or mount point.

Type annotations and code completion for `#!python session.create_client("opsworks").update_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/client/update_volume.html)

```python
# update_volume method definition

await def update_volume(
    self,
    *,
    VolumeId: str,
    Name: str = ...,
    MountPoint: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_volume method usage example with argument unpacking

kwargs: UpdateVolumeRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
}

parent.update_volume(**kwargs)
```

1. See [:material-code-braces: UpdateVolumeRequestRequestTypeDef](./type_defs.md#updatevolumerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("opsworks").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "OpsWorksClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("opsworks").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client)

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

Type annotations and code completion for `#!python session.create_client("opsworks").get_paginator` method with overloads.

- `client.get_paginator("describe_ecs_clusters")` -> [DescribeEcsClustersPaginator](./paginators.md#describeecsclusterspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("opsworks").get_waiter` method with overloads.

- `client.get_waiter("app_exists")` -> [AppExistsWaiter](./waiters.md#appexistswaiter)
- `client.get_waiter("deployment_successful")` -> [DeploymentSuccessfulWaiter](./waiters.md#deploymentsuccessfulwaiter)
- `client.get_waiter("instance_online")` -> [InstanceOnlineWaiter](./waiters.md#instanceonlinewaiter)
- `client.get_waiter("instance_registered")` -> [InstanceRegisteredWaiter](./waiters.md#instanceregisteredwaiter)
- `client.get_waiter("instance_stopped")` -> [InstanceStoppedWaiter](./waiters.md#instancestoppedwaiter)
- `client.get_waiter("instance_terminated")` -> [InstanceTerminatedWaiter](./waiters.md#instanceterminatedwaiter)

