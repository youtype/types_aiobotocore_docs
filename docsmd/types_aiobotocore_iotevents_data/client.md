# IoTEventsDataClient

> [Index](../README.md) > [IoTEventsData](./README.md) > IoTEventsDataClient

!!! note ""

    Auto-generated documentation for [IoTEventsData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
    type annotations stubs module [types-aiobotocore-iotevents-data](https://pypi.org/project/types-aiobotocore-iotevents-data/).

## IoTEventsDataClient

Type annotations and code completion for `#!python session.create_client("iotevents-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client)

```python
# IoTEventsDataClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iotevents_data.client import IoTEventsDataClient

session = get_session()
async with session.create_client("iotevents-data") as client:
    client: IoTEventsDataClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iotevents-data").exceptions` structure.

```python
# IoTEventsDataClient.exceptions usage example

async with session.create_client("iotevents-data") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalFailureException,
        client.InvalidRequestException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# IoTEventsDataClient usage type checking example

from types_aiobotocore_iotevents_data.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### batch\_acknowledge\_alarm

Acknowledges one or more alarms.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_acknowledge_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_acknowledge_alarm)

```python
# batch_acknowledge_alarm method definition

await def batch_acknowledge_alarm(
    self,
    *,
    acknowledgeActionRequests: Sequence[AcknowledgeAlarmActionRequestTypeDef],  # (1)
) -> BatchAcknowledgeAlarmResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AcknowledgeAlarmActionRequestTypeDef](./type_defs.md#acknowledgealarmactionrequesttypedef) 
2. See [:material-code-braces: BatchAcknowledgeAlarmResponseTypeDef](./type_defs.md#batchacknowledgealarmresponsetypedef) 


```python
# batch_acknowledge_alarm method usage example with argument unpacking

kwargs: BatchAcknowledgeAlarmRequestRequestTypeDef = {  # (1)
    "acknowledgeActionRequests": ...,
}

parent.batch_acknowledge_alarm(**kwargs)
```

1. See [:material-code-braces: BatchAcknowledgeAlarmRequestRequestTypeDef](./type_defs.md#batchacknowledgealarmrequestrequesttypedef) 

### batch\_delete\_detector

Deletes one or more detectors that were created.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_delete_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_delete_detector)

```python
# batch_delete_detector method definition

await def batch_delete_detector(
    self,
    *,
    detectors: Sequence[DeleteDetectorRequestTypeDef],  # (1)
) -> BatchDeleteDetectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeleteDetectorRequestTypeDef](./type_defs.md#deletedetectorrequesttypedef) 
2. See [:material-code-braces: BatchDeleteDetectorResponseTypeDef](./type_defs.md#batchdeletedetectorresponsetypedef) 


```python
# batch_delete_detector method usage example with argument unpacking

kwargs: BatchDeleteDetectorRequestRequestTypeDef = {  # (1)
    "detectors": ...,
}

parent.batch_delete_detector(**kwargs)
```

1. See [:material-code-braces: BatchDeleteDetectorRequestRequestTypeDef](./type_defs.md#batchdeletedetectorrequestrequesttypedef) 

### batch\_disable\_alarm

Disables one or more alarms.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_disable_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_disable_alarm)

```python
# batch_disable_alarm method definition

await def batch_disable_alarm(
    self,
    *,
    disableActionRequests: Sequence[DisableAlarmActionRequestTypeDef],  # (1)
) -> BatchDisableAlarmResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DisableAlarmActionRequestTypeDef](./type_defs.md#disablealarmactionrequesttypedef) 
2. See [:material-code-braces: BatchDisableAlarmResponseTypeDef](./type_defs.md#batchdisablealarmresponsetypedef) 


```python
# batch_disable_alarm method usage example with argument unpacking

kwargs: BatchDisableAlarmRequestRequestTypeDef = {  # (1)
    "disableActionRequests": ...,
}

parent.batch_disable_alarm(**kwargs)
```

1. See [:material-code-braces: BatchDisableAlarmRequestRequestTypeDef](./type_defs.md#batchdisablealarmrequestrequesttypedef) 

### batch\_enable\_alarm

Enables one or more alarms.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_enable_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_enable_alarm)

```python
# batch_enable_alarm method definition

await def batch_enable_alarm(
    self,
    *,
    enableActionRequests: Sequence[EnableAlarmActionRequestTypeDef],  # (1)
) -> BatchEnableAlarmResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnableAlarmActionRequestTypeDef](./type_defs.md#enablealarmactionrequesttypedef) 
2. See [:material-code-braces: BatchEnableAlarmResponseTypeDef](./type_defs.md#batchenablealarmresponsetypedef) 


```python
# batch_enable_alarm method usage example with argument unpacking

kwargs: BatchEnableAlarmRequestRequestTypeDef = {  # (1)
    "enableActionRequests": ...,
}

parent.batch_enable_alarm(**kwargs)
```

1. See [:material-code-braces: BatchEnableAlarmRequestRequestTypeDef](./type_defs.md#batchenablealarmrequestrequesttypedef) 

### batch\_put\_message

Sends a set of messages to the IoT Events system.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_put_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_put_message)

```python
# batch_put_message method definition

await def batch_put_message(
    self,
    *,
    messages: Sequence[MessageTypeDef],  # (1)
) -> BatchPutMessageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef) 


```python
# batch_put_message method usage example with argument unpacking

kwargs: BatchPutMessageRequestRequestTypeDef = {  # (1)
    "messages": ...,
}

parent.batch_put_message(**kwargs)
```

1. See [:material-code-braces: BatchPutMessageRequestRequestTypeDef](./type_defs.md#batchputmessagerequestrequesttypedef) 

### batch\_reset\_alarm

Resets one or more alarms.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_reset_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_reset_alarm)

```python
# batch_reset_alarm method definition

await def batch_reset_alarm(
    self,
    *,
    resetActionRequests: Sequence[ResetAlarmActionRequestTypeDef],  # (1)
) -> BatchResetAlarmResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResetAlarmActionRequestTypeDef](./type_defs.md#resetalarmactionrequesttypedef) 
2. See [:material-code-braces: BatchResetAlarmResponseTypeDef](./type_defs.md#batchresetalarmresponsetypedef) 


```python
# batch_reset_alarm method usage example with argument unpacking

kwargs: BatchResetAlarmRequestRequestTypeDef = {  # (1)
    "resetActionRequests": ...,
}

parent.batch_reset_alarm(**kwargs)
```

1. See [:material-code-braces: BatchResetAlarmRequestRequestTypeDef](./type_defs.md#batchresetalarmrequestrequesttypedef) 

### batch\_snooze\_alarm

Changes one or more alarms to the snooze mode.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_snooze_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_snooze_alarm)

```python
# batch_snooze_alarm method definition

await def batch_snooze_alarm(
    self,
    *,
    snoozeActionRequests: Sequence[SnoozeAlarmActionRequestTypeDef],  # (1)
) -> BatchSnoozeAlarmResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SnoozeAlarmActionRequestTypeDef](./type_defs.md#snoozealarmactionrequesttypedef) 
2. See [:material-code-braces: BatchSnoozeAlarmResponseTypeDef](./type_defs.md#batchsnoozealarmresponsetypedef) 


```python
# batch_snooze_alarm method usage example with argument unpacking

kwargs: BatchSnoozeAlarmRequestRequestTypeDef = {  # (1)
    "snoozeActionRequests": ...,
}

parent.batch_snooze_alarm(**kwargs)
```

1. See [:material-code-braces: BatchSnoozeAlarmRequestRequestTypeDef](./type_defs.md#batchsnoozealarmrequestrequesttypedef) 

### batch\_update\_detector

Updates the state, variable values, and timer settings of one or more detectors
(instances) of a specified detector
model.

Type annotations and code completion for `#!python session.create_client("iotevents-data").batch_update_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.batch_update_detector)

```python
# batch_update_detector method definition

await def batch_update_detector(
    self,
    *,
    detectors: Sequence[UpdateDetectorRequestTypeDef],  # (1)
) -> BatchUpdateDetectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateDetectorRequestTypeDef](./type_defs.md#updatedetectorrequesttypedef) 
2. See [:material-code-braces: BatchUpdateDetectorResponseTypeDef](./type_defs.md#batchupdatedetectorresponsetypedef) 


```python
# batch_update_detector method usage example with argument unpacking

kwargs: BatchUpdateDetectorRequestRequestTypeDef = {  # (1)
    "detectors": ...,
}

parent.batch_update_detector(**kwargs)
```

1. See [:material-code-braces: BatchUpdateDetectorRequestRequestTypeDef](./type_defs.md#batchupdatedetectorrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("iotevents-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("iotevents-data").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### describe\_alarm

Retrieves information about an alarm.

Type annotations and code completion for `#!python session.create_client("iotevents-data").describe_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.describe_alarm)

```python
# describe_alarm method definition

await def describe_alarm(
    self,
    *,
    alarmModelName: str,
    keyValue: str = ...,
) -> DescribeAlarmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAlarmResponseTypeDef](./type_defs.md#describealarmresponsetypedef) 


```python
# describe_alarm method usage example with argument unpacking

kwargs: DescribeAlarmRequestRequestTypeDef = {  # (1)
    "alarmModelName": ...,
}

parent.describe_alarm(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmRequestRequestTypeDef](./type_defs.md#describealarmrequestrequesttypedef) 

### describe\_detector

Returns information about the specified detector (instance).

Type annotations and code completion for `#!python session.create_client("iotevents-data").describe_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.describe_detector)

```python
# describe_detector method definition

await def describe_detector(
    self,
    *,
    detectorModelName: str,
    keyValue: str = ...,
) -> DescribeDetectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDetectorResponseTypeDef](./type_defs.md#describedetectorresponsetypedef) 


```python
# describe_detector method usage example with argument unpacking

kwargs: DescribeDetectorRequestRequestTypeDef = {  # (1)
    "detectorModelName": ...,
}

parent.describe_detector(**kwargs)
```

1. See [:material-code-braces: DescribeDetectorRequestRequestTypeDef](./type_defs.md#describedetectorrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("iotevents-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.generate_presigned_url)

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


### list\_alarms

Lists one or more alarms.

Type annotations and code completion for `#!python session.create_client("iotevents-data").list_alarms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.list_alarms)

```python
# list_alarms method definition

await def list_alarms(
    self,
    *,
    alarmModelName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAlarmsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAlarmsResponseTypeDef](./type_defs.md#listalarmsresponsetypedef) 


```python
# list_alarms method usage example with argument unpacking

kwargs: ListAlarmsRequestRequestTypeDef = {  # (1)
    "alarmModelName": ...,
}

parent.list_alarms(**kwargs)
```

1. See [:material-code-braces: ListAlarmsRequestRequestTypeDef](./type_defs.md#listalarmsrequestrequesttypedef) 

### list\_detectors

Lists detectors (the instances of a detector model).

Type annotations and code completion for `#!python session.create_client("iotevents-data").list_detectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.list_detectors)

```python
# list_detectors method definition

await def list_detectors(
    self,
    *,
    detectorModelName: str,
    stateName: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDetectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDetectorsResponseTypeDef](./type_defs.md#listdetectorsresponsetypedef) 


```python
# list_detectors method usage example with argument unpacking

kwargs: ListDetectorsRequestRequestTypeDef = {  # (1)
    "detectorModelName": ...,
}

parent.list_detectors(**kwargs)
```

1. See [:material-code-braces: ListDetectorsRequestRequestTypeDef](./type_defs.md#listdetectorsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iotevents-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "IoTEventsDataClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iotevents-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData.Client.__aexit__)

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





