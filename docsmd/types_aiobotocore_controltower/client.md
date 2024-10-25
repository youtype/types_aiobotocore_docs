# ControlTowerClient

> [Index](../README.md) > [ControlTower](./README.md) > ControlTowerClient

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## ControlTowerClient

Type annotations and code completion for `#!python session.create_client("controltower")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client)

```python
# ControlTowerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_controltower.client import ControlTowerClient

session = get_session()
async with session.create_client("controltower") as client:
    client: ControlTowerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("controltower").exceptions` structure.

```python
# ControlTowerClient.exceptions usage example

async with session.create_client("controltower") as client:
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
# ControlTowerClient usage type checking example

from types_aiobotocore_controltower.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("controltower").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("controltower").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_landing\_zone

Creates a new landing zone.

Type annotations and code completion for `#!python session.create_client("controltower").create_landing_zone` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.create_landing_zone)

```python
# create_landing_zone method definition

await def create_landing_zone(
    self,
    *,
    manifest: Mapping[str, Any],
    version: str,
    tags: Mapping[str, str] = ...,
) -> CreateLandingZoneOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLandingZoneOutputTypeDef](./type_defs.md#createlandingzoneoutputtypedef) 


```python
# create_landing_zone method usage example with argument unpacking

kwargs: CreateLandingZoneInputRequestTypeDef = {  # (1)
    "manifest": ...,
    "version": ...,
}

parent.create_landing_zone(**kwargs)
```

1. See [:material-code-braces: CreateLandingZoneInputRequestTypeDef](./type_defs.md#createlandingzoneinputrequesttypedef) 

### delete\_landing\_zone

Decommissions a landing zone.

Type annotations and code completion for `#!python session.create_client("controltower").delete_landing_zone` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.delete_landing_zone)

```python
# delete_landing_zone method definition

await def delete_landing_zone(
    self,
    *,
    landingZoneIdentifier: str,
) -> DeleteLandingZoneOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteLandingZoneOutputTypeDef](./type_defs.md#deletelandingzoneoutputtypedef) 


```python
# delete_landing_zone method usage example with argument unpacking

kwargs: DeleteLandingZoneInputRequestTypeDef = {  # (1)
    "landingZoneIdentifier": ...,
}

parent.delete_landing_zone(**kwargs)
```

1. See [:material-code-braces: DeleteLandingZoneInputRequestTypeDef](./type_defs.md#deletelandingzoneinputrequesttypedef) 

### disable\_baseline

Disable an `EnabledBaseline` resource on the specified Target.

Type annotations and code completion for `#!python session.create_client("controltower").disable_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.disable_baseline)

```python
# disable_baseline method definition

await def disable_baseline(
    self,
    *,
    enabledBaselineIdentifier: str,
) -> DisableBaselineOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableBaselineOutputTypeDef](./type_defs.md#disablebaselineoutputtypedef) 


```python
# disable_baseline method usage example with argument unpacking

kwargs: DisableBaselineInputRequestTypeDef = {  # (1)
    "enabledBaselineIdentifier": ...,
}

parent.disable_baseline(**kwargs)
```

1. See [:material-code-braces: DisableBaselineInputRequestTypeDef](./type_defs.md#disablebaselineinputrequesttypedef) 

### disable\_control

This API call turns off a control.

Type annotations and code completion for `#!python session.create_client("controltower").disable_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.disable_control)

```python
# disable_control method definition

await def disable_control(
    self,
    *,
    controlIdentifier: str,
    targetIdentifier: str,
) -> DisableControlOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableControlOutputTypeDef](./type_defs.md#disablecontroloutputtypedef) 


```python
# disable_control method usage example with argument unpacking

kwargs: DisableControlInputRequestTypeDef = {  # (1)
    "controlIdentifier": ...,
    "targetIdentifier": ...,
}

parent.disable_control(**kwargs)
```

1. See [:material-code-braces: DisableControlInputRequestTypeDef](./type_defs.md#disablecontrolinputrequesttypedef) 

### enable\_baseline

Enable (apply) a `Baseline` to a Target.

Type annotations and code completion for `#!python session.create_client("controltower").enable_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.enable_baseline)

```python
# enable_baseline method definition

await def enable_baseline(
    self,
    *,
    baselineIdentifier: str,
    baselineVersion: str,
    targetIdentifier: str,
    parameters: Sequence[EnabledBaselineParameterTypeDef] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> EnableBaselineOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnabledBaselineParameterTypeDef](./type_defs.md#enabledbaselineparametertypedef) 
2. See [:material-code-braces: EnableBaselineOutputTypeDef](./type_defs.md#enablebaselineoutputtypedef) 


```python
# enable_baseline method usage example with argument unpacking

