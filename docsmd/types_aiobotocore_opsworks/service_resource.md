# OpsWorksServiceResource

> [Index](../README.md) > [OpsWorks](./README.md) > OpsWorksServiceResource

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## OpsWorksServiceResource

Type annotations and code completion for `#!python session.resource("opsworks")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource)

```python
# OpsWorksServiceResource usage example

from types_aiobotocore_opsworks.service_resource import OpsWorksServiceResource

def get_opsworks_resource() -> OpsWorksServiceResource:
    return session.resource("opsworks")
```


## Attributes


- `meta`: [OpsWorksResourceMeta](#opsworksresourcemeta)

- `stacks`: [ServiceResourceStacksCollection](#serviceresourcestackscollection)




## Collections

### ServiceResourceStacksCollection

Provides access to [Stack](#stack) resource.

Type annotations and code completion for `#!python session.resource("opsworks").stacks` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.stacks)

```python
# ServiceResourceStacksCollection usage example

from types_aiobotocore_opsworks.service_resource import ServiceResourceStacksCollection

def get_collection() -> ServiceResourceStacksCollection:
    return session.resource("opsworks").stacks
```



## Methods

### OpsWorksServiceResource.Layer method

Creates a Layer resource.

Type annotations and code completion for `#!python session.resource("opsworks").Layer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Layer)

```python
# Layer method definition

await def Layer(
    self,
    id: str,
) -> Layer:
    ...
```


### OpsWorksServiceResource.Stack method

Creates a Stack resource.

Type annotations and code completion for `#!python session.resource("opsworks").Stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Stack)

```python
# Stack method definition

await def Stack(
    self,
    id: str,
) -> Stack:
    ...
```


### OpsWorksServiceResource.StackSummary method

Creates a StackSummary resource.

Type annotations and code completion for `#!python session.resource("opsworks").StackSummary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.StackSummary)

```python
# StackSummary method definition

await def StackSummary(
    self,
    stack_id: str,
) -> StackSummary:
    ...
```


### OpsWorksServiceResource.create\_stack method

Creates a new stack.

Type annotations and code completion for `#!python session.resource("opsworks").create_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.create_stack)

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
) -> Stack:
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

### OpsWorksServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python session.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```




## Layer

Type annotations and code completion for `#!python session.resource("opsworks").Layer` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Layer)

```python
# Layer usage example

from types_aiobotocore_opsworks.service_resource import Layer

def get_resource() -> Layer:
    return session.resource("opsworks").Layer(...)
```


### Layer attributes


