# CloudWatchLogsClient

> [Index](../README.md) > [CloudWatchLogs](./README.md) > CloudWatchLogsClient

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## CloudWatchLogsClient

Type annotations and code completion for `#!python session.create_client("logs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)

```python
# CloudWatchLogsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_logs.client import CloudWatchLogsClient

session = get_session()
async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("logs").exceptions` structure.

```python
# CloudWatchLogsClient.exceptions usage example

async with session.create_client("logs") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.DataAlreadyAcceptedException,
        client.InvalidOperationException,
        client.InvalidParameterException,
        client.InvalidSequenceTokenException,
        client.LimitExceededException,
        client.MalformedQueryException,
        client.OperationAbortedException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
        client.SessionStreamingException,
        client.SessionTimeoutException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.UnrecognizedClientException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CloudWatchLogsClient usage type checking example

from types_aiobotocore_logs.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_kms\_key

Associates the specified KMS key with either one log group in the account, or
with all stored CloudWatch Logs query insights results in the
account.

Type annotations and code completion for `#!python session.create_client("logs").associate_kms_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.associate_kms_key)

```python
# associate_kms_key method definition

await def associate_kms_key(
    self,
    *,
    kmsKeyId: str,
    logGroupName: str = ...,
    resourceIdentifier: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_kms_key method usage example with argument unpacking

kwargs: AssociateKmsKeyRequestRequestTypeDef = {  # (1)
    "kmsKeyId": ...,
}

parent.associate_kms_key(**kwargs)
```

1. See [:material-code-braces: AssociateKmsKeyRequestRequestTypeDef](./type_defs.md#associatekmskeyrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("logs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_export\_task

Cancels the specified export task.

Type annotations and code completion for `#!python session.create_client("logs").cancel_export_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.cancel_export_task)

```python
# cancel_export_task method definition

await def cancel_export_task(
    self,
    *,
    taskId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_export_task method usage example with argument unpacking

kwargs: CancelExportTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.cancel_export_task(**kwargs)
```

1. See [:material-code-braces: CancelExportTaskRequestRequestTypeDef](./type_defs.md#cancelexporttaskrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("logs").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_delivery

Creates a *delivery*.

Type annotations and code completion for `#!python session.create_client("logs").create_delivery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_delivery)

```python
# create_delivery method definition

await def create_delivery(
    self,
    *,
    deliverySourceName: str,
    deliveryDestinationArn: str,
    recordFields: Sequence[str] = ...,
    fieldDelimiter: str = ...,
    s3DeliveryConfiguration: S3DeliveryConfigurationTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateDeliveryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef) 
2. See [:material-code-braces: CreateDeliveryResponseTypeDef](./type_defs.md#createdeliveryresponsetypedef) 


```python
# create_delivery method usage example with argument unpacking

kwargs: CreateDeliveryRequestRequestTypeDef = {  # (1)
    "deliverySourceName": ...,
    "deliveryDestinationArn": ...,
}

parent.create_delivery(**kwargs)
```

1. See [:material-code-braces: CreateDeliveryRequestRequestTypeDef](./type_defs.md#createdeliveryrequestrequesttypedef) 

### create\_export\_task

Creates an export task so that you can efficiently export data from a log group
to an Amazon S3
bucket.

Type annotations and code completion for `#!python session.create_client("logs").create_export_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_export_task)

```python
# create_export_task method definition

await def create_export_task(
    self,
    *,
    logGroupName: str,
    fromTime: int,
    to: int,
    destination: str,
    taskName: str = ...,
    logStreamNamePrefix: str = ...,
    destinationPrefix: str = ...,
) -> CreateExportTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateExportTaskResponseTypeDef](./type_defs.md#createexporttaskresponsetypedef) 


```python
# create_export_task method usage example with argument unpacking

kwargs: CreateExportTaskRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "fromTime": ...,
    "to": ...,
    "destination": ...,
}

parent.create_export_task(**kwargs)
```

1. See [:material-code-braces: CreateExportTaskRequestRequestTypeDef](./type_defs.md#createexporttaskrequestrequesttypedef) 

### create\_log\_anomaly\_detector

Creates an *anomaly detector* that regularly scans one or more log groups and
look for patterns and anomalies in the
logs.

Type annotations and code completion for `#!python session.create_client("logs").create_log_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_anomaly_detector)

```python
# create_log_anomaly_detector method definition

await def create_log_anomaly_detector(
    self,
    *,
    logGroupArnList: Sequence[str],
    detectorName: str = ...,
    evaluationFrequency: EvaluationFrequencyType = ...,  # (1)
    filterPattern: str = ...,
    kmsKeyId: str = ...,
    anomalyVisibilityTime: int = ...,
    tags: Mapping[str, str] = ...,
) -> CreateLogAnomalyDetectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EvaluationFrequencyType](./literals.md#evaluationfrequencytype) 
2. See [:material-code-braces: CreateLogAnomalyDetectorResponseTypeDef](./type_defs.md#createloganomalydetectorresponsetypedef) 


```python
# create_log_anomaly_detector method usage example with argument unpacking

kwargs: CreateLogAnomalyDetectorRequestRequestTypeDef = {  # (1)
    "logGroupArnList": ...,
}

parent.create_log_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: CreateLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#createloganomalydetectorrequestrequesttypedef) 

### create\_log\_group

Creates a log group with the specified name.

Type annotations and code completion for `#!python session.create_client("logs").create_log_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_group)

```python
# create_log_group method definition

await def create_log_group(
    self,
    *,
    logGroupName: str,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
    logGroupClass: LogGroupClassType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LogGroupClassType](./literals.md#loggroupclasstype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_log_group method usage example with argument unpacking

kwargs: CreateLogGroupRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.create_log_group(**kwargs)
```

1. See [:material-code-braces: CreateLogGroupRequestRequestTypeDef](./type_defs.md#createloggrouprequestrequesttypedef) 

### create\_log\_stream

Creates a log stream for the specified log group.

Type annotations and code completion for `#!python session.create_client("logs").create_log_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_stream)

```python
# create_log_stream method definition

await def create_log_stream(
    self,
    *,
    logGroupName: str,
    logStreamName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_log_stream method usage example with argument unpacking

kwargs: CreateLogStreamRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "logStreamName": ...,
}

parent.create_log_stream(**kwargs)
```

1. See [:material-code-braces: CreateLogStreamRequestRequestTypeDef](./type_defs.md#createlogstreamrequestrequesttypedef) 

### delete\_account\_policy

Deletes a CloudWatch Logs account policy.

Type annotations and code completion for `#!python session.create_client("logs").delete_account_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_account_policy)

```python
# delete_account_policy method definition

await def delete_account_policy(
    self,
    *,
    policyName: str,
    policyType: PolicyTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_account_policy method usage example with argument unpacking

kwargs: DeleteAccountPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "policyType": ...,
}

parent.delete_account_policy(**kwargs)
```

1. See [:material-code-braces: DeleteAccountPolicyRequestRequestTypeDef](./type_defs.md#deleteaccountpolicyrequestrequesttypedef) 

### delete\_data\_protection\_policy

Deletes the data protection policy from the specified log group.

Type annotations and code completion for `#!python session.create_client("logs").delete_data_protection_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_data_protection_policy)

```python
# delete_data_protection_policy method definition

await def delete_data_protection_policy(
    self,
    *,
    logGroupIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_data_protection_policy method usage example with argument unpacking

kwargs: DeleteDataProtectionPolicyRequestRequestTypeDef = {  # (1)
    "logGroupIdentifier": ...,
}

parent.delete_data_protection_policy(**kwargs)
```

1. See [:material-code-braces: DeleteDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#deletedataprotectionpolicyrequestrequesttypedef) 

### delete\_delivery

Deletes s *delivery*.

Type annotations and code completion for `#!python session.create_client("logs").delete_delivery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_delivery)

```python
# delete_delivery method definition

await def delete_delivery(
    self,
    *,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_delivery method usage example with argument unpacking

kwargs: DeleteDeliveryRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_delivery(**kwargs)
```

1. See [:material-code-braces: DeleteDeliveryRequestRequestTypeDef](./type_defs.md#deletedeliveryrequestrequesttypedef) 

### delete\_delivery\_destination

Deletes a *delivery destination*.

Type annotations and code completion for `#!python session.create_client("logs").delete_delivery_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_delivery_destination)

```python
# delete_delivery_destination method definition

await def delete_delivery_destination(
    self,
    *,
    name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_delivery_destination method usage example with argument unpacking

kwargs: DeleteDeliveryDestinationRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_delivery_destination(**kwargs)
```

1. See [:material-code-braces: DeleteDeliveryDestinationRequestRequestTypeDef](./type_defs.md#deletedeliverydestinationrequestrequesttypedef) 

### delete\_delivery\_destination\_policy

Deletes a delivery destination policy.

Type annotations and code completion for `#!python session.create_client("logs").delete_delivery_destination_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_delivery_destination_policy)

```python
# delete_delivery_destination_policy method definition

await def delete_delivery_destination_policy(
    self,
    *,
    deliveryDestinationName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_delivery_destination_policy method usage example with argument unpacking

kwargs: DeleteDeliveryDestinationPolicyRequestRequestTypeDef = {  # (1)
    "deliveryDestinationName": ...,
}

parent.delete_delivery_destination_policy(**kwargs)
```

1. See [:material-code-braces: DeleteDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#deletedeliverydestinationpolicyrequestrequesttypedef) 

### delete\_delivery\_source

Deletes a *delivery source*.

Type annotations and code completion for `#!python session.create_client("logs").delete_delivery_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_delivery_source)

```python
# delete_delivery_source method definition

await def delete_delivery_source(
    self,
    *,
    name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_delivery_source method usage example with argument unpacking

kwargs: DeleteDeliverySourceRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_delivery_source(**kwargs)
```

1. See [:material-code-braces: DeleteDeliverySourceRequestRequestTypeDef](./type_defs.md#deletedeliverysourcerequestrequesttypedef) 

### delete\_destination

Deletes the specified destination, and eventually disables all the subscription
filters that publish to
it.

Type annotations and code completion for `#!python session.create_client("logs").delete_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_destination)

```python
# delete_destination method definition

await def delete_destination(
    self,
    *,
    destinationName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_destination method usage example with argument unpacking

kwargs: DeleteDestinationRequestRequestTypeDef = {  # (1)
    "destinationName": ...,
}

parent.delete_destination(**kwargs)
```

1. See [:material-code-braces: DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef) 

### delete\_log\_anomaly\_detector

Deletes the specified CloudWatch Logs anomaly detector.

Type annotations and code completion for `#!python session.create_client("logs").delete_log_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_log_anomaly_detector)

```python
# delete_log_anomaly_detector method definition

await def delete_log_anomaly_detector(
    self,
    *,
    anomalyDetectorArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_log_anomaly_detector method usage example with argument unpacking

kwargs: DeleteLogAnomalyDetectorRequestRequestTypeDef = {  # (1)
    "anomalyDetectorArn": ...,
}

parent.delete_log_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: DeleteLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#deleteloganomalydetectorrequestrequesttypedef) 

### delete\_log\_group

Deletes the specified log group and permanently deletes all the archived log
events associated with the log
group.

Type annotations and code completion for `#!python session.create_client("logs").delete_log_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_log_group)

```python
# delete_log_group method definition

await def delete_log_group(
    self,
    *,
    logGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_log_group method usage example with argument unpacking

kwargs: DeleteLogGroupRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.delete_log_group(**kwargs)
```

1. See [:material-code-braces: DeleteLogGroupRequestRequestTypeDef](./type_defs.md#deleteloggrouprequestrequesttypedef) 

### delete\_log\_stream

Deletes the specified log stream and permanently deletes all the archived log
events associated with the log
stream.

Type annotations and code completion for `#!python session.create_client("logs").delete_log_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_log_stream)

```python
# delete_log_stream method definition

await def delete_log_stream(
    self,
    *,
    logGroupName: str,
    logStreamName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_log_stream method usage example with argument unpacking

kwargs: DeleteLogStreamRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "logStreamName": ...,
}

parent.delete_log_stream(**kwargs)
```

1. See [:material-code-braces: DeleteLogStreamRequestRequestTypeDef](./type_defs.md#deletelogstreamrequestrequesttypedef) 

### delete\_metric\_filter

Deletes the specified metric filter.

Type annotations and code completion for `#!python session.create_client("logs").delete_metric_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_metric_filter)

```python
# delete_metric_filter method definition

await def delete_metric_filter(
    self,
    *,
    logGroupName: str,
    filterName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_metric_filter method usage example with argument unpacking

kwargs: DeleteMetricFilterRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "filterName": ...,
}

parent.delete_metric_filter(**kwargs)
```

1. See [:material-code-braces: DeleteMetricFilterRequestRequestTypeDef](./type_defs.md#deletemetricfilterrequestrequesttypedef) 

### delete\_query\_definition

Deletes a saved CloudWatch Logs Insights query definition.

Type annotations and code completion for `#!python session.create_client("logs").delete_query_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_query_definition)

```python
# delete_query_definition method definition

await def delete_query_definition(
    self,
    *,
    queryDefinitionId: str,
) -> DeleteQueryDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteQueryDefinitionResponseTypeDef](./type_defs.md#deletequerydefinitionresponsetypedef) 


```python
# delete_query_definition method usage example with argument unpacking

kwargs: DeleteQueryDefinitionRequestRequestTypeDef = {  # (1)
    "queryDefinitionId": ...,
}

parent.delete_query_definition(**kwargs)
```

1. See [:material-code-braces: DeleteQueryDefinitionRequestRequestTypeDef](./type_defs.md#deletequerydefinitionrequestrequesttypedef) 

### delete\_resource\_policy

Deletes a resource policy from this account.

Type annotations and code completion for `#!python session.create_client("logs").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_resource_policy)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    policyName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_retention\_policy

Deletes the specified retention policy.

Type annotations and code completion for `#!python session.create_client("logs").delete_retention_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_retention_policy)

```python
# delete_retention_policy method definition

await def delete_retention_policy(
    self,
    *,
    logGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_retention_policy method usage example with argument unpacking

kwargs: DeleteRetentionPolicyRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.delete_retention_policy(**kwargs)
```

1. See [:material-code-braces: DeleteRetentionPolicyRequestRequestTypeDef](./type_defs.md#deleteretentionpolicyrequestrequesttypedef) 

### delete\_subscription\_filter

Deletes the specified subscription filter.

Type annotations and code completion for `#!python session.create_client("logs").delete_subscription_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_subscription_filter)

```python
# delete_subscription_filter method definition

await def delete_subscription_filter(
    self,
    *,
    logGroupName: str,
    filterName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_subscription_filter method usage example with argument unpacking

kwargs: DeleteSubscriptionFilterRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "filterName": ...,
}

parent.delete_subscription_filter(**kwargs)
```

1. See [:material-code-braces: DeleteSubscriptionFilterRequestRequestTypeDef](./type_defs.md#deletesubscriptionfilterrequestrequesttypedef) 

### describe\_account\_policies

Returns a list of all CloudWatch Logs account policies in the account.

Type annotations and code completion for `#!python session.create_client("logs").describe_account_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_account_policies)

```python
# describe_account_policies method definition

await def describe_account_policies(
    self,
    *,
    policyType: PolicyTypeType,  # (1)
    policyName: str = ...,
    accountIdentifiers: Sequence[str] = ...,
) -> DescribeAccountPoliciesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: DescribeAccountPoliciesResponseTypeDef](./type_defs.md#describeaccountpoliciesresponsetypedef) 


```python
# describe_account_policies method usage example with argument unpacking

kwargs: DescribeAccountPoliciesRequestRequestTypeDef = {  # (1)
    "policyType": ...,
}

parent.describe_account_policies(**kwargs)
```

1. See [:material-code-braces: DescribeAccountPoliciesRequestRequestTypeDef](./type_defs.md#describeaccountpoliciesrequestrequesttypedef) 

### describe\_configuration\_templates

Use this operation to return the valid and default values that are used when
creating delivery sources, delivery destinations, and
deliveries.

Type annotations and code completion for `#!python session.create_client("logs").describe_configuration_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_configuration_templates)

```python
# describe_configuration_templates method definition

await def describe_configuration_templates(
    self,
    *,
    service: str = ...,
    logTypes: Sequence[str] = ...,
    resourceTypes: Sequence[str] = ...,
    deliveryDestinationTypes: Sequence[DeliveryDestinationTypeType] = ...,  # (1)
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeConfigurationTemplatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype) 
2. See [:material-code-braces: DescribeConfigurationTemplatesResponseTypeDef](./type_defs.md#describeconfigurationtemplatesresponsetypedef) 


```python
# describe_configuration_templates method usage example with argument unpacking

kwargs: DescribeConfigurationTemplatesRequestRequestTypeDef = {  # (1)
    "service": ...,
}

parent.describe_configuration_templates(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describeconfigurationtemplatesrequestrequesttypedef) 

### describe\_deliveries

Retrieves a list of the deliveries that have been created in the account.

Type annotations and code completion for `#!python session.create_client("logs").describe_deliveries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_deliveries)

```python
# describe_deliveries method definition

await def describe_deliveries(
    self,
    *,
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeDeliveriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeliveriesResponseTypeDef](./type_defs.md#describedeliveriesresponsetypedef) 


```python
# describe_deliveries method usage example with argument unpacking

kwargs: DescribeDeliveriesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.describe_deliveries(**kwargs)
```

1. See [:material-code-braces: DescribeDeliveriesRequestRequestTypeDef](./type_defs.md#describedeliveriesrequestrequesttypedef) 

### describe\_delivery\_destinations

Retrieves a list of the delivery destinations that have been created in the
account.

Type annotations and code completion for `#!python session.create_client("logs").describe_delivery_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_delivery_destinations)

```python
# describe_delivery_destinations method definition

await def describe_delivery_destinations(
    self,
    *,
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeDeliveryDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeliveryDestinationsResponseTypeDef](./type_defs.md#describedeliverydestinationsresponsetypedef) 


```python
# describe_delivery_destinations method usage example with argument unpacking

kwargs: DescribeDeliveryDestinationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.describe_delivery_destinations(**kwargs)
```

1. See [:material-code-braces: DescribeDeliveryDestinationsRequestRequestTypeDef](./type_defs.md#describedeliverydestinationsrequestrequesttypedef) 

### describe\_delivery\_sources

Retrieves a list of the delivery sources that have been created in the account.

Type annotations and code completion for `#!python session.create_client("logs").describe_delivery_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_delivery_sources)

```python
# describe_delivery_sources method definition

await def describe_delivery_sources(
    self,
    *,
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeDeliverySourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeliverySourcesResponseTypeDef](./type_defs.md#describedeliverysourcesresponsetypedef) 


```python
# describe_delivery_sources method usage example with argument unpacking

kwargs: DescribeDeliverySourcesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.describe_delivery_sources(**kwargs)
```

1. See [:material-code-braces: DescribeDeliverySourcesRequestRequestTypeDef](./type_defs.md#describedeliverysourcesrequestrequesttypedef) 

### describe\_destinations

Lists all your destinations.

Type annotations and code completion for `#!python session.create_client("logs").describe_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_destinations)

```python
# describe_destinations method definition

await def describe_destinations(
    self,
    *,
    DestinationNamePrefix: str = ...,
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef) 


```python
# describe_destinations method usage example with argument unpacking

kwargs: DescribeDestinationsRequestRequestTypeDef = {  # (1)
    "DestinationNamePrefix": ...,
}

parent.describe_destinations(**kwargs)
```

1. See [:material-code-braces: DescribeDestinationsRequestRequestTypeDef](./type_defs.md#describedestinationsrequestrequesttypedef) 

### describe\_export\_tasks

Lists the specified export tasks.

Type annotations and code completion for `#!python session.create_client("logs").describe_export_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_export_tasks)

```python
# describe_export_tasks method definition

await def describe_export_tasks(
    self,
    *,
    taskId: str = ...,
    statusCode: ExportTaskStatusCodeType = ...,  # (1)
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeExportTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype) 
2. See [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


```python
# describe_export_tasks method usage example with argument unpacking

kwargs: DescribeExportTasksRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.describe_export_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestRequestTypeDef](./type_defs.md#describeexporttasksrequestrequesttypedef) 

### describe\_log\_groups

Lists the specified log groups.

Type annotations and code completion for `#!python session.create_client("logs").describe_log_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_groups)

```python
# describe_log_groups method definition

await def describe_log_groups(
    self,
    *,
    accountIdentifiers: Sequence[str] = ...,
    logGroupNamePrefix: str = ...,
    logGroupNamePattern: str = ...,
    nextToken: str = ...,
    limit: int = ...,
    includeLinkedAccounts: bool = ...,
    logGroupClass: LogGroupClassType = ...,  # (1)
) -> DescribeLogGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LogGroupClassType](./literals.md#loggroupclasstype) 
2. See [:material-code-braces: DescribeLogGroupsResponseTypeDef](./type_defs.md#describeloggroupsresponsetypedef) 


```python
# describe_log_groups method usage example with argument unpacking

kwargs: DescribeLogGroupsRequestRequestTypeDef = {  # (1)
    "accountIdentifiers": ...,
}

parent.describe_log_groups(**kwargs)
```

1. See [:material-code-braces: DescribeLogGroupsRequestRequestTypeDef](./type_defs.md#describeloggroupsrequestrequesttypedef) 

### describe\_log\_streams

Lists the log streams for the specified log group.

Type annotations and code completion for `#!python session.create_client("logs").describe_log_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_streams)

```python
# describe_log_streams method definition

await def describe_log_streams(
    self,
    *,
    logGroupName: str = ...,
    logGroupIdentifier: str = ...,
    logStreamNamePrefix: str = ...,
    orderBy: OrderByType = ...,  # (1)
    descending: bool = ...,
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeLogStreamsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
2. See [:material-code-braces: DescribeLogStreamsResponseTypeDef](./type_defs.md#describelogstreamsresponsetypedef) 


```python
# describe_log_streams method usage example with argument unpacking

kwargs: DescribeLogStreamsRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.describe_log_streams(**kwargs)
```

1. See [:material-code-braces: DescribeLogStreamsRequestRequestTypeDef](./type_defs.md#describelogstreamsrequestrequesttypedef) 

### describe\_metric\_filters

Lists the specified metric filters.

Type annotations and code completion for `#!python session.create_client("logs").describe_metric_filters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_metric_filters)

```python
# describe_metric_filters method definition

await def describe_metric_filters(
    self,
    *,
    logGroupName: str = ...,
    filterNamePrefix: str = ...,
    nextToken: str = ...,
    limit: int = ...,
    metricName: str = ...,
    metricNamespace: str = ...,
) -> DescribeMetricFiltersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMetricFiltersResponseTypeDef](./type_defs.md#describemetricfiltersresponsetypedef) 


```python
# describe_metric_filters method usage example with argument unpacking

kwargs: DescribeMetricFiltersRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.describe_metric_filters(**kwargs)
```

1. See [:material-code-braces: DescribeMetricFiltersRequestRequestTypeDef](./type_defs.md#describemetricfiltersrequestrequesttypedef) 

### describe\_queries

Returns a list of CloudWatch Logs Insights queries that are scheduled, running,
or have been run recently in this
account.

Type annotations and code completion for `#!python session.create_client("logs").describe_queries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_queries)

```python
# describe_queries method definition

await def describe_queries(
    self,
    *,
    logGroupName: str = ...,
    status: QueryStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeQueriesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: DescribeQueriesResponseTypeDef](./type_defs.md#describequeriesresponsetypedef) 


```python
# describe_queries method usage example with argument unpacking

kwargs: DescribeQueriesRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.describe_queries(**kwargs)
```

1. See [:material-code-braces: DescribeQueriesRequestRequestTypeDef](./type_defs.md#describequeriesrequestrequesttypedef) 

### describe\_query\_definitions

This operation returns a paginated list of your saved CloudWatch Logs Insights
query
definitions.

Type annotations and code completion for `#!python session.create_client("logs").describe_query_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_query_definitions)

```python
# describe_query_definitions method definition

await def describe_query_definitions(
    self,
    *,
    queryDefinitionNamePrefix: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeQueryDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeQueryDefinitionsResponseTypeDef](./type_defs.md#describequerydefinitionsresponsetypedef) 


```python
# describe_query_definitions method usage example with argument unpacking

kwargs: DescribeQueryDefinitionsRequestRequestTypeDef = {  # (1)
    "queryDefinitionNamePrefix": ...,
}

parent.describe_query_definitions(**kwargs)
```

1. See [:material-code-braces: DescribeQueryDefinitionsRequestRequestTypeDef](./type_defs.md#describequerydefinitionsrequestrequesttypedef) 

### describe\_resource\_policies

Lists the resource policies in this account.

Type annotations and code completion for `#!python session.create_client("logs").describe_resource_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_resource_policies)

```python
# describe_resource_policies method definition

await def describe_resource_policies(
    self,
    *,
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeResourcePoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourcePoliciesResponseTypeDef](./type_defs.md#describeresourcepoliciesresponsetypedef) 


```python
# describe_resource_policies method usage example with argument unpacking

kwargs: DescribeResourcePoliciesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.describe_resource_policies(**kwargs)
```

1. See [:material-code-braces: DescribeResourcePoliciesRequestRequestTypeDef](./type_defs.md#describeresourcepoliciesrequestrequesttypedef) 

### describe\_subscription\_filters

Lists the subscription filters for the specified log group.

Type annotations and code completion for `#!python session.create_client("logs").describe_subscription_filters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_subscription_filters)

```python
# describe_subscription_filters method definition

await def describe_subscription_filters(
    self,
    *,
    logGroupName: str,
    filterNamePrefix: str = ...,
    nextToken: str = ...,
    limit: int = ...,
) -> DescribeSubscriptionFiltersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSubscriptionFiltersResponseTypeDef](./type_defs.md#describesubscriptionfiltersresponsetypedef) 


```python
# describe_subscription_filters method usage example with argument unpacking

kwargs: DescribeSubscriptionFiltersRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.describe_subscription_filters(**kwargs)
```

1. See [:material-code-braces: DescribeSubscriptionFiltersRequestRequestTypeDef](./type_defs.md#describesubscriptionfiltersrequestrequesttypedef) 

### disassociate\_kms\_key

Disassociates the specified KMS key from the specified log group or from all
CloudWatch Logs Insights query results in the
account.

Type annotations and code completion for `#!python session.create_client("logs").disassociate_kms_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.disassociate_kms_key)

```python
# disassociate_kms_key method definition

await def disassociate_kms_key(
    self,
    *,
    logGroupName: str = ...,
    resourceIdentifier: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_kms_key method usage example with argument unpacking

kwargs: DisassociateKmsKeyRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.disassociate_kms_key(**kwargs)
```

1. See [:material-code-braces: DisassociateKmsKeyRequestRequestTypeDef](./type_defs.md#disassociatekmskeyrequestrequesttypedef) 

### filter\_log\_events

Lists log events from the specified log group.

Type annotations and code completion for `#!python session.create_client("logs").filter_log_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.filter_log_events)

```python
# filter_log_events method definition

await def filter_log_events(
    self,
    *,
    logGroupName: str = ...,
    logGroupIdentifier: str = ...,
    logStreamNames: Sequence[str] = ...,
    logStreamNamePrefix: str = ...,
    startTime: int = ...,
    endTime: int = ...,
    filterPattern: str = ...,
    nextToken: str = ...,
    limit: int = ...,
    interleaved: bool = ...,
    unmask: bool = ...,
) -> FilterLogEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FilterLogEventsResponseTypeDef](./type_defs.md#filterlogeventsresponsetypedef) 


```python
# filter_log_events method usage example with argument unpacking

kwargs: FilterLogEventsRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.filter_log_events(**kwargs)
```

1. See [:material-code-braces: FilterLogEventsRequestRequestTypeDef](./type_defs.md#filterlogeventsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("logs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.generate_presigned_url)

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


### get\_data\_protection\_policy

Returns information about a log group data protection policy.

Type annotations and code completion for `#!python session.create_client("logs").get_data_protection_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_data_protection_policy)

```python
# get_data_protection_policy method definition

await def get_data_protection_policy(
    self,
    *,
    logGroupIdentifier: str,
) -> GetDataProtectionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataProtectionPolicyResponseTypeDef](./type_defs.md#getdataprotectionpolicyresponsetypedef) 


```python
# get_data_protection_policy method usage example with argument unpacking

kwargs: GetDataProtectionPolicyRequestRequestTypeDef = {  # (1)
    "logGroupIdentifier": ...,
}

parent.get_data_protection_policy(**kwargs)
```

1. See [:material-code-braces: GetDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#getdataprotectionpolicyrequestrequesttypedef) 

### get\_delivery

Returns complete information about one logical *delivery*.

Type annotations and code completion for `#!python session.create_client("logs").get_delivery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_delivery)

```python
# get_delivery method definition

await def get_delivery(
    self,
    *,
    id: str,
) -> GetDeliveryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeliveryResponseTypeDef](./type_defs.md#getdeliveryresponsetypedef) 


```python
# get_delivery method usage example with argument unpacking

kwargs: GetDeliveryRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_delivery(**kwargs)
```

1. See [:material-code-braces: GetDeliveryRequestRequestTypeDef](./type_defs.md#getdeliveryrequestrequesttypedef) 

### get\_delivery\_destination

Retrieves complete information about one delivery destination.

Type annotations and code completion for `#!python session.create_client("logs").get_delivery_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_delivery_destination)

```python
# get_delivery_destination method definition

await def get_delivery_destination(
    self,
    *,
    name: str,
) -> GetDeliveryDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeliveryDestinationResponseTypeDef](./type_defs.md#getdeliverydestinationresponsetypedef) 


```python
# get_delivery_destination method usage example with argument unpacking

kwargs: GetDeliveryDestinationRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_delivery_destination(**kwargs)
```

1. See [:material-code-braces: GetDeliveryDestinationRequestRequestTypeDef](./type_defs.md#getdeliverydestinationrequestrequesttypedef) 

### get\_delivery\_destination\_policy

Retrieves the delivery destination policy assigned to the delivery destination
that you
specify.

Type annotations and code completion for `#!python session.create_client("logs").get_delivery_destination_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_delivery_destination_policy)

```python
# get_delivery_destination_policy method definition

await def get_delivery_destination_policy(
    self,
    *,
    deliveryDestinationName: str,
) -> GetDeliveryDestinationPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeliveryDestinationPolicyResponseTypeDef](./type_defs.md#getdeliverydestinationpolicyresponsetypedef) 


```python
# get_delivery_destination_policy method usage example with argument unpacking

kwargs: GetDeliveryDestinationPolicyRequestRequestTypeDef = {  # (1)
    "deliveryDestinationName": ...,
}

parent.get_delivery_destination_policy(**kwargs)
```

1. See [:material-code-braces: GetDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#getdeliverydestinationpolicyrequestrequesttypedef) 

### get\_delivery\_source

Retrieves complete information about one delivery source.

Type annotations and code completion for `#!python session.create_client("logs").get_delivery_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_delivery_source)

```python
# get_delivery_source method definition

await def get_delivery_source(
    self,
    *,
    name: str,
) -> GetDeliverySourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeliverySourceResponseTypeDef](./type_defs.md#getdeliverysourceresponsetypedef) 


```python
# get_delivery_source method usage example with argument unpacking

kwargs: GetDeliverySourceRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_delivery_source(**kwargs)
```

1. See [:material-code-braces: GetDeliverySourceRequestRequestTypeDef](./type_defs.md#getdeliverysourcerequestrequesttypedef) 

### get\_log\_anomaly\_detector

Retrieves information about the log anomaly detector that you specify.

Type annotations and code completion for `#!python session.create_client("logs").get_log_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_anomaly_detector)

```python
# get_log_anomaly_detector method definition

await def get_log_anomaly_detector(
    self,
    *,
    anomalyDetectorArn: str,
) -> GetLogAnomalyDetectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLogAnomalyDetectorResponseTypeDef](./type_defs.md#getloganomalydetectorresponsetypedef) 


```python
# get_log_anomaly_detector method usage example with argument unpacking

kwargs: GetLogAnomalyDetectorRequestRequestTypeDef = {  # (1)
    "anomalyDetectorArn": ...,
}

parent.get_log_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: GetLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#getloganomalydetectorrequestrequesttypedef) 

### get\_log\_events

Lists log events from the specified log stream.

Type annotations and code completion for `#!python session.create_client("logs").get_log_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_events)

```python
# get_log_events method definition

await def get_log_events(
    self,
    *,
    logStreamName: str,
    logGroupName: str = ...,
    logGroupIdentifier: str = ...,
    startTime: int = ...,
    endTime: int = ...,
    nextToken: str = ...,
    limit: int = ...,
    startFromHead: bool = ...,
    unmask: bool = ...,
) -> GetLogEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLogEventsResponseTypeDef](./type_defs.md#getlogeventsresponsetypedef) 


```python
# get_log_events method usage example with argument unpacking

kwargs: GetLogEventsRequestRequestTypeDef = {  # (1)
    "logStreamName": ...,
}

parent.get_log_events(**kwargs)
```

1. See [:material-code-braces: GetLogEventsRequestRequestTypeDef](./type_defs.md#getlogeventsrequestrequesttypedef) 

### get\_log\_group\_fields

Returns a list of the fields that are included in log events in the specified
log
group.

Type annotations and code completion for `#!python session.create_client("logs").get_log_group_fields` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_group_fields)

```python
# get_log_group_fields method definition

await def get_log_group_fields(
    self,
    *,
    logGroupName: str = ...,
    time: int = ...,
    logGroupIdentifier: str = ...,
) -> GetLogGroupFieldsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLogGroupFieldsResponseTypeDef](./type_defs.md#getloggroupfieldsresponsetypedef) 


```python
# get_log_group_fields method usage example with argument unpacking

kwargs: GetLogGroupFieldsRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.get_log_group_fields(**kwargs)
```

1. See [:material-code-braces: GetLogGroupFieldsRequestRequestTypeDef](./type_defs.md#getloggroupfieldsrequestrequesttypedef) 

### get\_log\_record

Retrieves all of the fields and values of a single log event.

Type annotations and code completion for `#!python session.create_client("logs").get_log_record` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_record)

```python
# get_log_record method definition

await def get_log_record(
    self,
    *,
    logRecordPointer: str,
    unmask: bool = ...,
) -> GetLogRecordResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLogRecordResponseTypeDef](./type_defs.md#getlogrecordresponsetypedef) 


```python
# get_log_record method usage example with argument unpacking

kwargs: GetLogRecordRequestRequestTypeDef = {  # (1)
    "logRecordPointer": ...,
}

parent.get_log_record(**kwargs)
```

1. See [:material-code-braces: GetLogRecordRequestRequestTypeDef](./type_defs.md#getlogrecordrequestrequesttypedef) 

### get\_query\_results

Returns the results from the specified query.

Type annotations and code completion for `#!python session.create_client("logs").get_query_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_query_results)

```python
# get_query_results method definition

await def get_query_results(
    self,
    *,
    queryId: str,
) -> GetQueryResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryResultsResponseTypeDef](./type_defs.md#getqueryresultsresponsetypedef) 


```python
# get_query_results method usage example with argument unpacking

kwargs: GetQueryResultsRequestRequestTypeDef = {  # (1)
    "queryId": ...,
}

parent.get_query_results(**kwargs)
```

1. See [:material-code-braces: GetQueryResultsRequestRequestTypeDef](./type_defs.md#getqueryresultsrequestrequesttypedef) 

### list\_anomalies

Returns a list of anomalies that log anomaly detectors have found.

Type annotations and code completion for `#!python session.create_client("logs").list_anomalies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_anomalies)

```python
# list_anomalies method definition

await def list_anomalies(
    self,
    *,
    anomalyDetectorArn: str = ...,
    suppressionState: SuppressionStateType = ...,  # (1)
    limit: int = ...,
    nextToken: str = ...,
) -> ListAnomaliesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SuppressionStateType](./literals.md#suppressionstatetype) 
2. See [:material-code-braces: ListAnomaliesResponseTypeDef](./type_defs.md#listanomaliesresponsetypedef) 


```python
# list_anomalies method usage example with argument unpacking

kwargs: ListAnomaliesRequestRequestTypeDef = {  # (1)
    "anomalyDetectorArn": ...,
}

parent.list_anomalies(**kwargs)
```

1. See [:material-code-braces: ListAnomaliesRequestRequestTypeDef](./type_defs.md#listanomaliesrequestrequesttypedef) 

### list\_log\_anomaly\_detectors

Retrieves a list of the log anomaly detectors in the account.

Type annotations and code completion for `#!python session.create_client("logs").list_log_anomaly_detectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_log_anomaly_detectors)

```python
# list_log_anomaly_detectors method definition

await def list_log_anomaly_detectors(
    self,
    *,
    filterLogGroupArn: str = ...,
    limit: int = ...,
    nextToken: str = ...,
) -> ListLogAnomalyDetectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLogAnomalyDetectorsResponseTypeDef](./type_defs.md#listloganomalydetectorsresponsetypedef) 


```python
# list_log_anomaly_detectors method usage example with argument unpacking

kwargs: ListLogAnomalyDetectorsRequestRequestTypeDef = {  # (1)
    "filterLogGroupArn": ...,
}

parent.list_log_anomaly_detectors(**kwargs)
```

1. See [:material-code-braces: ListLogAnomalyDetectorsRequestRequestTypeDef](./type_defs.md#listloganomalydetectorsrequestrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with a CloudWatch Logs resource.

Type annotations and code completion for `#!python session.create_client("logs").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_tags\_log\_group

.

Type annotations and code completion for `#!python session.create_client("logs").list_tags_log_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_log_group)

```python
# list_tags_log_group method definition

await def list_tags_log_group(
    self,
    *,
    logGroupName: str,
) -> ListTagsLogGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsLogGroupResponseTypeDef](./type_defs.md#listtagsloggroupresponsetypedef) 


```python
# list_tags_log_group method usage example with argument unpacking

kwargs: ListTagsLogGroupRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.list_tags_log_group(**kwargs)
```

1. See [:material-code-braces: ListTagsLogGroupRequestRequestTypeDef](./type_defs.md#listtagsloggrouprequestrequesttypedef) 

### put\_account\_policy

Creates an account-level data protection policy or subscription filter policy
that applies to all log groups or a subset of log groups in the
account.

Type annotations and code completion for `#!python session.create_client("logs").put_account_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_account_policy)

```python
# put_account_policy method definition

await def put_account_policy(
    self,
    *,
    policyName: str,
    policyDocument: str,
    policyType: PolicyTypeType,  # (1)
    scope: ScopeType = ...,  # (2)
    selectionCriteria: str = ...,
) -> PutAccountPolicyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
3. See [:material-code-braces: PutAccountPolicyResponseTypeDef](./type_defs.md#putaccountpolicyresponsetypedef) 


```python
# put_account_policy method usage example with argument unpacking

kwargs: PutAccountPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "policyDocument": ...,
    "policyType": ...,
}

parent.put_account_policy(**kwargs)
```

1. See [:material-code-braces: PutAccountPolicyRequestRequestTypeDef](./type_defs.md#putaccountpolicyrequestrequesttypedef) 

### put\_data\_protection\_policy

Creates a data protection policy for the specified log group.

Type annotations and code completion for `#!python session.create_client("logs").put_data_protection_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_data_protection_policy)

```python
# put_data_protection_policy method definition

await def put_data_protection_policy(
    self,
    *,
    logGroupIdentifier: str,
    policyDocument: str,
) -> PutDataProtectionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutDataProtectionPolicyResponseTypeDef](./type_defs.md#putdataprotectionpolicyresponsetypedef) 


```python
# put_data_protection_policy method usage example with argument unpacking

kwargs: PutDataProtectionPolicyRequestRequestTypeDef = {  # (1)
    "logGroupIdentifier": ...,
    "policyDocument": ...,
}

parent.put_data_protection_policy(**kwargs)
```

1. See [:material-code-braces: PutDataProtectionPolicyRequestRequestTypeDef](./type_defs.md#putdataprotectionpolicyrequestrequesttypedef) 

### put\_delivery\_destination

Creates or updates a logical *delivery destination*.

Type annotations and code completion for `#!python session.create_client("logs").put_delivery_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_delivery_destination)

```python
# put_delivery_destination method definition

await def put_delivery_destination(
    self,
    *,
    name: str,
    deliveryDestinationConfiguration: DeliveryDestinationConfigurationTypeDef,  # (1)
    outputFormat: OutputFormatType = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> PutDeliveryDestinationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DeliveryDestinationConfigurationTypeDef](./type_defs.md#deliverydestinationconfigurationtypedef) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
3. See [:material-code-braces: PutDeliveryDestinationResponseTypeDef](./type_defs.md#putdeliverydestinationresponsetypedef) 


```python
# put_delivery_destination method usage example with argument unpacking

kwargs: PutDeliveryDestinationRequestRequestTypeDef = {  # (1)
    "name": ...,
    "deliveryDestinationConfiguration": ...,
}

parent.put_delivery_destination(**kwargs)
```

1. See [:material-code-braces: PutDeliveryDestinationRequestRequestTypeDef](./type_defs.md#putdeliverydestinationrequestrequesttypedef) 

### put\_delivery\_destination\_policy

Creates and assigns an IAM policy that grants permissions to CloudWatch Logs to
deliver logs cross-account to a specified destination in this
account.

Type annotations and code completion for `#!python session.create_client("logs").put_delivery_destination_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_delivery_destination_policy)

```python
# put_delivery_destination_policy method definition

await def put_delivery_destination_policy(
    self,
    *,
    deliveryDestinationName: str,
    deliveryDestinationPolicy: str,
) -> PutDeliveryDestinationPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutDeliveryDestinationPolicyResponseTypeDef](./type_defs.md#putdeliverydestinationpolicyresponsetypedef) 


```python
# put_delivery_destination_policy method usage example with argument unpacking

kwargs: PutDeliveryDestinationPolicyRequestRequestTypeDef = {  # (1)
    "deliveryDestinationName": ...,
    "deliveryDestinationPolicy": ...,
}

parent.put_delivery_destination_policy(**kwargs)
```

1. See [:material-code-braces: PutDeliveryDestinationPolicyRequestRequestTypeDef](./type_defs.md#putdeliverydestinationpolicyrequestrequesttypedef) 

### put\_delivery\_source

Creates or updates a logical *delivery source*.

Type annotations and code completion for `#!python session.create_client("logs").put_delivery_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_delivery_source)

```python
# put_delivery_source method definition

await def put_delivery_source(
    self,
    *,
    name: str,
    resourceArn: str,
    logType: str,
    tags: Mapping[str, str] = ...,
) -> PutDeliverySourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutDeliverySourceResponseTypeDef](./type_defs.md#putdeliverysourceresponsetypedef) 


```python
# put_delivery_source method usage example with argument unpacking

kwargs: PutDeliverySourceRequestRequestTypeDef = {  # (1)
    "name": ...,
    "resourceArn": ...,
    "logType": ...,
}

parent.put_delivery_source(**kwargs)
```

1. See [:material-code-braces: PutDeliverySourceRequestRequestTypeDef](./type_defs.md#putdeliverysourcerequestrequesttypedef) 

### put\_destination

Creates or updates a destination.

Type annotations and code completion for `#!python session.create_client("logs").put_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_destination)

```python
# put_destination method definition

await def put_destination(
    self,
    *,
    destinationName: str,
    targetArn: str,
    roleArn: str,
    tags: Mapping[str, str] = ...,
) -> PutDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutDestinationResponseTypeDef](./type_defs.md#putdestinationresponsetypedef) 


```python
# put_destination method usage example with argument unpacking

kwargs: PutDestinationRequestRequestTypeDef = {  # (1)
    "destinationName": ...,
    "targetArn": ...,
    "roleArn": ...,
}

parent.put_destination(**kwargs)
```

1. See [:material-code-braces: PutDestinationRequestRequestTypeDef](./type_defs.md#putdestinationrequestrequesttypedef) 

### put\_destination\_policy

Creates or updates an access policy associated with an existing destination.

Type annotations and code completion for `#!python session.create_client("logs").put_destination_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_destination_policy)

```python
# put_destination_policy method definition

await def put_destination_policy(
    self,
    *,
    destinationName: str,
    accessPolicy: str,
    forceUpdate: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_destination_policy method usage example with argument unpacking

kwargs: PutDestinationPolicyRequestRequestTypeDef = {  # (1)
    "destinationName": ...,
    "accessPolicy": ...,
}

parent.put_destination_policy(**kwargs)
```

1. See [:material-code-braces: PutDestinationPolicyRequestRequestTypeDef](./type_defs.md#putdestinationpolicyrequestrequesttypedef) 

### put\_log\_events

Uploads a batch of log events to the specified log stream.

Type annotations and code completion for `#!python session.create_client("logs").put_log_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_log_events)

```python
# put_log_events method definition

await def put_log_events(
    self,
    *,
    logGroupName: str,
    logStreamName: str,
    logEvents: Sequence[InputLogEventTypeDef],  # (1)
    sequenceToken: str = ...,
    entity: EntityTypeDef = ...,  # (2)
) -> PutLogEventsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InputLogEventTypeDef](./type_defs.md#inputlogeventtypedef) 
2. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
3. See [:material-code-braces: PutLogEventsResponseTypeDef](./type_defs.md#putlogeventsresponsetypedef) 


```python
# put_log_events method usage example with argument unpacking

kwargs: PutLogEventsRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "logStreamName": ...,
    "logEvents": ...,
}

parent.put_log_events(**kwargs)
```

1. See [:material-code-braces: PutLogEventsRequestRequestTypeDef](./type_defs.md#putlogeventsrequestrequesttypedef) 

### put\_metric\_filter

Creates or updates a metric filter and associates it with the specified log
group.

Type annotations and code completion for `#!python session.create_client("logs").put_metric_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)

```python
# put_metric_filter method definition

await def put_metric_filter(
    self,
    *,
    logGroupName: str,
    filterName: str,
    filterPattern: str,
    metricTransformations: Sequence[MetricTransformationUnionTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MetricTransformationTypeDef](./type_defs.md#metrictransformationtypedef) [:material-code-braces: MetricTransformationOutputTypeDef](./type_defs.md#metrictransformationoutputtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_metric_filter method usage example with argument unpacking

kwargs: PutMetricFilterRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "filterName": ...,
    "filterPattern": ...,
    "metricTransformations": ...,
}

parent.put_metric_filter(**kwargs)
```

1. See [:material-code-braces: PutMetricFilterRequestRequestTypeDef](./type_defs.md#putmetricfilterrequestrequesttypedef) 

### put\_query\_definition

Creates or updates a query definition for CloudWatch Logs Insights.

Type annotations and code completion for `#!python session.create_client("logs").put_query_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_query_definition)

```python
# put_query_definition method definition

await def put_query_definition(
    self,
    *,
    name: str,
    queryString: str,
    queryDefinitionId: str = ...,
    logGroupNames: Sequence[str] = ...,
    clientToken: str = ...,
) -> PutQueryDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutQueryDefinitionResponseTypeDef](./type_defs.md#putquerydefinitionresponsetypedef) 


```python
# put_query_definition method usage example with argument unpacking

kwargs: PutQueryDefinitionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "queryString": ...,
}

parent.put_query_definition(**kwargs)
```

1. See [:material-code-braces: PutQueryDefinitionRequestRequestTypeDef](./type_defs.md#putquerydefinitionrequestrequesttypedef) 

### put\_resource\_policy

Creates or updates a resource policy allowing other Amazon Web Services
services to put log events to this account, such as Amazon Route
53.

Type annotations and code completion for `#!python session.create_client("logs").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_resource_policy)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    policyName: str = ...,
    policyDocument: str = ...,
) -> PutResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### put\_retention\_policy

Sets the retention of the specified log group.

Type annotations and code completion for `#!python session.create_client("logs").put_retention_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_retention_policy)

```python
# put_retention_policy method definition

await def put_retention_policy(
    self,
    *,
    logGroupName: str,
    retentionInDays: int,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_retention_policy method usage example with argument unpacking

kwargs: PutRetentionPolicyRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "retentionInDays": ...,
}

parent.put_retention_policy(**kwargs)
```

1. See [:material-code-braces: PutRetentionPolicyRequestRequestTypeDef](./type_defs.md#putretentionpolicyrequestrequesttypedef) 

### put\_subscription\_filter

Creates or updates a subscription filter and associates it with the specified
log
group.

Type annotations and code completion for `#!python session.create_client("logs").put_subscription_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_subscription_filter)

```python
# put_subscription_filter method definition

await def put_subscription_filter(
    self,
    *,
    logGroupName: str,
    filterName: str,
    filterPattern: str,
    destinationArn: str,
    roleArn: str = ...,
    distribution: DistributionType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DistributionType](./literals.md#distributiontype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_subscription_filter method usage example with argument unpacking

kwargs: PutSubscriptionFilterRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "filterName": ...,
    "filterPattern": ...,
    "destinationArn": ...,
}

parent.put_subscription_filter(**kwargs)
```

1. See [:material-code-braces: PutSubscriptionFilterRequestRequestTypeDef](./type_defs.md#putsubscriptionfilterrequestrequesttypedef) 

### start\_live\_tail

Starts a Live Tail streaming session for one or more log groups.

Type annotations and code completion for `#!python session.create_client("logs").start_live_tail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_live_tail)

```python
# start_live_tail method definition

await def start_live_tail(
    self,
    *,
    logGroupIdentifiers: Sequence[str],
    logStreamNames: Sequence[str] = ...,
    logStreamNamePrefixes: Sequence[str] = ...,
    logEventFilterPattern: str = ...,
) -> StartLiveTailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartLiveTailResponseTypeDef](./type_defs.md#startlivetailresponsetypedef) 


```python
# start_live_tail method usage example with argument unpacking

kwargs: StartLiveTailRequestRequestTypeDef = {  # (1)
    "logGroupIdentifiers": ...,
}

parent.start_live_tail(**kwargs)
```

1. See [:material-code-braces: StartLiveTailRequestRequestTypeDef](./type_defs.md#startlivetailrequestrequesttypedef) 

### start\_query

Schedules a query of a log group using CloudWatch Logs Insights.

Type annotations and code completion for `#!python session.create_client("logs").start_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_query)

```python
# start_query method definition

await def start_query(
    self,
    *,
    startTime: int,
    endTime: int,
    queryString: str,
    logGroupName: str = ...,
    logGroupNames: Sequence[str] = ...,
    logGroupIdentifiers: Sequence[str] = ...,
    limit: int = ...,
) -> StartQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartQueryResponseTypeDef](./type_defs.md#startqueryresponsetypedef) 


```python
# start_query method usage example with argument unpacking

kwargs: StartQueryRequestRequestTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
    "queryString": ...,
}

parent.start_query(**kwargs)
```

1. See [:material-code-braces: StartQueryRequestRequestTypeDef](./type_defs.md#startqueryrequestrequesttypedef) 

### stop\_query

Stops a CloudWatch Logs Insights query that is in progress.

Type annotations and code completion for `#!python session.create_client("logs").stop_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.stop_query)

```python
# stop_query method definition

await def stop_query(
    self,
    *,
    queryId: str,
) -> StopQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopQueryResponseTypeDef](./type_defs.md#stopqueryresponsetypedef) 


```python
# stop_query method usage example with argument unpacking

kwargs: StopQueryRequestRequestTypeDef = {  # (1)
    "queryId": ...,
}

parent.stop_query(**kwargs)
```

1. See [:material-code-braces: StopQueryRequestRequestTypeDef](./type_defs.md#stopqueryrequestrequesttypedef) 

### tag\_log\_group

.

Type annotations and code completion for `#!python session.create_client("logs").tag_log_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.tag_log_group)

```python
# tag_log_group method definition

await def tag_log_group(
    self,
    *,
    logGroupName: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_log_group method usage example with argument unpacking

kwargs: TagLogGroupRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "tags": ...,
}

parent.tag_log_group(**kwargs)
```

1. See [:material-code-braces: TagLogGroupRequestRequestTypeDef](./type_defs.md#tagloggrouprequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified CloudWatch Logs
resource.

Type annotations and code completion for `#!python session.create_client("logs").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_metric\_filter

Tests the filter pattern of a metric filter against a sample of log event
messages.

Type annotations and code completion for `#!python session.create_client("logs").test_metric_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.test_metric_filter)

```python
# test_metric_filter method definition

await def test_metric_filter(
    self,
    *,
    filterPattern: str,
    logEventMessages: Sequence[str],
) -> TestMetricFilterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestMetricFilterResponseTypeDef](./type_defs.md#testmetricfilterresponsetypedef) 


```python
# test_metric_filter method usage example with argument unpacking

kwargs: TestMetricFilterRequestRequestTypeDef = {  # (1)
    "filterPattern": ...,
    "logEventMessages": ...,
}

parent.test_metric_filter(**kwargs)
```

1. See [:material-code-braces: TestMetricFilterRequestRequestTypeDef](./type_defs.md#testmetricfilterrequestrequesttypedef) 

### untag\_log\_group

.

Type annotations and code completion for `#!python session.create_client("logs").untag_log_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.untag_log_group)

```python
# untag_log_group method definition

await def untag_log_group(
    self,
    *,
    logGroupName: str,
    tags: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_log_group method usage example with argument unpacking

kwargs: UntagLogGroupRequestRequestTypeDef = {  # (1)
    "logGroupName": ...,
    "tags": ...,
}

parent.untag_log_group(**kwargs)
```

1. See [:material-code-braces: UntagLogGroupRequestRequestTypeDef](./type_defs.md#untagloggrouprequestrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("logs").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_anomaly

Use this operation to *suppress* anomaly detection for a specified anomaly or
pattern.

Type annotations and code completion for `#!python session.create_client("logs").update_anomaly` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.update_anomaly)

```python
# update_anomaly method definition

await def update_anomaly(
    self,
    *,
    anomalyDetectorArn: str,
    anomalyId: str = ...,
    patternId: str = ...,
    suppressionType: SuppressionTypeType = ...,  # (1)
    suppressionPeriod: SuppressionPeriodTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SuppressionTypeType](./literals.md#suppressiontypetype) 
2. See [:material-code-braces: SuppressionPeriodTypeDef](./type_defs.md#suppressionperiodtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_anomaly method usage example with argument unpacking

kwargs: UpdateAnomalyRequestRequestTypeDef = {  # (1)
    "anomalyDetectorArn": ...,
}

parent.update_anomaly(**kwargs)
```

1. See [:material-code-braces: UpdateAnomalyRequestRequestTypeDef](./type_defs.md#updateanomalyrequestrequesttypedef) 

### update\_delivery\_configuration

Use this operation to update the configuration of a
[delivery](https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_Delivery.html)
to change either the S3 path pattern or the format of the delivered
logs.

Type annotations and code completion for `#!python session.create_client("logs").update_delivery_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.update_delivery_configuration)

```python
# update_delivery_configuration method definition

await def update_delivery_configuration(
    self,
    *,
    id: str,
    recordFields: Sequence[str] = ...,
    fieldDelimiter: str = ...,
    s3DeliveryConfiguration: S3DeliveryConfigurationTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef) 


```python
# update_delivery_configuration method usage example with argument unpacking

kwargs: UpdateDeliveryConfigurationRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_delivery_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateDeliveryConfigurationRequestRequestTypeDef](./type_defs.md#updatedeliveryconfigurationrequestrequesttypedef) 

### update\_log\_anomaly\_detector

Updates an existing log anomaly detector.

Type annotations and code completion for `#!python session.create_client("logs").update_log_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.update_log_anomaly_detector)

```python
# update_log_anomaly_detector method definition

await def update_log_anomaly_detector(
    self,
    *,
    anomalyDetectorArn: str,
    enabled: bool,
    evaluationFrequency: EvaluationFrequencyType = ...,  # (1)
    filterPattern: str = ...,
    anomalyVisibilityTime: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EvaluationFrequencyType](./literals.md#evaluationfrequencytype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_log_anomaly_detector method usage example with argument unpacking

kwargs: UpdateLogAnomalyDetectorRequestRequestTypeDef = {  # (1)
    "anomalyDetectorArn": ...,
    "enabled": ...,
}

parent.update_log_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: UpdateLogAnomalyDetectorRequestRequestTypeDef](./type_defs.md#updateloganomalydetectorrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("logs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CloudWatchLogsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("logs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator` method with overloads.

- `client.get_paginator("describe_configuration_templates")` -> [DescribeConfigurationTemplatesPaginator](./paginators.md#describeconfigurationtemplatespaginator)
- `client.get_paginator("describe_deliveries")` -> [DescribeDeliveriesPaginator](./paginators.md#describedeliveriespaginator)
- `client.get_paginator("describe_delivery_destinations")` -> [DescribeDeliveryDestinationsPaginator](./paginators.md#describedeliverydestinationspaginator)
- `client.get_paginator("describe_delivery_sources")` -> [DescribeDeliverySourcesPaginator](./paginators.md#describedeliverysourcespaginator)
- `client.get_paginator("describe_destinations")` -> [DescribeDestinationsPaginator](./paginators.md#describedestinationspaginator)
- `client.get_paginator("describe_export_tasks")` -> [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
- `client.get_paginator("describe_log_groups")` -> [DescribeLogGroupsPaginator](./paginators.md#describeloggroupspaginator)
- `client.get_paginator("describe_log_streams")` -> [DescribeLogStreamsPaginator](./paginators.md#describelogstreamspaginator)
- `client.get_paginator("describe_metric_filters")` -> [DescribeMetricFiltersPaginator](./paginators.md#describemetricfilterspaginator)
- `client.get_paginator("describe_queries")` -> [DescribeQueriesPaginator](./paginators.md#describequeriespaginator)
- `client.get_paginator("describe_resource_policies")` -> [DescribeResourcePoliciesPaginator](./paginators.md#describeresourcepoliciespaginator)
- `client.get_paginator("describe_subscription_filters")` -> [DescribeSubscriptionFiltersPaginator](./paginators.md#describesubscriptionfilterspaginator)
- `client.get_paginator("filter_log_events")` -> [FilterLogEventsPaginator](./paginators.md#filterlogeventspaginator)
- `client.get_paginator("list_anomalies")` -> [ListAnomaliesPaginator](./paginators.md#listanomaliespaginator)
- `client.get_paginator("list_log_anomaly_detectors")` -> [ListLogAnomalyDetectorsPaginator](./paginators.md#listloganomalydetectorspaginator)