kwargs: EnableBaselineInputRequestTypeDef = {  # (1)
    "baselineIdentifier": ...,
    "baselineVersion": ...,
    "targetIdentifier": ...,
}

parent.enable_baseline(**kwargs)
```

1. See [:material-code-braces: EnableBaselineInputRequestTypeDef](./type_defs.md#enablebaselineinputrequesttypedef) 

### enable\_control

This API call activates a control.

Type annotations and code completion for `#!python session.create_client("controltower").enable_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.enable_control)

```python
# enable_control method definition

await def enable_control(
    self,
    *,
    controlIdentifier: str,
    targetIdentifier: str,
    parameters: Sequence[EnabledControlParameterTypeDef] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> EnableControlOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
2. See [:material-code-braces: EnableControlOutputTypeDef](./type_defs.md#enablecontroloutputtypedef) 


```python
# enable_control method usage example with argument unpacking

kwargs: EnableControlInputRequestTypeDef = {  # (1)
    "controlIdentifier": ...,
    "targetIdentifier": ...,
}

parent.enable_control(**kwargs)
```

1. See [:material-code-braces: EnableControlInputRequestTypeDef](./type_defs.md#enablecontrolinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("controltower").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.generate_presigned_url)

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


### get\_baseline

Retrieve details about an existing `Baseline` resource by specifying its
identifier.

Type annotations and code completion for `#!python session.create_client("controltower").get_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_baseline)

```python
# get_baseline method definition

await def get_baseline(
    self,
    *,
    baselineIdentifier: str,
) -> GetBaselineOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBaselineOutputTypeDef](./type_defs.md#getbaselineoutputtypedef) 


```python
# get_baseline method usage example with argument unpacking

kwargs: GetBaselineInputRequestTypeDef = {  # (1)
    "baselineIdentifier": ...,
}

parent.get_baseline(**kwargs)
```

1. See [:material-code-braces: GetBaselineInputRequestTypeDef](./type_defs.md#getbaselineinputrequesttypedef) 

### get\_baseline\_operation

Returns the details of an asynchronous baseline operation, as initiated by any
of these APIs: `EnableBaseline`, `DisableBaseline`, `UpdateEnabledBaseline`,
`ResetEnabledBaseline`.

Type annotations and code completion for `#!python session.create_client("controltower").get_baseline_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_baseline_operation)

```python
# get_baseline_operation method definition

await def get_baseline_operation(
    self,
    *,
    operationIdentifier: str,
) -> GetBaselineOperationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBaselineOperationOutputTypeDef](./type_defs.md#getbaselineoperationoutputtypedef) 


```python
# get_baseline_operation method usage example with argument unpacking

kwargs: GetBaselineOperationInputRequestTypeDef = {  # (1)
    "operationIdentifier": ...,
}

parent.get_baseline_operation(**kwargs)
```

1. See [:material-code-braces: GetBaselineOperationInputRequestTypeDef](./type_defs.md#getbaselineoperationinputrequesttypedef) 

### get\_control\_operation

Returns the status of a particular `EnableControl` or `DisableControl`
operation.

Type annotations and code completion for `#!python session.create_client("controltower").get_control_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_control_operation)

```python
# get_control_operation method definition

await def get_control_operation(
    self,
    *,
    operationIdentifier: str,
) -> GetControlOperationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetControlOperationOutputTypeDef](./type_defs.md#getcontroloperationoutputtypedef) 


```python
# get_control_operation method usage example with argument unpacking

kwargs: GetControlOperationInputRequestTypeDef = {  # (1)
    "operationIdentifier": ...,
}

parent.get_control_operation(**kwargs)
```

1. See [:material-code-braces: GetControlOperationInputRequestTypeDef](./type_defs.md#getcontroloperationinputrequesttypedef) 

### get\_enabled\_baseline

Retrieve details of an `EnabledBaseline` resource by specifying its identifier.

Type annotations and code completion for `#!python session.create_client("controltower").get_enabled_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_enabled_baseline)

```python
# get_enabled_baseline method definition

await def get_enabled_baseline(
    self,
    *,
    enabledBaselineIdentifier: str,
) -> GetEnabledBaselineOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnabledBaselineOutputTypeDef](./type_defs.md#getenabledbaselineoutputtypedef) 


```python
# get_enabled_baseline method usage example with argument unpacking

