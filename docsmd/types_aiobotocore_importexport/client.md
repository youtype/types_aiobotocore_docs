# ImportExportClient

> [Index](../README.md) > [ImportExport](./README.md) > ImportExportClient

!!! note ""

    Auto-generated documentation for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
    type annotations stubs module [types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

## ImportExportClient

Type annotations and code completion for `#!python session.create_client("importexport")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_importexport.client import ImportExportClient

session = get_session()
async with session.create_client("importexport") as client:
    client: ImportExportClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("importexport").exceptions` structure.

```python title="Usage example"
async with session.create_client("importexport") as client:
    try:
        do_something(client)
    except (
            client.BucketPermissionException,
        client.CanceledJobIdException,
        client.ClientError,
        client.CreateJobQuotaExceededException,
        client.ExpiredJobIdException,
        client.InvalidAccessKeyIdException,
        client.InvalidAddressException,
        client.InvalidCustomsException,
        client.InvalidFileSystemException,
        client.InvalidJobIdException,
        client.InvalidManifestFieldException,
        client.InvalidParameterException,
        client.InvalidVersionException,
        client.MalformedManifestException,
        client.MissingCustomsException,
        client.MissingManifestFieldException,
        client.MissingParameterException,
        client.MultipleRegionsException,
        client.NoSuchBucketException,
        client.UnableToCancelJobIdException,
        client.UnableToUpdateJobIdException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_importexport.client import Exceptions

def handle_error(exc: Exceptions.BucketPermissionException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("importexport").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_job

This operation cancels a specified job.

Type annotations and code completion for `#!python session.create_client("importexport").cancel_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.cancel_job)

```python title="Method definition"
await def cancel_job(
    self,
    *,
    JobId: str,
    APIVersion: str = ...,
) -> CancelJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef) 


```python title="Usage example with kwargs"
kwargs: CancelJobInputRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobInputRequestTypeDef](./type_defs.md#canceljobinputrequesttypedef) 

### create\_job

This operation initiates the process of scheduling an upload or download of your
data.

Type annotations and code completion for `#!python session.create_client("importexport").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.create_job)

```python title="Method definition"
await def create_job(
    self,
    *,
    JobType: JobTypeType,  # (1)
    Manifest: str,
    ValidateOnly: bool,
    ManifestAddendum: str = ...,
    APIVersion: str = ...,
) -> CreateJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef) 


```python title="Usage example with kwargs"
kwargs: CreateJobInputRequestTypeDef = {  # (1)
    "JobType": ...,
    "Manifest": ...,
    "ValidateOnly": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobInputRequestTypeDef](./type_defs.md#createjobinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("importexport").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_shipping\_label

This operation generates a pre-paid UPS shipping label that you will use to ship
your device to AWS for processing.

Type annotations and code completion for `#!python session.create_client("importexport").get_shipping_label` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.get_shipping_label)

```python title="Method definition"
await def get_shipping_label(
    self,
    *,
    jobIds: Sequence[str],
    name: str = ...,
    company: str = ...,
    phoneNumber: str = ...,
    country: str = ...,
    stateOrProvince: str = ...,
    city: str = ...,
    postalCode: str = ...,
    street1: str = ...,
    street2: str = ...,
    street3: str = ...,
    APIVersion: str = ...,
) -> GetShippingLabelOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetShippingLabelOutputTypeDef](./type_defs.md#getshippinglabeloutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetShippingLabelInputRequestTypeDef = {  # (1)
    "jobIds": ...,
}

parent.get_shipping_label(**kwargs)
```

1. See [:material-code-braces: GetShippingLabelInputRequestTypeDef](./type_defs.md#getshippinglabelinputrequesttypedef) 

### get\_status

This operation returns information about a job, including where the job is in
the processing pipeline, the status of the results, and the signature value
associated with the job.

Type annotations and code completion for `#!python session.create_client("importexport").get_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.get_status)

```python title="Method definition"
await def get_status(
    self,
    *,
    JobId: str,
    APIVersion: str = ...,
) -> GetStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStatusOutputTypeDef](./type_defs.md#getstatusoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetStatusInputRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_status(**kwargs)
```

1. See [:material-code-braces: GetStatusInputRequestTypeDef](./type_defs.md#getstatusinputrequesttypedef) 

### list\_jobs

This operation returns the jobs associated with the requester.

Type annotations and code completion for `#!python session.create_client("importexport").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.list_jobs)

```python title="Method definition"
await def list_jobs(
    self,
    *,
    MaxJobs: int = ...,
    Marker: str = ...,
    APIVersion: str = ...,
) -> ListJobsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsInputRequestTypeDef = {  # (1)
    "MaxJobs": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsInputRequestTypeDef](./type_defs.md#listjobsinputrequesttypedef) 

### update\_job

You use this operation to change the parameters specified in the original
manifest file by supplying a new manifest file.

Type annotations and code completion for `#!python session.create_client("importexport").update_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.update_job)

```python title="Method definition"
await def update_job(
    self,
    *,
    JobId: str,
    Manifest: str,
    JobType: JobTypeType,  # (1)
    ValidateOnly: bool,
    APIVersion: str = ...,
) -> UpdateJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: UpdateJobOutputTypeDef](./type_defs.md#updatejoboutputtypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateJobInputRequestTypeDef = {  # (1)
    "JobId": ...,
    "Manifest": ...,
    "JobType": ...,
    "ValidateOnly": ...,
}

parent.update_job(**kwargs)
```

1. See [:material-code-braces: UpdateJobInputRequestTypeDef](./type_defs.md#updatejobinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("importexport").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> ImportExportClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("importexport").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("importexport").get_paginator` method with overloads.

- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)



