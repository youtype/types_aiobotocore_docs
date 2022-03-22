<a id="paginators-for-aiobotocore-cloudformation-module"></a>

# Paginators for aiobotocore CloudFormation module

> [Index](../README.md) > [CloudFormation](./README.md) > Paginators

Auto-generated documentation for
[CloudFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
type annotations stubs module
[types-aiobotocore-cloudformation](https://pypi.org/project/types-aiobotocore-cloudformation/).

- [Paginators for aiobotocore CloudFormation module](#paginators-for-aiobotocore-cloudformation-module)
  - [DescribeAccountLimitsPaginator](#describeaccountlimitspaginator)
  - [DescribeChangeSetPaginator](#describechangesetpaginator)
  - [DescribeStackEventsPaginator](#describestackeventspaginator)
  - [DescribeStacksPaginator](#describestackspaginator)
  - [ListChangeSetsPaginator](#listchangesetspaginator)
  - [ListExportsPaginator](#listexportspaginator)
  - [ListImportsPaginator](#listimportspaginator)
  - [ListStackInstancesPaginator](#liststackinstancespaginator)
  - [ListStackResourcesPaginator](#liststackresourcespaginator)
  - [ListStackSetOperationResultsPaginator](#liststacksetoperationresultspaginator)
  - [ListStackSetOperationsPaginator](#liststacksetoperationspaginator)
  - [ListStackSetsPaginator](#liststacksetspaginator)
  - [ListStacksPaginator](#liststackspaginator)
  - [ListTypesPaginator](#listtypespaginator)

<a id="describeaccountlimitspaginator"></a>

## DescribeAccountLimitsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("describe_account_limits")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeAccountLimitsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
```

Boto3 documentation:
[CloudFormation.Paginator.DescribeAccountLimits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)

Arguments for `DescribeAccountLimitsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAccountLimitsPaginator.paginate` returns
`AsyncIterator`\[[DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef)\].

<a id="describechangesetpaginator"></a>

## DescribeChangeSetPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("describe_change_set")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeChangeSetPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: DescribeChangeSetPaginator = client.get_paginator("describe_change_set")
```

Boto3 documentation:
[CloudFormation.Paginator.DescribeChangeSet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet)

Arguments for `DescribeChangeSetPaginator.paginate` method:

- `ChangeSetName`: `str` *(required)*
- `StackName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeChangeSetPaginator.paginate` returns
`AsyncIterator`\[[DescribeChangeSetOutputTypeDef](./type_defs.md#describechangesetoutputtypedef)\].

<a id="describestackeventspaginator"></a>

## DescribeStackEventsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("describe_stack_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeStackEventsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: DescribeStackEventsPaginator = client.get_paginator("describe_stack_events")
```

Boto3 documentation:
[CloudFormation.Paginator.DescribeStackEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)

Arguments for `DescribeStackEventsPaginator.paginate` method:

- `StackName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeStackEventsPaginator.paginate` returns
`AsyncIterator`\[[DescribeStackEventsOutputTypeDef](./type_defs.md#describestackeventsoutputtypedef)\].

<a id="describestackspaginator"></a>

## DescribeStacksPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("describe_stacks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import DescribeStacksPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: DescribeStacksPaginator = client.get_paginator("describe_stacks")
```

Boto3 documentation:
[CloudFormation.Paginator.DescribeStacks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)

Arguments for `DescribeStacksPaginator.paginate` method:

- `StackName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeStacksPaginator.paginate` returns
`AsyncIterator`\[[DescribeStacksOutputTypeDef](./type_defs.md#describestacksoutputtypedef)\].

<a id="listchangesetspaginator"></a>

## ListChangeSetsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_change_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListChangeSetsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListChangeSetsPaginator = client.get_paginator("list_change_sets")
```

Boto3 documentation:
[CloudFormation.Paginator.ListChangeSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)

Arguments for `ListChangeSetsPaginator.paginate` method:

- `StackName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChangeSetsPaginator.paginate` returns
`AsyncIterator`\[[ListChangeSetsOutputTypeDef](./type_defs.md#listchangesetsoutputtypedef)\].

<a id="listexportspaginator"></a>

## ListExportsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_exports")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListExportsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListExportsPaginator = client.get_paginator("list_exports")
```

Boto3 documentation:
[CloudFormation.Paginator.ListExports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)

Arguments for `ListExportsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListExportsPaginator.paginate` returns
`AsyncIterator`\[[ListExportsOutputTypeDef](./type_defs.md#listexportsoutputtypedef)\].

<a id="listimportspaginator"></a>

## ListImportsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_imports")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListImportsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListImportsPaginator = client.get_paginator("list_imports")
```

Boto3 documentation:
[CloudFormation.Paginator.ListImports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)

Arguments for `ListImportsPaginator.paginate` method:

- `ExportName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListImportsPaginator.paginate` returns
`AsyncIterator`\[[ListImportsOutputTypeDef](./type_defs.md#listimportsoutputtypedef)\].

<a id="liststackinstancespaginator"></a>

## ListStackInstancesPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_stack_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackInstancesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListStackInstancesPaginator = client.get_paginator("list_stack_instances")
```

Boto3 documentation:
[CloudFormation.Paginator.ListStackInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances)

Arguments for `ListStackInstancesPaginator.paginate` method:

- `StackSetName`: `str` *(required)*
- `Filters`:
  `Sequence`\[[StackInstanceFilterTypeDef](./type_defs.md#stackinstancefiltertypedef)\]
- `StackInstanceAccount`: `str`
- `StackInstanceRegion`: `str`
- `CallAs`: [CallAsType](./literals.md#callastype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStackInstancesPaginator.paginate` returns
`AsyncIterator`\[[ListStackInstancesOutputTypeDef](./type_defs.md#liststackinstancesoutputtypedef)\].

<a id="liststackresourcespaginator"></a>

## ListStackResourcesPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_stack_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackResourcesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListStackResourcesPaginator = client.get_paginator("list_stack_resources")
```

Boto3 documentation:
[CloudFormation.Paginator.ListStackResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)

Arguments for `ListStackResourcesPaginator.paginate` method:

- `StackName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStackResourcesPaginator.paginate` returns
`AsyncIterator`\[[ListStackResourcesOutputTypeDef](./type_defs.md#liststackresourcesoutputtypedef)\].

<a id="liststacksetoperationresultspaginator"></a>

## ListStackSetOperationResultsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_stack_set_operation_results")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackSetOperationResultsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListStackSetOperationResultsPaginator = client.get_paginator("list_stack_set_operation_results")
```

Boto3 documentation:
[CloudFormation.Paginator.ListStackSetOperationResults](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults)

Arguments for `ListStackSetOperationResultsPaginator.paginate` method:

- `StackSetName`: `str` *(required)*
- `OperationId`: `str` *(required)*
- `CallAs`: [CallAsType](./literals.md#callastype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStackSetOperationResultsPaginator.paginate` returns
`AsyncIterator`\[[ListStackSetOperationResultsOutputTypeDef](./type_defs.md#liststacksetoperationresultsoutputtypedef)\].

<a id="liststacksetoperationspaginator"></a>

## ListStackSetOperationsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_stack_set_operations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackSetOperationsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListStackSetOperationsPaginator = client.get_paginator("list_stack_set_operations")
```

Boto3 documentation:
[CloudFormation.Paginator.ListStackSetOperations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations)

Arguments for `ListStackSetOperationsPaginator.paginate` method:

- `StackSetName`: `str` *(required)*
- `CallAs`: [CallAsType](./literals.md#callastype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStackSetOperationsPaginator.paginate` returns
`AsyncIterator`\[[ListStackSetOperationsOutputTypeDef](./type_defs.md#liststacksetoperationsoutputtypedef)\].

<a id="liststacksetspaginator"></a>

## ListStackSetsPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_stack_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStackSetsPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListStackSetsPaginator = client.get_paginator("list_stack_sets")
```

Boto3 documentation:
[CloudFormation.Paginator.ListStackSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets)

Arguments for `ListStackSetsPaginator.paginate` method:

- `Status`: [StackSetStatusType](./literals.md#stacksetstatustype)
- `CallAs`: [CallAsType](./literals.md#callastype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStackSetsPaginator.paginate` returns
`AsyncIterator`\[[ListStackSetsOutputTypeDef](./type_defs.md#liststacksetsoutputtypedef)\].

<a id="liststackspaginator"></a>

## ListStacksPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_stacks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListStacksPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListStacksPaginator = client.get_paginator("list_stacks")
```

Boto3 documentation:
[CloudFormation.Paginator.ListStacks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks)

Arguments for `ListStacksPaginator.paginate` method:

- `StackStatusFilter`:
  `Sequence`\[[StackStatusType](./literals.md#stackstatustype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStacksPaginator.paginate` returns
`AsyncIterator`\[[ListStacksOutputTypeDef](./type_defs.md#liststacksoutputtypedef)\].

<a id="listtypespaginator"></a>

## ListTypesPaginator

Type annotations for
`session.create_client("cloudformation").get_paginator("list_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudformation.paginator import ListTypesPaginator

session = get_session()
async with session.create_client("cloudformation") as client:
    client: CloudFormationClient
    paginator: ListTypesPaginator = client.get_paginator("list_types")
```

Boto3 documentation:
[CloudFormation.Paginator.ListTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes)

Arguments for `ListTypesPaginator.paginate` method:

- `Visibility`: [VisibilityType](./literals.md#visibilitytype)
- `ProvisioningType`:
  [ProvisioningTypeType](./literals.md#provisioningtypetype)
- `DeprecatedStatus`:
  [DeprecatedStatusType](./literals.md#deprecatedstatustype)
- `Type`: [RegistryTypeType](./literals.md#registrytypetype)
- `Filters`: [TypeFiltersTypeDef](./type_defs.md#typefilterstypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTypesPaginator.paginate` returns
`AsyncIterator`\[[ListTypesOutputTypeDef](./type_defs.md#listtypesoutputtypedef)\].