kwargs: GetEnabledBaselineInputRequestTypeDef = {  # (1)
    "enabledBaselineIdentifier": ...,
}

parent.get_enabled_baseline(**kwargs)
```

1. See [:material-code-braces: GetEnabledBaselineInputRequestTypeDef](./type_defs.md#getenabledbaselineinputrequesttypedef) 

### get\_enabled\_control

Retrieves details about an enabled control.

Type annotations and code completion for `#!python session.create_client("controltower").get_enabled_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_enabled_control)

```python
# get_enabled_control method definition

await def get_enabled_control(
    self,
    *,
    enabledControlIdentifier: str,
) -> GetEnabledControlOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnabledControlOutputTypeDef](./type_defs.md#getenabledcontroloutputtypedef) 


```python
# get_enabled_control method usage example with argument unpacking

kwargs: GetEnabledControlInputRequestTypeDef = {  # (1)
    "enabledControlIdentifier": ...,
}

parent.get_enabled_control(**kwargs)
```

1. See [:material-code-braces: GetEnabledControlInputRequestTypeDef](./type_defs.md#getenabledcontrolinputrequesttypedef) 

### get\_landing\_zone

Returns details about the landing zone.

Type annotations and code completion for `#!python session.create_client("controltower").get_landing_zone` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_landing_zone)

```python
# get_landing_zone method definition

await def get_landing_zone(
    self,
    *,
    landingZoneIdentifier: str,
) -> GetLandingZoneOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLandingZoneOutputTypeDef](./type_defs.md#getlandingzoneoutputtypedef) 


```python
# get_landing_zone method usage example with argument unpacking

kwargs: GetLandingZoneInputRequestTypeDef = {  # (1)
    "landingZoneIdentifier": ...,
}

parent.get_landing_zone(**kwargs)
```

1. See [:material-code-braces: GetLandingZoneInputRequestTypeDef](./type_defs.md#getlandingzoneinputrequesttypedef) 

### get\_landing\_zone\_operation

Returns the status of the specified landing zone operation.

Type annotations and code completion for `#!python session.create_client("controltower").get_landing_zone_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_landing_zone_operation)

```python
# get_landing_zone_operation method definition

await def get_landing_zone_operation(
    self,
    *,
    operationIdentifier: str,
) -> GetLandingZoneOperationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLandingZoneOperationOutputTypeDef](./type_defs.md#getlandingzoneoperationoutputtypedef) 


```python
# get_landing_zone_operation method usage example with argument unpacking

kwargs: GetLandingZoneOperationInputRequestTypeDef = {  # (1)
    "operationIdentifier": ...,
}

parent.get_landing_zone_operation(**kwargs)
```

1. See [:material-code-braces: GetLandingZoneOperationInputRequestTypeDef](./type_defs.md#getlandingzoneoperationinputrequesttypedef) 

### list\_baselines

Returns a summary list of all available baselines.

Type annotations and code completion for `#!python session.create_client("controltower").list_baselines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_baselines)

```python
# list_baselines method definition

await def list_baselines(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBaselinesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBaselinesOutputTypeDef](./type_defs.md#listbaselinesoutputtypedef) 


```python
# list_baselines method usage example with argument unpacking

kwargs: ListBaselinesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_baselines(**kwargs)
```

1. See [:material-code-braces: ListBaselinesInputRequestTypeDef](./type_defs.md#listbaselinesinputrequesttypedef) 

### list\_control\_operations

Provides a list of operations in progress or queued.

Type annotations and code completion for `#!python session.create_client("controltower").list_control_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_control_operations)

```python
# list_control_operations method definition

await def list_control_operations(
    self,
    *,
    filter: ControlOperationFilterTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListControlOperationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ControlOperationFilterTypeDef](./type_defs.md#controloperationfiltertypedef) 
2. See [:material-code-braces: ListControlOperationsOutputTypeDef](./type_defs.md#listcontroloperationsoutputtypedef) 


```python
# list_control_operations method usage example with argument unpacking

kwargs: ListControlOperationsInputRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.list_control_operations(**kwargs)
```

1. See [:material-code-braces: ListControlOperationsInputRequestTypeDef](./type_defs.md#listcontroloperationsinputrequesttypedef) 

### list\_enabled\_baselines

Returns a list of summaries describing `EnabledBaseline` resources.

Type annotations and code completion for `#!python session.create_client("controltower").list_enabled_baselines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_enabled_baselines)

