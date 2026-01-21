# EventBridgePipes module

> [Index](../README.md) > EventBridgePipes


!!! note ""

    Auto-generated documentation for [EventBridgePipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#eventbridgepipes)
    type annotations stubs module [types-aiobotocore-pipes](https://pypi.org/project/types-aiobotocore-pipes/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EventBridgePipes` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `EventBridgePipes` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[pipes]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pipes]'

# standalone installation
python -m pip install types-aiobotocore-pipes
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pipes
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EventBridgePipesClient

Type annotations and code completion for  `#!python session.create_client("pipes")` as [EventBridgePipesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# EventBridgePipesClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_pipes.client import EventBridgePipesClient


session = get_session()
async with session.create_client("pipes") as client:
    client: EventBridgePipesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("pipes").get_paginator("...")`.

```python
# ListPipesPaginator usage example

from types_aiobotocore_pipes.paginator import ListPipesPaginator

def get_list_pipes_paginator() -> ListPipesPaginator:
    return client.get_paginator("list_pipes"))
```

- [ListPipesPaginator](./paginators.md#listpipespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AssignPublicIpType usage example

from types_aiobotocore_pipes.literals import AssignPublicIpType

def get_value() -> AssignPublicIpType:
    return "DISABLED"
```

- [AssignPublicIpType](./literals.md#assignpubliciptype)
- [BatchJobDependencyTypeType](./literals.md#batchjobdependencytypetype)
- [BatchResourceRequirementTypeType](./literals.md#batchresourcerequirementtypetype)
- [DimensionValueTypeType](./literals.md#dimensionvaluetypetype)
- [DynamoDBStreamStartPositionType](./literals.md#dynamodbstreamstartpositiontype)
- [EcsEnvironmentFileTypeType](./literals.md#ecsenvironmentfiletypetype)
- [EcsResourceRequirementTypeType](./literals.md#ecsresourcerequirementtypetype)
- [EpochTimeUnitType](./literals.md#epochtimeunittype)
- [IncludeExecutionDataOptionType](./literals.md#includeexecutiondataoptiontype)
- [KinesisStreamStartPositionType](./literals.md#kinesisstreamstartpositiontype)
- [LaunchTypeType](./literals.md#launchtypetype)
- [ListPipesPaginatorName](./literals.md#listpipespaginatorname)
- [LogLevelType](./literals.md#logleveltype)
- [MSKStartPositionType](./literals.md#mskstartpositiontype)
- [MeasureValueTypeType](./literals.md#measurevaluetypetype)
- [OnPartialBatchItemFailureStreamsType](./literals.md#onpartialbatchitemfailurestreamstype)
- [PipeStateType](./literals.md#pipestatetype)
- [PipeTargetInvocationTypeType](./literals.md#pipetargetinvocationtypetype)
- [PlacementConstraintTypeType](./literals.md#placementconstrainttypetype)
- [PlacementStrategyTypeType](./literals.md#placementstrategytypetype)
- [PropagateTagsType](./literals.md#propagatetagstype)
- [RequestedPipeStateDescribeResponseType](./literals.md#requestedpipestatedescriberesponsetype)
- [RequestedPipeStateType](./literals.md#requestedpipestatetype)
- [S3OutputFormatType](./literals.md#s3outputformattype)
- [SelfManagedKafkaStartPositionType](./literals.md#selfmanagedkafkastartpositiontype)
- [TimeFieldTypeType](./literals.md#timefieldtypetype)
- [EventBridgePipesServiceName](./literals.md#eventbridgepipesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AwsVpcConfigurationOutputTypeDef](./type_defs.md#awsvpcconfigurationoutputtypedef)
- [AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef)
- [BatchArrayPropertiesTypeDef](./type_defs.md#batcharraypropertiestypedef)
- [BatchEnvironmentVariableTypeDef](./type_defs.md#batchenvironmentvariabletypedef)
- [BatchResourceRequirementTypeDef](./type_defs.md#batchresourcerequirementtypedef)
- [BatchJobDependencyTypeDef](./type_defs.md#batchjobdependencytypedef)
- [BatchRetryStrategyTypeDef](./type_defs.md#batchretrystrategytypedef)
- [CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef)
- [CloudwatchLogsLogDestinationParametersTypeDef](./type_defs.md#cloudwatchlogslogdestinationparameterstypedef)
- [CloudwatchLogsLogDestinationTypeDef](./type_defs.md#cloudwatchlogslogdestinationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef)
- [DeletePipeRequestTypeDef](./type_defs.md#deletepiperequesttypedef)
- [DescribePipeRequestTypeDef](./type_defs.md#describepiperequesttypedef)
- [DimensionMappingTypeDef](./type_defs.md#dimensionmappingtypedef)
- [EcsEnvironmentFileTypeDef](./type_defs.md#ecsenvironmentfiletypedef)
- [EcsEnvironmentVariableTypeDef](./type_defs.md#ecsenvironmentvariabletypedef)
- [EcsResourceRequirementTypeDef](./type_defs.md#ecsresourcerequirementtypedef)
- [EcsEphemeralStorageTypeDef](./type_defs.md#ecsephemeralstoragetypedef)
- [EcsInferenceAcceleratorOverrideTypeDef](./type_defs.md#ecsinferenceacceleratoroverridetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [FirehoseLogDestinationParametersTypeDef](./type_defs.md#firehoselogdestinationparameterstypedef)
- [FirehoseLogDestinationTypeDef](./type_defs.md#firehoselogdestinationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListPipesRequestTypeDef](./type_defs.md#listpipesrequesttypedef)
- [PipeTypeDef](./type_defs.md#pipetypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MQBrokerAccessCredentialsTypeDef](./type_defs.md#mqbrokeraccesscredentialstypedef)
- [MSKAccessCredentialsTypeDef](./type_defs.md#mskaccesscredentialstypedef)
- [MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef)
- [PipeEnrichmentHttpParametersOutputTypeDef](./type_defs.md#pipeenrichmenthttpparametersoutputtypedef)
- [PipeEnrichmentHttpParametersTypeDef](./type_defs.md#pipeenrichmenthttpparameterstypedef)
- [S3LogDestinationParametersTypeDef](./type_defs.md#s3logdestinationparameterstypedef)
- [S3LogDestinationTypeDef](./type_defs.md#s3logdestinationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PipeSourceSqsQueueParametersTypeDef](./type_defs.md#pipesourcesqsqueueparameterstypedef)
- [SelfManagedKafkaAccessConfigurationCredentialsTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationcredentialstypedef)
- [SelfManagedKafkaAccessConfigurationVpcOutputTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationvpcoutputtypedef)
- [SelfManagedKafkaAccessConfigurationVpcTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationvpctypedef)
- [PipeTargetCloudWatchLogsParametersTypeDef](./type_defs.md#pipetargetcloudwatchlogsparameterstypedef)
- [PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef)
- [PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [PipeTargetEventBridgeEventBusParametersOutputTypeDef](./type_defs.md#pipetargeteventbridgeeventbusparametersoutputtypedef)
- [PipeTargetEventBridgeEventBusParametersTypeDef](./type_defs.md#pipetargeteventbridgeeventbusparameterstypedef)
- [PipeTargetHttpParametersOutputTypeDef](./type_defs.md#pipetargethttpparametersoutputtypedef)
- [PipeTargetHttpParametersTypeDef](./type_defs.md#pipetargethttpparameterstypedef)
- [PipeTargetKinesisStreamParametersTypeDef](./type_defs.md#pipetargetkinesisstreamparameterstypedef)
- [PipeTargetLambdaFunctionParametersTypeDef](./type_defs.md#pipetargetlambdafunctionparameterstypedef)
- [PipeTargetRedshiftDataParametersOutputTypeDef](./type_defs.md#pipetargetredshiftdataparametersoutputtypedef)
- [PipeTargetSqsQueueParametersTypeDef](./type_defs.md#pipetargetsqsqueueparameterstypedef)
- [PipeTargetStateMachineParametersTypeDef](./type_defs.md#pipetargetstatemachineparameterstypedef)
- [PipeTargetRedshiftDataParametersTypeDef](./type_defs.md#pipetargetredshiftdataparameterstypedef)
- [SageMakerPipelineParameterTypeDef](./type_defs.md#sagemakerpipelineparametertypedef)
- [SingleMeasureMappingTypeDef](./type_defs.md#singlemeasuremappingtypedef)
- [StartPipeRequestTypeDef](./type_defs.md#startpiperequesttypedef)
- [StopPipeRequestTypeDef](./type_defs.md#stoppiperequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdatePipeSourceSqsQueueParametersTypeDef](./type_defs.md#updatepipesourcesqsqueueparameterstypedef)
- [NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef)
- [NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
- [BatchContainerOverridesOutputTypeDef](./type_defs.md#batchcontaineroverridesoutputtypedef)
- [BatchContainerOverridesTypeDef](./type_defs.md#batchcontaineroverridestypedef)
- [CreatePipeResponseTypeDef](./type_defs.md#createpiperesponsetypedef)
- [DeletePipeResponseTypeDef](./type_defs.md#deletepiperesponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartPipeResponseTypeDef](./type_defs.md#startpiperesponsetypedef)
- [StopPipeResponseTypeDef](./type_defs.md#stoppiperesponsetypedef)
- [UpdatePipeResponseTypeDef](./type_defs.md#updatepiperesponsetypedef)
- [PipeSourceDynamoDBStreamParametersTypeDef](./type_defs.md#pipesourcedynamodbstreamparameterstypedef)
- [PipeSourceKinesisStreamParametersOutputTypeDef](./type_defs.md#pipesourcekinesisstreamparametersoutputtypedef)
- [UpdatePipeSourceDynamoDBStreamParametersTypeDef](./type_defs.md#updatepipesourcedynamodbstreamparameterstypedef)
- [UpdatePipeSourceKinesisStreamParametersTypeDef](./type_defs.md#updatepipesourcekinesisstreamparameterstypedef)
- [EcsContainerOverrideOutputTypeDef](./type_defs.md#ecscontaineroverrideoutputtypedef)
- [EcsContainerOverrideTypeDef](./type_defs.md#ecscontaineroverridetypedef)
- [FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef)
- [FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef)
- [ListPipesRequestPaginateTypeDef](./type_defs.md#listpipesrequestpaginatetypedef)
- [ListPipesResponseTypeDef](./type_defs.md#listpipesresponsetypedef)
- [PipeSourceActiveMQBrokerParametersTypeDef](./type_defs.md#pipesourceactivemqbrokerparameterstypedef)
- [PipeSourceRabbitMQBrokerParametersTypeDef](./type_defs.md#pipesourcerabbitmqbrokerparameterstypedef)
- [UpdatePipeSourceActiveMQBrokerParametersTypeDef](./type_defs.md#updatepipesourceactivemqbrokerparameterstypedef)
- [UpdatePipeSourceRabbitMQBrokerParametersTypeDef](./type_defs.md#updatepipesourcerabbitmqbrokerparameterstypedef)
- [PipeSourceManagedStreamingKafkaParametersTypeDef](./type_defs.md#pipesourcemanagedstreamingkafkaparameterstypedef)
- [UpdatePipeSourceManagedStreamingKafkaParametersTypeDef](./type_defs.md#updatepipesourcemanagedstreamingkafkaparameterstypedef)
- [MultiMeasureMappingOutputTypeDef](./type_defs.md#multimeasuremappingoutputtypedef)
- [MultiMeasureMappingTypeDef](./type_defs.md#multimeasuremappingtypedef)
- [PipeEnrichmentParametersOutputTypeDef](./type_defs.md#pipeenrichmentparametersoutputtypedef)
- [PipeEnrichmentParametersTypeDef](./type_defs.md#pipeenrichmentparameterstypedef)
- [PipeLogConfigurationParametersTypeDef](./type_defs.md#pipelogconfigurationparameterstypedef)
- [PipeLogConfigurationTypeDef](./type_defs.md#pipelogconfigurationtypedef)
- [PipeSourceKinesisStreamParametersTypeDef](./type_defs.md#pipesourcekinesisstreamparameterstypedef)
- [PipeSourceSelfManagedKafkaParametersOutputTypeDef](./type_defs.md#pipesourceselfmanagedkafkaparametersoutputtypedef)
- [PipeSourceSelfManagedKafkaParametersTypeDef](./type_defs.md#pipesourceselfmanagedkafkaparameterstypedef)
- [SelfManagedKafkaAccessConfigurationVpcUnionTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationvpcuniontypedef)
- [PipeTargetSageMakerPipelineParametersOutputTypeDef](./type_defs.md#pipetargetsagemakerpipelineparametersoutputtypedef)
- [PipeTargetSageMakerPipelineParametersTypeDef](./type_defs.md#pipetargetsagemakerpipelineparameterstypedef)
- [PipeTargetBatchJobParametersOutputTypeDef](./type_defs.md#pipetargetbatchjobparametersoutputtypedef)
- [PipeTargetBatchJobParametersTypeDef](./type_defs.md#pipetargetbatchjobparameterstypedef)
- [EcsTaskOverrideOutputTypeDef](./type_defs.md#ecstaskoverrideoutputtypedef)
- [EcsTaskOverrideTypeDef](./type_defs.md#ecstaskoverridetypedef)
- [FilterCriteriaUnionTypeDef](./type_defs.md#filtercriteriauniontypedef)
- [PipeTargetTimestreamParametersOutputTypeDef](./type_defs.md#pipetargettimestreamparametersoutputtypedef)
- [PipeTargetTimestreamParametersTypeDef](./type_defs.md#pipetargettimestreamparameterstypedef)
- [PipeEnrichmentParametersUnionTypeDef](./type_defs.md#pipeenrichmentparametersuniontypedef)
- [PipeSourceParametersOutputTypeDef](./type_defs.md#pipesourceparametersoutputtypedef)
- [PipeSourceParametersTypeDef](./type_defs.md#pipesourceparameterstypedef)
- [UpdatePipeSourceSelfManagedKafkaParametersTypeDef](./type_defs.md#updatepipesourceselfmanagedkafkaparameterstypedef)
- [PipeTargetEcsTaskParametersOutputTypeDef](./type_defs.md#pipetargetecstaskparametersoutputtypedef)
- [PipeTargetEcsTaskParametersTypeDef](./type_defs.md#pipetargetecstaskparameterstypedef)
- [PipeSourceParametersUnionTypeDef](./type_defs.md#pipesourceparametersuniontypedef)
- [UpdatePipeSourceParametersTypeDef](./type_defs.md#updatepipesourceparameterstypedef)
- [PipeTargetParametersOutputTypeDef](./type_defs.md#pipetargetparametersoutputtypedef)
- [PipeTargetParametersTypeDef](./type_defs.md#pipetargetparameterstypedef)
- [DescribePipeResponseTypeDef](./type_defs.md#describepiperesponsetypedef)
- [PipeTargetParametersUnionTypeDef](./type_defs.md#pipetargetparametersuniontypedef)
- [CreatePipeRequestTypeDef](./type_defs.md#createpiperequesttypedef)
- [UpdatePipeRequestTypeDef](./type_defs.md#updatepiperequesttypedef)

