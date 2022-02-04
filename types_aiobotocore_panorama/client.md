<a id="panoramaclient-for-aiobotocore-panorama-module"></a>

# PanoramaClient for aiobotocore Panorama module

> [Index](..) > [Panorama](.) > PanoramaClient

Auto-generated documentation for
[Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
type annotations stubs module
[types-aiobotocore-panorama](https://pypi.org/project/types-aiobotocore-panorama/).

- [PanoramaClient for aiobotocore Panorama module](#panoramaclient-for-aiobotocore-panorama-module)
  - [PanoramaClient](#panoramaclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_application_instance](#create_application_instance)
    - [create_job_for_devices](#create_job_for_devices)
    - [create_node_from_template_job](#create_node_from_template_job)
    - [create_package](#create_package)
    - [create_package_import_job](#create_package_import_job)
    - [delete_device](#delete_device)
    - [delete_package](#delete_package)
    - [deregister_package_version](#deregister_package_version)
    - [describe_application_instance](#describe_application_instance)
    - [describe_application_instance_details](#describe_application_instance_details)
    - [describe_device](#describe_device)
    - [describe_device_job](#describe_device_job)
    - [describe_node](#describe_node)
    - [describe_node_from_template_job](#describe_node_from_template_job)
    - [describe_package](#describe_package)
    - [describe_package_import_job](#describe_package_import_job)
    - [describe_package_version](#describe_package_version)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_application_instance_dependencies](#list_application_instance_dependencies)
    - [list_application_instance_node_instances](#list_application_instance_node_instances)
    - [list_application_instances](#list_application_instances)
    - [list_devices](#list_devices)
    - [list_devices_jobs](#list_devices_jobs)
    - [list_node_from_template_jobs](#list_node_from_template_jobs)
    - [list_nodes](#list_nodes)
    - [list_package_import_jobs](#list_package_import_jobs)
    - [list_packages](#list_packages)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [provision_device](#provision_device)
    - [register_package_version](#register_package_version)
    - [remove_application_instance](#remove_application_instance)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_device_metadata](#update_device_metadata)

<a id="panoramaclient"></a>

## PanoramaClient

Type annotations for `aiobotocore.create_client("panorama")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_panorama.client import PanoramaClient

def get_panorama_client() -> PanoramaClient:
    return Session().client("panorama")
```

Boto3 documentation:
[Panorama.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_panorama.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

PanoramaClient exceptions.

Type annotations for `aiobotocore.create_client("panorama").exceptions` method.

Boto3 documentation:
[Panorama.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("panorama").can_paginate`
method.

Boto3 documentation:
[Panorama.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_application_instance"></a>

### create_application_instance

Creates an application instance and deploys it to a device.

Type annotations for
`aiobotocore.create_client("panorama").create_application_instance` method.

Boto3 documentation:
[Panorama.Client.create_application_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_application_instance)

Asynchronous method. Use `await create_application_instance(...)` for a
synchronous call.

Arguments mapping described in
[CreateApplicationInstanceRequestRequestTypeDef](./type_defs.md#createapplicationinstancerequestrequesttypedef).

Keyword-only arguments:

- `ManifestPayload`:
  [ManifestPayloadTypeDef](./type_defs.md#manifestpayloadtypedef) *(required)*
- `DefaultRuntimeContextDevice`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `ManifestOverridesPayload`:
  [ManifestOverridesPayloadTypeDef](./type_defs.md#manifestoverridespayloadtypedef)
- `ApplicationInstanceIdToReplace`: `str`
- `RuntimeRoleArn`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateApplicationInstanceResponseTypeDef](./type_defs.md#createapplicationinstanceresponsetypedef).

<a id="create_job_for_devices"></a>

### create_job_for_devices

Creates a job to run on one or more devices.

Type annotations for
`aiobotocore.create_client("panorama").create_job_for_devices` method.

Boto3 documentation:
[Panorama.Client.create_job_for_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_job_for_devices)

Asynchronous method. Use `await create_job_for_devices(...)` for a synchronous
call.

Arguments mapping described in
[CreateJobForDevicesRequestRequestTypeDef](./type_defs.md#createjobfordevicesrequestrequesttypedef).

Keyword-only arguments:

- `DeviceIds`: `Sequence`\[`str`\] *(required)*
- `DeviceJobConfig`:
  [DeviceJobConfigTypeDef](./type_defs.md#devicejobconfigtypedef) *(required)*
- `JobType`: `Literal['OTA']` (see [JobTypeType](./literals.md#jobtypetype))
  *(required)*

Returns a `Coroutine` for
[CreateJobForDevicesResponseTypeDef](./type_defs.md#createjobfordevicesresponsetypedef).

<a id="create_node_from_template_job"></a>

### create_node_from_template_job

Creates a camera stream node.

Type annotations for
`aiobotocore.create_client("panorama").create_node_from_template_job` method.

Boto3 documentation:
[Panorama.Client.create_node_from_template_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)

Asynchronous method. Use `await create_node_from_template_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateNodeFromTemplateJobRequestRequestTypeDef](./type_defs.md#createnodefromtemplatejobrequestrequesttypedef).

Keyword-only arguments:

- `TemplateType`: `Literal['RTSP_CAMERA_STREAM']` (see
  [TemplateTypeType](./literals.md#templatetypetype)) *(required)*
- `OutputPackageName`: `str` *(required)*
- `OutputPackageVersion`: `str` *(required)*
- `NodeName`: `str` *(required)*
- `TemplateParameters`: `Mapping`\[`str`, `str`\] *(required)*
- `NodeDescription`: `str`
- `JobTags`:
  `Sequence`\[[JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef)\]

Returns a `Coroutine` for
[CreateNodeFromTemplateJobResponseTypeDef](./type_defs.md#createnodefromtemplatejobresponsetypedef).

<a id="create_package"></a>

### create_package

Creates a package and storage location in an Amazon S3 access point.

Type annotations for `aiobotocore.create_client("panorama").create_package`
method.

Boto3 documentation:
[Panorama.Client.create_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package)

Asynchronous method. Use `await create_package(...)` for a synchronous call.

Arguments mapping described in
[CreatePackageRequestRequestTypeDef](./type_defs.md#createpackagerequestrequesttypedef).

Keyword-only arguments:

- `PackageName`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreatePackageResponseTypeDef](./type_defs.md#createpackageresponsetypedef).

<a id="create_package_import_job"></a>

### create_package_import_job

Imports a node package.

Type annotations for
`aiobotocore.create_client("panorama").create_package_import_job` method.

Boto3 documentation:
[Panorama.Client.create_package_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)

Asynchronous method. Use `await create_package_import_job(...)` for a
synchronous call.

Arguments mapping described in
[CreatePackageImportJobRequestRequestTypeDef](./type_defs.md#createpackageimportjobrequestrequesttypedef).

Keyword-only arguments:

- `JobType`: `Literal['NODE_PACKAGE_VERSION']` (see
  [PackageImportJobTypeType](./literals.md#packageimportjobtypetype))
  *(required)*
- `InputConfig`:
  [PackageImportJobInputConfigTypeDef](./type_defs.md#packageimportjobinputconfigtypedef)
  *(required)*
- `OutputConfig`:
  [PackageImportJobOutputConfigTypeDef](./type_defs.md#packageimportjoboutputconfigtypedef)
  *(required)*
- `ClientToken`: `str` *(required)*
- `JobTags`:
  `Sequence`\[[JobResourceTagsTypeDef](./type_defs.md#jobresourcetagstypedef)\]

Returns a `Coroutine` for
[CreatePackageImportJobResponseTypeDef](./type_defs.md#createpackageimportjobresponsetypedef).

<a id="delete_device"></a>

### delete_device

Deletes a device.

Type annotations for `aiobotocore.create_client("panorama").delete_device`
method.

Boto3 documentation:
[Panorama.Client.delete_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.delete_device)

Asynchronous method. Use `await delete_device(...)` for a synchronous call.

Arguments mapping described in
[DeleteDeviceRequestRequestTypeDef](./type_defs.md#deletedevicerequestrequesttypedef).

Keyword-only arguments:

- `DeviceId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteDeviceResponseTypeDef](./type_defs.md#deletedeviceresponsetypedef).

<a id="delete_package"></a>

### delete_package

Deletes a package.

Type annotations for `aiobotocore.create_client("panorama").delete_package`
method.

Boto3 documentation:
[Panorama.Client.delete_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.delete_package)

Asynchronous method. Use `await delete_package(...)` for a synchronous call.

Arguments mapping described in
[DeletePackageRequestRequestTypeDef](./type_defs.md#deletepackagerequestrequesttypedef).

Keyword-only arguments:

- `PackageId`: `str` *(required)*
- `ForceDelete`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="deregister_package_version"></a>

### deregister_package_version

Deregisters a package version.

Type annotations for
`aiobotocore.create_client("panorama").deregister_package_version` method.

Boto3 documentation:
[Panorama.Client.deregister_package_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.deregister_package_version)

Asynchronous method. Use `await deregister_package_version(...)` for a
synchronous call.

Arguments mapping described in
[DeregisterPackageVersionRequestRequestTypeDef](./type_defs.md#deregisterpackageversionrequestrequesttypedef).

Keyword-only arguments:

- `PackageId`: `str` *(required)*
- `PackageVersion`: `str` *(required)*
- `PatchVersion`: `str` *(required)*
- `OwnerAccount`: `str`
- `UpdatedLatestPatchVersion`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_application_instance"></a>

### describe_application_instance

Returns information about an application instance on a device.

Type annotations for
`aiobotocore.create_client("panorama").describe_application_instance` method.

Boto3 documentation:
[Panorama.Client.describe_application_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_application_instance)

Asynchronous method. Use `await describe_application_instance(...)` for a
synchronous call.

Arguments mapping described in
[DescribeApplicationInstanceRequestRequestTypeDef](./type_defs.md#describeapplicationinstancerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationInstanceId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeApplicationInstanceResponseTypeDef](./type_defs.md#describeapplicationinstanceresponsetypedef).

<a id="describe_application_instance_details"></a>

### describe_application_instance_details

Returns information about an application instance's configuration manifest.

Type annotations for
`aiobotocore.create_client("panorama").describe_application_instance_details`
method.

Boto3 documentation:
[Panorama.Client.describe_application_instance_details](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_application_instance_details)

Asynchronous method. Use `await describe_application_instance_details(...)` for
a synchronous call.

Arguments mapping described in
[DescribeApplicationInstanceDetailsRequestRequestTypeDef](./type_defs.md#describeapplicationinstancedetailsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationInstanceId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeApplicationInstanceDetailsResponseTypeDef](./type_defs.md#describeapplicationinstancedetailsresponsetypedef).

<a id="describe_device"></a>

### describe_device

Returns information about a device.

Type annotations for `aiobotocore.create_client("panorama").describe_device`
method.

Boto3 documentation:
[Panorama.Client.describe_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_device)

Asynchronous method. Use `await describe_device(...)` for a synchronous call.

Arguments mapping described in
[DescribeDeviceRequestRequestTypeDef](./type_defs.md#describedevicerequestrequesttypedef).

Keyword-only arguments:

- `DeviceId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDeviceResponseTypeDef](./type_defs.md#describedeviceresponsetypedef).

<a id="describe_device_job"></a>

### describe_device_job

Returns information about a device job.

Type annotations for
`aiobotocore.create_client("panorama").describe_device_job` method.

Boto3 documentation:
[Panorama.Client.describe_device_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_device_job)

Asynchronous method. Use `await describe_device_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDeviceJobRequestRequestTypeDef](./type_defs.md#describedevicejobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDeviceJobResponseTypeDef](./type_defs.md#describedevicejobresponsetypedef).

<a id="describe_node"></a>

### describe_node

Returns information about a node.

Type annotations for `aiobotocore.create_client("panorama").describe_node`
method.

Boto3 documentation:
[Panorama.Client.describe_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_node)

Asynchronous method. Use `await describe_node(...)` for a synchronous call.

Arguments mapping described in
[DescribeNodeRequestRequestTypeDef](./type_defs.md#describenoderequestrequesttypedef).

Keyword-only arguments:

- `NodeId`: `str` *(required)*
- `OwnerAccount`: `str`

Returns a `Coroutine` for
[DescribeNodeResponseTypeDef](./type_defs.md#describenoderesponsetypedef).

<a id="describe_node_from_template_job"></a>

### describe_node_from_template_job

Returns information about a job to create a camera stream node.

Type annotations for
`aiobotocore.create_client("panorama").describe_node_from_template_job` method.

Boto3 documentation:
[Panorama.Client.describe_node_from_template_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_node_from_template_job)

Asynchronous method. Use `await describe_node_from_template_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeNodeFromTemplateJobRequestRequestTypeDef](./type_defs.md#describenodefromtemplatejobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeNodeFromTemplateJobResponseTypeDef](./type_defs.md#describenodefromtemplatejobresponsetypedef).

<a id="describe_package"></a>

### describe_package

Returns information about a package.

Type annotations for `aiobotocore.create_client("panorama").describe_package`
method.

Boto3 documentation:
[Panorama.Client.describe_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package)

Asynchronous method. Use `await describe_package(...)` for a synchronous call.

Arguments mapping described in
[DescribePackageRequestRequestTypeDef](./type_defs.md#describepackagerequestrequesttypedef).

Keyword-only arguments:

- `PackageId`: `str` *(required)*

Returns a `Coroutine` for
[DescribePackageResponseTypeDef](./type_defs.md#describepackageresponsetypedef).

<a id="describe_package_import_job"></a>

### describe_package_import_job

Returns information about a package import job.

Type annotations for
`aiobotocore.create_client("panorama").describe_package_import_job` method.

Boto3 documentation:
[Panorama.Client.describe_package_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package_import_job)

Asynchronous method. Use `await describe_package_import_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribePackageImportJobRequestRequestTypeDef](./type_defs.md#describepackageimportjobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribePackageImportJobResponseTypeDef](./type_defs.md#describepackageimportjobresponsetypedef).

<a id="describe_package_version"></a>

### describe_package_version

Returns information about a package version.

Type annotations for
`aiobotocore.create_client("panorama").describe_package_version` method.

Boto3 documentation:
[Panorama.Client.describe_package_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.describe_package_version)

Asynchronous method. Use `await describe_package_version(...)` for a
synchronous call.

Arguments mapping described in
[DescribePackageVersionRequestRequestTypeDef](./type_defs.md#describepackageversionrequestrequesttypedef).

Keyword-only arguments:

- `PackageId`: `str` *(required)*
- `PackageVersion`: `str` *(required)*
- `OwnerAccount`: `str`
- `PatchVersion`: `str`

Returns a `Coroutine` for
[DescribePackageVersionResponseTypeDef](./type_defs.md#describepackageversionresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("panorama").generate_presigned_url` method.

Boto3 documentation:
[Panorama.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_application_instance_dependencies"></a>

### list_application_instance_dependencies

Returns a list of application instance dependencies.

Type annotations for
`aiobotocore.create_client("panorama").list_application_instance_dependencies`
method.

Boto3 documentation:
[Panorama.Client.list_application_instance_dependencies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instance_dependencies)

Asynchronous method. Use `await list_application_instance_dependencies(...)`
for a synchronous call.

Arguments mapping described in
[ListApplicationInstanceDependenciesRequestRequestTypeDef](./type_defs.md#listapplicationinstancedependenciesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationInstanceId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListApplicationInstanceDependenciesResponseTypeDef](./type_defs.md#listapplicationinstancedependenciesresponsetypedef).

<a id="list_application_instance_node_instances"></a>

### list_application_instance_node_instances

Returns a list of application node instances.

Type annotations for
`aiobotocore.create_client("panorama").list_application_instance_node_instances`
method.

Boto3 documentation:
[Panorama.Client.list_application_instance_node_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instance_node_instances)

Asynchronous method. Use `await list_application_instance_node_instances(...)`
for a synchronous call.

Arguments mapping described in
[ListApplicationInstanceNodeInstancesRequestRequestTypeDef](./type_defs.md#listapplicationinstancenodeinstancesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationInstanceId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListApplicationInstanceNodeInstancesResponseTypeDef](./type_defs.md#listapplicationinstancenodeinstancesresponsetypedef).

<a id="list_application_instances"></a>

### list_application_instances

Returns a list of application instances.

Type annotations for
`aiobotocore.create_client("panorama").list_application_instances` method.

Boto3 documentation:
[Panorama.Client.list_application_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_application_instances)

Asynchronous method. Use `await list_application_instances(...)` for a
synchronous call.

Arguments mapping described in
[ListApplicationInstancesRequestRequestTypeDef](./type_defs.md#listapplicationinstancesrequestrequesttypedef).

Keyword-only arguments:

- `DeviceId`: `str`
- `StatusFilter`: [StatusFilterType](./literals.md#statusfiltertype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListApplicationInstancesResponseTypeDef](./type_defs.md#listapplicationinstancesresponsetypedef).

<a id="list_devices"></a>

### list_devices

Returns a list of devices.

Type annotations for `aiobotocore.create_client("panorama").list_devices`
method.

Boto3 documentation:
[Panorama.Client.list_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_devices)

Asynchronous method. Use `await list_devices(...)` for a synchronous call.

Arguments mapping described in
[ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef).

<a id="list_devices_jobs"></a>

### list_devices_jobs

Returns a list of jobs.

Type annotations for `aiobotocore.create_client("panorama").list_devices_jobs`
method.

Boto3 documentation:
[Panorama.Client.list_devices_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_devices_jobs)

Asynchronous method. Use `await list_devices_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListDevicesJobsRequestRequestTypeDef](./type_defs.md#listdevicesjobsrequestrequesttypedef).

Keyword-only arguments:

- `DeviceId`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDevicesJobsResponseTypeDef](./type_defs.md#listdevicesjobsresponsetypedef).

<a id="list_node_from_template_jobs"></a>

### list_node_from_template_jobs

Returns a list of camera stream node jobs.

Type annotations for
`aiobotocore.create_client("panorama").list_node_from_template_jobs` method.

Boto3 documentation:
[Panorama.Client.list_node_from_template_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_node_from_template_jobs)

Asynchronous method. Use `await list_node_from_template_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListNodeFromTemplateJobsRequestRequestTypeDef](./type_defs.md#listnodefromtemplatejobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListNodeFromTemplateJobsResponseTypeDef](./type_defs.md#listnodefromtemplatejobsresponsetypedef).

<a id="list_nodes"></a>

### list_nodes

Returns a list of nodes.

Type annotations for `aiobotocore.create_client("panorama").list_nodes` method.

Boto3 documentation:
[Panorama.Client.list_nodes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_nodes)

Asynchronous method. Use `await list_nodes(...)` for a synchronous call.

Arguments mapping described in
[ListNodesRequestRequestTypeDef](./type_defs.md#listnodesrequestrequesttypedef).

Keyword-only arguments:

- `Category`: [NodeCategoryType](./literals.md#nodecategorytype)
- `OwnerAccount`: `str`
- `PackageName`: `str`
- `PackageVersion`: `str`
- `PatchVersion`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef).

<a id="list_package_import_jobs"></a>

### list_package_import_jobs

Returns a list of package import jobs.

Type annotations for
`aiobotocore.create_client("panorama").list_package_import_jobs` method.

Boto3 documentation:
[Panorama.Client.list_package_import_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_package_import_jobs)

Asynchronous method. Use `await list_package_import_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListPackageImportJobsRequestRequestTypeDef](./type_defs.md#listpackageimportjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListPackageImportJobsResponseTypeDef](./type_defs.md#listpackageimportjobsresponsetypedef).

<a id="list_packages"></a>

### list_packages

Returns a list of packages.

Type annotations for `aiobotocore.create_client("panorama").list_packages`
method.

Boto3 documentation:
[Panorama.Client.list_packages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_packages)

Asynchronous method. Use `await list_packages(...)` for a synchronous call.

Arguments mapping described in
[ListPackagesRequestRequestTypeDef](./type_defs.md#listpackagesrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListPackagesResponseTypeDef](./type_defs.md#listpackagesresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns a list of tags for a resource.

Type annotations for
`aiobotocore.create_client("panorama").list_tags_for_resource` method.

Boto3 documentation:
[Panorama.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="provision_device"></a>

### provision_device

Creates a device and returns a configuration archive.

Type annotations for `aiobotocore.create_client("panorama").provision_device`
method.

Boto3 documentation:
[Panorama.Client.provision_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)

Asynchronous method. Use `await provision_device(...)` for a synchronous call.

Arguments mapping described in
[ProvisionDeviceRequestRequestTypeDef](./type_defs.md#provisiondevicerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Description`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]
- `NetworkingConfiguration`:
  [NetworkPayloadTypeDef](./type_defs.md#networkpayloadtypedef)

Returns a `Coroutine` for
[ProvisionDeviceResponseTypeDef](./type_defs.md#provisiondeviceresponsetypedef).

<a id="register_package_version"></a>

### register_package_version

Registers a package version.

Type annotations for
`aiobotocore.create_client("panorama").register_package_version` method.

Boto3 documentation:
[Panorama.Client.register_package_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.register_package_version)

Asynchronous method. Use `await register_package_version(...)` for a
synchronous call.

Arguments mapping described in
[RegisterPackageVersionRequestRequestTypeDef](./type_defs.md#registerpackageversionrequestrequesttypedef).

Keyword-only arguments:

- `PackageId`: `str` *(required)*
- `PackageVersion`: `str` *(required)*
- `PatchVersion`: `str` *(required)*
- `OwnerAccount`: `str`
- `MarkLatest`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="remove_application_instance"></a>

### remove_application_instance

Removes an application instance.

Type annotations for
`aiobotocore.create_client("panorama").remove_application_instance` method.

Boto3 documentation:
[Panorama.Client.remove_application_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.remove_application_instance)

Asynchronous method. Use `await remove_application_instance(...)` for a
synchronous call.

Arguments mapping described in
[RemoveApplicationInstanceRequestRequestTypeDef](./type_defs.md#removeapplicationinstancerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationInstanceId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag_resource"></a>

### tag_resource

Tags a resource.

Type annotations for `aiobotocore.create_client("panorama").tag_resource`
method.

Boto3 documentation:
[Panorama.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes tags from a resource.

Type annotations for `aiobotocore.create_client("panorama").untag_resource`
method.

Boto3 documentation:
[Panorama.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_device_metadata"></a>

### update_device_metadata

Updates a device's metadata.

Type annotations for
`aiobotocore.create_client("panorama").update_device_metadata` method.

Boto3 documentation:
[Panorama.Client.update_device_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.update_device_metadata)

Asynchronous method. Use `await update_device_metadata(...)` for a synchronous
call.

Arguments mapping described in
[UpdateDeviceMetadataRequestRequestTypeDef](./type_defs.md#updatedevicemetadatarequestrequesttypedef).

Keyword-only arguments:

- `DeviceId`: `str` *(required)*
- `Description`: `str`

Returns a `Coroutine` for
[UpdateDeviceMetadataResponseTypeDef](./type_defs.md#updatedevicemetadataresponsetypedef).