```python
# list_enabled_baselines method definition

await def list_enabled_baselines(
    self,
    *,
    filter: EnabledBaselineFilterTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEnabledBaselinesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnabledBaselineFilterTypeDef](./type_defs.md#enabledbaselinefiltertypedef) 
2. See [:material-code-braces: ListEnabledBaselinesOutputTypeDef](./type_defs.md#listenabledbaselinesoutputtypedef) 


```python
# list_enabled_baselines method usage example with argument unpacking

kwargs: ListEnabledBaselinesInputRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.list_enabled_baselines(**kwargs)
```

1. See [:material-code-braces: ListEnabledBaselinesInputRequestTypeDef](./type_defs.md#listenabledbaselinesinputrequesttypedef) 

### list\_enabled\_controls

Lists the controls enabled by Amazon Web Services Control Tower on the
specified organizational unit and the accounts it
contains.

Type annotations and code completion for `#!python session.create_client("controltower").list_enabled_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_enabled_controls)

```python
# list_enabled_controls method definition

await def list_enabled_controls(
    self,
    *,
    filter: EnabledControlFilterTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    targetIdentifier: str = ...,
) -> ListEnabledControlsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnabledControlFilterTypeDef](./type_defs.md#enabledcontrolfiltertypedef) 
2. See [:material-code-braces: ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef) 


```python
# list_enabled_controls method usage example with argument unpacking

kwargs: ListEnabledControlsInputRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.list_enabled_controls(**kwargs)
```

1. See [:material-code-braces: ListEnabledControlsInputRequestTypeDef](./type_defs.md#listenabledcontrolsinputrequesttypedef) 

### list\_landing\_zone\_operations

Lists all landing zone operations from the past 90 days.

Type annotations and code completion for `#!python session.create_client("controltower").list_landing_zone_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_landing_zone_operations)

```python
# list_landing_zone_operations method definition

await def list_landing_zone_operations(
    self,
    *,
    filter: LandingZoneOperationFilterTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListLandingZoneOperationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LandingZoneOperationFilterTypeDef](./type_defs.md#landingzoneoperationfiltertypedef) 
2. See [:material-code-braces: ListLandingZoneOperationsOutputTypeDef](./type_defs.md#listlandingzoneoperationsoutputtypedef) 


```python
# list_landing_zone_operations method usage example with argument unpacking

kwargs: ListLandingZoneOperationsInputRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.list_landing_zone_operations(**kwargs)
```

1. See [:material-code-braces: ListLandingZoneOperationsInputRequestTypeDef](./type_defs.md#listlandingzoneoperationsinputrequesttypedef) 

### list\_landing\_zones

Returns the landing zone ARN for the landing zone deployed in your managed
account.

Type annotations and code completion for `#!python session.create_client("controltower").list_landing_zones` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_landing_zones)

```python
# list_landing_zones method definition

await def list_landing_zones(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListLandingZonesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLandingZonesOutputTypeDef](./type_defs.md#listlandingzonesoutputtypedef) 


```python
# list_landing_zones method usage example with argument unpacking

kwargs: ListLandingZonesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_landing_zones(**kwargs)
```

1. See [:material-code-braces: ListLandingZonesInputRequestTypeDef](./type_defs.md#listlandingzonesinputrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags associated with the resource.

Type annotations and code completion for `#!python session.create_client("controltower").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### reset\_enabled\_baseline

Re-enables an `EnabledBaseline` resource.

Type annotations and code completion for `#!python session.create_client("controltower").reset_enabled_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.reset_enabled_baseline)

```python
# reset_enabled_baseline method definition

