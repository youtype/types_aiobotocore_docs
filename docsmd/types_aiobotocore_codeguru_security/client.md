# CodeGuruSecurityClient

> [Index](../README.md) > [CodeGuruSecurity](./README.md) > CodeGuruSecurityClient

!!! note ""

    Auto-generated documentation for [CodeGuruSecurity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#codegurusecurity)
    type annotations stubs module [types-aiobotocore-codeguru-security](https://pypi.org/project/types-aiobotocore-codeguru-security/).

## CodeGuruSecurityClient

Type annotations and code completion for `#!python session.create_client("codeguru-security")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client)

```python
# CodeGuruSecurityClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_codeguru_security.client import CodeGuruSecurityClient

session = get_session()
async with session.create_client("codeguru-security") as client:
    client: CodeGuruSecurityClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("codeguru-security").exceptions` structure.

```python
# CodeGuruSecurityClient.exceptions usage example

async with session.create_client("codeguru-security") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CodeGuruSecurityClient usage type checking example

from types_aiobotocore_codeguru_security.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("codeguru-security").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("codeguru-security").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("codeguru-security").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### batch\_get\_findings

Returns a list of requested findings from standard scans.

Type annotations and code completion for `#!python session.create_client("codeguru-security").batch_get_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/batch_get_findings.html)

```python
# batch_get_findings method definition

await def batch_get_findings(
    self,
    *,
    findingIdentifiers: Sequence[FindingIdentifierTypeDef],  # (1)
) -> BatchGetFindingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FindingIdentifierTypeDef](./type_defs.md#findingidentifiertypedef) 
2. See [:material-code-braces: BatchGetFindingsResponseTypeDef](./type_defs.md#batchgetfindingsresponsetypedef) 


```python
# batch_get_findings method usage example with argument unpacking

kwargs: BatchGetFindingsRequestRequestTypeDef = {  # (1)
    "findingIdentifiers": ...,
}

parent.batch_get_findings(**kwargs)
```

1. See [:material-code-braces: BatchGetFindingsRequestRequestTypeDef](./type_defs.md#batchgetfindingsrequestrequesttypedef) 

### create\_scan

Use to create a scan using code uploaded to an Amazon S3 bucket.

Type annotations and code completion for `#!python session.create_client("codeguru-security").create_scan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/create_scan.html)

```python
# create_scan method definition

await def create_scan(
    self,
    *,
    resourceId: ResourceIdTypeDef,  # (1)
    scanName: str,
    analysisType: AnalysisTypeType = ...,  # (2)
    clientToken: str = ...,
    scanType: ScanTypeType = ...,  # (3)
    tags: Mapping[str, str] = ...,
) -> CreateScanResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ResourceIdTypeDef](./type_defs.md#resourceidtypedef) 
2. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
3. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
4. See [:material-code-braces: CreateScanResponseTypeDef](./type_defs.md#createscanresponsetypedef) 


```python
# create_scan method usage example with argument unpacking

kwargs: CreateScanRequestRequestTypeDef = {  # (1)
    "resourceId": ...,
    "scanName": ...,
}

parent.create_scan(**kwargs)
```

1. See [:material-code-braces: CreateScanRequestRequestTypeDef](./type_defs.md#createscanrequestrequesttypedef) 

### create\_upload\_url

Generates a pre-signed URL, request headers used to upload a code resource, and
code artifact identifier for the uploaded resource.

Type annotations and code completion for `#!python session.create_client("codeguru-security").create_upload_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/create_upload_url.html)

```python
# create_upload_url method definition

await def create_upload_url(
    self,
    *,
    scanName: str,
) -> CreateUploadUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateUploadUrlResponseTypeDef](./type_defs.md#createuploadurlresponsetypedef) 


```python
# create_upload_url method usage example with argument unpacking

kwargs: CreateUploadUrlRequestRequestTypeDef = {  # (1)
    "scanName": ...,
}

parent.create_upload_url(**kwargs)
```

1. See [:material-code-braces: CreateUploadUrlRequestRequestTypeDef](./type_defs.md#createuploadurlrequestrequesttypedef) 

### get\_account\_configuration

Use to get the encryption configuration for an account.

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/get_account_configuration.html)

```python
# get_account_configuration method definition

await def get_account_configuration(
    self,
) -> GetAccountConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountConfigurationResponseTypeDef](./type_defs.md#getaccountconfigurationresponsetypedef) 

### get\_findings

Returns a list of all findings generated by a particular scan.

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/get_findings.html)

```python
# get_findings method definition

await def get_findings(
    self,
    *,
    scanName: str,
    maxResults: int = ...,
    nextToken: str = ...,
    status: StatusType = ...,  # (1)
) -> GetFindingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


```python
# get_findings method usage example with argument unpacking

kwargs: GetFindingsRequestRequestTypeDef = {  # (1)
    "scanName": ...,
}

parent.get_findings(**kwargs)
```

1. See [:material-code-braces: GetFindingsRequestRequestTypeDef](./type_defs.md#getfindingsrequestrequesttypedef) 

### get\_metrics\_summary

Returns a summary of metrics for an account from a specified date, including
number of open findings, the categories with most findings, the scans with most
open findings, and scans with most open critical findings.

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_metrics_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/get_metrics_summary.html)

```python
# get_metrics_summary method definition

await def get_metrics_summary(
    self,
    *,
    date: TimestampTypeDef,
) -> GetMetricsSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMetricsSummaryResponseTypeDef](./type_defs.md#getmetricssummaryresponsetypedef) 


```python
# get_metrics_summary method usage example with argument unpacking

kwargs: GetMetricsSummaryRequestRequestTypeDef = {  # (1)
    "date": ...,
}

parent.get_metrics_summary(**kwargs)
```

1. See [:material-code-braces: GetMetricsSummaryRequestRequestTypeDef](./type_defs.md#getmetricssummaryrequestrequesttypedef) 

### get\_scan

Returns details about a scan, including whether or not a scan has completed.

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_scan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/get_scan.html)

```python
# get_scan method definition

await def get_scan(
    self,
    *,
    scanName: str,
    runId: str = ...,
) -> GetScanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetScanResponseTypeDef](./type_defs.md#getscanresponsetypedef) 


```python
# get_scan method usage example with argument unpacking

kwargs: GetScanRequestRequestTypeDef = {  # (1)
    "scanName": ...,
}

parent.get_scan(**kwargs)
```

1. See [:material-code-braces: GetScanRequestRequestTypeDef](./type_defs.md#getscanrequestrequesttypedef) 

### list\_findings\_metrics

Returns metrics about all findings in an account within a specified time range.

Type annotations and code completion for `#!python session.create_client("codeguru-security").list_findings_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/list_findings_metrics.html)

```python
# list_findings_metrics method definition

await def list_findings_metrics(
    self,
    *,
    endDate: TimestampTypeDef,
    startDate: TimestampTypeDef,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFindingsMetricsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFindingsMetricsResponseTypeDef](./type_defs.md#listfindingsmetricsresponsetypedef) 


```python
# list_findings_metrics method usage example with argument unpacking

kwargs: ListFindingsMetricsRequestRequestTypeDef = {  # (1)
    "endDate": ...,
    "startDate": ...,
}

parent.list_findings_metrics(**kwargs)
```

1. See [:material-code-braces: ListFindingsMetricsRequestRequestTypeDef](./type_defs.md#listfindingsmetricsrequestrequesttypedef) 

### list\_scans

Returns a list of all scans in an account.

Type annotations and code completion for `#!python session.create_client("codeguru-security").list_scans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/list_scans.html)

```python
# list_scans method definition

await def list_scans(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListScansResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScansResponseTypeDef](./type_defs.md#listscansresponsetypedef) 


```python
# list_scans method usage example with argument unpacking

kwargs: ListScansRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_scans(**kwargs)
```

1. See [:material-code-braces: ListScansRequestRequestTypeDef](./type_defs.md#listscansrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of all tags associated with a scan.

Type annotations and code completion for `#!python session.create_client("codeguru-security").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Use to add one or more tags to an existing scan.

Type annotations and code completion for `#!python session.create_client("codeguru-security").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/tag_resource.html)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Use to remove one or more tags from an existing scan.

Type annotations and code completion for `#!python session.create_client("codeguru-security").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/untag_resource.html)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_account\_configuration

Use to update the encryption configuration for an account.

Type annotations and code completion for `#!python session.create_client("codeguru-security").update_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security/client/update_account_configuration.html)

```python
# update_account_configuration method definition

await def update_account_configuration(
    self,
    *,
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
) -> UpdateAccountConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
2. See [:material-code-braces: UpdateAccountConfigurationResponseTypeDef](./type_defs.md#updateaccountconfigurationresponsetypedef) 


```python
# update_account_configuration method usage example with argument unpacking

kwargs: UpdateAccountConfigurationRequestRequestTypeDef = {  # (1)
    "encryptionConfig": ...,
}

parent.update_account_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateAccountConfigurationRequestRequestTypeDef](./type_defs.md#updateaccountconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("codeguru-security").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CodeGuruSecurityClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("codeguru-security").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client)

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

Type annotations and code completion for `#!python session.create_client("codeguru-security").get_paginator` method with overloads.

- `client.get_paginator("get_findings")` -> [GetFindingsPaginator](./paginators.md#getfindingspaginator)
- `client.get_paginator("list_findings_metrics")` -> [ListFindingsMetricsPaginator](./paginators.md#listfindingsmetricspaginator)
- `client.get_paginator("list_scans")` -> [ListScansPaginator](./paginators.md#listscanspaginator)



