<a id="type-annotations-for-aiobotocore-augmentedairuntime-module"></a>

# Type annotations for aiobotocore AugmentedAIRuntime module

> [Index](..) > AugmentedAIRuntime

Auto-generated documentation for
[AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
type annotations stubs module
[types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[sagemaker-a2i-runtime]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sagemaker-a2i-runtime]'

# standalone installation
pip install types-aiobotocore-sagemaker-a2i-runtime
```

- [Type annotations for aiobotocore AugmentedAIRuntime module](#type-annotations-for-aiobotocore-augmentedairuntime-module)
  - [AugmentedAIRuntimeClient](#augmentedairuntimeclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="augmentedairuntimeclient"></a>

## AugmentedAIRuntimeClient

Type annotations for `session.create_client("sagemaker-a2i-runtime")` as
[AugmentedAIRuntimeClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [delete_human_loop](./client.md#delete_human_loop)
- [describe_human_loop](./client.md#describe_human_loop)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_paginator](./client.md#get_paginator)
- [list_human_loops](./client.md#list_human_loops)
- [start_human_loop](./client.md#start_human_loop)
- [stop_human_loop](./client.md#stop_human_loop)

<a id="exceptions"></a>

### Exceptions

AugmentedAIRuntimeClient [exceptions](./client.md#exceptions)

- ClientError
- ConflictException
- InternalServerException
- ResourceNotFoundException
- ServiceQuotaExceededException
- ThrottlingException
- ValidationException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("sagemaker-a2i-runtime").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_sagemaker_a2i_runtime.paginator import ListHumanLoopsPaginator, ...
```

- [ListHumanLoopsPaginator](./paginators.md#listhumanloopspaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_sagemaker_a2i_runtime.literals import ContentClassifierType, ...
```

- [ContentClassifierType](./literals.md#contentclassifiertype)
- [HumanLoopStatusType](./literals.md#humanloopstatustype)
- [ListHumanLoopsPaginatorName](./literals.md#listhumanloopspaginatorname)
- [SortOrderType](./literals.md#sortordertype)
- [ServiceName](./literals.md#servicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef, ...
```

- [DeleteHumanLoopRequestRequestTypeDef](./type_defs.md#deletehumanlooprequestrequesttypedef)
- [DescribeHumanLoopRequestRequestTypeDef](./type_defs.md#describehumanlooprequestrequesttypedef)
- [DescribeHumanLoopResponseTypeDef](./type_defs.md#describehumanloopresponsetypedef)
- [HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef)
- [HumanLoopInputTypeDef](./type_defs.md#humanloopinputtypedef)
- [HumanLoopOutputTypeDef](./type_defs.md#humanloopoutputtypedef)
- [HumanLoopSummaryTypeDef](./type_defs.md#humanloopsummarytypedef)
- [ListHumanLoopsRequestRequestTypeDef](./type_defs.md#listhumanloopsrequestrequesttypedef)
- [ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartHumanLoopRequestRequestTypeDef](./type_defs.md#starthumanlooprequestrequesttypedef)
- [StartHumanLoopResponseTypeDef](./type_defs.md#starthumanloopresponsetypedef)
- [StopHumanLoopRequestRequestTypeDef](./type_defs.md#stophumanlooprequestrequesttypedef)
