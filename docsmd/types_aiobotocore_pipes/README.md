# EventBridgePipes module

> [Index](../README.md) > EventBridgePipes


!!! note ""

    Auto-generated documentation for [EventBridgePipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
    type annotations stubs module [types-aiobotocore-pipes](https://pypi.org/project/types-aiobotocore-pipes/).

## How to install



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
- [DeletePipeRequestRequestTypeDef](./type_defs.md#deletepiperequestrequesttypedef)
- [DescribePipeRequestRequestTypeDef](./type_defs.md#describepiperequestrequesttypedef)
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
- [ListPipesRequestRequestTypeDef](./type_defs.md#listpipesrequestrequesttypedef)
- [PipeTypeDef](./type_defs.md#pipetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
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
- [SelfManagedKafkaAccessConfigurationVpcTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationvpctypedef)
- [StartPipeRequestRequestTypeDef](./type_defs.md#startpiperequestrequesttypedef)
- [StopPipeRequestRequestTypeDef](./type_defs.md#stoppiperequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePipeSourceSqsQueueParametersTypeDef](./type_defs.md#updatepipesourcesqsqueueparameterstypedef)
- [NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef)
- [AwsVpcConfigurationUnionTypeDef](./type_defs.md#awsvpcconfigurationuniontypedef)
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
- [ListPipesRequestListPipesPaginateTypeDef](./type_defs.md#listpipesrequestlistpipespaginatetypedef)
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
- [PipeEnrichmentHttpParametersUnionTypeDef](./type_defs.md#pipeenrichmenthttpparametersuniontypedef)
- [PipeLogConfigurationParametersTypeDef](./type_defs.md#pipelogconfigurationparameterstypedef)
- [PipeLogConfigurationTypeDef](./type_defs.md#pipelogconfigurationtypedef)
- [PipeSourceKinesisStreamParametersTypeDef](./type_defs.md#pipesourcekinesisstreamparameterstypedef)
- [PipeSourceSelfManagedKafkaParametersOutputTypeDef](./type_defs.md#pipesourceselfmanagedkafkaparametersoutputtypedef)
- [PipeTargetEventBridgeEventBusParametersUnionTypeDef](./type_defs.md#pipetargeteventbridgeeventbusparametersuniontypedef)
- [PipeTargetHttpParametersUnionTypeDef](./type_defs.md#pipetargethttpparametersuniontypedef)
- [PipeTargetRedshiftDataParametersUnionTypeDef](./type_defs.md#pipetargetredshiftdataparametersuniontypedef)
- [PipeTargetSageMakerPipelineParametersOutputTypeDef](./type_defs.md#pipetargetsagemakerpipelineparametersoutputtypedef)
- [PipeTargetSageMakerPipelineParametersTypeDef](./type_defs.md#pipetargetsagemakerpipelineparameterstypedef)
- [SelfManagedKafkaAccessConfigurationVpcUnionTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationvpcuniontypedef)
- [NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
- [PipeTargetBatchJobParametersOutputTypeDef](./type_defs.md#pipetargetbatchjobparametersoutputtypedef)
- [BatchContainerOverridesUnionTypeDef](./type_defs.md#batchcontaineroverridesuniontypedef)
- [EcsTaskOverrideOutputTypeDef](./type_defs.md#ecstaskoverrideoutputtypedef)
- [EcsContainerOverrideUnionTypeDef](./type_defs.md#ecscontaineroverrideuniontypedef)
- [FilterCriteriaUnionTypeDef](./type_defs.md#filtercriteriauniontypedef)
- [PipeTargetTimestreamParametersOutputTypeDef](./type_defs.md#pipetargettimestreamparametersoutputtypedef)
- [MultiMeasureMappingUnionTypeDef](./type_defs.md#multimeasuremappinguniontypedef)
- [PipeEnrichmentParametersTypeDef](./type_defs.md#pipeenrichmentparameterstypedef)
- [PipeSourceKinesisStreamParametersUnionTypeDef](./type_defs.md#pipesourcekinesisstreamparametersuniontypedef)
- [PipeSourceParametersOutputTypeDef](./type_defs.md#pipesourceparametersoutputtypedef)
- [PipeTargetSageMakerPipelineParametersUnionTypeDef](./type_defs.md#pipetargetsagemakerpipelineparametersuniontypedef)
- [PipeSourceSelfManagedKafkaParametersTypeDef](./type_defs.md#pipesourceselfmanagedkafkaparameterstypedef)
- [UpdatePipeSourceSelfManagedKafkaParametersTypeDef](./type_defs.md#updatepipesourceselfmanagedkafkaparameterstypedef)
- [NetworkConfigurationUnionTypeDef](./type_defs.md#networkconfigurationuniontypedef)
- [PipeTargetBatchJobParametersTypeDef](./type_defs.md#pipetargetbatchjobparameterstypedef)
- [PipeTargetEcsTaskParametersOutputTypeDef](./type_defs.md#pipetargetecstaskparametersoutputtypedef)
- [EcsTaskOverrideTypeDef](./type_defs.md#ecstaskoverridetypedef)
- [PipeTargetTimestreamParametersTypeDef](./type_defs.md#pipetargettimestreamparameterstypedef)
- [PipeSourceSelfManagedKafkaParametersUnionTypeDef](./type_defs.md#pipesourceselfmanagedkafkaparametersuniontypedef)
- [UpdatePipeSourceParametersTypeDef](./type_defs.md#updatepipesourceparameterstypedef)
- [PipeTargetBatchJobParametersUnionTypeDef](./type_defs.md#pipetargetbatchjobparametersuniontypedef)
- [PipeTargetParametersOutputTypeDef](./type_defs.md#pipetargetparametersoutputtypedef)
- [EcsTaskOverrideUnionTypeDef](./type_defs.md#ecstaskoverrideuniontypedef)
- [PipeTargetTimestreamParametersUnionTypeDef](./type_defs.md#pipetargettimestreamparametersuniontypedef)
- [PipeSourceParametersTypeDef](./type_defs.md#pipesourceparameterstypedef)
- [DescribePipeResponseTypeDef](./type_defs.md#describepiperesponsetypedef)
- [PipeTargetEcsTaskParametersTypeDef](./type_defs.md#pipetargetecstaskparameterstypedef)
- [PipeTargetEcsTaskParametersUnionTypeDef](./type_defs.md#pipetargetecstaskparametersuniontypedef)
- [PipeTargetParametersTypeDef](./type_defs.md#pipetargetparameterstypedef)
- [CreatePipeRequestRequestTypeDef](./type_defs.md#createpiperequestrequesttypedef)
- [UpdatePipeRequestRequestTypeDef](./type_defs.md#updatepiperequestrequesttypedef)

