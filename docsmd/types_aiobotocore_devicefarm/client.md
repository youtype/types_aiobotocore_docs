# DeviceFarmClient

> [Index](../README.md) > [DeviceFarm](./README.md) > DeviceFarmClient

!!! note ""

    Auto-generated documentation for [DeviceFarm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#devicefarm)
    type annotations stubs module [types-aiobotocore-devicefarm](https://pypi.org/project/types-aiobotocore-devicefarm/).

## DeviceFarmClient

Type annotations and code completion for `#!python session.create_client("devicefarm")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client)

```python
# DeviceFarmClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_devicefarm.client import DeviceFarmClient

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("devicefarm").exceptions` structure.

```python
# DeviceFarmClient.exceptions usage example

async with session.create_client("devicefarm") as client:
    try:
        do_something(client)
    except (
            client.ArgumentException,
        client.CannotDeleteException,
        client.ClientError,
        client.IdempotencyException,
        client.InternalServiceException,
        client.InvalidOperationException,
        client.LimitExceededException,
        client.NotEligibleException,
        client.NotFoundException,
        client.ServiceAccountException,
        client.TagOperationException,
        client.TagPolicyException,
        client.TooManyTagsException,
    ) as e:
        print(e)
```

```python
# DeviceFarmClient usage type checking example

from types_aiobotocore_devicefarm.client import Exceptions

def handle_error(exc: Exceptions.ArgumentException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("devicefarm").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("devicefarm").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/generate_presigned_url.html)

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


### create\_device\_pool

Creates a device pool.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_device_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_device_pool.html)

```python
# create_device_pool method definition

await def create_device_pool(
    self,
    *,
    projectArn: str,
    name: str,
    rules: Sequence[RuleTypeDef],  # (1)
    description: str = ...,
    maxDevices: int = ...,
) -> CreateDevicePoolResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: CreateDevicePoolResultTypeDef](./type_defs.md#createdevicepoolresulttypedef) 


```python
# create_device_pool method usage example with argument unpacking

kwargs: CreateDevicePoolRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
    "name": ...,
    "rules": ...,
}

parent.create_device_pool(**kwargs)
```

1. See [:material-code-braces: CreateDevicePoolRequestRequestTypeDef](./type_defs.md#createdevicepoolrequestrequesttypedef) 

### create\_instance\_profile

Creates a profile that can be applied to one or more private fleet device
instances.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_instance_profile.html)

```python
# create_instance_profile method definition

await def create_instance_profile(
    self,
    *,
    name: str,
    description: str = ...,
    packageCleanup: bool = ...,
    excludeAppPackagesFromCleanup: Sequence[str] = ...,
    rebootAfterUse: bool = ...,
) -> CreateInstanceProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateInstanceProfileResultTypeDef](./type_defs.md#createinstanceprofileresulttypedef) 


```python
# create_instance_profile method usage example with argument unpacking

kwargs: CreateInstanceProfileRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_instance_profile(**kwargs)
```

1. See [:material-code-braces: CreateInstanceProfileRequestRequestTypeDef](./type_defs.md#createinstanceprofilerequestrequesttypedef) 

### create\_network\_profile

Creates a network profile.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_network_profile.html)

```python
# create_network_profile method definition

await def create_network_profile(
    self,
    *,
    projectArn: str,
    name: str,
    description: str = ...,
    type: NetworkProfileTypeType = ...,  # (1)
    uplinkBandwidthBits: int = ...,
    downlinkBandwidthBits: int = ...,
    uplinkDelayMs: int = ...,
    downlinkDelayMs: int = ...,
    uplinkJitterMs: int = ...,
    downlinkJitterMs: int = ...,
    uplinkLossPercent: int = ...,
    downlinkLossPercent: int = ...,
) -> CreateNetworkProfileResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
2. See [:material-code-braces: CreateNetworkProfileResultTypeDef](./type_defs.md#createnetworkprofileresulttypedef) 


```python
# create_network_profile method usage example with argument unpacking

kwargs: CreateNetworkProfileRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
    "name": ...,
}

parent.create_network_profile(**kwargs)
```

1. See [:material-code-braces: CreateNetworkProfileRequestRequestTypeDef](./type_defs.md#createnetworkprofilerequestrequesttypedef) 

### create\_project

Creates a project.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_project.html)

```python
# create_project method definition

await def create_project(
    self,
    *,
    name: str,
    defaultJobTimeoutMinutes: int = ...,
    vpcConfig: VpcConfigTypeDef = ...,  # (1)
) -> CreateProjectResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: CreateProjectResultTypeDef](./type_defs.md#createprojectresulttypedef) 


```python
# create_project method usage example with argument unpacking

kwargs: CreateProjectRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_project(**kwargs)
```

1. See [:material-code-braces: CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef) 

### create\_remote\_access\_session

Specifies and starts a remote access session.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_remote_access_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_remote_access_session.html)

```python
# create_remote_access_session method definition

await def create_remote_access_session(
    self,
    *,
    projectArn: str,
    deviceArn: str,
    instanceArn: str = ...,
    sshPublicKey: str = ...,
    remoteDebugEnabled: bool = ...,
    remoteRecordEnabled: bool = ...,
    remoteRecordAppArn: str = ...,
    name: str = ...,
    clientId: str = ...,
    configuration: CreateRemoteAccessSessionConfigurationTypeDef = ...,  # (1)
    interactionMode: InteractionModeType = ...,  # (2)
    skipAppResign: bool = ...,
) -> CreateRemoteAccessSessionResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CreateRemoteAccessSessionConfigurationTypeDef](./type_defs.md#createremoteaccesssessionconfigurationtypedef) 
2. See [:material-code-brackets: InteractionModeType](./literals.md#interactionmodetype) 
3. See [:material-code-braces: CreateRemoteAccessSessionResultTypeDef](./type_defs.md#createremoteaccesssessionresulttypedef) 


```python
# create_remote_access_session method usage example with argument unpacking

kwargs: CreateRemoteAccessSessionRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
    "deviceArn": ...,
}

parent.create_remote_access_session(**kwargs)
```

1. See [:material-code-braces: CreateRemoteAccessSessionRequestRequestTypeDef](./type_defs.md#createremoteaccesssessionrequestrequesttypedef) 

### create\_test\_grid\_project

Creates a Selenium testing project.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_test_grid_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_test_grid_project.html)

```python
# create_test_grid_project method definition

