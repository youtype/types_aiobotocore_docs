# ResourceGroupsTaggingAPIClient

> [Index](../README.md) > [ResourceGroupsTaggingAPI](./README.md) > ResourceGroupsTaggingAPIClient

!!! note ""

    Auto-generated documentation for [ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#resourcegroupstaggingapi)
    type annotations stubs module [types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).

## ResourceGroupsTaggingAPIClient

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client)

```python
# ResourceGroupsTaggingAPIClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("resourcegroupstaggingapi").exceptions` structure.

```python
# ResourceGroupsTaggingAPIClient.exceptions usage example

async with session.create_client("resourcegroupstaggingapi") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConcurrentModificationException,
        client.ConstraintViolationException,
        client.InternalServiceException,
        client.InvalidParameterException,
        client.PaginationTokenExpiredException,
        client.ThrottledException,
    ) as e:
        print(e)
```

```python
# ResourceGroupsTaggingAPIClient usage type checking example

from types_aiobotocore_resourcegroupstaggingapi.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/generate_presigned_url.html)

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


### describe\_report\_creation

Describes the status of the <code>StartReportCreation</code> operation.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").describe_report_creation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/describe_report_creation.html)

```python
# describe_report_creation method definition

await def describe_report_creation(
    self,
) -> DescribeReportCreationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReportCreationOutputTypeDef](./type_defs.md#describereportcreationoutputtypedef) 

### get\_compliance\_summary

Returns a table that shows counts of resources that are noncompliant with their
tag policies.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_compliance_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/get_compliance_summary.html)

```python
# get_compliance_summary method definition

await def get_compliance_summary(
    self,
    *,
    TargetIdFilters: Sequence[str] = ...,
    RegionFilters: Sequence[str] = ...,
    ResourceTypeFilters: Sequence[str] = ...,
    TagKeyFilters: Sequence[str] = ...,
    GroupBy: Sequence[GroupByAttributeType] = ...,  # (1)
    MaxResults: int = ...,
    PaginationToken: str = ...,
) -> GetComplianceSummaryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GroupByAttributeType](./literals.md#groupbyattributetype) 
2. See [:material-code-braces: GetComplianceSummaryOutputTypeDef](./type_defs.md#getcompliancesummaryoutputtypedef) 


```python
# get_compliance_summary method usage example with argument unpacking

kwargs: GetComplianceSummaryInputTypeDef = {  # (1)
    "TargetIdFilters": ...,
}

parent.get_compliance_summary(**kwargs)
```

1. See [:material-code-braces: GetComplianceSummaryInputTypeDef](./type_defs.md#getcompliancesummaryinputtypedef) 

### get\_resources

Returns all the tagged or previously tagged resources that are located in the
specified Amazon Web Services Region for the account.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/get_resources.html)

```python
# get_resources method definition

