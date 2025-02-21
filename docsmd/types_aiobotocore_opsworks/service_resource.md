# OpsWorksServiceResource

> [Index](../README.md) > [OpsWorks](./README.md) > OpsWorksServiceResource

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## OpsWorksServiceResource

Type annotations and code completion for `#!python session.resource("opsworks")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/index.html)

```python
# OpsWorksServiceResource usage example

from types_aiobotocore_opsworks.service_resource import OpsWorksServiceResource

def get_opsworks_resource() -> OpsWorksServiceResource:
    return session.resource("opsworks")
```


## Attributes


- `meta`: `OpsWorksResourceMeta`

- `stacks`: `ServiceResourceStacksCollection`




## Collections

### ServiceResourceStacksCollection

Provides access to [Stack](#stack) resource.

Type annotations and code completion for `#!python session.resource("opsworks").stacks` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/stacks.html#OpsWorks.ServiceResource.stacks)

```python
# ServiceResourceStacksCollection usage example

from types_aiobotocore_opsworks.service_resource import ServiceResourceStacksCollection

def get_collection() -> ServiceResourceStacksCollection:
    return session.resource("opsworks").stacks
```



## Methods

### OpsWorksServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this resource.

Type annotations and code completion for `#!python session.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


### OpsWorksServiceResource.create\_stack method

Creates a new stack.

Type annotations and code completion for `#!python session.resource("opsworks").create_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/create_stack.html)

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
) -> _Stack:
    ...
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 


```python
# create_stack method usage example with argument unpacking

kwargs: CreateStackRequestServiceResourceCreateStackTypeDef = {  # (1)
    "Name": ...,
    "Region": ...,
    "ServiceRoleArn": ...,
    "DefaultInstanceProfileArn": ...,
}

parent.create_stack(**kwargs)
```

