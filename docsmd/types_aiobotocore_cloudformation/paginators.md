# Paginators

> [Index](../README.md) > [CloudFormation](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#cloudformation)
    type annotations stubs module [types-aiobotocore-cloudformation](https://pypi.org/project/types-aiobotocore-cloudformation/).

## DescribeAccountLimitsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("describe_account_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/DescribeAccountLimits.html#CloudFormation.Paginator.DescribeAccountLimits)

```python
# DescribeAccountLimitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeAccountLimitsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
3. item: `AioPageIterator[DescribeAccountLimitsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAccountLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeAccountLimitsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeAccountLimitsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccountLimitsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsInputPaginateTypeDef](./type_defs.md#describeaccountlimitsinputpaginatetypedef)
## DescribeChangeSetPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("describe_change_set")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/DescribeChangeSet.html#CloudFormation.Paginator.DescribeChangeSet)

```python
# DescribeChangeSetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeChangeSetPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: DescribeChangeSetPaginator = client.get_paginator("describe_change_set")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeChangeSetOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [DescribeChangeSetPaginator](./paginators.md#describechangesetpaginator)
3. item: `AioPageIterator[DescribeChangeSetOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeChangeSetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChangeSetName: str,
    StackName: str = ...,
    IncludePropertyValues: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeChangeSetOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeChangeSetOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeChangeSetInputPaginateTypeDef = {  # (1)
    "ChangeSetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeChangeSetInputPaginateTypeDef](./type_defs.md#describechangesetinputpaginatetypedef)
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/DescribeEvents.html#CloudFormation.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: `AioPageIterator[DescribeEventsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str = ...,
    ChangeSetName: str = ...,
    OperationId: str = ...,
    Filters: EventFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeEventsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeEventsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsInputPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsInputPaginateTypeDef](./type_defs.md#describeeventsinputpaginatetypedef)
## DescribeStackEventsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("describe_stack_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/DescribeStackEvents.html#CloudFormation.Paginator.DescribeStackEvents)

```python
# DescribeStackEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeStackEventsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: DescribeStackEventsPaginator = client.get_paginator("describe_stack_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStackEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [DescribeStackEventsPaginator](./paginators.md#describestackeventspaginator)
3. item: `AioPageIterator[DescribeStackEventsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeStackEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeStackEventsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeStackEventsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStackEventsInputPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStackEventsInputPaginateTypeDef](./type_defs.md#describestackeventsinputpaginatetypedef)
## DescribeStacksPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("describe_stacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/DescribeStacks.html#CloudFormation.Paginator.DescribeStacks)

```python
# DescribeStacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeStacksPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: DescribeStacksPaginator = client.get_paginator("describe_stacks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStacksOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [DescribeStacksPaginator](./paginators.md#describestackspaginator)
3. item: `AioPageIterator[DescribeStacksOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeStacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeStacksOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeStacksOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStacksInputPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStacksInputPaginateTypeDef](./type_defs.md#describestacksinputpaginatetypedef)
## ListChangeSetsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_change_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListChangeSets.html#CloudFormation.Paginator.ListChangeSets)

```python
# ListChangeSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListChangeSetsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListChangeSetsPaginator = client.get_paginator("list_change_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListChangeSetsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListChangeSetsPaginator](./paginators.md#listchangesetspaginator)
3. item: `AioPageIterator[ListChangeSetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListChangeSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListChangeSetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListChangeSetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListChangeSetsInputPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChangeSetsInputPaginateTypeDef](./type_defs.md#listchangesetsinputpaginatetypedef)
## ListExportsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListExports.html#CloudFormation.Paginator.ListExports)

```python
# ListExportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListExportsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListExportsPaginator = client.get_paginator("list_exports")  # (2)
    async for item in paginator.paginate(...):
        item: ListExportsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListExportsPaginator](./paginators.md#listexportspaginator)
3. item: `AioPageIterator[ListExportsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListExportsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListExportsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListExportsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExportsInputPaginateTypeDef](./type_defs.md#listexportsinputpaginatetypedef)
## ListGeneratedTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_generated_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListGeneratedTemplates.html#CloudFormation.Paginator.ListGeneratedTemplates)

```python
# ListGeneratedTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListGeneratedTemplatesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListGeneratedTemplatesPaginator = client.get_paginator("list_generated_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListGeneratedTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListGeneratedTemplatesPaginator](./paginators.md#listgeneratedtemplatespaginator)
3. item: `AioPageIterator[ListGeneratedTemplatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGeneratedTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGeneratedTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGeneratedTemplatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGeneratedTemplatesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeneratedTemplatesInputPaginateTypeDef](./type_defs.md#listgeneratedtemplatesinputpaginatetypedef)
## ListImportsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_imports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListImports.html#CloudFormation.Paginator.ListImports)

```python
# ListImportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListImportsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListImportsPaginator = client.get_paginator("list_imports")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListImportsPaginator](./paginators.md#listimportspaginator)
3. item: `AioPageIterator[ListImportsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListImportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ExportName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListImportsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListImportsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListImportsInputPaginateTypeDef = {  # (1)
    "ExportName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportsInputPaginateTypeDef](./type_defs.md#listimportsinputpaginatetypedef)
## ListResourceScanRelatedResourcesPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_resource_scan_related_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListResourceScanRelatedResources.html#CloudFormation.Paginator.ListResourceScanRelatedResources)

```python
# ListResourceScanRelatedResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListResourceScanRelatedResourcesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListResourceScanRelatedResourcesPaginator = client.get_paginator("list_resource_scan_related_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceScanRelatedResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListResourceScanRelatedResourcesPaginator](./paginators.md#listresourcescanrelatedresourcespaginator)
3. item: `AioPageIterator[ListResourceScanRelatedResourcesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResourceScanRelatedResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceScanId: str,
    Resources: Sequence[ScannedResourceIdentifierTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListResourceScanRelatedResourcesOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[ScannedResourceIdentifierTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListResourceScanRelatedResourcesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceScanRelatedResourcesInputPaginateTypeDef = {  # (1)
    "ResourceScanId": ...,
    "Resources": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceScanRelatedResourcesInputPaginateTypeDef](./type_defs.md#listresourcescanrelatedresourcesinputpaginatetypedef)
## ListResourceScanResourcesPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_resource_scan_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListResourceScanResources.html#CloudFormation.Paginator.ListResourceScanResources)

```python
# ListResourceScanResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListResourceScanResourcesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListResourceScanResourcesPaginator = client.get_paginator("list_resource_scan_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceScanResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListResourceScanResourcesPaginator](./paginators.md#listresourcescanresourcespaginator)
3. item: `AioPageIterator[ListResourceScanResourcesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResourceScanResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceScanId: str,
    ResourceIdentifier: str = ...,
    ResourceTypePrefix: str = ...,
    TagKey: str = ...,
    TagValue: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListResourceScanResourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListResourceScanResourcesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceScanResourcesInputPaginateTypeDef = {  # (1)
    "ResourceScanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceScanResourcesInputPaginateTypeDef](./type_defs.md#listresourcescanresourcesinputpaginatetypedef)
## ListResourceScansPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_resource_scans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListResourceScans.html#CloudFormation.Paginator.ListResourceScans)

```python
# ListResourceScansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListResourceScansPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListResourceScansPaginator = client.get_paginator("list_resource_scans")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceScansOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListResourceScansPaginator](./paginators.md#listresourcescanspaginator)
3. item: `AioPageIterator[ListResourceScansOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResourceScansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ScanTypeFilter: ScanTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListResourceScansOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListResourceScansOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceScansInputPaginateTypeDef = {  # (1)
    "ScanTypeFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceScansInputPaginateTypeDef](./type_defs.md#listresourcescansinputpaginatetypedef)
## ListStackInstancesPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stack_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStackInstances.html#CloudFormation.Paginator.ListStackInstances)

```python
# ListStackInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackInstancesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStackInstancesPaginator = client.get_paginator("list_stack_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListStackInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStackInstancesPaginator](./paginators.md#liststackinstancespaginator)
3. item: `AioPageIterator[ListStackInstancesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStackInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackSetName: str,
    Filters: Sequence[StackInstanceFilterTypeDef] = ...,  # (1)
    StackInstanceAccount: str = ...,
    StackInstanceRegion: str = ...,
    CallAs: CallAsType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListStackInstancesOutputTypeDef]:  # (4)
    ...
```

1. See `Sequence[StackInstanceFilterTypeDef]`
2. See [:material-code-brackets: CallAsType](./literals.md#callastype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListStackInstancesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStackInstancesInputPaginateTypeDef = {  # (1)
    "StackSetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStackInstancesInputPaginateTypeDef](./type_defs.md#liststackinstancesinputpaginatetypedef)
## ListStackRefactorActionsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stack_refactor_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStackRefactorActions.html#CloudFormation.Paginator.ListStackRefactorActions)

```python
# ListStackRefactorActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackRefactorActionsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStackRefactorActionsPaginator = client.get_paginator("list_stack_refactor_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListStackRefactorActionsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStackRefactorActionsPaginator](./paginators.md#liststackrefactoractionspaginator)
3. item: `AioPageIterator[ListStackRefactorActionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStackRefactorActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackRefactorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStackRefactorActionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStackRefactorActionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStackRefactorActionsInputPaginateTypeDef = {  # (1)
    "StackRefactorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStackRefactorActionsInputPaginateTypeDef](./type_defs.md#liststackrefactoractionsinputpaginatetypedef)
## ListStackRefactorsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stack_refactors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStackRefactors.html#CloudFormation.Paginator.ListStackRefactors)

```python
# ListStackRefactorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackRefactorsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStackRefactorsPaginator = client.get_paginator("list_stack_refactors")  # (2)
    async for item in paginator.paginate(...):
        item: ListStackRefactorsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStackRefactorsPaginator](./paginators.md#liststackrefactorspaginator)
3. item: `AioPageIterator[ListStackRefactorsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStackRefactorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ExecutionStatusFilter: Sequence[StackRefactorExecutionStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListStackRefactorsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[StackRefactorExecutionStatusType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListStackRefactorsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStackRefactorsInputPaginateTypeDef = {  # (1)
    "ExecutionStatusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStackRefactorsInputPaginateTypeDef](./type_defs.md#liststackrefactorsinputpaginatetypedef)
## ListStackResourcesPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stack_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStackResources.html#CloudFormation.Paginator.ListStackResources)

```python
# ListStackResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackResourcesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStackResourcesPaginator = client.get_paginator("list_stack_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListStackResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStackResourcesPaginator](./paginators.md#liststackresourcespaginator)
3. item: `AioPageIterator[ListStackResourcesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStackResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStackResourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStackResourcesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStackResourcesInputPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStackResourcesInputPaginateTypeDef](./type_defs.md#liststackresourcesinputpaginatetypedef)
## ListStackSetOperationResultsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stack_set_operation_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStackSetOperationResults.html#CloudFormation.Paginator.ListStackSetOperationResults)

```python
# ListStackSetOperationResultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackSetOperationResultsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStackSetOperationResultsPaginator = client.get_paginator("list_stack_set_operation_results")  # (2)
    async for item in paginator.paginate(...):
        item: ListStackSetOperationResultsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStackSetOperationResultsPaginator](./paginators.md#liststacksetoperationresultspaginator)
3. item: `AioPageIterator[ListStackSetOperationResultsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStackSetOperationResultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackSetName: str,
    OperationId: str,
    CallAs: CallAsType = ...,  # (1)
    Filters: Sequence[OperationResultFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListStackSetOperationResultsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: CallAsType](./literals.md#callastype)
2. See `Sequence[OperationResultFilterTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListStackSetOperationResultsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStackSetOperationResultsInputPaginateTypeDef = {  # (1)
    "StackSetName": ...,
    "OperationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStackSetOperationResultsInputPaginateTypeDef](./type_defs.md#liststacksetoperationresultsinputpaginatetypedef)
## ListStackSetOperationsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stack_set_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStackSetOperations.html#CloudFormation.Paginator.ListStackSetOperations)

```python
# ListStackSetOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackSetOperationsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStackSetOperationsPaginator = client.get_paginator("list_stack_set_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListStackSetOperationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStackSetOperationsPaginator](./paginators.md#liststacksetoperationspaginator)
3. item: `AioPageIterator[ListStackSetOperationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStackSetOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackSetName: str,
    CallAs: CallAsType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListStackSetOperationsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CallAsType](./literals.md#callastype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListStackSetOperationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStackSetOperationsInputPaginateTypeDef = {  # (1)
    "StackSetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStackSetOperationsInputPaginateTypeDef](./type_defs.md#liststacksetoperationsinputpaginatetypedef)
## ListStackSetsPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stack_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStackSets.html#CloudFormation.Paginator.ListStackSets)

```python
# ListStackSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackSetsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStackSetsPaginator = client.get_paginator("list_stack_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListStackSetsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStackSetsPaginator](./paginators.md#liststacksetspaginator)
3. item: `AioPageIterator[ListStackSetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStackSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: StackSetStatusType = ...,  # (1)
    CallAs: CallAsType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListStackSetsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: StackSetStatusType](./literals.md#stacksetstatustype)
2. See [:material-code-brackets: CallAsType](./literals.md#callastype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListStackSetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStackSetsInputPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStackSetsInputPaginateTypeDef](./type_defs.md#liststacksetsinputpaginatetypedef)
## ListStacksPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_stacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListStacks.html#CloudFormation.Paginator.ListStacks)

```python
# ListStacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStacksPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListStacksPaginator = client.get_paginator("list_stacks")  # (2)
    async for item in paginator.paginate(...):
        item: ListStacksOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListStacksPaginator](./paginators.md#liststackspaginator)
3. item: `AioPageIterator[ListStacksOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackStatusFilter: Sequence[StackStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListStacksOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[StackStatusType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListStacksOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStacksInputPaginateTypeDef = {  # (1)
    "StackStatusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStacksInputPaginateTypeDef](./type_defs.md#liststacksinputpaginatetypedef)
## ListTypesPaginator

Type annotations and code completion for `#!python session.create_client("cloudformation").get_paginator("list_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation/paginator/ListTypes.html#CloudFormation.Paginator.ListTypes)

```python
# ListTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListTypesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:  # (1)
    paginator: ListTypesPaginator = client.get_paginator("list_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListTypesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudFormationClient](./client.md)
2. paginator: [ListTypesPaginator](./paginators.md#listtypespaginator)
3. item: `AioPageIterator[ListTypesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Visibility: VisibilityType = ...,  # (1)
    ProvisioningType: ProvisioningTypeType = ...,  # (2)
    DeprecatedStatus: DeprecatedStatusType = ...,  # (3)
    Type: RegistryTypeType = ...,  # (4)
    Filters: TypeFiltersTypeDef = ...,  # (5)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> aiobotocore.paginate.AioPageIterator[ListTypesOutputTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype)
2. See [:material-code-brackets: ProvisioningTypeType](./literals.md#provisioningtypetype)
3. See [:material-code-brackets: DeprecatedStatusType](./literals.md#deprecatedstatustype)
4. See [:material-code-brackets: RegistryTypeType](./literals.md#registrytypetype)
5. See [:material-code-braces: TypeFiltersTypeDef](./type_defs.md#typefilterstypedef)
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
7. See `AioPageIterator[ListTypesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTypesInputPaginateTypeDef = {  # (1)
    "Visibility": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTypesInputPaginateTypeDef](./type_defs.md#listtypesinputpaginatetypedef)