await def reset_enabled_baseline(
    self,
    *,
    enabledBaselineIdentifier: str,
) -> ResetEnabledBaselineOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetEnabledBaselineOutputTypeDef](./type_defs.md#resetenabledbaselineoutputtypedef) 


```python
# reset_enabled_baseline method usage example with argument unpacking

kwargs: ResetEnabledBaselineInputRequestTypeDef = {  # (1)
    "enabledBaselineIdentifier": ...,
}

parent.reset_enabled_baseline(**kwargs)
```

1. See [:material-code-braces: ResetEnabledBaselineInputRequestTypeDef](./type_defs.md#resetenabledbaselineinputrequesttypedef) 

### reset\_landing\_zone

This API call resets a landing zone.

Type annotations and code completion for `#!python session.create_client("controltower").reset_landing_zone` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.reset_landing_zone)

```python
# reset_landing_zone method definition

await def reset_landing_zone(
    self,
    *,
    landingZoneIdentifier: str,
) -> ResetLandingZoneOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetLandingZoneOutputTypeDef](./type_defs.md#resetlandingzoneoutputtypedef) 


```python
# reset_landing_zone method usage example with argument unpacking

kwargs: ResetLandingZoneInputRequestTypeDef = {  # (1)
    "landingZoneIdentifier": ...,
}

parent.reset_landing_zone(**kwargs)
```

1. See [:material-code-braces: ResetLandingZoneInputRequestTypeDef](./type_defs.md#resetlandingzoneinputrequesttypedef) 

### tag\_resource

Applies tags to a resource.

Type annotations and code completion for `#!python session.create_client("controltower").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("controltower").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_enabled\_baseline

Updates an `EnabledBaseline` resource's applied parameters or version.

Type annotations and code completion for `#!python session.create_client("controltower").update_enabled_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.update_enabled_baseline)

```python
# update_enabled_baseline method definition

await def update_enabled_baseline(
    self,
    *,
    baselineVersion: str,
    enabledBaselineIdentifier: str,
    parameters: Sequence[EnabledBaselineParameterTypeDef] = ...,  # (1)
) -> UpdateEnabledBaselineOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnabledBaselineParameterTypeDef](./type_defs.md#enabledbaselineparametertypedef) 
2. See [:material-code-braces: UpdateEnabledBaselineOutputTypeDef](./type_defs.md#updateenabledbaselineoutputtypedef) 


```python
# update_enabled_baseline method usage example with argument unpacking

kwargs: UpdateEnabledBaselineInputRequestTypeDef = {  # (1)
    "baselineVersion": ...,
    "enabledBaselineIdentifier": ...,
}

parent.update_enabled_baseline(**kwargs)
```

1. See [:material-code-braces: UpdateEnabledBaselineInputRequestTypeDef](./type_defs.md#updateenabledbaselineinputrequesttypedef) 

### update\_enabled\_control

Updates the configuration of an already enabled control.

Type annotations and code completion for `#!python session.create_client("controltower").update_enabled_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.update_enabled_control)

```python
# update_enabled_control method definition

await def update_enabled_control(
    self,
    *,
    enabledControlIdentifier: str,
    parameters: Sequence[EnabledControlParameterTypeDef],  # (1)
) -> UpdateEnabledControlOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
2. See [:material-code-braces: UpdateEnabledControlOutputTypeDef](./type_defs.md#updateenabledcontroloutputtypedef) 


```python
# update_enabled_control method usage example with argument unpacking

kwargs: UpdateEnabledControlInputRequestTypeDef = {  # (1)
    "enabledControlIdentifier": ...,
    "parameters": ...,
}

parent.update_enabled_control(**kwargs)
```

1. See [:material-code-braces: UpdateEnabledControlInputRequestTypeDef](./type_defs.md#updateenabledcontrolinputrequesttypedef) 

### update\_landing\_zone

This API call updates the landing zone.

Type annotations and code completion for `#!python session.create_client("controltower").update_landing_zone` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.update_landing_zone)

```python
# update_landing_zone method definition

await def update_landing_zone(
    self,
    *,
    landingZoneIdentifier: str,
    manifest: Mapping[str, Any],
    version: str,
) -> UpdateLandingZoneOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateLandingZoneOutputTypeDef](./type_defs.md#updatelandingzoneoutputtypedef) 


```python
# update_landing_zone method usage example with argument unpacking

kwargs: UpdateLandingZoneInputRequestTypeDef = {  # (1)
    "landingZoneIdentifier": ...,
    "manifest": ...,
    "version": ...,
}

parent.update_landing_zone(**kwargs)
```

1. See [:material-code-braces: UpdateLandingZoneInputRequestTypeDef](./type_defs.md#updatelandingzoneinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("controltower").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ControlTowerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("controltower").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator` method with overloads.

- `client.get_paginator("list_baselines")` -> [ListBaselinesPaginator](./paginators.md#listbaselinespaginator)
- `client.get_paginator("list_control_operations")` -> [ListControlOperationsPaginator](./paginators.md#listcontroloperationspaginator)
- `client.get_paginator("list_enabled_baselines")` -> [ListEnabledBaselinesPaginator](./paginators.md#listenabledbaselinespaginator)
- `client.get_paginator("list_enabled_controls")` -> [ListEnabledControlsPaginator](./paginators.md#listenabledcontrolspaginator)
- `client.get_paginator("list_landing_zone_operations")` -> [ListLandingZoneOperationsPaginator](./paginators.md#listlandingzoneoperationspaginator)
- `client.get_paginator("list_landing_zones")` -> [ListLandingZonesPaginator](./paginators.md#listlandingzonespaginator)



