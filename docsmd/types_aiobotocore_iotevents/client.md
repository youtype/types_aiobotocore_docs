# IoTEventsClient

> [Index](../README.md) > [IoTEvents](./README.md) > IoTEventsClient

!!! note ""

    Auto-generated documentation for [IoTEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#iotevents)
    type annotations stubs module [types-aiobotocore-iotevents](https://pypi.org/project/types-aiobotocore-iotevents/).

## IoTEventsClient

Type annotations and code completion for `#!python session.create_client("iotevents")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)

```python
# IoTEventsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iotevents.client import IoTEventsClient

session = get_session()
async with session.create_client("iotevents") as client:
    client: IoTEventsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iotevents").exceptions` structure.

```python
# IoTEventsClient.exceptions usage example

async with session.create_client("iotevents") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalFailureException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.UnsupportedOperationException,
    ) as e:
        print(e)
```

```python
# IoTEventsClient usage type checking example

from types_aiobotocore_iotevents.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iotevents").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iotevents").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/generate_presigned_url.html)

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


### create\_alarm\_model

Creates an alarm model to monitor an AWS IoT Events input attribute.

Type annotations and code completion for `#!python session.create_client("iotevents").create_alarm_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/create_alarm_model.html)

```python
# create_alarm_model method definition

await def create_alarm_model(
    self,
    *,
    alarmModelName: str,
    roleArn: str,
    alarmRule: AlarmRuleTypeDef,  # (1)
    alarmModelDescription: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
    key: str = ...,
    severity: int = ...,
    alarmNotification: AlarmNotificationUnionTypeDef = ...,  # (3)
    alarmEventActions: AlarmEventActionsUnionTypeDef = ...,  # (4)
    alarmCapabilities: AlarmCapabilitiesTypeDef = ...,  # (5)
) -> CreateAlarmModelResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) [:material-code-braces: AlarmNotificationOutputTypeDef](./type_defs.md#alarmnotificationoutputtypedef) 
4. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) [:material-code-braces: AlarmEventActionsOutputTypeDef](./type_defs.md#alarmeventactionsoutputtypedef) 
5. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
6. See [:material-code-braces: CreateAlarmModelResponseTypeDef](./type_defs.md#createalarmmodelresponsetypedef) 


```python
# create_alarm_model method usage example with argument unpacking

kwargs: CreateAlarmModelRequestTypeDef = {  # (1)
    "alarmModelName": ...,
    "roleArn": ...,
    "alarmRule": ...,
}

parent.create_alarm_model(**kwargs)
```

1. See [:material-code-braces: CreateAlarmModelRequestTypeDef](./type_defs.md#createalarmmodelrequesttypedef) 

### create\_detector\_model

Creates a detector model.

Type annotations and code completion for `#!python session.create_client("iotevents").create_detector_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/create_detector_model.html)

```python
# create_detector_model method definition

await def create_detector_model(
    self,
    *,
    detectorModelName: str,
    detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,  # (1)
    roleArn: str,
    detectorModelDescription: str = ...,
    key: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
    evaluationMethod: EvaluationMethodType = ...,  # (3)
) -> CreateDetectorModelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
4. See [:material-code-braces: CreateDetectorModelResponseTypeDef](./type_defs.md#createdetectormodelresponsetypedef) 


```python
# create_detector_model method usage example with argument unpacking

kwargs: CreateDetectorModelRequestTypeDef = {  # (1)
    "detectorModelName": ...,
    "detectorModelDefinition": ...,
    "roleArn": ...,
}

parent.create_detector_model(**kwargs)
```

1. See [:material-code-braces: CreateDetectorModelRequestTypeDef](./type_defs.md#createdetectormodelrequesttypedef) 

### create\_input

Creates an input.

Type annotations and code completion for `#!python session.create_client("iotevents").create_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/create_input.html)

```python
# create_input method definition

await def create_input(
    self,
    *,
    inputName: str,
    inputDefinition: InputDefinitionUnionTypeDef,  # (1)
    inputDescription: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateInputResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) [:material-code-braces: InputDefinitionOutputTypeDef](./type_defs.md#inputdefinitionoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateInputResponseTypeDef](./type_defs.md#createinputresponsetypedef) 


```python
# create_input method usage example with argument unpacking

kwargs: CreateInputRequestTypeDef = {  # (1)
    "inputName": ...,
    "inputDefinition": ...,
}

parent.create_input(**kwargs)
```

1. See [:material-code-braces: CreateInputRequestTypeDef](./type_defs.md#createinputrequesttypedef) 

### delete\_alarm\_model

Deletes an alarm model.

Type annotations and code completion for `#!python session.create_client("iotevents").delete_alarm_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/delete_alarm_model.html)

```python
# delete_alarm_model method definition

await def delete_alarm_model(
    self,
    *,
    alarmModelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_alarm_model method usage example with argument unpacking

kwargs: DeleteAlarmModelRequestTypeDef = {  # (1)
    "alarmModelName": ...,
}

parent.delete_alarm_model(**kwargs)
```

1. See [:material-code-braces: DeleteAlarmModelRequestTypeDef](./type_defs.md#deletealarmmodelrequesttypedef) 

### delete\_detector\_model

Deletes a detector model.

Type annotations and code completion for `#!python session.create_client("iotevents").delete_detector_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/delete_detector_model.html)

```python
# delete_detector_model method definition

await def delete_detector_model(
    self,
    *,
    detectorModelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_detector_model method usage example with argument unpacking

kwargs: DeleteDetectorModelRequestTypeDef = {  # (1)
    "detectorModelName": ...,
}

parent.delete_detector_model(**kwargs)
```

1. See [:material-code-braces: DeleteDetectorModelRequestTypeDef](./type_defs.md#deletedetectormodelrequesttypedef) 

### delete\_input

Deletes an input.

Type annotations and code completion for `#!python session.create_client("iotevents").delete_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/delete_input.html)

```python
# delete_input method definition

await def delete_input(
    self,
    *,
    inputName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_input method usage example with argument unpacking

kwargs: DeleteInputRequestTypeDef = {  # (1)
    "inputName": ...,
}

parent.delete_input(**kwargs)
```

1. See [:material-code-braces: DeleteInputRequestTypeDef](./type_defs.md#deleteinputrequesttypedef) 

### describe\_alarm\_model

Retrieves information about an alarm model.

Type annotations and code completion for `#!python session.create_client("iotevents").describe_alarm_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/describe_alarm_model.html)

```python
# describe_alarm_model method definition

await def describe_alarm_model(
    self,
    *,
    alarmModelName: str,
    alarmModelVersion: str = ...,
) -> DescribeAlarmModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAlarmModelResponseTypeDef](./type_defs.md#describealarmmodelresponsetypedef) 


```python
# describe_alarm_model method usage example with argument unpacking

kwargs: DescribeAlarmModelRequestTypeDef = {  # (1)
    "alarmModelName": ...,
}

parent.describe_alarm_model(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmModelRequestTypeDef](./type_defs.md#describealarmmodelrequesttypedef) 

### describe\_detector\_model

Describes a detector model.

Type annotations and code completion for `#!python session.create_client("iotevents").describe_detector_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/describe_detector_model.html)

```python
# describe_detector_model method definition

await def describe_detector_model(
    self,
    *,
    detectorModelName: str,
    detectorModelVersion: str = ...,
) -> DescribeDetectorModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDetectorModelResponseTypeDef](./type_defs.md#describedetectormodelresponsetypedef) 


```python
# describe_detector_model method usage example with argument unpacking

kwargs: DescribeDetectorModelRequestTypeDef = {  # (1)
    "detectorModelName": ...,
}

parent.describe_detector_model(**kwargs)
```

1. See [:material-code-braces: DescribeDetectorModelRequestTypeDef](./type_defs.md#describedetectormodelrequesttypedef) 

### describe\_detector\_model\_analysis

Retrieves runtime information about a detector model analysis.

Type annotations and code completion for `#!python session.create_client("iotevents").describe_detector_model_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/describe_detector_model_analysis.html)

```python
# describe_detector_model_analysis method definition

await def describe_detector_model_analysis(
    self,
    *,
    analysisId: str,
) -> DescribeDetectorModelAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDetectorModelAnalysisResponseTypeDef](./type_defs.md#describedetectormodelanalysisresponsetypedef) 


```python
# describe_detector_model_analysis method usage example with argument unpacking

kwargs: DescribeDetectorModelAnalysisRequestTypeDef = {  # (1)
    "analysisId": ...,
}

parent.describe_detector_model_analysis(**kwargs)
```

1. See [:material-code-braces: DescribeDetectorModelAnalysisRequestTypeDef](./type_defs.md#describedetectormodelanalysisrequesttypedef) 

### describe\_input

Describes an input.

Type annotations and code completion for `#!python session.create_client("iotevents").describe_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/describe_input.html)

```python
# describe_input method definition

await def describe_input(
    self,
    *,
    inputName: str,
) -> DescribeInputResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInputResponseTypeDef](./type_defs.md#describeinputresponsetypedef) 


```python
# describe_input method usage example with argument unpacking

kwargs: DescribeInputRequestTypeDef = {  # (1)
    "inputName": ...,
}

parent.describe_input(**kwargs)
```

1. See [:material-code-braces: DescribeInputRequestTypeDef](./type_defs.md#describeinputrequesttypedef) 

### describe\_logging\_options

Retrieves the current settings of the AWS IoT Events logging options.

Type annotations and code completion for `#!python session.create_client("iotevents").describe_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/describe_logging_options.html)

```python
# describe_logging_options method definition

await def describe_logging_options(
    self,
) -> DescribeLoggingOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef) 

### get\_detector\_model\_analysis\_results

Retrieves one or more analysis results of the detector model.

Type annotations and code completion for `#!python session.create_client("iotevents").get_detector_model_analysis_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/get_detector_model_analysis_results.html)

```python
# get_detector_model_analysis_results method definition

await def get_detector_model_analysis_results(
    self,
    *,
    analysisId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetDetectorModelAnalysisResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDetectorModelAnalysisResultsResponseTypeDef](./type_defs.md#getdetectormodelanalysisresultsresponsetypedef) 


```python
# get_detector_model_analysis_results method usage example with argument unpacking

kwargs: GetDetectorModelAnalysisResultsRequestTypeDef = {  # (1)
    "analysisId": ...,
}

parent.get_detector_model_analysis_results(**kwargs)
```

1. See [:material-code-braces: GetDetectorModelAnalysisResultsRequestTypeDef](./type_defs.md#getdetectormodelanalysisresultsrequesttypedef) 

### list\_alarm\_model\_versions

Lists all the versions of an alarm model.

Type annotations and code completion for `#!python session.create_client("iotevents").list_alarm_model_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/list_alarm_model_versions.html)

```python
# list_alarm_model_versions method definition

await def list_alarm_model_versions(
    self,
    *,
    alarmModelName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAlarmModelVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAlarmModelVersionsResponseTypeDef](./type_defs.md#listalarmmodelversionsresponsetypedef) 


```python
# list_alarm_model_versions method usage example with argument unpacking

kwargs: ListAlarmModelVersionsRequestTypeDef = {  # (1)
    "alarmModelName": ...,
}

parent.list_alarm_model_versions(**kwargs)
```

1. See [:material-code-braces: ListAlarmModelVersionsRequestTypeDef](./type_defs.md#listalarmmodelversionsrequesttypedef) 

### list\_alarm\_models

Lists the alarm models that you created.

Type annotations and code completion for `#!python session.create_client("iotevents").list_alarm_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/list_alarm_models.html)

```python
# list_alarm_models method definition

await def list_alarm_models(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAlarmModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAlarmModelsResponseTypeDef](./type_defs.md#listalarmmodelsresponsetypedef) 


```python
# list_alarm_models method usage example with argument unpacking

kwargs: ListAlarmModelsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_alarm_models(**kwargs)
```

1. See [:material-code-braces: ListAlarmModelsRequestTypeDef](./type_defs.md#listalarmmodelsrequesttypedef) 

### list\_detector\_model\_versions

Lists all the versions of a detector model.

Type annotations and code completion for `#!python session.create_client("iotevents").list_detector_model_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/list_detector_model_versions.html)

```python
# list_detector_model_versions method definition

await def list_detector_model_versions(
    self,
    *,
    detectorModelName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDetectorModelVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDetectorModelVersionsResponseTypeDef](./type_defs.md#listdetectormodelversionsresponsetypedef) 


```python
# list_detector_model_versions method usage example with argument unpacking

kwargs: ListDetectorModelVersionsRequestTypeDef = {  # (1)
    "detectorModelName": ...,
}

parent.list_detector_model_versions(**kwargs)
```

1. See [:material-code-braces: ListDetectorModelVersionsRequestTypeDef](./type_defs.md#listdetectormodelversionsrequesttypedef) 

### list\_detector\_models

Lists the detector models you have created.

Type annotations and code completion for `#!python session.create_client("iotevents").list_detector_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/list_detector_models.html)

```python
# list_detector_models method definition

await def list_detector_models(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDetectorModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDetectorModelsResponseTypeDef](./type_defs.md#listdetectormodelsresponsetypedef) 


```python
# list_detector_models method usage example with argument unpacking

kwargs: ListDetectorModelsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_detector_models(**kwargs)
```

1. See [:material-code-braces: ListDetectorModelsRequestTypeDef](./type_defs.md#listdetectormodelsrequesttypedef) 

### list\_input\_routings

Lists one or more input routings.

Type annotations and code completion for `#!python session.create_client("iotevents").list_input_routings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/list_input_routings.html)

```python
# list_input_routings method definition

await def list_input_routings(
    self,
    *,
    inputIdentifier: InputIdentifierTypeDef,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListInputRoutingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InputIdentifierTypeDef](./type_defs.md#inputidentifiertypedef) 
2. See [:material-code-braces: ListInputRoutingsResponseTypeDef](./type_defs.md#listinputroutingsresponsetypedef) 


```python
# list_input_routings method usage example with argument unpacking

kwargs: ListInputRoutingsRequestTypeDef = {  # (1)
    "inputIdentifier": ...,
}

parent.list_input_routings(**kwargs)
```

1. See [:material-code-braces: ListInputRoutingsRequestTypeDef](./type_defs.md#listinputroutingsrequesttypedef) 

### list\_inputs

Lists the inputs you have created.

Type annotations and code completion for `#!python session.create_client("iotevents").list_inputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/list_inputs.html)

```python
# list_inputs method definition

await def list_inputs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListInputsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInputsResponseTypeDef](./type_defs.md#listinputsresponsetypedef) 


```python
# list_inputs method usage example with argument unpacking

kwargs: ListInputsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_inputs(**kwargs)
```

1. See [:material-code-braces: ListInputsRequestTypeDef](./type_defs.md#listinputsrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags (metadata) you have assigned to the resource.

Type annotations and code completion for `#!python session.create_client("iotevents").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### put\_logging\_options

Sets or updates the AWS IoT Events logging options.

Type annotations and code completion for `#!python session.create_client("iotevents").put_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/put_logging_options.html)

```python
# put_logging_options method definition

await def put_logging_options(
    self,
    *,
    loggingOptions: LoggingOptionsUnionTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) [:material-code-braces: LoggingOptionsOutputTypeDef](./type_defs.md#loggingoptionsoutputtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_logging_options method usage example with argument unpacking

kwargs: PutLoggingOptionsRequestTypeDef = {  # (1)
    "loggingOptions": ...,
}

parent.put_logging_options(**kwargs)
```

1. See [:material-code-braces: PutLoggingOptionsRequestTypeDef](./type_defs.md#putloggingoptionsrequesttypedef) 

### start\_detector\_model\_analysis

Performs an analysis of your detector model.

Type annotations and code completion for `#!python session.create_client("iotevents").start_detector_model_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/start_detector_model_analysis.html)

```python
# start_detector_model_analysis method definition

await def start_detector_model_analysis(
    self,
    *,
    detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,  # (1)
) -> StartDetectorModelAnalysisResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 
2. See [:material-code-braces: StartDetectorModelAnalysisResponseTypeDef](./type_defs.md#startdetectormodelanalysisresponsetypedef) 


```python
# start_detector_model_analysis method usage example with argument unpacking

kwargs: StartDetectorModelAnalysisRequestTypeDef = {  # (1)
    "detectorModelDefinition": ...,
}

parent.start_detector_model_analysis(**kwargs)
```

1. See [:material-code-braces: StartDetectorModelAnalysisRequestTypeDef](./type_defs.md#startdetectormodelanalysisrequesttypedef) 

### tag\_resource

Adds to or modifies the tags of the given resource.

Type annotations and code completion for `#!python session.create_client("iotevents").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes the given tags (metadata) from the resource.

Type annotations and code completion for `#!python session.create_client("iotevents").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/untag_resource.html)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_alarm\_model

Updates an alarm model.

Type annotations and code completion for `#!python session.create_client("iotevents").update_alarm_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/update_alarm_model.html)

```python
# update_alarm_model method definition

await def update_alarm_model(
    self,
    *,
    alarmModelName: str,
    roleArn: str,
    alarmRule: AlarmRuleTypeDef,  # (1)
    alarmModelDescription: str = ...,
    severity: int = ...,
    alarmNotification: AlarmNotificationUnionTypeDef = ...,  # (2)
    alarmEventActions: AlarmEventActionsUnionTypeDef = ...,  # (3)
    alarmCapabilities: AlarmCapabilitiesTypeDef = ...,  # (4)
) -> UpdateAlarmModelResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AlarmRuleTypeDef](./type_defs.md#alarmruletypedef) 
2. See [:material-code-braces: AlarmNotificationTypeDef](./type_defs.md#alarmnotificationtypedef) [:material-code-braces: AlarmNotificationOutputTypeDef](./type_defs.md#alarmnotificationoutputtypedef) 
3. See [:material-code-braces: AlarmEventActionsTypeDef](./type_defs.md#alarmeventactionstypedef) [:material-code-braces: AlarmEventActionsOutputTypeDef](./type_defs.md#alarmeventactionsoutputtypedef) 
4. See [:material-code-braces: AlarmCapabilitiesTypeDef](./type_defs.md#alarmcapabilitiestypedef) 
5. See [:material-code-braces: UpdateAlarmModelResponseTypeDef](./type_defs.md#updatealarmmodelresponsetypedef) 


```python
# update_alarm_model method usage example with argument unpacking

kwargs: UpdateAlarmModelRequestTypeDef = {  # (1)
    "alarmModelName": ...,
    "roleArn": ...,
    "alarmRule": ...,
}

parent.update_alarm_model(**kwargs)
```

1. See [:material-code-braces: UpdateAlarmModelRequestTypeDef](./type_defs.md#updatealarmmodelrequesttypedef) 

### update\_detector\_model

Updates a detector model.

Type annotations and code completion for `#!python session.create_client("iotevents").update_detector_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/update_detector_model.html)

```python
# update_detector_model method definition

await def update_detector_model(
    self,
    *,
    detectorModelName: str,
    detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,  # (1)
    roleArn: str,
    detectorModelDescription: str = ...,
    evaluationMethod: EvaluationMethodType = ...,  # (2)
) -> UpdateDetectorModelResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DetectorModelDefinitionTypeDef](./type_defs.md#detectormodeldefinitiontypedef) [:material-code-braces: DetectorModelDefinitionOutputTypeDef](./type_defs.md#detectormodeldefinitionoutputtypedef) 
2. See [:material-code-brackets: EvaluationMethodType](./literals.md#evaluationmethodtype) 
3. See [:material-code-braces: UpdateDetectorModelResponseTypeDef](./type_defs.md#updatedetectormodelresponsetypedef) 


```python
# update_detector_model method usage example with argument unpacking

kwargs: UpdateDetectorModelRequestTypeDef = {  # (1)
    "detectorModelName": ...,
    "detectorModelDefinition": ...,
    "roleArn": ...,
}

parent.update_detector_model(**kwargs)
```

1. See [:material-code-braces: UpdateDetectorModelRequestTypeDef](./type_defs.md#updatedetectormodelrequesttypedef) 

### update\_input

Updates an input.

Type annotations and code completion for `#!python session.create_client("iotevents").update_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents/client/update_input.html)

```python
# update_input method definition

await def update_input(
    self,
    *,
    inputName: str,
    inputDefinition: InputDefinitionUnionTypeDef,  # (1)
    inputDescription: str = ...,
) -> UpdateInputResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InputDefinitionTypeDef](./type_defs.md#inputdefinitiontypedef) [:material-code-braces: InputDefinitionOutputTypeDef](./type_defs.md#inputdefinitionoutputtypedef) 
2. See [:material-code-braces: UpdateInputResponseTypeDef](./type_defs.md#updateinputresponsetypedef) 


```python
# update_input method usage example with argument unpacking

kwargs: UpdateInputRequestTypeDef = {  # (1)
    "inputName": ...,
    "inputDefinition": ...,
}

parent.update_input(**kwargs)
```

1. See [:material-code-braces: UpdateInputRequestTypeDef](./type_defs.md#updateinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iotevents").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iotevents").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)

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





