# DataPipeline module

> [Index](../README.md) > DataPipeline


!!! note ""

    Auto-generated documentation for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
    type annotations stubs module [types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `DataPipeline`.

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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_datapipeline.paginator import DescribeObjectsPaginator

def get_describe_objects_paginator() -> DescribeObjectsPaginator:
    return client.get_paginator("describe_objects"))
```

- [DescribeObjectsPaginator](./paginators.md#describeobjectspaginator)
- [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- [QueryObjectsPaginator](./paginators.md#queryobjectspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
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




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_datapipeline.type_defs import ParameterValueTypeDef

def get_value() -> ParameterValueTypeDef:
    return {
        "id": ...,
        "stringValue": ...,
    }
```

- [ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeactivatePipelineInputRequestTypeDef](./type_defs.md#deactivatepipelineinputrequesttypedef)
- [DeletePipelineInputRequestTypeDef](./type_defs.md#deletepipelineinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeObjectsInputRequestTypeDef](./type_defs.md#describeobjectsinputrequesttypedef)
- [DescribePipelinesInputRequestTypeDef](./type_defs.md#describepipelinesinputrequesttypedef)
- [EvaluateExpressionInputRequestTypeDef](./type_defs.md#evaluateexpressioninputrequesttypedef)
- [FieldTypeDef](./type_defs.md#fieldtypedef)
- [GetPipelineDefinitionInputRequestTypeDef](./type_defs.md#getpipelinedefinitioninputrequesttypedef)
- [InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef)
- [ListPipelinesInputRequestTypeDef](./type_defs.md#listpipelinesinputrequesttypedef)
- [PipelineIdNameTypeDef](./type_defs.md#pipelineidnametypedef)
- [OperatorTypeDef](./type_defs.md#operatortypedef)
- [ParameterAttributeTypeDef](./type_defs.md#parameterattributetypedef)
- [ValidationErrorTypeDef](./type_defs.md#validationerrortypedef)
- [ValidationWarningTypeDef](./type_defs.md#validationwarningtypedef)
- [RemoveTagsInputRequestTypeDef](./type_defs.md#removetagsinputrequesttypedef)
- [ReportTaskRunnerHeartbeatInputRequestTypeDef](./type_defs.md#reporttaskrunnerheartbeatinputrequesttypedef)
- [SetStatusInputRequestTypeDef](./type_defs.md#setstatusinputrequesttypedef)
- [SetTaskStatusInputRequestTypeDef](./type_defs.md#settaskstatusinputrequesttypedef)
- [ActivatePipelineInputRequestTypeDef](./type_defs.md#activatepipelineinputrequesttypedef)
- [AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef)
- [CreatePipelineInputRequestTypeDef](./type_defs.md#createpipelineinputrequesttypedef)
- [CreatePipelineOutputTypeDef](./type_defs.md#createpipelineoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EvaluateExpressionOutputTypeDef](./type_defs.md#evaluateexpressionoutputtypedef)
- [QueryObjectsOutputTypeDef](./type_defs.md#queryobjectsoutputtypedef)
- [ReportTaskProgressOutputTypeDef](./type_defs.md#reporttaskprogressoutputtypedef)
- [ReportTaskRunnerHeartbeatOutputTypeDef](./type_defs.md#reporttaskrunnerheartbeatoutputtypedef)
- [DescribeObjectsInputDescribeObjectsPaginateTypeDef](./type_defs.md#describeobjectsinputdescribeobjectspaginatetypedef)
- [ListPipelinesInputListPipelinesPaginateTypeDef](./type_defs.md#listpipelinesinputlistpipelinespaginatetypedef)
- [PipelineDescriptionTypeDef](./type_defs.md#pipelinedescriptiontypedef)
- [PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef)
- [ReportTaskProgressInputRequestTypeDef](./type_defs.md#reporttaskprogressinputrequesttypedef)
- [PollForTaskInputRequestTypeDef](./type_defs.md#pollfortaskinputrequesttypedef)
- [ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef)
- [SelectorTypeDef](./type_defs.md#selectortypedef)
- [ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef)
- [PutPipelineDefinitionOutputTypeDef](./type_defs.md#putpipelinedefinitionoutputtypedef)
- [ValidatePipelineDefinitionOutputTypeDef](./type_defs.md#validatepipelinedefinitionoutputtypedef)
- [DescribePipelinesOutputTypeDef](./type_defs.md#describepipelinesoutputtypedef)
- [DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef)
- [TaskObjectTypeDef](./type_defs.md#taskobjecttypedef)
- [QueryTypeDef](./type_defs.md#querytypedef)
- [GetPipelineDefinitionOutputTypeDef](./type_defs.md#getpipelinedefinitionoutputtypedef)
- [PutPipelineDefinitionInputRequestTypeDef](./type_defs.md#putpipelinedefinitioninputrequesttypedef)
- [ValidatePipelineDefinitionInputRequestTypeDef](./type_defs.md#validatepipelinedefinitioninputrequesttypedef)
- [PollForTaskOutputTypeDef](./type_defs.md#pollfortaskoutputtypedef)
- [QueryObjectsInputQueryObjectsPaginateTypeDef](./type_defs.md#queryobjectsinputqueryobjectspaginatetypedef)
- [QueryObjectsInputRequestTypeDef](./type_defs.md#queryobjectsinputrequesttypedef)

