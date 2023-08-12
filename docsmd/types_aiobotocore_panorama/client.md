# PanoramaClient

> [Index](../README.md) > [Panorama](./README.md) > PanoramaClient

!!! note ""

    Auto-generated documentation for [Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
    type annotations stubs module [types-aiobotocore-panorama](https://pypi.org/project/types-aiobotocore-panorama/).

## PanoramaClient

Type annotations and code completion for `#!python session.create_client("panorama")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client)

```python
PanoramaClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_panorama.client import PanoramaClient

session = get_session()
async with session.create_client("panorama") as client:
    client: PanoramaClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("panorama").exceptions` structure.

```python
PanoramaClient.exceptions usage example

async with session.create_client("panorama") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
PanoramaClient usage type checking example

from types_aiobotocore_panorama.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("panorama").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("panorama").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_application\_instance

Creates an application instance and deploys it to a device.

Type annotations and code completion for `#!python session.create_client("panorama").create_application_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_application_instance)

```python
# create_application_instance method definition

await def create_application_instance(
    self,
    *,
    DefaultRuntimeContextDevice: str,
    ManifestPayload: ManifestPayloadTypeDef,  # (1)
    ApplicationInstanceIdToReplace: str = ...,
    Description: str = ...,
    ManifestOverridesPayload: ManifestOverridesPayloadTypeDef = ...,  # (2)
    Name: str = ...,
    RuntimeRoleArn: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateApplicationInstanceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ManifestPayloadTypeDef](./type_defs.md#manifestpayloadtypedef) 
2. See [:material-code-braces: ManifestOverridesPayloadTypeDef](./type_defs.md#manifestoverridespayloadtypedef) 
3. See [:material-code-braces: CreateApplicationInstanceResponseTypeDef](./type_defs.md#createapplicationinstanceresponsetypedef) 


```python
# create_application_instance method usage example with argument unpacking

kwargs: CreateApplicationInstanceRequestRequestTypeDef = {  # (1)
    "DefaultRuntimeContextDevice": ...,
    "ManifestPayload": ...,
}

parent.create_application_instance(**kwargs)
```

1. See [:material-code-braces: CreateApplicationInstanceRequestRequestTypeDef](./type_defs.md#createapplicationinstancerequestrequesttypedef) 

### create\_job\_for\_devices

Creates a job to run on a device.

Type annotations and code completion for `#!python session.create_client("panorama").create_job_for_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_job_for_devices)

```python
# create_job_for_devices method definition

await def create_job_for_devices(
    self,
    *,
    DeviceIds: Sequence[str],
    JobType: JobTypeType,  # (1)
    DeviceJobConfig: DeviceJobConfigTypeDef = ...,  # (2)
) -> CreateJobForDevicesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: DeviceJobConfigTypeDef](./type_defs.md#devicejobconfigtypedef) 
3. See [:material-code-braces: CreateJobForDevicesResponseTypeDef](./type_defs.md#createjobfordevicesresponsetypedef) 


```python
# create_job_for_devices method usage example with argument unpacking

kwargs: CreateJobForDevicesRequestRequestTypeDef = {  # (1)
    "DeviceIds": ...,
    "JobType": ...,
}

parent.create_job_for_devices(**kwargs)
```

1. See [:material-code-braces: CreateJobForDevicesRequestRequestTypeDef](./type_defs.md#createjobfordevicesrequestrequesttypedef) 

### create\_node\_from\_template\_job

Creates a camera stream node.

Type annotations and code completion for `#!python session.create_client("panorama").create_node_from_template_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)

```python
# create_node_from_template_job method definition

await def create_node_from_template_job(
    self,
    *,
    NodeName: str,
    OutputPackageName: str,
    OutputPackageVersion: str,
    TemplateParameters: Mapping[str, str],
    TemplateType: TemplateTypeType,  # (1)
    JobTags: Sequence[JobResourceTagsTypeDef] = ...,  # (2)
    NodeDescription: str = ...,
) -> CreateNodeFromTemplateJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
2. See [:material-code-braces: JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef) 
3. See [:material-code-braces: CreateNodeFromTemplateJobResponseTypeDef](./type_defs.md#createnodefromtemplatejobresponsetypedef) 


```python
# create_node_from_template_job method usage example with argument unpacking

kwargs: CreateNodeFromTemplateJobRequestRequestTypeDef = {  # (1)
    "NodeName": ...,
    "OutputPackageName": ...,
    "OutputPackageVersion": ...,
    "TemplateParameters": ...,
    "TemplateType": ...,
}

parent.create_node_from_template_job(**kwargs)
```

1. See [:material-code-braces: CreateNodeFromTemplateJobRequestRequestTypeDef](./type_defs.md#createnodefromtemplatejobrequestrequesttypedef) 

### create\_package

Creates a package and storage location in an Amazon S3 access point.

Type annotations and code completion for `#!python session.create_client("panorama").create_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package)

```python
# create_package method definition

await def create_package(
    self,
    *,
    PackageName: str,
    Tags: Mapping[str, str] = ...,
) -> CreatePackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePackageResponseTypeDef](./type_defs.md#createpackageresponsetypedef) 


```python
# create_package method usage example with argument unpacking

kwargs: CreatePackageRequestRequestTypeDef = {  # (1)
    "PackageName": ...,
}

parent.create_package(**kwargs)
```

1. See [:material-code-braces: CreatePackageRequestRequestTypeDef](./type_defs.md#createpackagerequestrequesttypedef) 

### create\_package\_import\_job

Imports a node package.

Type annotations and code completion for `#!python session.create_client("panorama").create_package_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)

```python
# create_package_import_job method definition

await def create_package_import_job(
    self,
    *,
    ClientToken: str,
    InputConfig: PackageImportJobInputConfigTypeDef,  # (1)
    JobType: PackageImportJobTypeType,  # (2)
    OutputConfig: PackageImportJobOutputConfigTypeDef,  # (3)
    JobTags: Sequence[JobResourceTagsTypeDef] = ...,  # (4)
) -> CreatePackageImportJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: PackageImportJobInputConfigTypeDef](./type_defs.md#packageimportjobinputconfigtypedef) 
2. See [:material-code-brackets: PackageImportJobTypeType](./literals.md#packageimportjobtypetype) 
3. See [:material-code-braces: PackageImportJobOutputConfigTypeDef](./type_defs.md#packageimportjoboutputconfigtypedef) 
4. See [:material-code-braces: JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef) 
5. See [:material-code-braces: CreatePackageImportJobResponseTypeDef](./type_defs.md#createpackageimportjobresponsetypedef) 


```python
# create_package_import_job method usage example with argument unpacking

kwargs: CreatePackageImportJobRequestRequestTypeDef = {  # (1)
    "ClientToken": ...,
    "InputConfig": ...,
    "JobType": ...,
    "OutputConfig": ...,
}

parent.create_package_import_job(**kwargs)
```

1. See [:material-code-braces: CreatePackageImportJobRequestRequestTypeDef](./type_defs.md#createpackageimportjobrequestrequesttypedef) 

### delete\_device

Deletes a device.

Type annotations and code completion for `#!python session.create_client("panorama").delete_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.delete_device)

```python
# delete_device method definition

await def delete_device(
    self,
    *,
    DeviceId: str,
) -> DeleteDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDeviceResponseTypeDef](./type_defs.md#deletedeviceresponsetypedef) 


```python
# delete_device method usage example with argument unpacking

kwargs: DeleteDeviceRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.delete_device(**kwargs)
```

1. See [:material-code-braces: DeleteDeviceRequestRequestTypeDef](./type_defs.md#deletedevicerequestrequesttypedef) 

### delete\_package

Deletes a package.

Type annotations and code completion for `#!python session.create_client("panorama").delete_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.delete_package)

```python
# delete_package method definition

await def delete_package(
    self,
    *,
    PackageId: str,
    ForceDelete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_package method usage example with argument unpacking

kwargs: DeletePackageRequestRequestTypeDef = {  # (1)
    "PackageId": ...,
}

parent.delete_package(**kwargs)
```

1. See [:material-code-braces: DeletePackageRequestRequestTypeDef](./type_defs.md#deletepackagerequestrequesttypedef) 

### deregister\_package\_version

Deregisters a package version.

Type annotations and code completion for `#!python session.create_client("panorama").deregister_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.deregister_package_version)

```python
# deregister_package_version method definition

await def deregister_package_version(
    self,
    *,
    PackageId: str,
    PackageVersion: str,
    PatchVersion: str,
    OwnerAccount: str = ...,
    UpdatedLatestPatchVersion: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_package_version method usage example with argument unpacking

kwargs: DeregisterPackageVersionRequestRequestTypeDef = {  # (1)
    "PackageId": ...,
    "PackageVersion": ...,
    "PatchVersion": ...,
}

parent.deregister_package_version(**kwargs)
```

1. See [:material-code-braces: DeregisterPackageVersionRequestRequestTypeDef](./type_defs.md#deregisterpackageversionrequestrequesttypedef) 

### describe\_application\_instance

Returns information about an application instance on a device.

Type annotations and code completion for `#!python session.create_client("panorama").describe_application_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_application_instance)

```python
# describe_application_instance method definition

await def describe_application_instance(
    self,
    *,
    ApplicationInstanceId: str,
) -> DescribeApplicationInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationInstanceResponseTypeDef](./type_defs.md#describeapplicationinstanceresponsetypedef) 


```python
# describe_application_instance method usage example with argument unpacking

kwargs: DescribeApplicationInstanceRequestRequestTypeDef = {  # (1)
    "ApplicationInstanceId": ...,
}

parent.describe_application_instance(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationInstanceRequestRequestTypeDef](./type_defs.md#describeapplicationinstancerequestrequesttypedef) 

### describe\_application\_instance\_details

Returns information about an application instance's configuration manifest.

Type annotations and code completion for `#!python session.create_client("panorama").describe_application_instance_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_application_instance_details)

```python
# describe_application_instance_details method definition

await def describe_application_instance_details(
    self,
    *,
    ApplicationInstanceId: str,
) -> DescribeApplicationInstanceDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationInstanceDetailsResponseTypeDef](./type_defs.md#describeapplicationinstancedetailsresponsetypedef) 


```python
# describe_application_instance_details method usage example with argument unpacking

kwargs: DescribeApplicationInstanceDetailsRequestRequestTypeDef = {  # (1)
    "ApplicationInstanceId": ...,
}

parent.describe_application_instance_details(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationInstanceDetailsRequestRequestTypeDef](./type_defs.md#describeapplicationinstancedetailsrequestrequesttypedef) 

### describe\_device

Returns information about a device.

Type annotations and code completion for `#!python session.create_client("panorama").describe_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_device)

```python
# describe_device method definition

await def describe_device(
    self,
    *,
    DeviceId: str,
) -> DescribeDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeviceResponseTypeDef](./type_defs.md#describedeviceresponsetypedef) 


```python
# describe_device method usage example with argument unpacking

kwargs: DescribeDeviceRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.describe_device(**kwargs)
```

1. See [:material-code-braces: DescribeDeviceRequestRequestTypeDef](./type_defs.md#describedevicerequestrequesttypedef) 

### describe\_device\_job

Returns information about a device job.

Type annotations and code completion for `#!python session.create_client("panorama").describe_device_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_device_job)

```python
# describe_device_job method definition

await def describe_device_job(
    self,
    *,
    JobId: str,
) -> DescribeDeviceJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeviceJobResponseTypeDef](./type_defs.md#describedevicejobresponsetypedef) 


```python
# describe_device_job method usage example with argument unpacking

kwargs: DescribeDeviceJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_device_job(**kwargs)
```

1. See [:material-code-braces: DescribeDeviceJobRequestRequestTypeDef](./type_defs.md#describedevicejobrequestrequesttypedef) 

### describe\_node

Returns information about a node.

Type annotations and code completion for `#!python session.create_client("panorama").describe_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_node)

```python
# describe_node method definition

await def describe_node(
    self,
    *,
    NodeId: str,
    OwnerAccount: str = ...,
) -> DescribeNodeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNodeResponseTypeDef](./type_defs.md#describenoderesponsetypedef) 


```python
# describe_node method usage example with argument unpacking

kwargs: DescribeNodeRequestRequestTypeDef = {  # (1)
    "NodeId": ...,
}

parent.describe_node(**kwargs)
```

1. See [:material-code-braces: DescribeNodeRequestRequestTypeDef](./type_defs.md#describenoderequestrequesttypedef) 

### describe\_node\_from\_template\_job

Returns information about a job to create a camera stream node.

Type annotations and code completion for `#!python session.create_client("panorama").describe_node_from_template_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_node_from_template_job)

```python
# describe_node_from_template_job method definition

await def describe_node_from_template_job(
    self,
    *,
    JobId: str,
) -> DescribeNodeFromTemplateJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNodeFromTemplateJobResponseTypeDef](./type_defs.md#describenodefromtemplatejobresponsetypedef) 


```python
# describe_node_from_template_job method usage example with argument unpacking

kwargs: DescribeNodeFromTemplateJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_node_from_template_job(**kwargs)
```

1. See [:material-code-braces: DescribeNodeFromTemplateJobRequestRequestTypeDef](./type_defs.md#describenodefromtemplatejobrequestrequesttypedef) 

### describe\_package

Returns information about a package.

Type annotations and code completion for `#!python session.create_client("panorama").describe_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package)

```python
# describe_package method definition

await def describe_package(
    self,
    *,
    PackageId: str,
) -> DescribePackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePackageResponseTypeDef](./type_defs.md#describepackageresponsetypedef) 


```python
# describe_package method usage example with argument unpacking

kwargs: DescribePackageRequestRequestTypeDef = {  # (1)
    "PackageId": ...,
}

parent.describe_package(**kwargs)
```

1. See [:material-code-braces: DescribePackageRequestRequestTypeDef](./type_defs.md#describepackagerequestrequesttypedef) 

### describe\_package\_import\_job

Returns information about a package import job.

Type annotations and code completion for `#!python session.create_client("panorama").describe_package_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package_import_job)

```python
# describe_package_import_job method definition

await def describe_package_import_job(
    self,
    *,
    JobId: str,
) -> DescribePackageImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePackageImportJobResponseTypeDef](./type_defs.md#describepackageimportjobresponsetypedef) 


```python
# describe_package_import_job method usage example with argument unpacking

kwargs: DescribePackageImportJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_package_import_job(**kwargs)
```

1. See [:material-code-braces: DescribePackageImportJobRequestRequestTypeDef](./type_defs.md#describepackageimportjobrequestrequesttypedef) 

### describe\_package\_version

Returns information about a package version.

Type annotations and code completion for `#!python session.create_client("panorama").describe_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package_version)

```python
# describe_package_version method definition

await def describe_package_version(
    self,
    *,
    PackageId: str,
    PackageVersion: str,
    OwnerAccount: str = ...,
    PatchVersion: str = ...,
) -> DescribePackageVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePackageVersionResponseTypeDef](./type_defs.md#describepackageversionresponsetypedef) 


```python
# describe_package_version method usage example with argument unpacking

kwargs: DescribePackageVersionRequestRequestTypeDef = {  # (1)
    "PackageId": ...,
    "PackageVersion": ...,
}

parent.describe_package_version(**kwargs)
```

1. See [:material-code-braces: DescribePackageVersionRequestRequestTypeDef](./type_defs.md#describepackageversionrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("panorama").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.generate_presigned_url)

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


### list\_application\_instance\_dependencies

Returns a list of application instance dependencies.

Type annotations and code completion for `#!python session.create_client("panorama").list_application_instance_dependencies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instance_dependencies)

```python
# list_application_instance_dependencies method definition

await def list_application_instance_dependencies(
    self,
    *,
    ApplicationInstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListApplicationInstanceDependenciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationInstanceDependenciesResponseTypeDef](./type_defs.md#listapplicationinstancedependenciesresponsetypedef) 


```python
# list_application_instance_dependencies method usage example with argument unpacking

kwargs: ListApplicationInstanceDependenciesRequestRequestTypeDef = {  # (1)
    "ApplicationInstanceId": ...,
}

parent.list_application_instance_dependencies(**kwargs)
```

1. See [:material-code-braces: ListApplicationInstanceDependenciesRequestRequestTypeDef](./type_defs.md#listapplicationinstancedependenciesrequestrequesttypedef) 

### list\_application\_instance\_node\_instances

Returns a list of application node instances.

Type annotations and code completion for `#!python session.create_client("panorama").list_application_instance_node_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instance_node_instances)

```python
# list_application_instance_node_instances method definition

await def list_application_instance_node_instances(
    self,
    *,
    ApplicationInstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListApplicationInstanceNodeInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationInstanceNodeInstancesResponseTypeDef](./type_defs.md#listapplicationinstancenodeinstancesresponsetypedef) 


```python
# list_application_instance_node_instances method usage example with argument unpacking

kwargs: ListApplicationInstanceNodeInstancesRequestRequestTypeDef = {  # (1)
    "ApplicationInstanceId": ...,
}

parent.list_application_instance_node_instances(**kwargs)
```

1. See [:material-code-braces: ListApplicationInstanceNodeInstancesRequestRequestTypeDef](./type_defs.md#listapplicationinstancenodeinstancesrequestrequesttypedef) 

### list\_application\_instances

Returns a list of application instances.

Type annotations and code completion for `#!python session.create_client("panorama").list_application_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instances)

```python
# list_application_instances method definition

await def list_application_instances(
    self,
    *,
    DeviceId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    StatusFilter: StatusFilterType = ...,  # (1)
) -> ListApplicationInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusFilterType](./literals.md#statusfiltertype) 
2. See [:material-code-braces: ListApplicationInstancesResponseTypeDef](./type_defs.md#listapplicationinstancesresponsetypedef) 


```python
# list_application_instances method usage example with argument unpacking

kwargs: ListApplicationInstancesRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.list_application_instances(**kwargs)
```

1. See [:material-code-braces: ListApplicationInstancesRequestRequestTypeDef](./type_defs.md#listapplicationinstancesrequestrequesttypedef) 

### list\_devices

Returns a list of devices.

Type annotations and code completion for `#!python session.create_client("panorama").list_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_devices)

```python
# list_devices method definition

await def list_devices(
    self,
    *,
    DeviceAggregatedStatusFilter: DeviceAggregatedStatusType = ...,  # (1)
    MaxResults: int = ...,
    NameFilter: str = ...,
    NextToken: str = ...,
    SortBy: ListDevicesSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
) -> ListDevicesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: DeviceAggregatedStatusType](./literals.md#deviceaggregatedstatustype) 
2. See [:material-code-brackets: ListDevicesSortByType](./literals.md#listdevicessortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python
# list_devices method usage example with argument unpacking

kwargs: ListDevicesRequestRequestTypeDef = {  # (1)
    "DeviceAggregatedStatusFilter": ...,
}

parent.list_devices(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef) 

### list\_devices\_jobs

Returns a list of jobs.

Type annotations and code completion for `#!python session.create_client("panorama").list_devices_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_devices_jobs)

```python
# list_devices_jobs method definition

await def list_devices_jobs(
    self,
    *,
    DeviceId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDevicesJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDevicesJobsResponseTypeDef](./type_defs.md#listdevicesjobsresponsetypedef) 


```python
# list_devices_jobs method usage example with argument unpacking

kwargs: ListDevicesJobsRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.list_devices_jobs(**kwargs)
```

1. See [:material-code-braces: ListDevicesJobsRequestRequestTypeDef](./type_defs.md#listdevicesjobsrequestrequesttypedef) 

### list\_node\_from\_template\_jobs

Returns a list of camera stream node jobs.

Type annotations and code completion for `#!python session.create_client("panorama").list_node_from_template_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_node_from_template_jobs)

```python
# list_node_from_template_jobs method definition

await def list_node_from_template_jobs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListNodeFromTemplateJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNodeFromTemplateJobsResponseTypeDef](./type_defs.md#listnodefromtemplatejobsresponsetypedef) 


```python
# list_node_from_template_jobs method usage example with argument unpacking

kwargs: ListNodeFromTemplateJobsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_node_from_template_jobs(**kwargs)
```

1. See [:material-code-braces: ListNodeFromTemplateJobsRequestRequestTypeDef](./type_defs.md#listnodefromtemplatejobsrequestrequesttypedef) 

### list\_nodes

Returns a list of nodes.

Type annotations and code completion for `#!python session.create_client("panorama").list_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_nodes)

```python
# list_nodes method definition

await def list_nodes(
    self,
    *,
    Category: NodeCategoryType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
    OwnerAccount: str = ...,
    PackageName: str = ...,
    PackageVersion: str = ...,
    PatchVersion: str = ...,
) -> ListNodesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NodeCategoryType](./literals.md#nodecategorytype) 
2. See [:material-code-braces: ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef) 


```python
# list_nodes method usage example with argument unpacking

kwargs: ListNodesRequestRequestTypeDef = {  # (1)
    "Category": ...,
}

parent.list_nodes(**kwargs)
```

1. See [:material-code-braces: ListNodesRequestRequestTypeDef](./type_defs.md#listnodesrequestrequesttypedef) 

### list\_package\_import\_jobs

Returns a list of package import jobs.

Type annotations and code completion for `#!python session.create_client("panorama").list_package_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_package_import_jobs)

```python
# list_package_import_jobs method definition

await def list_package_import_jobs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPackageImportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPackageImportJobsResponseTypeDef](./type_defs.md#listpackageimportjobsresponsetypedef) 


```python
# list_package_import_jobs method usage example with argument unpacking

kwargs: ListPackageImportJobsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_package_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListPackageImportJobsRequestRequestTypeDef](./type_defs.md#listpackageimportjobsrequestrequesttypedef) 

### list\_packages

Returns a list of packages.

Type annotations and code completion for `#!python session.create_client("panorama").list_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_packages)

```python
# list_packages method definition

await def list_packages(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPackagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPackagesResponseTypeDef](./type_defs.md#listpackagesresponsetypedef) 


```python
# list_packages method usage example with argument unpacking

kwargs: ListPackagesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_packages(**kwargs)
```

1. See [:material-code-braces: ListPackagesRequestRequestTypeDef](./type_defs.md#listpackagesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for a resource.

Type annotations and code completion for `#!python session.create_client("panorama").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### provision\_device

Creates a device and returns a configuration archive.

Type annotations and code completion for `#!python session.create_client("panorama").provision_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)

```python
# provision_device method definition

await def provision_device(
    self,
    *,
    Name: str,
    Description: str = ...,
    NetworkingConfiguration: NetworkPayloadTypeDef = ...,  # (1)
    Tags: Mapping[str, str] = ...,
) -> ProvisionDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NetworkPayloadTypeDef](./type_defs.md#networkpayloadtypedef) 
2. See [:material-code-braces: ProvisionDeviceResponseTypeDef](./type_defs.md#provisiondeviceresponsetypedef) 


```python
# provision_device method usage example with argument unpacking

kwargs: ProvisionDeviceRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.provision_device(**kwargs)
```

1. See [:material-code-braces: ProvisionDeviceRequestRequestTypeDef](./type_defs.md#provisiondevicerequestrequesttypedef) 

### register\_package\_version

Registers a package version.

Type annotations and code completion for `#!python session.create_client("panorama").register_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.register_package_version)

```python
# register_package_version method definition

await def register_package_version(
    self,
    *,
    PackageId: str,
    PackageVersion: str,
    PatchVersion: str,
    MarkLatest: bool = ...,
    OwnerAccount: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# register_package_version method usage example with argument unpacking

kwargs: RegisterPackageVersionRequestRequestTypeDef = {  # (1)
    "PackageId": ...,
    "PackageVersion": ...,
    "PatchVersion": ...,
}

parent.register_package_version(**kwargs)
```

1. See [:material-code-braces: RegisterPackageVersionRequestRequestTypeDef](./type_defs.md#registerpackageversionrequestrequesttypedef) 

### remove\_application\_instance

Removes an application instance.

Type annotations and code completion for `#!python session.create_client("panorama").remove_application_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.remove_application_instance)

```python
# remove_application_instance method definition

await def remove_application_instance(
    self,
    *,
    ApplicationInstanceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# remove_application_instance method usage example with argument unpacking

kwargs: RemoveApplicationInstanceRequestRequestTypeDef = {  # (1)
    "ApplicationInstanceId": ...,
}

parent.remove_application_instance(**kwargs)
```

1. See [:material-code-braces: RemoveApplicationInstanceRequestRequestTypeDef](./type_defs.md#removeapplicationinstancerequestrequesttypedef) 

### signal\_application\_instance\_node\_instances

Signal camera nodes to stop or resume.

Type annotations and code completion for `#!python session.create_client("panorama").signal_application_instance_node_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.signal_application_instance_node_instances)

```python
# signal_application_instance_node_instances method definition

await def signal_application_instance_node_instances(
    self,
    *,
    ApplicationInstanceId: str,
    NodeSignals: Sequence[NodeSignalTypeDef],  # (1)
) -> SignalApplicationInstanceNodeInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NodeSignalTypeDef](./type_defs.md#nodesignaltypedef) 
2. See [:material-code-braces: SignalApplicationInstanceNodeInstancesResponseTypeDef](./type_defs.md#signalapplicationinstancenodeinstancesresponsetypedef) 


```python
# signal_application_instance_node_instances method usage example with argument unpacking

kwargs: SignalApplicationInstanceNodeInstancesRequestRequestTypeDef = {  # (1)
    "ApplicationInstanceId": ...,
    "NodeSignals": ...,
}

parent.signal_application_instance_node_instances(**kwargs)
```

1. See [:material-code-braces: SignalApplicationInstanceNodeInstancesRequestRequestTypeDef](./type_defs.md#signalapplicationinstancenodeinstancesrequestrequesttypedef) 

### tag\_resource

Tags a resource.

Type annotations and code completion for `#!python session.create_client("panorama").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("panorama").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_device\_metadata

Updates a device's metadata.

Type annotations and code completion for `#!python session.create_client("panorama").update_device_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.update_device_metadata)

```python
# update_device_metadata method definition

await def update_device_metadata(
    self,
    *,
    DeviceId: str,
    Description: str = ...,
) -> UpdateDeviceMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDeviceMetadataResponseTypeDef](./type_defs.md#updatedevicemetadataresponsetypedef) 


```python
# update_device_metadata method usage example with argument unpacking

kwargs: UpdateDeviceMetadataRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.update_device_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateDeviceMetadataRequestRequestTypeDef](./type_defs.md#updatedevicemetadatarequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("panorama").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> PanoramaClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("panorama").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.__aexit__)

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