await def get_resources(
    self,
    *,
    PaginationToken: str = ...,
    TagFilters: Sequence[TagFilterTypeDef] = ...,  # (1)
    ResourcesPerPage: int = ...,
    TagsPerPage: int = ...,
    ResourceTypeFilters: Sequence[str] = ...,
    IncludeComplianceDetails: bool = ...,
    ExcludeCompliantResources: bool = ...,
    ResourceARNList: Sequence[str] = ...,
) -> GetResourcesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: GetResourcesOutputTypeDef](./type_defs.md#getresourcesoutputtypedef) 


```python
# get_resources method usage example with argument unpacking

kwargs: GetResourcesInputTypeDef = {  # (1)
    "PaginationToken": ...,
}

parent.get_resources(**kwargs)
```

1. See [:material-code-braces: GetResourcesInputTypeDef](./type_defs.md#getresourcesinputtypedef) 

### get\_tag\_keys

Returns all tag keys currently in use in the specified Amazon Web Services
Region for the calling account.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_tag_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/get_tag_keys.html)

```python
# get_tag_keys method definition

await def get_tag_keys(
    self,
    *,
    PaginationToken: str = ...,
) -> GetTagKeysOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTagKeysOutputTypeDef](./type_defs.md#gettagkeysoutputtypedef) 


```python
# get_tag_keys method usage example with argument unpacking

kwargs: GetTagKeysInputTypeDef = {  # (1)
    "PaginationToken": ...,
}

parent.get_tag_keys(**kwargs)
```

1. See [:material-code-braces: GetTagKeysInputTypeDef](./type_defs.md#gettagkeysinputtypedef) 

### get\_tag\_values

Returns all tag values for the specified key that are used in the specified
Amazon Web Services Region for the calling account.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_tag_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/get_tag_values.html)

```python
# get_tag_values method definition

await def get_tag_values(
    self,
    *,
    Key: str,
    PaginationToken: str = ...,
) -> GetTagValuesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTagValuesOutputTypeDef](./type_defs.md#gettagvaluesoutputtypedef) 


```python
# get_tag_values method usage example with argument unpacking

kwargs: GetTagValuesInputTypeDef = {  # (1)
    "Key": ...,
}

parent.get_tag_values(**kwargs)
```

1. See [:material-code-braces: GetTagValuesInputTypeDef](./type_defs.md#gettagvaluesinputtypedef) 

### start\_report\_creation

Generates a report that lists all tagged resources in the accounts across your
organization and tells whether each resource is compliant with the effective
tag policy.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").start_report_creation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/start_report_creation.html)

```python
# start_report_creation method definition

await def start_report_creation(
    self,
    *,
    S3Bucket: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_report_creation method usage example with argument unpacking

kwargs: StartReportCreationInputTypeDef = {  # (1)
    "S3Bucket": ...,
}

parent.start_report_creation(**kwargs)
```

1. See [:material-code-braces: StartReportCreationInputTypeDef](./type_defs.md#startreportcreationinputtypedef) 

### tag\_resources

Applies one or more tags to the specified resources.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").tag_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/tag_resources.html)

```python
# tag_resources method definition

await def tag_resources(
    self,
    *,
    ResourceARNList: Sequence[str],
    Tags: Mapping[str, str],
) -> TagResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TagResourcesOutputTypeDef](./type_defs.md#tagresourcesoutputtypedef) 


```python
# tag_resources method usage example with argument unpacking

kwargs: TagResourcesInputTypeDef = {  # (1)
    "ResourceARNList": ...,
    "Tags": ...,
}

parent.tag_resources(**kwargs)
```

1. See [:material-code-braces: TagResourcesInputTypeDef](./type_defs.md#tagresourcesinputtypedef) 

### untag\_resources

Removes the specified tags from the specified resources.

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").untag_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/client/untag_resources.html)

```python
# untag_resources method definition

await def untag_resources(
    self,
    *,
    ResourceARNList: Sequence[str],
    TagKeys: Sequence[str],
) -> UntagResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UntagResourcesOutputTypeDef](./type_defs.md#untagresourcesoutputtypedef) 


```python
# untag_resources method usage example with argument unpacking

kwargs: UntagResourcesInputTypeDef = {  # (1)
    "ResourceARNList": ...,
    "TagKeys": ...,
}

parent.untag_resources(**kwargs)
```

1. See [:material-code-braces: UntagResourcesInputTypeDef](./type_defs.md#untagresourcesinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client)

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

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_paginator` method with overloads.

- `client.get_paginator("get_compliance_summary")` -> [GetComplianceSummaryPaginator](./paginators.md#getcompliancesummarypaginator)
- `client.get_paginator("get_resources")` -> [GetResourcesPaginator](./paginators.md#getresourcespaginator)
- `client.get_paginator("get_tag_keys")` -> [GetTagKeysPaginator](./paginators.md#gettagkeyspaginator)
- `client.get_paginator("get_tag_values")` -> [GetTagValuesPaginator](./paginators.md#gettagvaluespaginator)