- `arn`: `Awaitable`[`str`]
- `stack_id`: `Awaitable`[`str`]
- `layer_id`: `Awaitable`[`str`]
- `type`: `Awaitable`[[LayerTypeType](./literals.md#layertypetype)]
- `name`: `Awaitable`[`str`]
- `shortname`: `Awaitable`[`str`]
- `attributes`: `Awaitable`[`Dict`[[LayerAttributesKeysType](./literals.md#layerattributeskeystype), `str`]]
- `cloud_watch_logs_configuration`: `Awaitable`[[CloudWatchLogsConfigurationResponseTypeDef](./type_defs.md#cloudwatchlogsconfigurationresponsetypedef)]
- `custom_instance_profile_arn`: `Awaitable`[`str`]
- `custom_json`: `Awaitable`[`str`]
- `custom_security_group_ids`: `Awaitable`[`List`[`str`]]
- `default_security_group_names`: `Awaitable`[`List`[`str`]]
- `packages`: `Awaitable`[`List`[`str`]]
- `volume_configurations`: `Awaitable`[`List`[[VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef)]]
- `enable_auto_healing`: `Awaitable`[`bool`]
- `auto_assign_elastic_ips`: `Awaitable`[`bool`]
- `auto_assign_public_ips`: `Awaitable`[`bool`]
- `default_recipes`: `Awaitable`[[RecipesResponseTypeDef](./type_defs.md#recipesresponsetypedef)]
- `custom_recipes`: `Awaitable`[[RecipesResponseTypeDef](./type_defs.md#recipesresponsetypedef)]
- `created_at`: `Awaitable`[`str`]
- `install_updates_on_boot`: `Awaitable`[`bool`]
- `use_ebs_optimized_instances`: `Awaitable`[`bool`]
- `lifecycle_event_configuration`: `Awaitable`[[LifecycleEventConfigurationResponseTypeDef](./type_defs.md#lifecycleeventconfigurationresponsetypedef)]
- `id`: `str`
- `stack`: [Stack](#stack)





### Layer methods


#### Layer.delete method

Deletes a specified layer.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Layer.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Layer.load method

Calls :py:meth:`OpsWorks.Client.describe_layers` to update the attributes of the
Layer resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Layer.reload method

Calls :py:meth:`OpsWorks.Client.describe_layers` to update the attributes of the
Layer resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## Stack

Type annotations and code completion for `#!python session.resource("opsworks").Stack` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Stack)

```python
# Stack usage example

from types_aiobotocore_opsworks.service_resource import Stack

def get_resource() -> Stack:
    return session.resource("opsworks").Stack(...)
```


### Stack attributes


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
- `configuration_manager`: `Awaitable`[[StackConfigurationManagerResponseTypeDef](./type_defs.md#stackconfigurationmanagerresponsetypedef)]
- `chef_configuration`: `Awaitable`[[ChefConfigurationResponseTypeDef](./type_defs.md#chefconfigurationresponsetypedef)]
- `use_custom_cookbooks`: `Awaitable`[`bool`]
- `use_opsworks_security_groups`: `Awaitable`[`bool`]
- `custom_cookbooks_source`: `Awaitable`[[SourceResponseTypeDef](./type_defs.md#sourceresponsetypedef)]
- `default_ssh_key_name`: `Awaitable`[`str`]
- `created_at`: `Awaitable`[`str`]
- `default_root_device_type`: `Awaitable`[[RootDeviceTypeType](./literals.md#rootdevicetypetype)]
- `agent_version`: `Awaitable`[`str`]
- `id`: `str`
- `layers`: [StackLayersCollection](#stacklayerscollection)



### Stack collections


#### Stack.layers

Provides access to [Layer](#layer) resource.

Type annotations and code completion for `#!python session.resource("opsworks").Stack(...).layers` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.layers)

```python
# StackLayersCollection usage example

from types_aiobotocore_opsworks.service_resource import StackLayersCollection

def get_collection() -> StackLayersCollection:
    resource = session.resource("opsworks").Stack(...)
    return resource.layers
```




### Stack methods


#### Stack.Summary method

Creates a StackSummary resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").Summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.Summary)

```python
# Summary method definition

await def Summary(
    self,
) -> StackSummary:
    ...
```


#### Stack.create\_layer method

Creates a layer.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").create_layer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.create_layer)

```python
# create_layer method definition

await def create_layer(
    self,
    *,
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
) -> Layer:
    ...
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) 
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Stack.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Stack.load method

Calls :py:meth:`OpsWorks.Client.describe_stacks` to update the attributes of the
Stack resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Stack.reload method

Calls :py:meth:`OpsWorks.Client.describe_stacks` to update the attributes of the
Stack resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## StackSummary

Type annotations and code completion for `#!python session.resource("opsworks").StackSummary` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.StackSummary)

```python
# StackSummary usage example

from types_aiobotocore_opsworks.service_resource import StackSummary

def get_resource() -> StackSummary:
    return session.resource("opsworks").StackSummary(...)
```


### StackSummary attributes


- `name`: `Awaitable`[`str`]
- `arn`: `Awaitable`[`str`]
- `layers_count`: `Awaitable`[`int`]
- `apps_count`: `Awaitable`[`int`]
- `instances_count`: `Awaitable`[[InstancesCountResponseTypeDef](./type_defs.md#instancescountresponsetypedef)]
- `stack_id`: `str`





### StackSummary methods


#### StackSummary.Stack method

Creates a Stack resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").Stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.Stack)

```python
# Stack method definition

await def Stack(
    self,
) -> Stack:
    ...
```


#### StackSummary.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### StackSummary.load method

Calls :py:meth:`OpsWorks.Client.describe_stack_summary` to update the attributes
of the StackSummary resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### StackSummary.reload method

Calls :py:meth:`OpsWorks.Client.describe_stack_summary` to update the attributes
of the StackSummary resource.

Type annotations and code completion for `#!python aiobotocore.resource("opsworks").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```