await def create_test_grid_project(
    self,
    *,
    name: str,
    description: str = ...,
    vpcConfig: TestGridVpcConfigTypeDef = ...,  # (1)
) -> CreateTestGridProjectResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TestGridVpcConfigTypeDef](./type_defs.md#testgridvpcconfigtypedef) 
2. See [:material-code-braces: CreateTestGridProjectResultTypeDef](./type_defs.md#createtestgridprojectresulttypedef) 


```python
# create_test_grid_project method usage example with argument unpacking

kwargs: CreateTestGridProjectRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_test_grid_project(**kwargs)
```

1. See [:material-code-braces: CreateTestGridProjectRequestRequestTypeDef](./type_defs.md#createtestgridprojectrequestrequesttypedef) 

### create\_test\_grid\_url

Creates a signed, short-term URL that can be passed to a Selenium
<code>RemoteWebDriver</code> constructor.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_test_grid_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_test_grid_url.html)

```python
# create_test_grid_url method definition

await def create_test_grid_url(
    self,
    *,
    projectArn: str,
    expiresInSeconds: int,
) -> CreateTestGridUrlResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateTestGridUrlResultTypeDef](./type_defs.md#createtestgridurlresulttypedef) 


```python
# create_test_grid_url method usage example with argument unpacking

kwargs: CreateTestGridUrlRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
    "expiresInSeconds": ...,
}

parent.create_test_grid_url(**kwargs)
```

1. See [:material-code-braces: CreateTestGridUrlRequestRequestTypeDef](./type_defs.md#createtestgridurlrequestrequesttypedef) 

### create\_upload

Uploads an app or test scripts.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_upload.html)

```python
# create_upload method definition

await def create_upload(
    self,
    *,
    projectArn: str,
    name: str,
    type: UploadTypeType,  # (1)
    contentType: str = ...,
) -> CreateUploadResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype) 
2. See [:material-code-braces: CreateUploadResultTypeDef](./type_defs.md#createuploadresulttypedef) 


```python
# create_upload method usage example with argument unpacking

kwargs: CreateUploadRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
    "name": ...,
    "type": ...,
}

parent.create_upload(**kwargs)
```

1. See [:material-code-braces: CreateUploadRequestRequestTypeDef](./type_defs.md#createuploadrequestrequesttypedef) 

### create\_vpce\_configuration

Creates a configuration record in Device Farm for your Amazon Virtual Private
Cloud (VPC) endpoint.

Type annotations and code completion for `#!python session.create_client("devicefarm").create_vpce_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/create_vpce_configuration.html)

```python
# create_vpce_configuration method definition

await def create_vpce_configuration(
    self,
    *,
    vpceConfigurationName: str,
    vpceServiceName: str,
    serviceDnsName: str,
    vpceConfigurationDescription: str = ...,
) -> CreateVPCEConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateVPCEConfigurationResultTypeDef](./type_defs.md#createvpceconfigurationresulttypedef) 


```python
# create_vpce_configuration method usage example with argument unpacking

kwargs: CreateVPCEConfigurationRequestRequestTypeDef = {  # (1)
    "vpceConfigurationName": ...,
    "vpceServiceName": ...,
    "serviceDnsName": ...,
}

parent.create_vpce_configuration(**kwargs)
```

1. See [:material-code-braces: CreateVPCEConfigurationRequestRequestTypeDef](./type_defs.md#createvpceconfigurationrequestrequesttypedef) 

### delete\_device\_pool

Deletes a device pool given the pool ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_device_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_device_pool.html)

```python
# delete_device_pool method definition

await def delete_device_pool(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_device_pool method usage example with argument unpacking

kwargs: DeleteDevicePoolRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_device_pool(**kwargs)
```

1. See [:material-code-braces: DeleteDevicePoolRequestRequestTypeDef](./type_defs.md#deletedevicepoolrequestrequesttypedef) 

### delete\_instance\_profile

Deletes a profile that can be applied to one or more private device instances.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_instance_profile.html)

```python
# delete_instance_profile method definition

await def delete_instance_profile(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_instance_profile method usage example with argument unpacking

kwargs: DeleteInstanceProfileRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_instance_profile(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceProfileRequestRequestTypeDef](./type_defs.md#deleteinstanceprofilerequestrequesttypedef) 

### delete\_network\_profile

Deletes a network profile.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_network_profile.html)

```python
# delete_network_profile method definition

await def delete_network_profile(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_network_profile method usage example with argument unpacking

kwargs: DeleteNetworkProfileRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_network_profile(**kwargs)
```

1. See [:material-code-braces: DeleteNetworkProfileRequestRequestTypeDef](./type_defs.md#deletenetworkprofilerequestrequesttypedef) 

### delete\_project

Deletes an AWS Device Farm project, given the project ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_project.html)

```python
# delete_project method definition

await def delete_project(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_project method usage example with argument unpacking

kwargs: DeleteProjectRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_project(**kwargs)
```

1. See [:material-code-braces: DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef) 

### delete\_remote\_access\_session

Deletes a completed remote access session and its results.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_remote_access_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_remote_access_session.html)

```python
# delete_remote_access_session method definition

await def delete_remote_access_session(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_remote_access_session method usage example with argument unpacking

kwargs: DeleteRemoteAccessSessionRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_remote_access_session(**kwargs)
```

1. See [:material-code-braces: DeleteRemoteAccessSessionRequestRequestTypeDef](./type_defs.md#deleteremoteaccesssessionrequestrequesttypedef) 

### delete\_run

Deletes the run, given the run ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_run.html)

```python
# delete_run method definition

await def delete_run(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_run method usage example with argument unpacking

kwargs: DeleteRunRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_run(**kwargs)
```

1. See [:material-code-braces: DeleteRunRequestRequestTypeDef](./type_defs.md#deleterunrequestrequesttypedef) 

### delete\_test\_grid\_project

Deletes a Selenium testing project and all content generated under it.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_test_grid_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_test_grid_project.html)

```python
# delete_test_grid_project method definition

await def delete_test_grid_project(
    self,
    *,
    projectArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_test_grid_project method usage example with argument unpacking

kwargs: DeleteTestGridProjectRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
}

parent.delete_test_grid_project(**kwargs)
```

1. See [:material-code-braces: DeleteTestGridProjectRequestRequestTypeDef](./type_defs.md#deletetestgridprojectrequestrequesttypedef) 

### delete\_upload

Deletes an upload given the upload ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_upload.html)

```python
# delete_upload method definition

await def delete_upload(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_upload method usage example with argument unpacking

kwargs: DeleteUploadRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_upload(**kwargs)
```

1. See [:material-code-braces: DeleteUploadRequestRequestTypeDef](./type_defs.md#deleteuploadrequestrequesttypedef) 

### delete\_vpce\_configuration

Deletes a configuration for your Amazon Virtual Private Cloud (VPC) endpoint.

Type annotations and code completion for `#!python session.create_client("devicefarm").delete_vpce_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/delete_vpce_configuration.html)

```python
# delete_vpce_configuration method definition

await def delete_vpce_configuration(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_vpce_configuration method usage example with argument unpacking

kwargs: DeleteVPCEConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_vpce_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteVPCEConfigurationRequestRequestTypeDef](./type_defs.md#deletevpceconfigurationrequestrequesttypedef) 

### get\_account\_settings

Returns the number of unmetered iOS or unmetered Android devices that have been
purchased by the account.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_account_settings.html)

```python
# get_account_settings method definition

await def get_account_settings(
    self,
) -> GetAccountSettingsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountSettingsResultTypeDef](./type_defs.md#getaccountsettingsresulttypedef) 

### get\_device

Gets information about a unique device type.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_device.html)

```python
# get_device method definition

await def get_device(
    self,
    *,
    arn: str,
) -> GetDeviceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceResultTypeDef](./type_defs.md#getdeviceresulttypedef) 


```python
# get_device method usage example with argument unpacking

kwargs: GetDeviceRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_device(**kwargs)
```

1. See [:material-code-braces: GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef) 

### get\_device\_instance

Returns information about a device instance that belongs to a private device
fleet.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_device_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_device_instance.html)

```python
# get_device_instance method definition

await def get_device_instance(
    self,
    *,
    arn: str,
) -> GetDeviceInstanceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceInstanceResultTypeDef](./type_defs.md#getdeviceinstanceresulttypedef) 


```python
# get_device_instance method usage example with argument unpacking

kwargs: GetDeviceInstanceRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_device_instance(**kwargs)
```

1. See [:material-code-braces: GetDeviceInstanceRequestRequestTypeDef](./type_defs.md#getdeviceinstancerequestrequesttypedef) 

### get\_device\_pool

Gets information about a device pool.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_device_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_device_pool.html)

```python
# get_device_pool method definition

await def get_device_pool(
    self,
    *,
    arn: str,
) -> GetDevicePoolResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDevicePoolResultTypeDef](./type_defs.md#getdevicepoolresulttypedef) 


```python
# get_device_pool method usage example with argument unpacking

kwargs: GetDevicePoolRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_device_pool(**kwargs)
```

1. See [:material-code-braces: GetDevicePoolRequestRequestTypeDef](./type_defs.md#getdevicepoolrequestrequesttypedef) 

### get\_device\_pool\_compatibility

Gets information about compatibility with a device pool.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_device_pool_compatibility` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_device_pool_compatibility.html)

```python
# get_device_pool_compatibility method definition

await def get_device_pool_compatibility(
    self,
    *,
    devicePoolArn: str,
    appArn: str = ...,
    testType: TestTypeType = ...,  # (1)
    test: ScheduleRunTestTypeDef = ...,  # (2)
    configuration: ScheduleRunConfigurationTypeDef = ...,  # (3)
) -> GetDevicePoolCompatibilityResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
2. See [:material-code-braces: ScheduleRunTestTypeDef](./type_defs.md#scheduleruntesttypedef) 
3. See [:material-code-braces: ScheduleRunConfigurationTypeDef](./type_defs.md#schedulerunconfigurationtypedef) 
4. See [:material-code-braces: GetDevicePoolCompatibilityResultTypeDef](./type_defs.md#getdevicepoolcompatibilityresulttypedef) 


```python
# get_device_pool_compatibility method usage example with argument unpacking

kwargs: GetDevicePoolCompatibilityRequestRequestTypeDef = {  # (1)
    "devicePoolArn": ...,
}

parent.get_device_pool_compatibility(**kwargs)
```

1. See [:material-code-braces: GetDevicePoolCompatibilityRequestRequestTypeDef](./type_defs.md#getdevicepoolcompatibilityrequestrequesttypedef) 

### get\_instance\_profile

Returns information about the specified instance profile.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_instance_profile.html)

```python
# get_instance_profile method definition

await def get_instance_profile(
    self,
    *,
    arn: str,
) -> GetInstanceProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInstanceProfileResultTypeDef](./type_defs.md#getinstanceprofileresulttypedef) 


```python
# get_instance_profile method usage example with argument unpacking

kwargs: GetInstanceProfileRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_instance_profile(**kwargs)
```

1. See [:material-code-braces: GetInstanceProfileRequestRequestTypeDef](./type_defs.md#getinstanceprofilerequestrequesttypedef) 

### get\_job

Gets information about a job.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_job.html)

```python
# get_job method definition

await def get_job(
    self,
    *,
    arn: str,
) -> GetJobResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobResultTypeDef](./type_defs.md#getjobresulttypedef) 


```python
# get_job method usage example with argument unpacking

kwargs: GetJobRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_job(**kwargs)
```

1. See [:material-code-braces: GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef) 

### get\_network\_profile

Returns information about a network profile.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_network_profile.html)

```python
# get_network_profile method definition

await def get_network_profile(
    self,
    *,
    arn: str,
) -> GetNetworkProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNetworkProfileResultTypeDef](./type_defs.md#getnetworkprofileresulttypedef) 


```python
# get_network_profile method usage example with argument unpacking

kwargs: GetNetworkProfileRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_network_profile(**kwargs)
```

1. See [:material-code-braces: GetNetworkProfileRequestRequestTypeDef](./type_defs.md#getnetworkprofilerequestrequesttypedef) 

### get\_offering\_status

Gets the current status and future status of all offerings purchased by an AWS
account.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_offering_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_offering_status.html)

```python
# get_offering_status method definition

await def get_offering_status(
    self,
    *,
    nextToken: str = ...,
) -> GetOfferingStatusResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOfferingStatusResultTypeDef](./type_defs.md#getofferingstatusresulttypedef) 


```python
# get_offering_status method usage example with argument unpacking

kwargs: GetOfferingStatusRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.get_offering_status(**kwargs)
```

1. See [:material-code-braces: GetOfferingStatusRequestRequestTypeDef](./type_defs.md#getofferingstatusrequestrequesttypedef) 

### get\_project

Gets information about a project.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_project.html)

```python
# get_project method definition

await def get_project(
    self,
    *,
    arn: str,
) -> GetProjectResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProjectResultTypeDef](./type_defs.md#getprojectresulttypedef) 


```python
# get_project method usage example with argument unpacking

kwargs: GetProjectRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_project(**kwargs)
```

1. See [:material-code-braces: GetProjectRequestRequestTypeDef](./type_defs.md#getprojectrequestrequesttypedef) 

### get\_remote\_access\_session

Returns a link to a currently running remote access session.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_remote_access_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_remote_access_session.html)

```python
# get_remote_access_session method definition

await def get_remote_access_session(
    self,
    *,
    arn: str,
) -> GetRemoteAccessSessionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRemoteAccessSessionResultTypeDef](./type_defs.md#getremoteaccesssessionresulttypedef) 


```python
# get_remote_access_session method usage example with argument unpacking

kwargs: GetRemoteAccessSessionRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_remote_access_session(**kwargs)
```

1. See [:material-code-braces: GetRemoteAccessSessionRequestRequestTypeDef](./type_defs.md#getremoteaccesssessionrequestrequesttypedef) 

### get\_run

Gets information about a run.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_run.html)

```python
# get_run method definition

await def get_run(
    self,
    *,
    arn: str,
) -> GetRunResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRunResultTypeDef](./type_defs.md#getrunresulttypedef) 


```python
# get_run method usage example with argument unpacking

kwargs: GetRunRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_run(**kwargs)
```

1. See [:material-code-braces: GetRunRequestRequestTypeDef](./type_defs.md#getrunrequestrequesttypedef) 

### get\_suite

Gets information about a suite.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_suite` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_suite.html)

```python
# get_suite method definition

await def get_suite(
    self,
    *,
    arn: str,
) -> GetSuiteResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSuiteResultTypeDef](./type_defs.md#getsuiteresulttypedef) 


```python
# get_suite method usage example with argument unpacking

kwargs: GetSuiteRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_suite(**kwargs)
```

1. See [:material-code-braces: GetSuiteRequestRequestTypeDef](./type_defs.md#getsuiterequestrequesttypedef) 

### get\_test

Gets information about a test.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_test` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_test.html)

```python
# get_test method definition

await def get_test(
    self,
    *,
    arn: str,
) -> GetTestResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestResultTypeDef](./type_defs.md#gettestresulttypedef) 


```python
# get_test method usage example with argument unpacking

kwargs: GetTestRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_test(**kwargs)
```

1. See [:material-code-braces: GetTestRequestRequestTypeDef](./type_defs.md#gettestrequestrequesttypedef) 

### get\_test\_grid\_project

Retrieves information about a Selenium testing project.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_test_grid_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_test_grid_project.html)

```python
# get_test_grid_project method definition

await def get_test_grid_project(
    self,
    *,
    projectArn: str,
) -> GetTestGridProjectResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestGridProjectResultTypeDef](./type_defs.md#gettestgridprojectresulttypedef) 


```python
# get_test_grid_project method usage example with argument unpacking

kwargs: GetTestGridProjectRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
}

parent.get_test_grid_project(**kwargs)
```

1. See [:material-code-braces: GetTestGridProjectRequestRequestTypeDef](./type_defs.md#gettestgridprojectrequestrequesttypedef) 

### get\_test\_grid\_session

A session is an instance of a browser created through a
<code>RemoteWebDriver</code> with the URL from
<a>CreateTestGridUrlResult$url</a>.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_test_grid_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_test_grid_session.html)

```python
# get_test_grid_session method definition

await def get_test_grid_session(
    self,
    *,
    projectArn: str = ...,
    sessionId: str = ...,
    sessionArn: str = ...,
) -> GetTestGridSessionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestGridSessionResultTypeDef](./type_defs.md#gettestgridsessionresulttypedef) 


```python
# get_test_grid_session method usage example with argument unpacking

kwargs: GetTestGridSessionRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
}

parent.get_test_grid_session(**kwargs)
```

1. See [:material-code-braces: GetTestGridSessionRequestRequestTypeDef](./type_defs.md#gettestgridsessionrequestrequesttypedef) 

### get\_upload

Gets information about an upload.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_upload.html)

```python
# get_upload method definition

await def get_upload(
    self,
    *,
    arn: str,
) -> GetUploadResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUploadResultTypeDef](./type_defs.md#getuploadresulttypedef) 


```python
# get_upload method usage example with argument unpacking

kwargs: GetUploadRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_upload(**kwargs)
```

1. See [:material-code-braces: GetUploadRequestRequestTypeDef](./type_defs.md#getuploadrequestrequesttypedef) 

### get\_vpce\_configuration

Returns information about the configuration settings for your Amazon Virtual
Private Cloud (VPC) endpoint.

Type annotations and code completion for `#!python session.create_client("devicefarm").get_vpce_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/get_vpce_configuration.html)

```python
# get_vpce_configuration method definition

await def get_vpce_configuration(
    self,
    *,
    arn: str,
) -> GetVPCEConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVPCEConfigurationResultTypeDef](./type_defs.md#getvpceconfigurationresulttypedef) 


```python
# get_vpce_configuration method usage example with argument unpacking

kwargs: GetVPCEConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_vpce_configuration(**kwargs)
```

1. See [:material-code-braces: GetVPCEConfigurationRequestRequestTypeDef](./type_defs.md#getvpceconfigurationrequestrequesttypedef) 

### install\_to\_remote\_access\_session

Installs an application to the device in a remote access session.

Type annotations and code completion for `#!python session.create_client("devicefarm").install_to_remote_access_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/install_to_remote_access_session.html)

```python
# install_to_remote_access_session method definition

await def install_to_remote_access_session(
    self,
    *,
    remoteAccessSessionArn: str,
    appArn: str,
) -> InstallToRemoteAccessSessionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InstallToRemoteAccessSessionResultTypeDef](./type_defs.md#installtoremoteaccesssessionresulttypedef) 


```python
# install_to_remote_access_session method usage example with argument unpacking

kwargs: InstallToRemoteAccessSessionRequestRequestTypeDef = {  # (1)
    "remoteAccessSessionArn": ...,
    "appArn": ...,
}

parent.install_to_remote_access_session(**kwargs)
```

1. See [:material-code-braces: InstallToRemoteAccessSessionRequestRequestTypeDef](./type_defs.md#installtoremoteaccesssessionrequestrequesttypedef) 

### list\_artifacts

Gets information about artifacts.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_artifacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_artifacts.html)

```python
# list_artifacts method definition

await def list_artifacts(
    self,
    *,
    arn: str,
    type: ArtifactCategoryType,  # (1)
    nextToken: str = ...,
) -> ListArtifactsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ArtifactCategoryType](./literals.md#artifactcategorytype) 
2. See [:material-code-braces: ListArtifactsResultTypeDef](./type_defs.md#listartifactsresulttypedef) 


```python
# list_artifacts method usage example with argument unpacking

kwargs: ListArtifactsRequestRequestTypeDef = {  # (1)
    "arn": ...,
    "type": ...,
}

parent.list_artifacts(**kwargs)
```

1. See [:material-code-braces: ListArtifactsRequestRequestTypeDef](./type_defs.md#listartifactsrequestrequesttypedef) 

### list\_device\_instances

Returns information about the private device instances associated with one or
more AWS accounts.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_device_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_device_instances.html)

```python
# list_device_instances method definition

await def list_device_instances(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDeviceInstancesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeviceInstancesResultTypeDef](./type_defs.md#listdeviceinstancesresulttypedef) 


```python
# list_device_instances method usage example with argument unpacking

kwargs: ListDeviceInstancesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_device_instances(**kwargs)
```

1. See [:material-code-braces: ListDeviceInstancesRequestRequestTypeDef](./type_defs.md#listdeviceinstancesrequestrequesttypedef) 

### list\_device\_pools

Gets information about device pools.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_device_pools` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_device_pools.html)

```python
# list_device_pools method definition

await def list_device_pools(
    self,
    *,
    arn: str,
    type: DevicePoolTypeType = ...,  # (1)
    nextToken: str = ...,
) -> ListDevicePoolsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DevicePoolTypeType](./literals.md#devicepooltypetype) 
2. See [:material-code-braces: ListDevicePoolsResultTypeDef](./type_defs.md#listdevicepoolsresulttypedef) 


```python
# list_device_pools method usage example with argument unpacking

kwargs: ListDevicePoolsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_device_pools(**kwargs)
```

1. See [:material-code-braces: ListDevicePoolsRequestRequestTypeDef](./type_defs.md#listdevicepoolsrequestrequesttypedef) 

### list\_devices

Gets information about unique device types.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_devices.html)

```python
# list_devices method definition

await def list_devices(
    self,
    *,
    arn: str = ...,
    nextToken: str = ...,
    filters: Sequence[DeviceFilterUnionTypeDef] = ...,  # (1)
) -> ListDevicesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeviceFilterTypeDef](./type_defs.md#devicefiltertypedef) [:material-code-braces: DeviceFilterOutputTypeDef](./type_defs.md#devicefilteroutputtypedef) 
2. See [:material-code-braces: ListDevicesResultTypeDef](./type_defs.md#listdevicesresulttypedef) 


```python
# list_devices method usage example with argument unpacking

kwargs: ListDevicesRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_devices(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef) 

### list\_instance\_profiles

Returns information about all the instance profiles in an AWS account.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_instance_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_instance_profiles.html)

```python
# list_instance_profiles method definition

await def list_instance_profiles(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListInstanceProfilesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstanceProfilesResultTypeDef](./type_defs.md#listinstanceprofilesresulttypedef) 


```python
# list_instance_profiles method usage example with argument unpacking

kwargs: ListInstanceProfilesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_instance_profiles(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesRequestRequestTypeDef](./type_defs.md#listinstanceprofilesrequestrequesttypedef) 

### list\_jobs

Gets information about jobs for a given test run.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_jobs.html)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    arn: str,
    nextToken: str = ...,
) -> ListJobsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef) 

### list\_network\_profiles

Returns the list of available network profiles.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_network_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_network_profiles.html)

```python
# list_network_profiles method definition

await def list_network_profiles(
    self,
    *,
    arn: str,
    type: NetworkProfileTypeType = ...,  # (1)
    nextToken: str = ...,
) -> ListNetworkProfilesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
2. See [:material-code-braces: ListNetworkProfilesResultTypeDef](./type_defs.md#listnetworkprofilesresulttypedef) 


```python
# list_network_profiles method usage example with argument unpacking

kwargs: ListNetworkProfilesRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_network_profiles(**kwargs)
```

1. See [:material-code-braces: ListNetworkProfilesRequestRequestTypeDef](./type_defs.md#listnetworkprofilesrequestrequesttypedef) 

### list\_offering\_promotions

Returns a list of offering promotions.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_offering_promotions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_offering_promotions.html)

```python
# list_offering_promotions method definition

await def list_offering_promotions(
    self,
    *,
    nextToken: str = ...,
) -> ListOfferingPromotionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOfferingPromotionsResultTypeDef](./type_defs.md#listofferingpromotionsresulttypedef) 


```python
# list_offering_promotions method usage example with argument unpacking

kwargs: ListOfferingPromotionsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_offering_promotions(**kwargs)
```

1. See [:material-code-braces: ListOfferingPromotionsRequestRequestTypeDef](./type_defs.md#listofferingpromotionsrequestrequesttypedef) 

### list\_offering\_transactions

Returns a list of all historical purchases, renewals, and system renewal
transactions for an AWS account.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_offering_transactions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_offering_transactions.html)

```python
# list_offering_transactions method definition

await def list_offering_transactions(
    self,
    *,
    nextToken: str = ...,
) -> ListOfferingTransactionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOfferingTransactionsResultTypeDef](./type_defs.md#listofferingtransactionsresulttypedef) 


```python
# list_offering_transactions method usage example with argument unpacking

kwargs: ListOfferingTransactionsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_offering_transactions(**kwargs)
```

1. See [:material-code-braces: ListOfferingTransactionsRequestRequestTypeDef](./type_defs.md#listofferingtransactionsrequestrequesttypedef) 

### list\_offerings

Returns a list of products or offerings that the user can manage through the
API.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_offerings.html)

```python
# list_offerings method definition

await def list_offerings(
    self,
    *,
    nextToken: str = ...,
) -> ListOfferingsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOfferingsResultTypeDef](./type_defs.md#listofferingsresulttypedef) 


```python
# list_offerings method usage example with argument unpacking

kwargs: ListOfferingsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_offerings(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestRequestTypeDef](./type_defs.md#listofferingsrequestrequesttypedef) 

### list\_projects

Gets information about projects.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_projects.html)

```python
# list_projects method definition

await def list_projects(
    self,
    *,
    arn: str = ...,
    nextToken: str = ...,
) -> ListProjectsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 


```python
# list_projects method usage example with argument unpacking

kwargs: ListProjectsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_projects(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef) 

### list\_remote\_access\_sessions

Returns a list of all currently running remote access sessions.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_remote_access_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_remote_access_sessions.html)

```python
# list_remote_access_sessions method definition

await def list_remote_access_sessions(
    self,
    *,
    arn: str,
    nextToken: str = ...,
) -> ListRemoteAccessSessionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRemoteAccessSessionsResultTypeDef](./type_defs.md#listremoteaccesssessionsresulttypedef) 


```python
# list_remote_access_sessions method usage example with argument unpacking

kwargs: ListRemoteAccessSessionsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_remote_access_sessions(**kwargs)
```

1. See [:material-code-braces: ListRemoteAccessSessionsRequestRequestTypeDef](./type_defs.md#listremoteaccesssessionsrequestrequesttypedef) 

### list\_runs

Gets information about runs, given an AWS Device Farm project ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_runs.html)

```python
# list_runs method definition

await def list_runs(
    self,
    *,
    arn: str,
    nextToken: str = ...,
) -> ListRunsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRunsResultTypeDef](./type_defs.md#listrunsresulttypedef) 


```python
# list_runs method usage example with argument unpacking

kwargs: ListRunsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_runs(**kwargs)
```

1. See [:material-code-braces: ListRunsRequestRequestTypeDef](./type_defs.md#listrunsrequestrequesttypedef) 

### list\_samples

Gets information about samples, given an AWS Device Farm job ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_samples` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_samples.html)

```python
# list_samples method definition

await def list_samples(
    self,
    *,
    arn: str,
    nextToken: str = ...,
) -> ListSamplesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSamplesResultTypeDef](./type_defs.md#listsamplesresulttypedef) 


```python
# list_samples method usage example with argument unpacking

kwargs: ListSamplesRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_samples(**kwargs)
```

1. See [:material-code-braces: ListSamplesRequestRequestTypeDef](./type_defs.md#listsamplesrequestrequesttypedef) 

### list\_suites

Gets information about test suites for a given job.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_suites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_suites.html)

```python
# list_suites method definition

await def list_suites(
    self,
    *,
    arn: str,
    nextToken: str = ...,
) -> ListSuitesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSuitesResultTypeDef](./type_defs.md#listsuitesresulttypedef) 


```python
# list_suites method usage example with argument unpacking

kwargs: ListSuitesRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_suites(**kwargs)
```

1. See [:material-code-braces: ListSuitesRequestRequestTypeDef](./type_defs.md#listsuitesrequestrequesttypedef) 

### list\_tags\_for\_resource

List the tags for an AWS Device Farm resource.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_test\_grid\_projects

Gets a list of all Selenium testing projects in your account.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_test_grid_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_test_grid_projects.html)

```python
# list_test_grid_projects method definition

await def list_test_grid_projects(
    self,
    *,
    maxResult: int = ...,
    nextToken: str = ...,
) -> ListTestGridProjectsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestGridProjectsResultTypeDef](./type_defs.md#listtestgridprojectsresulttypedef) 


```python
# list_test_grid_projects method usage example with argument unpacking

kwargs: ListTestGridProjectsRequestRequestTypeDef = {  # (1)
    "maxResult": ...,
}

parent.list_test_grid_projects(**kwargs)
```

1. See [:material-code-braces: ListTestGridProjectsRequestRequestTypeDef](./type_defs.md#listtestgridprojectsrequestrequesttypedef) 

### list\_test\_grid\_session\_actions

Returns a list of the actions taken in a <a>TestGridSession</a>.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_test_grid_session_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_test_grid_session_actions.html)

```python
# list_test_grid_session_actions method definition

await def list_test_grid_session_actions(
    self,
    *,
    sessionArn: str,
    maxResult: int = ...,
    nextToken: str = ...,
) -> ListTestGridSessionActionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestGridSessionActionsResultTypeDef](./type_defs.md#listtestgridsessionactionsresulttypedef) 


```python
# list_test_grid_session_actions method usage example with argument unpacking

kwargs: ListTestGridSessionActionsRequestRequestTypeDef = {  # (1)
    "sessionArn": ...,
}

parent.list_test_grid_session_actions(**kwargs)
```

1. See [:material-code-braces: ListTestGridSessionActionsRequestRequestTypeDef](./type_defs.md#listtestgridsessionactionsrequestrequesttypedef) 

### list\_test\_grid\_session\_artifacts

Retrieves a list of artifacts created during the session.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_test_grid_session_artifacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_test_grid_session_artifacts.html)

```python
# list_test_grid_session_artifacts method definition

await def list_test_grid_session_artifacts(
    self,
    *,
    sessionArn: str,
    type: TestGridSessionArtifactCategoryType = ...,  # (1)
    maxResult: int = ...,
    nextToken: str = ...,
) -> ListTestGridSessionArtifactsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TestGridSessionArtifactCategoryType](./literals.md#testgridsessionartifactcategorytype) 
2. See [:material-code-braces: ListTestGridSessionArtifactsResultTypeDef](./type_defs.md#listtestgridsessionartifactsresulttypedef) 


```python
# list_test_grid_session_artifacts method usage example with argument unpacking

kwargs: ListTestGridSessionArtifactsRequestRequestTypeDef = {  # (1)
    "sessionArn": ...,
}

parent.list_test_grid_session_artifacts(**kwargs)
```

1. See [:material-code-braces: ListTestGridSessionArtifactsRequestRequestTypeDef](./type_defs.md#listtestgridsessionartifactsrequestrequesttypedef) 

### list\_test\_grid\_sessions

Retrieves a list of sessions for a <a>TestGridProject</a>.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_test_grid_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_test_grid_sessions.html)

```python
# list_test_grid_sessions method definition

await def list_test_grid_sessions(
    self,
    *,
    projectArn: str,
    status: TestGridSessionStatusType = ...,  # (1)
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    endTimeAfter: TimestampTypeDef = ...,
    endTimeBefore: TimestampTypeDef = ...,
    maxResult: int = ...,
    nextToken: str = ...,
) -> ListTestGridSessionsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TestGridSessionStatusType](./literals.md#testgridsessionstatustype) 
2. See [:material-code-braces: ListTestGridSessionsResultTypeDef](./type_defs.md#listtestgridsessionsresulttypedef) 


```python
# list_test_grid_sessions method usage example with argument unpacking

kwargs: ListTestGridSessionsRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
}

parent.list_test_grid_sessions(**kwargs)
```

1. See [:material-code-braces: ListTestGridSessionsRequestRequestTypeDef](./type_defs.md#listtestgridsessionsrequestrequesttypedef) 

### list\_tests

Gets information about tests in a given test suite.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_tests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_tests.html)

```python
# list_tests method definition

await def list_tests(
    self,
    *,
    arn: str,
    nextToken: str = ...,
) -> ListTestsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestsResultTypeDef](./type_defs.md#listtestsresulttypedef) 


```python
# list_tests method usage example with argument unpacking

kwargs: ListTestsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_tests(**kwargs)
```

1. See [:material-code-braces: ListTestsRequestRequestTypeDef](./type_defs.md#listtestsrequestrequesttypedef) 

### list\_unique\_problems

Gets information about unique problems, such as exceptions or crashes.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_unique_problems` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_unique_problems.html)

```python
# list_unique_problems method definition

await def list_unique_problems(
    self,
    *,
    arn: str,
    nextToken: str = ...,
) -> ListUniqueProblemsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUniqueProblemsResultTypeDef](./type_defs.md#listuniqueproblemsresulttypedef) 


```python
# list_unique_problems method usage example with argument unpacking

kwargs: ListUniqueProblemsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_unique_problems(**kwargs)
```

1. See [:material-code-braces: ListUniqueProblemsRequestRequestTypeDef](./type_defs.md#listuniqueproblemsrequestrequesttypedef) 

### list\_uploads

Gets information about uploads, given an AWS Device Farm project ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_uploads` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_uploads.html)

```python
# list_uploads method definition

await def list_uploads(
    self,
    *,
    arn: str,
    type: UploadTypeType = ...,  # (1)
    nextToken: str = ...,
) -> ListUploadsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype) 
2. See [:material-code-braces: ListUploadsResultTypeDef](./type_defs.md#listuploadsresulttypedef) 


```python
# list_uploads method usage example with argument unpacking

kwargs: ListUploadsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_uploads(**kwargs)
```

1. See [:material-code-braces: ListUploadsRequestRequestTypeDef](./type_defs.md#listuploadsrequestrequesttypedef) 

### list\_vpce\_configurations

Returns information about all Amazon Virtual Private Cloud (VPC) endpoint
configurations in the AWS account.

Type annotations and code completion for `#!python session.create_client("devicefarm").list_vpce_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/list_vpce_configurations.html)

```python
# list_vpce_configurations method definition

await def list_vpce_configurations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListVPCEConfigurationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVPCEConfigurationsResultTypeDef](./type_defs.md#listvpceconfigurationsresulttypedef) 


```python
# list_vpce_configurations method usage example with argument unpacking

kwargs: ListVPCEConfigurationsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_vpce_configurations(**kwargs)
```

1. See [:material-code-braces: ListVPCEConfigurationsRequestRequestTypeDef](./type_defs.md#listvpceconfigurationsrequestrequesttypedef) 

### purchase\_offering

Immediately purchases offerings for an AWS account.

Type annotations and code completion for `#!python session.create_client("devicefarm").purchase_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/purchase_offering.html)

```python
# purchase_offering method definition

await def purchase_offering(
    self,
    *,
    offeringId: str,
    quantity: int,
    offeringPromotionId: str = ...,
) -> PurchaseOfferingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PurchaseOfferingResultTypeDef](./type_defs.md#purchaseofferingresulttypedef) 


```python
# purchase_offering method usage example with argument unpacking

kwargs: PurchaseOfferingRequestRequestTypeDef = {  # (1)
    "offeringId": ...,
    "quantity": ...,
}

parent.purchase_offering(**kwargs)
```

1. See [:material-code-braces: PurchaseOfferingRequestRequestTypeDef](./type_defs.md#purchaseofferingrequestrequesttypedef) 

### renew\_offering

Explicitly sets the quantity of devices to renew for an offering, starting from
the <code>effectiveDate</code> of the next period.

Type annotations and code completion for `#!python session.create_client("devicefarm").renew_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/renew_offering.html)

```python
# renew_offering method definition

await def renew_offering(
    self,
    *,
    offeringId: str,
    quantity: int,
) -> RenewOfferingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RenewOfferingResultTypeDef](./type_defs.md#renewofferingresulttypedef) 


```python
# renew_offering method usage example with argument unpacking

kwargs: RenewOfferingRequestRequestTypeDef = {  # (1)
    "offeringId": ...,
    "quantity": ...,
}

parent.renew_offering(**kwargs)
```

1. See [:material-code-braces: RenewOfferingRequestRequestTypeDef](./type_defs.md#renewofferingrequestrequesttypedef) 

### schedule\_run

Schedules a run.

Type annotations and code completion for `#!python session.create_client("devicefarm").schedule_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/schedule_run.html)

```python
# schedule_run method definition

await def schedule_run(
    self,
    *,
    projectArn: str,
    test: ScheduleRunTestTypeDef,  # (1)
    appArn: str = ...,
    devicePoolArn: str = ...,
    deviceSelectionConfiguration: DeviceSelectionConfigurationTypeDef = ...,  # (2)
    name: str = ...,
    configuration: ScheduleRunConfigurationTypeDef = ...,  # (3)
    executionConfiguration: ExecutionConfigurationTypeDef = ...,  # (4)
) -> ScheduleRunResultTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ScheduleRunTestTypeDef](./type_defs.md#scheduleruntesttypedef) 
2. See [:material-code-braces: DeviceSelectionConfigurationTypeDef](./type_defs.md#deviceselectionconfigurationtypedef) 
3. See [:material-code-braces: ScheduleRunConfigurationTypeDef](./type_defs.md#schedulerunconfigurationtypedef) 
4. See [:material-code-braces: ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef) 
5. See [:material-code-braces: ScheduleRunResultTypeDef](./type_defs.md#schedulerunresulttypedef) 


```python
# schedule_run method usage example with argument unpacking

kwargs: ScheduleRunRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
    "test": ...,
}

parent.schedule_run(**kwargs)
```

1. See [:material-code-braces: ScheduleRunRequestRequestTypeDef](./type_defs.md#schedulerunrequestrequesttypedef) 

### stop\_job

Initiates a stop request for the current job.

Type annotations and code completion for `#!python session.create_client("devicefarm").stop_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/stop_job.html)

```python
# stop_job method definition

await def stop_job(
    self,
    *,
    arn: str,
) -> StopJobResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopJobResultTypeDef](./type_defs.md#stopjobresulttypedef) 


```python
# stop_job method usage example with argument unpacking

kwargs: StopJobRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.stop_job(**kwargs)
```

1. See [:material-code-braces: StopJobRequestRequestTypeDef](./type_defs.md#stopjobrequestrequesttypedef) 

### stop\_remote\_access\_session

Ends a specified remote access session.

Type annotations and code completion for `#!python session.create_client("devicefarm").stop_remote_access_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/stop_remote_access_session.html)

```python
# stop_remote_access_session method definition

await def stop_remote_access_session(
    self,
    *,
    arn: str,
) -> StopRemoteAccessSessionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopRemoteAccessSessionResultTypeDef](./type_defs.md#stopremoteaccesssessionresulttypedef) 


```python
# stop_remote_access_session method usage example with argument unpacking

kwargs: StopRemoteAccessSessionRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.stop_remote_access_session(**kwargs)
```

1. See [:material-code-braces: StopRemoteAccessSessionRequestRequestTypeDef](./type_defs.md#stopremoteaccesssessionrequestrequesttypedef) 

### stop\_run

Initiates a stop request for the current test run.

Type annotations and code completion for `#!python session.create_client("devicefarm").stop_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/stop_run.html)

```python
# stop_run method definition

await def stop_run(
    self,
    *,
    arn: str,
) -> StopRunResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopRunResultTypeDef](./type_defs.md#stoprunresulttypedef) 


```python
# stop_run method usage example with argument unpacking

kwargs: StopRunRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.stop_run(**kwargs)
```

1. See [:material-code-braces: StopRunRequestRequestTypeDef](./type_defs.md#stoprunrequestrequesttypedef) 

### tag\_resource

Associates the specified tags to a resource with the specified
<code>resourceArn</code>.

Type annotations and code completion for `#!python session.create_client("devicefarm").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes the specified tags from a resource.

Type annotations and code completion for `#!python session.create_client("devicefarm").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_device\_instance

Updates information about a private device instance.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_device_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_device_instance.html)

```python
# update_device_instance method definition

await def update_device_instance(
    self,
    *,
    arn: str,
    profileArn: str = ...,
    labels: Sequence[str] = ...,
) -> UpdateDeviceInstanceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDeviceInstanceResultTypeDef](./type_defs.md#updatedeviceinstanceresulttypedef) 


```python
# update_device_instance method usage example with argument unpacking

kwargs: UpdateDeviceInstanceRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_device_instance(**kwargs)
```

1. See [:material-code-braces: UpdateDeviceInstanceRequestRequestTypeDef](./type_defs.md#updatedeviceinstancerequestrequesttypedef) 

### update\_device\_pool

Modifies the name, description, and rules in a device pool given the attributes
and the pool ARN.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_device_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_device_pool.html)

```python
# update_device_pool method definition

await def update_device_pool(
    self,
    *,
    arn: str,
    name: str = ...,
    description: str = ...,
    rules: Sequence[RuleTypeDef] = ...,  # (1)
    maxDevices: int = ...,
    clearMaxDevices: bool = ...,
) -> UpdateDevicePoolResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: UpdateDevicePoolResultTypeDef](./type_defs.md#updatedevicepoolresulttypedef) 


```python
# update_device_pool method usage example with argument unpacking

kwargs: UpdateDevicePoolRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_device_pool(**kwargs)
```

1. See [:material-code-braces: UpdateDevicePoolRequestRequestTypeDef](./type_defs.md#updatedevicepoolrequestrequesttypedef) 

### update\_instance\_profile

Updates information about an existing private device instance profile.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_instance_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_instance_profile.html)

```python
# update_instance_profile method definition

await def update_instance_profile(
    self,
    *,
    arn: str,
    name: str = ...,
    description: str = ...,
    packageCleanup: bool = ...,
    excludeAppPackagesFromCleanup: Sequence[str] = ...,
    rebootAfterUse: bool = ...,
) -> UpdateInstanceProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateInstanceProfileResultTypeDef](./type_defs.md#updateinstanceprofileresulttypedef) 


```python
# update_instance_profile method usage example with argument unpacking

kwargs: UpdateInstanceProfileRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_instance_profile(**kwargs)
```

1. See [:material-code-braces: UpdateInstanceProfileRequestRequestTypeDef](./type_defs.md#updateinstanceprofilerequestrequesttypedef) 

### update\_network\_profile

Updates the network profile.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_network_profile.html)

```python
# update_network_profile method definition

await def update_network_profile(
    self,
    *,
    arn: str,
    name: str = ...,
    description: str = ...,
    type: NetworkProfileTypeType = ...,  # (1)
    uplinkBandwidthBits: int = ...,
    downlinkBandwidthBits: int = ...,
    uplinkDelayMs: int = ...,
    downlinkDelayMs: int = ...,
    uplinkJitterMs: int = ...,
    downlinkJitterMs: int = ...,
    uplinkLossPercent: int = ...,
    downlinkLossPercent: int = ...,
) -> UpdateNetworkProfileResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
2. See [:material-code-braces: UpdateNetworkProfileResultTypeDef](./type_defs.md#updatenetworkprofileresulttypedef) 


```python
# update_network_profile method usage example with argument unpacking

kwargs: UpdateNetworkProfileRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_network_profile(**kwargs)
```

1. See [:material-code-braces: UpdateNetworkProfileRequestRequestTypeDef](./type_defs.md#updatenetworkprofilerequestrequesttypedef) 

### update\_project

Modifies the specified project name, given the project ARN and a new name.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_project.html)

```python
# update_project method definition

await def update_project(
    self,
    *,
    arn: str,
    name: str = ...,
    defaultJobTimeoutMinutes: int = ...,
    vpcConfig: VpcConfigTypeDef = ...,  # (1)
) -> UpdateProjectResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: UpdateProjectResultTypeDef](./type_defs.md#updateprojectresulttypedef) 


```python
# update_project method usage example with argument unpacking

kwargs: UpdateProjectRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_project(**kwargs)
```

1. See [:material-code-braces: UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef) 

### update\_test\_grid\_project

Change details of a project.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_test_grid_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_test_grid_project.html)

```python
# update_test_grid_project method definition

await def update_test_grid_project(
    self,
    *,
    projectArn: str,
    name: str = ...,
    description: str = ...,
    vpcConfig: TestGridVpcConfigTypeDef = ...,  # (1)
) -> UpdateTestGridProjectResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TestGridVpcConfigTypeDef](./type_defs.md#testgridvpcconfigtypedef) 
2. See [:material-code-braces: UpdateTestGridProjectResultTypeDef](./type_defs.md#updatetestgridprojectresulttypedef) 


```python
# update_test_grid_project method usage example with argument unpacking

kwargs: UpdateTestGridProjectRequestRequestTypeDef = {  # (1)
    "projectArn": ...,
}

parent.update_test_grid_project(**kwargs)
```

1. See [:material-code-braces: UpdateTestGridProjectRequestRequestTypeDef](./type_defs.md#updatetestgridprojectrequestrequesttypedef) 

### update\_upload

Updates an uploaded test spec.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_upload.html)

```python
# update_upload method definition

await def update_upload(
    self,
    *,
    arn: str,
    name: str = ...,
    contentType: str = ...,
    editContent: bool = ...,
) -> UpdateUploadResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateUploadResultTypeDef](./type_defs.md#updateuploadresulttypedef) 


```python
# update_upload method usage example with argument unpacking

kwargs: UpdateUploadRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_upload(**kwargs)
```

1. See [:material-code-braces: UpdateUploadRequestRequestTypeDef](./type_defs.md#updateuploadrequestrequesttypedef) 

### update\_vpce\_configuration

Updates information about an Amazon Virtual Private Cloud (VPC) endpoint
configuration.

Type annotations and code completion for `#!python session.create_client("devicefarm").update_vpce_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/client/update_vpce_configuration.html)

```python
# update_vpce_configuration method definition

await def update_vpce_configuration(
    self,
    *,
    arn: str,
    vpceConfigurationName: str = ...,
    vpceServiceName: str = ...,
    serviceDnsName: str = ...,
    vpceConfigurationDescription: str = ...,
) -> UpdateVPCEConfigurationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVPCEConfigurationResultTypeDef](./type_defs.md#updatevpceconfigurationresulttypedef) 


```python
# update_vpce_configuration method usage example with argument unpacking

kwargs: UpdateVPCEConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_vpce_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateVPCEConfigurationRequestRequestTypeDef](./type_defs.md#updatevpceconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("devicefarm").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("devicefarm").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator` method with overloads.

- `client.get_paginator("get_offering_status")` -> [GetOfferingStatusPaginator](./paginators.md#getofferingstatuspaginator)
- `client.get_paginator("list_artifacts")` -> [ListArtifactsPaginator](./paginators.md#listartifactspaginator)
- `client.get_paginator("list_device_instances")` -> [ListDeviceInstancesPaginator](./paginators.md#listdeviceinstancespaginator)
- `client.get_paginator("list_device_pools")` -> [ListDevicePoolsPaginator](./paginators.md#listdevicepoolspaginator)
- `client.get_paginator("list_devices")` -> [ListDevicesPaginator](./paginators.md#listdevicespaginator)
- `client.get_paginator("list_instance_profiles")` -> [ListInstanceProfilesPaginator](./paginators.md#listinstanceprofilespaginator)
- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_network_profiles")` -> [ListNetworkProfilesPaginator](./paginators.md#listnetworkprofilespaginator)
- `client.get_paginator("list_offering_promotions")` -> [ListOfferingPromotionsPaginator](./paginators.md#listofferingpromotionspaginator)
- `client.get_paginator("list_offering_transactions")` -> [ListOfferingTransactionsPaginator](./paginators.md#listofferingtransactionspaginator)
- `client.get_paginator("list_offerings")` -> [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
- `client.get_paginator("list_projects")` -> [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- `client.get_paginator("list_remote_access_sessions")` -> [ListRemoteAccessSessionsPaginator](./paginators.md#listremoteaccesssessionspaginator)
- `client.get_paginator("list_runs")` -> [ListRunsPaginator](./paginators.md#listrunspaginator)
- `client.get_paginator("list_samples")` -> [ListSamplesPaginator](./paginators.md#listsamplespaginator)
- `client.get_paginator("list_suites")` -> [ListSuitesPaginator](./paginators.md#listsuitespaginator)
- `client.get_paginator("list_tests")` -> [ListTestsPaginator](./paginators.md#listtestspaginator)
- `client.get_paginator("list_unique_problems")` -> [ListUniqueProblemsPaginator](./paginators.md#listuniqueproblemspaginator)
- `client.get_paginator("list_uploads")` -> [ListUploadsPaginator](./paginators.md#listuploadspaginator)
- `client.get_paginator("list_vpce_configurations")` -> [ListVPCEConfigurationsPaginator](./paginators.md#listvpceconfigurationspaginator)



