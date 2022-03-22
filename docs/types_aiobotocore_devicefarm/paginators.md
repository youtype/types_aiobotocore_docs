<a id="paginators-for-aiobotocore-devicefarm-module"></a>

# Paginators for aiobotocore DeviceFarm module

> [Index](../README.md) > [DeviceFarm](./README.md) > Paginators

Auto-generated documentation for
[DeviceFarm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
type annotations stubs module
[types-aiobotocore-devicefarm](https://pypi.org/project/types-aiobotocore-devicefarm/).

- [Paginators for aiobotocore DeviceFarm module](#paginators-for-aiobotocore-devicefarm-module)
  - [GetOfferingStatusPaginator](#getofferingstatuspaginator)
  - [ListArtifactsPaginator](#listartifactspaginator)
  - [ListDeviceInstancesPaginator](#listdeviceinstancespaginator)
  - [ListDevicePoolsPaginator](#listdevicepoolspaginator)
  - [ListDevicesPaginator](#listdevicespaginator)
  - [ListInstanceProfilesPaginator](#listinstanceprofilespaginator)
  - [ListJobsPaginator](#listjobspaginator)
  - [ListNetworkProfilesPaginator](#listnetworkprofilespaginator)
  - [ListOfferingPromotionsPaginator](#listofferingpromotionspaginator)
  - [ListOfferingTransactionsPaginator](#listofferingtransactionspaginator)
  - [ListOfferingsPaginator](#listofferingspaginator)
  - [ListProjectsPaginator](#listprojectspaginator)
  - [ListRemoteAccessSessionsPaginator](#listremoteaccesssessionspaginator)
  - [ListRunsPaginator](#listrunspaginator)
  - [ListSamplesPaginator](#listsamplespaginator)
  - [ListSuitesPaginator](#listsuitespaginator)
  - [ListTestsPaginator](#listtestspaginator)
  - [ListUniqueProblemsPaginator](#listuniqueproblemspaginator)
  - [ListUploadsPaginator](#listuploadspaginator)
  - [ListVPCEConfigurationsPaginator](#listvpceconfigurationspaginator)

<a id="getofferingstatuspaginator"></a>

## GetOfferingStatusPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("get_offering_status")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import GetOfferingStatusPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: GetOfferingStatusPaginator = client.get_paginator("get_offering_status")
```

Boto3 documentation:
[DeviceFarm.Paginator.GetOfferingStatus](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus)

Arguments for `GetOfferingStatusPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetOfferingStatusPaginator.paginate` returns
`AsyncIterator`\[[GetOfferingStatusResultTypeDef](./type_defs.md#getofferingstatusresulttypedef)\].

<a id="listartifactspaginator"></a>

## ListArtifactsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_artifacts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListArtifactsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListArtifactsPaginator = client.get_paginator("list_artifacts")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListArtifacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts)

Arguments for `ListArtifactsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `type`: [ArtifactCategoryType](./literals.md#artifactcategorytype)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListArtifactsPaginator.paginate` returns
`AsyncIterator`\[[ListArtifactsResultTypeDef](./type_defs.md#listartifactsresulttypedef)\].

<a id="listdeviceinstancespaginator"></a>

## ListDeviceInstancesPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_device_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListDeviceInstancesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListDeviceInstancesPaginator = client.get_paginator("list_device_instances")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListDeviceInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances)

Arguments for `ListDeviceInstancesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeviceInstancesPaginator.paginate` returns
`AsyncIterator`\[[ListDeviceInstancesResultTypeDef](./type_defs.md#listdeviceinstancesresulttypedef)\].

<a id="listdevicepoolspaginator"></a>

## ListDevicePoolsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_device_pools")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListDevicePoolsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListDevicePoolsPaginator = client.get_paginator("list_device_pools")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListDevicePools](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools)

Arguments for `ListDevicePoolsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `type`: [DevicePoolTypeType](./literals.md#devicepooltypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDevicePoolsPaginator.paginate` returns
`AsyncIterator`\[[ListDevicePoolsResultTypeDef](./type_defs.md#listdevicepoolsresulttypedef)\].

<a id="listdevicespaginator"></a>

## ListDevicesPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_devices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListDevicesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListDevices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices)

Arguments for `ListDevicesPaginator.paginate` method:

- `arn`: `str`
- `filters`:
  `Sequence`\[[DeviceFilterTypeDef](./type_defs.md#devicefiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDevicesPaginator.paginate` returns
`AsyncIterator`\[[ListDevicesResultTypeDef](./type_defs.md#listdevicesresulttypedef)\].

<a id="listinstanceprofilespaginator"></a>

## ListInstanceProfilesPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_instance_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListInstanceProfilesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListInstanceProfilesPaginator = client.get_paginator("list_instance_profiles")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListInstanceProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles)

Arguments for `ListInstanceProfilesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInstanceProfilesPaginator.paginate` returns
`AsyncIterator`\[[ListInstanceProfilesResultTypeDef](./type_defs.md#listinstanceprofilesresulttypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef)\].

<a id="listnetworkprofilespaginator"></a>

## ListNetworkProfilesPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_network_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListNetworkProfilesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListNetworkProfilesPaginator = client.get_paginator("list_network_profiles")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListNetworkProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles)

Arguments for `ListNetworkProfilesPaginator.paginate` method:

- `arn`: `str` *(required)*
- `type`: [NetworkProfileTypeType](./literals.md#networkprofiletypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListNetworkProfilesPaginator.paginate` returns
`AsyncIterator`\[[ListNetworkProfilesResultTypeDef](./type_defs.md#listnetworkprofilesresulttypedef)\].

<a id="listofferingpromotionspaginator"></a>

## ListOfferingPromotionsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_offering_promotions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListOfferingPromotionsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListOfferingPromotionsPaginator = client.get_paginator("list_offering_promotions")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListOfferingPromotions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions)

Arguments for `ListOfferingPromotionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOfferingPromotionsPaginator.paginate` returns
`AsyncIterator`\[[ListOfferingPromotionsResultTypeDef](./type_defs.md#listofferingpromotionsresulttypedef)\].

<a id="listofferingtransactionspaginator"></a>

## ListOfferingTransactionsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_offering_transactions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListOfferingTransactionsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListOfferingTransactionsPaginator = client.get_paginator("list_offering_transactions")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListOfferingTransactions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions)

Arguments for `ListOfferingTransactionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOfferingTransactionsPaginator.paginate` returns
`AsyncIterator`\[[ListOfferingTransactionsResultTypeDef](./type_defs.md#listofferingtransactionsresulttypedef)\].

<a id="listofferingspaginator"></a>

## ListOfferingsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_offerings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListOfferings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings)

Arguments for `ListOfferingsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOfferingsPaginator.paginate` returns
`AsyncIterator`\[[ListOfferingsResultTypeDef](./type_defs.md#listofferingsresulttypedef)\].

<a id="listprojectspaginator"></a>

## ListProjectsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects)

Arguments for `ListProjectsPaginator.paginate` method:

- `arn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectsPaginator.paginate` returns
`AsyncIterator`\[[ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef)\].

<a id="listremoteaccesssessionspaginator"></a>

## ListRemoteAccessSessionsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_remote_access_sessions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListRemoteAccessSessionsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListRemoteAccessSessionsPaginator = client.get_paginator("list_remote_access_sessions")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListRemoteAccessSessions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions)

Arguments for `ListRemoteAccessSessionsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRemoteAccessSessionsPaginator.paginate` returns
`AsyncIterator`\[[ListRemoteAccessSessionsResultTypeDef](./type_defs.md#listremoteaccesssessionsresulttypedef)\].

<a id="listrunspaginator"></a>

## ListRunsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_runs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListRunsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListRunsPaginator = client.get_paginator("list_runs")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListRuns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns)

Arguments for `ListRunsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRunsPaginator.paginate` returns
`AsyncIterator`\[[ListRunsResultTypeDef](./type_defs.md#listrunsresulttypedef)\].

<a id="listsamplespaginator"></a>

## ListSamplesPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_samples")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListSamplesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListSamplesPaginator = client.get_paginator("list_samples")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListSamples](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples)

Arguments for `ListSamplesPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSamplesPaginator.paginate` returns
`AsyncIterator`\[[ListSamplesResultTypeDef](./type_defs.md#listsamplesresulttypedef)\].

<a id="listsuitespaginator"></a>

## ListSuitesPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_suites")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListSuitesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListSuitesPaginator = client.get_paginator("list_suites")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListSuites](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites)

Arguments for `ListSuitesPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSuitesPaginator.paginate` returns
`AsyncIterator`\[[ListSuitesResultTypeDef](./type_defs.md#listsuitesresulttypedef)\].

<a id="listtestspaginator"></a>

## ListTestsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_tests")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListTestsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListTestsPaginator = client.get_paginator("list_tests")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListTests](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests)

Arguments for `ListTestsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTestsPaginator.paginate` returns
`AsyncIterator`\[[ListTestsResultTypeDef](./type_defs.md#listtestsresulttypedef)\].

<a id="listuniqueproblemspaginator"></a>

## ListUniqueProblemsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_unique_problems")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListUniqueProblemsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListUniqueProblemsPaginator = client.get_paginator("list_unique_problems")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListUniqueProblems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems)

Arguments for `ListUniqueProblemsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUniqueProblemsPaginator.paginate` returns
`AsyncIterator`\[[ListUniqueProblemsResultTypeDef](./type_defs.md#listuniqueproblemsresulttypedef)\].

<a id="listuploadspaginator"></a>

## ListUploadsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_uploads")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListUploadsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListUploadsPaginator = client.get_paginator("list_uploads")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListUploads](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads)

Arguments for `ListUploadsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `type`: [UploadTypeType](./literals.md#uploadtypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUploadsPaginator.paginate` returns
`AsyncIterator`\[[ListUploadsResultTypeDef](./type_defs.md#listuploadsresulttypedef)\].

<a id="listvpceconfigurationspaginator"></a>

## ListVPCEConfigurationsPaginator

Type annotations for
`session.create_client("devicefarm").get_paginator("list_vpce_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListVPCEConfigurationsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: ListVPCEConfigurationsPaginator = client.get_paginator("list_vpce_configurations")
```

Boto3 documentation:
[DeviceFarm.Paginator.ListVPCEConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations)

Arguments for `ListVPCEConfigurationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListVPCEConfigurationsPaginator.paginate` returns
`AsyncIterator`\[[ListVPCEConfigurationsResultTypeDef](./type_defs.md#listvpceconfigurationsresulttypedef)\].