1. See [:material-code-braces: CreateStackRequestServiceResourceCreateStackTypeDef](./type_defs.md#createstackrequestserviceresourcecreatestacktypedef) 

### OpsWorksServiceResource.Layer method

Creates a Layer resource.

Type annotations and code completion for `#!python session.resource("opsworks").Layer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/Layer.html)

```python
# Layer method definition

await def Layer(
    self,
    id: str,
) -> _Layer:
    ...
```


### OpsWorksServiceResource.Stack method

Creates a Stack resource.

Type annotations and code completion for `#!python session.resource("opsworks").Stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/Stack.html)

```python
# Stack method definition

await def Stack(
    self,
    id: str,
) -> _Stack:
    ...
```


### OpsWorksServiceResource.StackSummary method

Creates a StackSummary resource.

Type annotations and code completion for `#!python session.resource("opsworks").StackSummary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/StackSummary.html)

```python
# StackSummary method definition

await def StackSummary(
    self,
    stack_id: str,
) -> _StackSummary:
    ...
```




## Layer

Type annotations and code completion for `#!python session.resource("opsworks").Layer` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/layer/index.html#OpsWorks.Layer)

```python
# Layer usage example

from types_aiobotocore_opsworks.service_resource import Layer

def get_resource() -> Layer:
    return session.resource("opsworks").Layer(...)
```


### Layer attributes


- `id`: `str`
- `stack`: `Stack`
- `arn`: `Awaitable`[`str`]
- `stack_id`: `Awaitable`[`str`]
- `layer_id`: `Awaitable`[`str`]
- `type`: `Awaitable`[[LayerTypeType](./literals.md#layertypetype)]
- `name`: `Awaitable`[`str`]
- `shortname`: `Awaitable`[`str`]
- `attributes`: `Awaitable`[`Dict`[[LayerAttributesKeysType](./literals.md#layerattributeskeystype), `str`]]
- `cloud_watch_logs_configuration`: `Awaitable`[[CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef)]
- `custom_instance_profile_arn`: `Awaitable`[`str`]
- `custom_json`: `Awaitable`[`str`]
- `custom_security_group_ids`: `Awaitable`[`List`[`str`]]
- `default_security_group_names`: `Awaitable`[`List`[`str`]]
- `packages`: `Awaitable`[`List`[`str`]]
- `volume_configurations`: `Awaitable`[`List`[[VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef)]]
- `enable_auto_healing`: `Awaitable`[`bool`]
- `auto_assign_elastic_ips`: `Awaitable`[`bool`]
- `auto_assign_public_ips`: `Awaitable`[`bool`]
- `default_recipes`: `Awaitable`[[RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef)]
- `custom_recipes`: `Awaitable`[[RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef)]
- `created_at`: `Awaitable`[`str`]
- `install_updates_on_boot`: `Awaitable`[`bool`]
- `use_ebs_optimized_instances`: `Awaitable`[`bool`]
- `lifecycle_event_configuration`: `Awaitable`[[LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef)]
- `meta`: `OpsWorksResourceMeta`





### Layer methods


#### Layer.get\_available\_subresources method

Returns a list of all the available sub-resources for this Layer.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/layer/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Layer.delete method

Deletes a specified layer.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/layer/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Layer.load method



Type annotations and code completion for `#!python aiobotocore.resource("opsworks").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/layer/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Layer.reload method



Type annotations and code completion for `#!python aiobotocore.resource("opsworks").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/layer/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## Stack

Type annotations and code completion for `#!python session.resource("opsworks").Stack` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/index.html#OpsWorks.Stack)

```python
# Stack usage example

from types_aiobotocore_opsworks.service_resource import Stack

def get_resource() -> Stack:
    return session.resource("opsworks").Stack(...)
```


### Stack attributes


- `id`: `str`
- `layers`: `StackLayersCollection`
- `stack_id`: `Awaitable`[`str`]
- `name`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `region`: `Awaitable`[`str`]
- `vpc_id`: `Awaitable`[`str`]
- `attributes`: `Awaitable`[`Dict`[`Literal['Color']` (see [StackAttributesKeysType](./literals.md#stackattributeskeystype)), `str`]]
- `service_role_arn`: `Awaitable`[`str`]
- `default_instance_profile_arn`: `Awaitable`[`str`]
- `default_os`: `Awaitable`[`str`]
- `hostname_theme`: `Awaitable`[`str`]
- `default_availability_zone`: `Awaitable`[`str`]
- `default_subnet_id`: `Awaitable`[`str`]
- `custom_json`: `Awaitable`[`str`]
- `configuration_manager`: `Awaitable`[[StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef)]
- `chef_configuration`: `Awaitable`[[ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef)]
- `use_custom_cookbooks`: `Awaitable`[`bool`]
- `use_opsworks_security_groups`: `Awaitable`[`bool`]
- `custom_cookbooks_source`: `Awaitable`[[SourceTypeDef](./type_defs.md#sourcetypedef)]
- `default_ssh_key_name`: `Awaitable`[`str`]
- `created_at`: `Awaitable`[`str`]
- `default_root_device_type`: `Awaitable`[[RootDeviceTypeType](./literals.md#rootdevicetypetype)]
- `agent_version`: `Awaitable`[`str`]
- `meta`: `OpsWorksResourceMeta`



### Stack collections


#### Stack.layers

Provides access to [Layer](#layer) resource.

Type annotations and code completion for `#!python session.resource("opsworks").Stack(...).layers` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/layers.html#OpsWorks.Stack.layers)

```python
# StackLayersCollection usage example

from types_aiobotocore_opsworks.service_resource import StackLayersCollection

def get_collection() -> StackLayersCollection:
    resource = session.resource("opsworks").Stack(...)
    return resource.layers
```




### Stack methods


#### Stack.get\_available\_subresources method

Returns a list of all the available sub-resources for this Stack.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Stack.create\_layer method

Creates a layer.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").create_layer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/create_layer.html)

```python
# create_layer method definition

await def create_layer(
    self,
    *,
    Type: LayerTypeType,  # (1)
    Name: str,
    Shortname: str,
    Attributes: Mapping[LayerAttributesKeysType, str] = ...,  # (2)
    CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,  # (3)
    CustomInstanceProfileArn: str = ...,
    CustomJson: str = ...,
    CustomSecurityGroupIds: Sequence[str] = ...,
    Packages: Sequence[str] = ...,
    VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,  # (4)
    EnableAutoHealing: bool = ...,
    AutoAssignElasticIps: bool = ...,
    AutoAssignPublicIps: bool = ...,
    CustomRecipes: RecipesUnionTypeDef = ...,  # (5)
    InstallUpdatesOnBoot: bool = ...,
    UseEbsOptimizedInstances: bool = ...,
    LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,  # (6)
) -> _Layer:
    ...
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) [:material-code-braces: CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) [:material-code-braces: RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef) 
6. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 


```python
# create_layer method usage example with argument unpacking

kwargs: CreateLayerRequestStackCreateLayerTypeDef = {  # (1)
    "Type": ...,
    "Name": ...,
    "Shortname": ...,
}

parent.create_layer(**kwargs)
```

1. See [:material-code-braces: CreateLayerRequestStackCreateLayerTypeDef](./type_defs.md#createlayerrequeststackcreatelayertypedef) 

#### Stack.delete method

Deletes a specified stack.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Stack.Summary method

Creates a StackSummary resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").Summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/Summary.html)

```python
# Summary method definition

await def Summary(
    self,
) -> _StackSummary:
    ...
```


#### Stack.load method



Type annotations and code completion for `#!python aiobotocore.resource("opsworks").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Stack.reload method



Type annotations and code completion for `#!python aiobotocore.resource("opsworks").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stack/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## StackSummary

Type annotations and code completion for `#!python session.resource("opsworks").StackSummary` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stacksummary/index.html#OpsWorks.StackSummary)

```python
# StackSummary usage example

from types_aiobotocore_opsworks.service_resource import StackSummary

def get_resource() -> StackSummary:
    return session.resource("opsworks").StackSummary(...)
```


### StackSummary attributes


- `stack_id`: `str`
- `name`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `layers_count`: `Awaitable`[`int`]
- `apps_count`: `Awaitable`[`int`]
- `instances_count`: `Awaitable`[[InstancesCountTypeDef](./type_defs.md#instancescounttypedef)]
- `meta`: `OpsWorksResourceMeta`





### StackSummary methods


#### StackSummary.get\_available\_subresources method

Returns a list of all the available sub-resources for this StackSummary.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stacksummary/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### StackSummary.Stack method

Creates a Stack resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").Stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stacksummary/Stack.html)

```python
# Stack method definition

await def Stack(
    self,
) -> _Stack:
    ...
```


#### StackSummary.load method



Type annotations and code completion for `#!python aiobotocore.resource("opsworks").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stacksummary/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### StackSummary.reload method



Type annotations and code completion for `#!python aiobotocore.resource("opsworks").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/stacksummary/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```




