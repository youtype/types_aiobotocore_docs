<a id="snowballclient-for-aiobotocore-snowball-module"></a>

# SnowballClient for aiobotocore Snowball module

> [Index](../README.md) > [Snowball](./README.md) > SnowballClient

Auto-generated documentation for
[Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
type annotations stubs module
[types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

- [SnowballClient for aiobotocore Snowball module](#snowballclient-for-aiobotocore-snowball-module)
  - [SnowballClient](#snowballclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_cluster](#cancel_cluster)
    - [cancel_job](#cancel_job)
    - [create_address](#create_address)
    - [create_cluster](#create_cluster)
    - [create_job](#create_job)
    - [create_long_term_pricing](#create_long_term_pricing)
    - [create_return_shipping_label](#create_return_shipping_label)
    - [describe_address](#describe_address)
    - [describe_addresses](#describe_addresses)
    - [describe_cluster](#describe_cluster)
    - [describe_job](#describe_job)
    - [describe_return_shipping_label](#describe_return_shipping_label)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_job_manifest](#get_job_manifest)
    - [get_job_unlock_code](#get_job_unlock_code)
    - [get_snowball_usage](#get_snowball_usage)
    - [get_software_updates](#get_software_updates)
    - [list_cluster_jobs](#list_cluster_jobs)
    - [list_clusters](#list_clusters)
    - [list_compatible_images](#list_compatible_images)
    - [list_jobs](#list_jobs)
    - [list_long_term_pricing](#list_long_term_pricing)
    - [update_cluster](#update_cluster)
    - [update_job](#update_job)
    - [update_job_shipment_state](#update_job_shipment_state)
    - [update_long_term_pricing](#update_long_term_pricing)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="snowballclient"></a>

## SnowballClient

Type annotations for `session.create_client("snowball")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_snowball.client import SnowballClient

session = get_session()
async with session.create_client("snowball") as client:
    client: SnowballClient
```

Boto3 documentation:
[Snowball.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_snowball.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ClusterLimitExceededException`
- `Exceptions.ConflictException`
- `Exceptions.Ec2RequestFailedException`
- `Exceptions.InvalidAddressException`
- `Exceptions.InvalidInputCombinationException`
- `Exceptions.InvalidJobStateException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidResourceException`
- `Exceptions.KMSRequestFailedException`
- `Exceptions.ReturnShippingLabelAlreadyExistsException`
- `Exceptions.UnsupportedAddressException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SnowballClient exceptions.

Type annotations for `session.create_client("snowball").exceptions` method.

Boto3 documentation:
[Snowball.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("snowball").can_paginate` method.

Boto3 documentation:
[Snowball.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_cluster"></a>

### cancel_cluster

Cancels a cluster job.

Type annotations for `session.create_client("snowball").cancel_cluster` method.

Boto3 documentation:
[Snowball.Client.cancel_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.cancel_cluster)

Asynchronous method. Use `await cancel_cluster(...)` for a synchronous call.

Arguments mapping described in
[CancelClusterRequestRequestTypeDef](./type_defs.md#cancelclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="cancel\_job"></a>

### cancel_job

Cancels the specified job.

Type annotations for `session.create_client("snowball").cancel_job` method.

Boto3 documentation:
[Snowball.Client.cancel_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.cancel_job)

Asynchronous method. Use `await cancel_job(...)` for a synchronous call.

Arguments mapping described in
[CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create\_address"></a>

### create_address

Creates an address for a Snow device to be shipped to.

Type annotations for `session.create_client("snowball").create_address` method.

Boto3 documentation:
[Snowball.Client.create_address](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_address)

Asynchronous method. Use `await create_address(...)` for a synchronous call.

Arguments mapping described in
[CreateAddressRequestRequestTypeDef](./type_defs.md#createaddressrequestrequesttypedef).

Keyword-only arguments:

- `Address`: [AddressTypeDef](./type_defs.md#addresstypedef) *(required)*

Returns a `Coroutine` for
[CreateAddressResultTypeDef](./type_defs.md#createaddressresulttypedef).

<a id="create\_cluster"></a>

### create_cluster

Creates an empty cluster.

Type annotations for `session.create_client("snowball").create_cluster` method.

Boto3 documentation:
[Snowball.Client.create_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)

Asynchronous method. Use `await create_cluster(...)` for a synchronous call.

Arguments mapping described in
[CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef).

Keyword-only arguments:

- `JobType`: [JobTypeType](./literals.md#jobtypetype) *(required)*
- `Resources`: [JobResourceTypeDef](./type_defs.md#jobresourcetypedef)
  *(required)*
- `AddressId`: `str` *(required)*
- `RoleARN`: `str` *(required)*
- `SnowballType`: [SnowballTypeType](./literals.md#snowballtypetype)
  *(required)*
- `ShippingOption`: [ShippingOptionType](./literals.md#shippingoptiontype)
  *(required)*
- `OnDeviceServiceConfiguration`:
  [OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef)
- `Description`: `str`
- `KmsKeyARN`: `str`
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
- `ForwardingAddressId`: `str`
- `TaxDocuments`: [TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef)
- `RemoteManagement`:
  [RemoteManagementType](./literals.md#remotemanagementtype)

Returns a `Coroutine` for
[CreateClusterResultTypeDef](./type_defs.md#createclusterresulttypedef).

<a id="create\_job"></a>

### create_job

Creates a job to import or export data between Amazon S3 and your on-premises
data center.

Type annotations for `session.create_client("snowball").create_job` method.

Boto3 documentation:
[Snowball.Client.create_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)

Asynchronous method. Use `await create_job(...)` for a synchronous call.

Arguments mapping described in
[CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef).

Keyword-only arguments:

- `JobType`: [JobTypeType](./literals.md#jobtypetype)
- `Resources`: [JobResourceTypeDef](./type_defs.md#jobresourcetypedef)
- `OnDeviceServiceConfiguration`:
  [OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef)
- `Description`: `str`
- `AddressId`: `str`
- `KmsKeyARN`: `str`
- `RoleARN`: `str`
- `SnowballCapacityPreference`:
  [SnowballCapacityType](./literals.md#snowballcapacitytype)
- `ShippingOption`: [ShippingOptionType](./literals.md#shippingoptiontype)
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
- `ClusterId`: `str`
- `SnowballType`: [SnowballTypeType](./literals.md#snowballtypetype)
- `ForwardingAddressId`: `str`
- `TaxDocuments`: [TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef)
- `DeviceConfiguration`:
  [DeviceConfigurationTypeDef](./type_defs.md#deviceconfigurationtypedef)
- `RemoteManagement`:
  [RemoteManagementType](./literals.md#remotemanagementtype)
- `LongTermPricingId`: `str`

Returns a `Coroutine` for
[CreateJobResultTypeDef](./type_defs.md#createjobresulttypedef).

<a id="create\_long\_term\_pricing"></a>

### create_long_term_pricing

Creates a job with the long-term usage option for a device.

Type annotations for
`session.create_client("snowball").create_long_term_pricing` method.

Boto3 documentation:
[Snowball.Client.create_long_term_pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_long_term_pricing)

Asynchronous method. Use `await create_long_term_pricing(...)` for a
synchronous call.

Arguments mapping described in
[CreateLongTermPricingRequestRequestTypeDef](./type_defs.md#createlongtermpricingrequestrequesttypedef).

Keyword-only arguments:

- `LongTermPricingType`:
  [LongTermPricingTypeType](./literals.md#longtermpricingtypetype) *(required)*
- `IsLongTermPricingAutoRenew`: `bool`
- `SnowballType`: [SnowballTypeType](./literals.md#snowballtypetype)

Returns a `Coroutine` for
[CreateLongTermPricingResultTypeDef](./type_defs.md#createlongtermpricingresulttypedef).

<a id="create\_return\_shipping\_label"></a>

### create_return_shipping_label

Creates a shipping label that will be used to return the Snow device to Amazon
Web Services.

Type annotations for
`session.create_client("snowball").create_return_shipping_label` method.

Boto3 documentation:
[Snowball.Client.create_return_shipping_label](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_return_shipping_label)

Asynchronous method. Use `await create_return_shipping_label(...)` for a
synchronous call.

Arguments mapping described in
[CreateReturnShippingLabelRequestRequestTypeDef](./type_defs.md#createreturnshippinglabelrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*
- `ShippingOption`: [ShippingOptionType](./literals.md#shippingoptiontype)

Returns a `Coroutine` for
[CreateReturnShippingLabelResultTypeDef](./type_defs.md#createreturnshippinglabelresulttypedef).

<a id="describe\_address"></a>

### describe_address

Takes an `AddressId` and returns specific details about that address in the
form of an `Address` object.

Type annotations for `session.create_client("snowball").describe_address`
method.

Boto3 documentation:
[Snowball.Client.describe_address](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.describe_address)

Asynchronous method. Use `await describe_address(...)` for a synchronous call.

Arguments mapping described in
[DescribeAddressRequestRequestTypeDef](./type_defs.md#describeaddressrequestrequesttypedef).

Keyword-only arguments:

- `AddressId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAddressResultTypeDef](./type_defs.md#describeaddressresulttypedef).

<a id="describe\_addresses"></a>

### describe_addresses

Returns a specified number of `ADDRESS` objects.

Type annotations for `session.create_client("snowball").describe_addresses`
method.

Boto3 documentation:
[Snowball.Client.describe_addresses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.describe_addresses)

Asynchronous method. Use `await describe_addresses(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAddressesRequestRequestTypeDef](./type_defs.md#describeaddressesrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef).

<a id="describe\_cluster"></a>

### describe_cluster

Returns information about a specific cluster including shipping information,
cluster status, and other important metadata.

Type annotations for `session.create_client("snowball").describe_cluster`
method.

Boto3 documentation:
[Snowball.Client.describe_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.describe_cluster)

Asynchronous method. Use `await describe_cluster(...)` for a synchronous call.

Arguments mapping described in
[DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeClusterResultTypeDef](./type_defs.md#describeclusterresulttypedef).

<a id="describe\_job"></a>

### describe_job

Returns information about a specific job including shipping information, job
status, and other important metadata.

Type annotations for `session.create_client("snowball").describe_job` method.

Boto3 documentation:
[Snowball.Client.describe_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.describe_job)

Asynchronous method. Use `await describe_job(...)` for a synchronous call.

Arguments mapping described in
[DescribeJobRequestRequestTypeDef](./type_defs.md#describejobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeJobResultTypeDef](./type_defs.md#describejobresulttypedef).

<a id="describe\_return\_shipping\_label"></a>

### describe_return_shipping_label

Information on the shipping label of a Snow device that is being returned to
Amazon Web Services.

Type annotations for
`session.create_client("snowball").describe_return_shipping_label` method.

Boto3 documentation:
[Snowball.Client.describe_return_shipping_label](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.describe_return_shipping_label)

Asynchronous method. Use `await describe_return_shipping_label(...)` for a
synchronous call.

Arguments mapping described in
[DescribeReturnShippingLabelRequestRequestTypeDef](./type_defs.md#describereturnshippinglabelrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeReturnShippingLabelResultTypeDef](./type_defs.md#describereturnshippinglabelresulttypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("snowball").generate_presigned_url`
method.

Boto3 documentation:
[Snowball.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_job\_manifest"></a>

### get_job_manifest

Returns a link to an Amazon S3 presigned URL for the manifest file associated
with the specified `JobId` value.

Type annotations for `session.create_client("snowball").get_job_manifest`
method.

Boto3 documentation:
[Snowball.Client.get_job_manifest](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_job_manifest)

Asynchronous method. Use `await get_job_manifest(...)` for a synchronous call.

Arguments mapping described in
[GetJobManifestRequestRequestTypeDef](./type_defs.md#getjobmanifestrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[GetJobManifestResultTypeDef](./type_defs.md#getjobmanifestresulttypedef).

<a id="get\_job\_unlock\_code"></a>

### get_job_unlock_code

Returns the `UnlockCode` code value for the specified job.

Type annotations for `session.create_client("snowball").get_job_unlock_code`
method.

Boto3 documentation:
[Snowball.Client.get_job_unlock_code](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_job_unlock_code)

Asynchronous method. Use `await get_job_unlock_code(...)` for a synchronous
call.

Arguments mapping described in
[GetJobUnlockCodeRequestRequestTypeDef](./type_defs.md#getjobunlockcoderequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[GetJobUnlockCodeResultTypeDef](./type_defs.md#getjobunlockcoderesulttypedef).

<a id="get\_snowball\_usage"></a>

### get_snowball_usage

Returns information about the Snow Family service limit for your account, and
also the number of Snow devices your account has in use.

Type annotations for `session.create_client("snowball").get_snowball_usage`
method.

Boto3 documentation:
[Snowball.Client.get_snowball_usage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_snowball_usage)

Asynchronous method. Use `await get_snowball_usage(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetSnowballUsageResultTypeDef](./type_defs.md#getsnowballusageresulttypedef).

<a id="get\_software\_updates"></a>

### get_software_updates

Returns an Amazon S3 presigned URL for an update file associated with a
specified `JobId` .

Type annotations for `session.create_client("snowball").get_software_updates`
method.

Boto3 documentation:
[Snowball.Client.get_software_updates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_software_updates)

Asynchronous method. Use `await get_software_updates(...)` for a synchronous
call.

Arguments mapping described in
[GetSoftwareUpdatesRequestRequestTypeDef](./type_defs.md#getsoftwareupdatesrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[GetSoftwareUpdatesResultTypeDef](./type_defs.md#getsoftwareupdatesresulttypedef).

<a id="list\_cluster\_jobs"></a>

### list_cluster_jobs

Returns an array of `JobListEntry` objects of the specified length.

Type annotations for `session.create_client("snowball").list_cluster_jobs`
method.

Boto3 documentation:
[Snowball.Client.list_cluster_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_cluster_jobs)

Asynchronous method. Use `await list_cluster_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListClusterJobsRequestRequestTypeDef](./type_defs.md#listclusterjobsrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListClusterJobsResultTypeDef](./type_defs.md#listclusterjobsresulttypedef).

<a id="list\_clusters"></a>

### list_clusters

Returns an array of `ClusterListEntry` objects of the specified length.

Type annotations for `session.create_client("snowball").list_clusters` method.

Boto3 documentation:
[Snowball.Client.list_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_clusters)

Asynchronous method. Use `await list_clusters(...)` for a synchronous call.

Arguments mapping described in
[ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListClustersResultTypeDef](./type_defs.md#listclustersresulttypedef).

<a id="list\_compatible\_images"></a>

### list_compatible_images

This action returns a list of the different Amazon EC2 Amazon Machine Images
(AMIs) that are owned by your Amazon Web Services accountthat would be
supported for use on a Snow device.

Type annotations for `session.create_client("snowball").list_compatible_images`
method.

Boto3 documentation:
[Snowball.Client.list_compatible_images](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_compatible_images)

Asynchronous method. Use `await list_compatible_images(...)` for a synchronous
call.

Arguments mapping described in
[ListCompatibleImagesRequestRequestTypeDef](./type_defs.md#listcompatibleimagesrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListCompatibleImagesResultTypeDef](./type_defs.md#listcompatibleimagesresulttypedef).

<a id="list\_jobs"></a>

### list_jobs

Returns an array of `JobListEntry` objects of the specified length.

Type annotations for `session.create_client("snowball").list_jobs` method.

Boto3 documentation:
[Snowball.Client.list_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_jobs)

Asynchronous method. Use `await list_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef).

<a id="list\_long\_term\_pricing"></a>

### list_long_term_pricing

Lists all long-term pricing types.

Type annotations for `session.create_client("snowball").list_long_term_pricing`
method.

Boto3 documentation:
[Snowball.Client.list_long_term_pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_long_term_pricing)

Asynchronous method. Use `await list_long_term_pricing(...)` for a synchronous
call.

Arguments mapping described in
[ListLongTermPricingRequestRequestTypeDef](./type_defs.md#listlongtermpricingrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListLongTermPricingResultTypeDef](./type_defs.md#listlongtermpricingresulttypedef).

<a id="update\_cluster"></a>

### update_cluster

While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you
can update some of the information associated with a cluster.

Type annotations for `session.create_client("snowball").update_cluster` method.

Boto3 documentation:
[Snowball.Client.update_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)

Asynchronous method. Use `await update_cluster(...)` for a synchronous call.

Arguments mapping described in
[UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `RoleARN`: `str`
- `Description`: `str`
- `Resources`: [JobResourceTypeDef](./type_defs.md#jobresourcetypedef)
- `OnDeviceServiceConfiguration`:
  [OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef)
- `AddressId`: `str`
- `ShippingOption`: [ShippingOptionType](./literals.md#shippingoptiontype)
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
- `ForwardingAddressId`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_job"></a>

### update_job

While a job's `JobState` value is `New` , you can update some of the
information associated with a job.

Type annotations for `session.create_client("snowball").update_job` method.

Boto3 documentation:
[Snowball.Client.update_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)

Asynchronous method. Use `await update_job(...)` for a synchronous call.

Arguments mapping described in
[UpdateJobRequestRequestTypeDef](./type_defs.md#updatejobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*
- `RoleARN`: `str`
- `Notification`: [NotificationTypeDef](./type_defs.md#notificationtypedef)
- `Resources`: [JobResourceTypeDef](./type_defs.md#jobresourcetypedef)
- `OnDeviceServiceConfiguration`:
  [OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef)
- `AddressId`: `str`
- `ShippingOption`: [ShippingOptionType](./literals.md#shippingoptiontype)
- `Description`: `str`
- `SnowballCapacityPreference`:
  [SnowballCapacityType](./literals.md#snowballcapacitytype)
- `ForwardingAddressId`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_job\_shipment\_state"></a>

### update_job_shipment_state

Updates the state when a shipment state changes to a different state.

Type annotations for
`session.create_client("snowball").update_job_shipment_state` method.

Boto3 documentation:
[Snowball.Client.update_job_shipment_state](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job_shipment_state)

Asynchronous method. Use `await update_job_shipment_state(...)` for a
synchronous call.

Arguments mapping described in
[UpdateJobShipmentStateRequestRequestTypeDef](./type_defs.md#updatejobshipmentstaterequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*
- `ShipmentState`: [ShipmentStateType](./literals.md#shipmentstatetype)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_long\_term\_pricing"></a>

### update_long_term_pricing

Updates the long-term pricing type.

Type annotations for
`session.create_client("snowball").update_long_term_pricing` method.

Boto3 documentation:
[Snowball.Client.update_long_term_pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_long_term_pricing)

Asynchronous method. Use `await update_long_term_pricing(...)` for a
synchronous call.

Arguments mapping described in
[UpdateLongTermPricingRequestRequestTypeDef](./type_defs.md#updatelongtermpricingrequestrequesttypedef).

Keyword-only arguments:

- `LongTermPricingId`: `str` *(required)*
- `ReplacementJob`: `str`
- `IsLongTermPricingAutoRenew`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("snowball").__aenter__` method.

Boto3 documentation:
[Snowball.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [SnowballClient](#snowballclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("snowball").__aexit__` method.

Boto3 documentation:
[Snowball.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("snowball").get_paginator` method
with overloads.

- `client.get_paginator("describe_addresses")` ->
  [DescribeAddressesPaginator](./paginators.md#describeaddressespaginator)
- `client.get_paginator("list_cluster_jobs")` ->
  [ListClusterJobsPaginator](./paginators.md#listclusterjobspaginator)
- `client.get_paginator("list_clusters")` ->
  [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_compatible_images")` ->
  [ListCompatibleImagesPaginator](./paginators.md#listcompatibleimagespaginator)
- `client.get_paginator("list_jobs")` ->
  [ListJobsPaginator](./paginators.md#listjobspaginator)
