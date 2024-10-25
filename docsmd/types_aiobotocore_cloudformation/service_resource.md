# CloudFormationServiceResource

> [Index](../README.md) > [CloudFormation](./README.md) > CloudFormationServiceResource

!!! note ""

    Auto-generated documentation for [CloudFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
    type annotations stubs module [types-aiobotocore-cloudformation](https://pypi.org/project/types-aiobotocore-cloudformation/).

## CloudFormationServiceResource

Type annotations and code completion for `#!python session.resource("cloudformation")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource)

```python
# CloudFormationServiceResource usage example

from types_aiobotocore_cloudformation.service_resource import CloudFormationServiceResource

def get_cloudformation_resource() -> CloudFormationServiceResource:
    return session.resource("cloudformation")
```


## Attributes


- `meta`: `"CloudFormationResourceMeta"`

- `stacks`: `ServiceResourceStacksCollection`




## Collections

### ServiceResourceStacksCollection

Provides access to [Stack](#stack) resource.

Type annotations and code completion for `#!python session.resource("cloudformation").stacks` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.stacks)

```python
# ServiceResourceStacksCollection usage example

from types_aiobotocore_cloudformation.service_resource import ServiceResourceStacksCollection

def get_collection() -> ServiceResourceStacksCollection:
    return session.resource("cloudformation").stacks
```



## Methods

### CloudFormationServiceResource.Event method

Creates a Event resource.

Type annotations and code completion for `#!python session.resource("cloudformation").Event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Event)

```python
# Event method definition

await def Event(
    self,
    id: str,
) -> "_Event":
    ...
```


### CloudFormationServiceResource.Stack method

Creates a Stack resource.

Type annotations and code completion for `#!python session.resource("cloudformation").Stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Stack)

```python
# Stack method definition

await def Stack(
    self,
    name: str,
) -> "_Stack":
    ...
```


### CloudFormationServiceResource.StackResource method

Creates a StackResource resource.

Type annotations and code completion for `#!python session.resource("cloudformation").StackResource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResource)

```python
# StackResource method definition

await def StackResource(
    self,
    stack_name: str,
    logical_id: str,
) -> "_StackResource":
    ...
```


### CloudFormationServiceResource.StackResourceSummary method

Creates a StackResourceSummary resource.

Type annotations and code completion for `#!python session.resource("cloudformation").StackResourceSummary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResourceSummary)

```python
# StackResourceSummary method definition

await def StackResourceSummary(
    self,
    stack_name: str,
    logical_id: str,
) -> "_StackResourceSummary":
    ...
```


### CloudFormationServiceResource.create\_stack method

Creates a stack as specified in the template.

Type annotations and code completion for `#!python session.resource("cloudformation").create_stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.create_stack)

```python
# create_stack method definition

await def create_stack(
    self,
    *,
    StackName: str,
    TemplateBody: str = ...,
    TemplateURL: str = ...,
    Parameters: Sequence[ParameterTypeDef] = ...,  # (1)
    DisableRollback: bool = ...,
    RollbackConfiguration: RollbackConfigurationTypeDef = ...,  # (2)
    TimeoutInMinutes: int = ...,
    NotificationARNs: Sequence[str] = ...,
    Capabilities: Sequence[CapabilityType] = ...,  # (3)
    ResourceTypes: Sequence[str] = ...,
    RoleARN: str = ...,
    OnFailure: OnFailureType = ...,  # (4)
    StackPolicyBody: str = ...,
    StackPolicyURL: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    ClientRequestToken: str = ...,
    EnableTerminationProtection: bool = ...,
    RetainExceptOnCreate: bool = ...,
) -> "_Stack":
    ...
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: RollbackConfigurationTypeDef](./type_defs.md#rollbackconfigurationtypedef) 
3. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
4. See [:material-code-brackets: OnFailureType](./literals.md#onfailuretype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_stack method usage example with argument unpacking

kwargs: CreateStackInputServiceResourceCreateStackTypeDef = {  # (1)
    "StackName": ...,
}

parent.create_stack(**kwargs)
```

1. See [:material-code-braces: CreateStackInputServiceResourceCreateStackTypeDef](./type_defs.md#createstackinputserviceresourcecreatestacktypedef) 

### CloudFormationServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python session.resource("cloudformation").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```




## Event

Type annotations and code completion for `#!python session.resource("cloudformation").Event` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Event)

```python
# Event usage example

from types_aiobotocore_cloudformation.service_resource import Event

def get_resource() -> Event:
    return session.resource("cloudformation").Event(...)
```


### Event attributes


- `stack_id`: `Awaitable`[`str`]
- `event_id`: `Awaitable`[`str`]
- `stack_name`: `Awaitable`[`str`]
- `logical_resource_id`: `Awaitable`[`str`]
- `physical_resource_id`: `Awaitable`[`str`]
- `resource_type`: `Awaitable`[`str`]
- `timestamp`: `Awaitable`[`datetime`]
- `resource_status`: `Awaitable`[[ResourceStatusType](./literals.md#resourcestatustype)]
- `resource_status_reason`: `Awaitable`[`str`]
- `resource_properties`: `Awaitable`[`str`]
- `client_request_token`: `Awaitable`[`str`]
- `hook_type`: `Awaitable`[`str`]
- `hook_status`: `Awaitable`[[HookStatusType](./literals.md#hookstatustype)]
- `hook_status_reason`: `Awaitable`[`str`]
- `hook_invocation_point`: `Awaitable`[`Literal['PRE_PROVISION']` (see [HookInvocationPointType](./literals.md#hookinvocationpointtype))]
- `hook_failure_mode`: `Awaitable`[[HookFailureModeType](./literals.md#hookfailuremodetype)]
- `detailed_status`: `Awaitable`[[DetailedStatusType](./literals.md#detailedstatustype)]
- `id`: `str`
- `meta`: `"CloudFormationResourceMeta"`





### Event methods


#### Event.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Event.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```





## Stack

Type annotations and code completion for `#!python session.resource("cloudformation").Stack` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.Stack)

```python
# Stack usage example

from types_aiobotocore_cloudformation.service_resource import Stack

def get_resource() -> Stack:
    return session.resource("cloudformation").Stack(...)
```


### Stack attributes


- `stack_id`: `Awaitable`[`str`]
- `stack_name`: `Awaitable`[`str`]
- `change_set_id`: `Awaitable`[`str`]
- `description`: `Awaitable`[`str`]
- `parameters`: `Awaitable`[`List`[[ParameterTypeDef](./type_defs.md#parametertypedef)]]
- `creation_time`: `Awaitable`[`datetime`]
- `deletion_time`: `Awaitable`[`datetime`]
- `last_updated_time`: `Awaitable`[`datetime`]
- `rollback_configuration`: `Awaitable`[[RollbackConfigurationOutputTypeDef](./type_defs.md#rollbackconfigurationoutputtypedef)]
- `stack_status`: `Awaitable`[[StackStatusType](./literals.md#stackstatustype)]
- `stack_status_reason`: `Awaitable`[`str`]
- `disable_rollback`: `Awaitable`[`bool`]
- `notification_arns`: `Awaitable`[`List`[`str`]]
- `timeout_in_minutes`: `Awaitable`[`int`]
- `capabilities`: `Awaitable`[`List`[[CapabilityType](./literals.md#capabilitytype)]]
- `outputs`: `Awaitable`[`List`[[OutputTypeDef](./type_defs.md#outputtypedef)]]
- `role_arn`: `Awaitable`[`str`]
- `tags`: `Awaitable`[`List`[[TagTypeDef](./type_defs.md#tagtypedef)]]
- `enable_termination_protection`: `Awaitable`[`bool`]
- `parent_id`: `Awaitable`[`str`]
- `root_id`: `Awaitable`[`str`]
- `drift_information`: `Awaitable`[[StackDriftInformationTypeDef](./type_defs.md#stackdriftinformationtypedef)]
- `retain_except_on_create`: `Awaitable`[`bool`]
- `deletion_mode`: `Awaitable`[[DeletionModeType](./literals.md#deletionmodetype)]
- `detailed_status`: `Awaitable`[[DetailedStatusType](./literals.md#detailedstatustype)]
- `name`: `str`
- `events`: `StackEventsCollection`
- `resource_summaries`: `StackResourceSummariesCollection`
- `meta`: `"CloudFormationResourceMeta"`



### Stack collections


#### Stack.events

Provides access to [Event](#event) resource.

Type annotations and code completion for `#!python session.resource("cloudformation").Stack(...).events` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.events)

```python
# StackEventsCollection usage example

from types_aiobotocore_cloudformation.service_resource import StackEventsCollection

def get_collection() -> StackEventsCollection:
    resource = session.resource("cloudformation").Stack(...)
    return resource.events
```

#### Stack.resource_summaries

Provides access to [StackResourceSummary](#stackresourcesummary) resource.

Type annotations and code completion for `#!python session.resource("cloudformation").Stack(...).resource_summaries` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.resource_summaries)

```python
# StackResourceSummariesCollection usage example

from types_aiobotocore_cloudformation.service_resource import StackResourceSummariesCollection

def get_collection() -> StackResourceSummariesCollection:
    resource = session.resource("cloudformation").Stack(...)
    return resource.resource_summaries
```




### Stack methods


#### Stack.Resource method

Creates a StackResource resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").Resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.Resource)

```python
# Resource method definition

await def Resource(
    self,
    logical_id: str,
) -> "_StackResource":
    ...
```


#### Stack.cancel\_update method

Cancels an update on the specified stack.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").cancel_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.cancel_update)

```python
# cancel_update method definition

await def cancel_update(
    self,
    *,
    ClientRequestToken: str = ...,
) -> None:
    ...
```



```python
# cancel_update method usage example with argument unpacking

kwargs: CancelUpdateStackInputStackCancelUpdateTypeDef = {  # (1)
    "ClientRequestToken": ...,
}

parent.cancel_update(**kwargs)
```

1. See [:material-code-braces: CancelUpdateStackInputStackCancelUpdateTypeDef](./type_defs.md#cancelupdatestackinputstackcancelupdatetypedef) 

#### Stack.delete method

Deletes a specified stack.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.delete)

```python
# delete method definition

await def delete(
    self,
    *,
    RetainResources: Sequence[str] = ...,
    RoleARN: str = ...,
    ClientRequestToken: str = ...,
    DeletionMode: DeletionModeType = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: DeletionModeType](./literals.md#deletionmodetype) 


```python
# delete method usage example with argument unpacking

kwargs: DeleteStackInputStackDeleteTypeDef = {  # (1)
    "RetainResources": ...,
}

parent.delete(**kwargs)
```

1. See [:material-code-braces: DeleteStackInputStackDeleteTypeDef](./type_defs.md#deletestackinputstackdeletetypedef) 

#### Stack.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Stack.load method

Calls :py:meth:`CloudFormation.Client.describe_stacks` to update the attributes
of the Stack
resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Stack.reload method

Calls :py:meth:`CloudFormation.Client.describe_stacks` to update the attributes
of the Stack
resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### Stack.update method

Updates a stack as specified in the template.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.update)

```python
# update method definition

await def update(
    self,
    *,
    TemplateBody: str = ...,
    TemplateURL: str = ...,
    UsePreviousTemplate: bool = ...,
    StackPolicyDuringUpdateBody: str = ...,
    StackPolicyDuringUpdateURL: str = ...,
    Parameters: Sequence[ParameterTypeDef] = ...,  # (1)
    Capabilities: Sequence[CapabilityType] = ...,  # (2)
    ResourceTypes: Sequence[str] = ...,
    RoleARN: str = ...,
    RollbackConfiguration: RollbackConfigurationTypeDef = ...,  # (3)
    StackPolicyBody: str = ...,
    StackPolicyURL: str = ...,
    NotificationARNs: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    DisableRollback: bool = ...,
    ClientRequestToken: str = ...,
    RetainExceptOnCreate: bool = ...,
) -> UpdateStackOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
3. See [:material-code-braces: RollbackConfigurationTypeDef](./type_defs.md#rollbackconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: UpdateStackOutputTypeDef](./type_defs.md#updatestackoutputtypedef) 


```python
# update method usage example with argument unpacking

kwargs: UpdateStackInputStackUpdateTypeDef = {  # (1)
    "TemplateBody": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateStackInputStackUpdateTypeDef](./type_defs.md#updatestackinputstackupdatetypedef) 




## StackResource

Type annotations and code completion for `#!python session.resource("cloudformation").StackResource` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResource)

```python
# StackResource usage example

from types_aiobotocore_cloudformation.service_resource import StackResource

def get_resource() -> StackResource:
    return session.resource("cloudformation").StackResource(...)
```


### StackResource attributes


- `stack_id`: `Awaitable`[`str`]
- `logical_resource_id`: `Awaitable`[`str`]
- `physical_resource_id`: `Awaitable`[`str`]
- `resource_type`: `Awaitable`[`str`]
- `last_updated_timestamp`: `Awaitable`[`datetime`]
- `resource_status`: `Awaitable`[[ResourceStatusType](./literals.md#resourcestatustype)]
- `resource_status_reason`: `Awaitable`[`str`]
- `description`: `Awaitable`[`str`]
- `metadata`: `Awaitable`[`str`]
- `drift_information`: `Awaitable`[[StackResourceDriftInformationTypeDef](./type_defs.md#stackresourcedriftinformationtypedef)]
- `module_info`: `Awaitable`[[ModuleInfoTypeDef](./type_defs.md#moduleinfotypedef)]
- `stack_name`: `str`
- `logical_id`: `str`
- `meta`: `"CloudFormationResourceMeta"`





### StackResource methods


#### StackResource.Stack method

Creates a Stack resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").Stack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResource.Stack)

```python
# Stack method definition

await def Stack(
    self,
) -> "_Stack":
    ...
```


#### StackResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResource.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### StackResource.load method

Calls :py:meth:`CloudFormation.Client.describe_stack_resource` to update the
attributes of the StackResource
resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResource.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### StackResource.reload method

Calls :py:meth:`CloudFormation.Client.describe_stack_resource` to update the
attributes of the StackResource
resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResource.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## StackResourceSummary

Type annotations and code completion for `#!python session.resource("cloudformation").StackResourceSummary` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.StackResourceSummary)

```python
# StackResourceSummary usage example

from types_aiobotocore_cloudformation.service_resource import StackResourceSummary

def get_resource() -> StackResourceSummary:
    return session.resource("cloudformation").StackResourceSummary(...)
```


### StackResourceSummary attributes


- `logical_resource_id`: `Awaitable`[`str`]
- `physical_resource_id`: `Awaitable`[`str`]
- `resource_type`: `Awaitable`[`str`]
- `last_updated_timestamp`: `Awaitable`[`datetime`]
- `resource_status`: `Awaitable`[[ResourceStatusType](./literals.md#resourcestatustype)]
- `resource_status_reason`: `Awaitable`[`str`]
- `drift_information`: `Awaitable`[[StackResourceDriftInformationSummaryTypeDef](./type_defs.md#stackresourcedriftinformationsummarytypedef)]
- `module_info`: `Awaitable`[[ModuleInfoTypeDef](./type_defs.md#moduleinfotypedef)]
- `stack_name`: `str`
- `logical_id`: `str`
- `meta`: `"CloudFormationResourceMeta"`





### StackResourceSummary methods


#### StackResourceSummary.Resource method

Creates a StackResource resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").Resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResourceSummary.Resource)

```python
# Resource method definition

await def Resource(
    self,
) -> "_StackResource":
    ...
```


#### StackResourceSummary.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("cloudformation").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.StackResourceSummary.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```




