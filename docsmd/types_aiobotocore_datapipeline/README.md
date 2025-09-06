# DataPipeline module

> [Index](../README.md) > DataPipeline


!!! note ""

    Auto-generated documentation for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#datapipeline)
    type annotations stubs module [types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DataPipeline` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DataPipeline` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[datapipeline]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[datapipeline]'

# standalone installation
python -m pip install types-aiobotocore-datapipeline
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-datapipeline
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DataPipelineClient

Type annotations and code completion for  `#!python session.create_client("datapipeline")` as [DataPipelineClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client)

```python
# DataPipelineClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_datapipeline.client import DataPipelineClient


session = get_session()
async with session.create_client("datapipeline") as client:
    client: DataPipelineClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("datapipeline").get_paginator("...")`.

```python
# DescribeObjectsPaginator usage example

from types_aiobotocore_datapipeline.paginator import DescribeObjectsPaginator

def get_describe_objects_paginator() -> DescribeObjectsPaginator:
    return client.get_paginator("describe_objects"))
```

- [DescribeObjectsPaginator](./paginators.md#describeobjectspaginator)
- [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- [QueryObjectsPaginator](./paginators.md#queryobjectspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DescribeObjectsPaginatorName usage example

from types_aiobotocore_datapipeline.literals import DescribeObjectsPaginatorName

def get_value() -> DescribeObjectsPaginatorName:
    return "describe_objects"
```

- [DescribeObjectsPaginatorName](./literals.md#describeobjectspaginatorname)
- [ListPipelinesPaginatorName](./literals.md#listpipelinespaginatorname)
- [OperatorTypeType](./literals.md#operatortypetype)
- [QueryObjectsPaginatorName](./literals.md#queryobjectspaginatorname)
- [TaskStatusType](./literals.md#taskstatustype)
- [DataPipelineServiceName](./literals.md#datapipelineservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeactivatePipelineInputTypeDef](./type_defs.md#deactivatepipelineinputtypedef)
- [DeletePipelineInputTypeDef](./type_defs.md#deletepipelineinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeObjectsInputTypeDef](./type_defs.md#describeobjectsinputtypedef)
- [DescribePipelinesInputTypeDef](./type_defs.md#describepipelinesinputtypedef)
- [EvaluateExpressionInputTypeDef](./type_defs.md#evaluateexpressioninputtypedef)
- [FieldTypeDef](./type_defs.md#fieldtypedef)
- [GetPipelineDefinitionInputTypeDef](./type_defs.md#getpipelinedefinitioninputtypedef)
- [InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef)
- [ListPipelinesInputTypeDef](./type_defs.md#listpipelinesinputtypedef)
- [PipelineIdNameTypeDef](./type_defs.md#pipelineidnametypedef)
- [OperatorTypeDef](./type_defs.md#operatortypedef)
- [ParameterAttributeTypeDef](./type_defs.md#parameterattributetypedef)
- [ValidationErrorTypeDef](./type_defs.md#validationerrortypedef)
- [ValidationWarningTypeDef](./type_defs.md#validationwarningtypedef)
- [RemoveTagsInputTypeDef](./type_defs.md#removetagsinputtypedef)
- [ReportTaskRunnerHeartbeatInputTypeDef](./type_defs.md#reporttaskrunnerheartbeatinputtypedef)
- [SetStatusInputTypeDef](./type_defs.md#setstatusinputtypedef)
- [SetTaskStatusInputTypeDef](./type_defs.md#settaskstatusinputtypedef)
- [ActivatePipelineInputTypeDef](./type_defs.md#activatepipelineinputtypedef)
- [AddTagsInputTypeDef](./type_defs.md#addtagsinputtypedef)
- [CreatePipelineInputTypeDef](./type_defs.md#createpipelineinputtypedef)
- [CreatePipelineOutputTypeDef](./type_defs.md#createpipelineoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EvaluateExpressionOutputTypeDef](./type_defs.md#evaluateexpressionoutputtypedef)
- [QueryObjectsOutputTypeDef](./type_defs.md#queryobjectsoutputtypedef)
- [ReportTaskProgressOutputTypeDef](./type_defs.md#reporttaskprogressoutputtypedef)
- [ReportTaskRunnerHeartbeatOutputTypeDef](./type_defs.md#reporttaskrunnerheartbeatoutputtypedef)
- [DescribeObjectsInputPaginateTypeDef](./type_defs.md#describeobjectsinputpaginatetypedef)
- [ListPipelinesInputPaginateTypeDef](./type_defs.md#listpipelinesinputpaginatetypedef)
- [PipelineDescriptionTypeDef](./type_defs.md#pipelinedescriptiontypedef)
- [PipelineObjectOutputTypeDef](./type_defs.md#pipelineobjectoutputtypedef)
- [PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef)
- [ReportTaskProgressInputTypeDef](./type_defs.md#reporttaskprogressinputtypedef)
- [PollForTaskInputTypeDef](./type_defs.md#pollfortaskinputtypedef)
- [ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef)
- [SelectorTypeDef](./type_defs.md#selectortypedef)
- [ParameterObjectOutputTypeDef](./type_defs.md#parameterobjectoutputtypedef)
- [ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef)
- [PutPipelineDefinitionOutputTypeDef](./type_defs.md#putpipelinedefinitionoutputtypedef)
- [ValidatePipelineDefinitionOutputTypeDef](./type_defs.md#validatepipelinedefinitionoutputtypedef)
- [DescribePipelinesOutputTypeDef](./type_defs.md#describepipelinesoutputtypedef)
- [DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef)
- [TaskObjectTypeDef](./type_defs.md#taskobjecttypedef)
- [PipelineObjectUnionTypeDef](./type_defs.md#pipelineobjectuniontypedef)
- [QueryTypeDef](./type_defs.md#querytypedef)
- [GetPipelineDefinitionOutputTypeDef](./type_defs.md#getpipelinedefinitionoutputtypedef)
- [ParameterObjectUnionTypeDef](./type_defs.md#parameterobjectuniontypedef)
- [PollForTaskOutputTypeDef](./type_defs.md#pollfortaskoutputtypedef)
- [QueryObjectsInputPaginateTypeDef](./type_defs.md#queryobjectsinputpaginatetypedef)
- [QueryObjectsInputTypeDef](./type_defs.md#queryobjectsinputtypedef)
- [PutPipelineDefinitionInputTypeDef](./type_defs.md#putpipelinedefinitioninputtypedef)
- [ValidatePipelineDefinitionInputTypeDef](./type_defs.md#validatepipelinedefinitioninputtypedef)

