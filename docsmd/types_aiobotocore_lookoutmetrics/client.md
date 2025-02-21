# LookoutMetricsClient

> [Index](../README.md) > [LookoutMetrics](./README.md) > LookoutMetricsClient

!!! note ""

    Auto-generated documentation for [LookoutMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#lookoutmetrics)
    type annotations stubs module [types-aiobotocore-lookoutmetrics](https://pypi.org/project/types-aiobotocore-lookoutmetrics/).

## LookoutMetricsClient

Type annotations and code completion for `#!python session.create_client("lookoutmetrics")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client)

```python
# LookoutMetricsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_lookoutmetrics.client import LookoutMetricsClient

session = get_session()
async with session.create_client("lookoutmetrics") as client:
    client: LookoutMetricsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("lookoutmetrics").exceptions` structure.

```python
# LookoutMetricsClient.exceptions usage example

async with session.create_client("lookoutmetrics") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.TooManyRequestsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# LookoutMetricsClient usage type checking example

from types_aiobotocore_lookoutmetrics.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("lookoutmetrics").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("lookoutmetrics").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/generate_presigned_url.html)

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


### activate\_anomaly\_detector

Activates an anomaly detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").activate_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/activate_anomaly_detector.html)

```python
# activate_anomaly_detector method definition

await def activate_anomaly_detector(
    self,
    *,
    AnomalyDetectorArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# activate_anomaly_detector method usage example with argument unpacking

kwargs: ActivateAnomalyDetectorRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.activate_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: ActivateAnomalyDetectorRequestTypeDef](./type_defs.md#activateanomalydetectorrequesttypedef) 

### back\_test\_anomaly\_detector

Runs a backtest for anomaly detection for the specified resource.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").back_test_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/back_test_anomaly_detector.html)

```python
# back_test_anomaly_detector method definition

await def back_test_anomaly_detector(
    self,
    *,
    AnomalyDetectorArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# back_test_anomaly_detector method usage example with argument unpacking

kwargs: BackTestAnomalyDetectorRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.back_test_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: BackTestAnomalyDetectorRequestTypeDef](./type_defs.md#backtestanomalydetectorrequesttypedef) 

### create\_alert

Creates an alert for an anomaly detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").create_alert` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/create_alert.html)

```python
# create_alert method definition

await def create_alert(
    self,
    *,
    AlertName: str,
    AnomalyDetectorArn: str,
    Action: ActionTypeDef,  # (1)
    AlertSensitivityThreshold: int = ...,
    AlertDescription: str = ...,
    Tags: Mapping[str, str] = ...,
    AlertFilters: AlertFiltersUnionTypeDef = ...,  # (2)
) -> CreateAlertResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) [:material-code-braces: AlertFiltersOutputTypeDef](./type_defs.md#alertfiltersoutputtypedef) 
3. See [:material-code-braces: CreateAlertResponseTypeDef](./type_defs.md#createalertresponsetypedef) 


```python
# create_alert method usage example with argument unpacking

kwargs: CreateAlertRequestTypeDef = {  # (1)
    "AlertName": ...,
    "AnomalyDetectorArn": ...,
    "Action": ...,
}

parent.create_alert(**kwargs)
```

1. See [:material-code-braces: CreateAlertRequestTypeDef](./type_defs.md#createalertrequesttypedef) 

### create\_anomaly\_detector

Creates an anomaly detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").create_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/create_anomaly_detector.html)

```python
# create_anomaly_detector method definition

await def create_anomaly_detector(
    self,
    *,
    AnomalyDetectorName: str,
    AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef,  # (1)
    AnomalyDetectorDescription: str = ...,
    KmsKeyArn: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateAnomalyDetectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnomalyDetectorConfigTypeDef](./type_defs.md#anomalydetectorconfigtypedef) 
2. See [:material-code-braces: CreateAnomalyDetectorResponseTypeDef](./type_defs.md#createanomalydetectorresponsetypedef) 


```python
# create_anomaly_detector method usage example with argument unpacking

kwargs: CreateAnomalyDetectorRequestTypeDef = {  # (1)
    "AnomalyDetectorName": ...,
    "AnomalyDetectorConfig": ...,
}

parent.create_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: CreateAnomalyDetectorRequestTypeDef](./type_defs.md#createanomalydetectorrequesttypedef) 

### create\_metric\_set

Creates a dataset.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").create_metric_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/create_metric_set.html)

```python
# create_metric_set method definition

await def create_metric_set(
    self,
    *,
    AnomalyDetectorArn: str,
    MetricSetName: str,
    MetricList: Sequence[MetricTypeDef],  # (1)
    MetricSource: MetricSourceUnionTypeDef,  # (2)
    MetricSetDescription: str = ...,
    Offset: int = ...,
    TimestampColumn: TimestampColumnTypeDef = ...,  # (3)
    DimensionList: Sequence[str] = ...,
    MetricSetFrequency: FrequencyType = ...,  # (4)
    Timezone: str = ...,
    Tags: Mapping[str, str] = ...,
    DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...,  # (5)
) -> CreateMetricSetResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) [:material-code-braces: MetricSourceOutputTypeDef](./type_defs.md#metricsourceoutputtypedef) 
3. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
4. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
5. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) [:material-code-braces: MetricSetDimensionFilterOutputTypeDef](./type_defs.md#metricsetdimensionfilteroutputtypedef) 
6. See [:material-code-braces: CreateMetricSetResponseTypeDef](./type_defs.md#createmetricsetresponsetypedef) 


```python
# create_metric_set method usage example with argument unpacking

kwargs: CreateMetricSetRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
    "MetricSetName": ...,
    "MetricList": ...,
    "MetricSource": ...,
}

parent.create_metric_set(**kwargs)
```

1. See [:material-code-braces: CreateMetricSetRequestTypeDef](./type_defs.md#createmetricsetrequesttypedef) 

### deactivate\_anomaly\_detector

Deactivates an anomaly detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").deactivate_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/deactivate_anomaly_detector.html)

```python
# deactivate_anomaly_detector method definition

await def deactivate_anomaly_detector(
    self,
    *,
    AnomalyDetectorArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# deactivate_anomaly_detector method usage example with argument unpacking

kwargs: DeactivateAnomalyDetectorRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.deactivate_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: DeactivateAnomalyDetectorRequestTypeDef](./type_defs.md#deactivateanomalydetectorrequesttypedef) 

### delete\_alert

Deletes an alert.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").delete_alert` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/delete_alert.html)

```python
# delete_alert method definition

await def delete_alert(
    self,
    *,
    AlertArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_alert method usage example with argument unpacking

kwargs: DeleteAlertRequestTypeDef = {  # (1)
    "AlertArn": ...,
}

parent.delete_alert(**kwargs)
```

1. See [:material-code-braces: DeleteAlertRequestTypeDef](./type_defs.md#deletealertrequesttypedef) 

### delete\_anomaly\_detector

Deletes a detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").delete_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/delete_anomaly_detector.html)

```python
# delete_anomaly_detector method definition

await def delete_anomaly_detector(
    self,
    *,
    AnomalyDetectorArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_anomaly_detector method usage example with argument unpacking

kwargs: DeleteAnomalyDetectorRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.delete_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: DeleteAnomalyDetectorRequestTypeDef](./type_defs.md#deleteanomalydetectorrequesttypedef) 

### describe\_alert

Describes an alert.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").describe_alert` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/describe_alert.html)

```python
# describe_alert method definition

await def describe_alert(
    self,
    *,
    AlertArn: str,
) -> DescribeAlertResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAlertResponseTypeDef](./type_defs.md#describealertresponsetypedef) 


```python
# describe_alert method usage example with argument unpacking

kwargs: DescribeAlertRequestTypeDef = {  # (1)
    "AlertArn": ...,
}

parent.describe_alert(**kwargs)
```

1. See [:material-code-braces: DescribeAlertRequestTypeDef](./type_defs.md#describealertrequesttypedef) 

### describe\_anomaly\_detection\_executions

Returns information about the status of the specified anomaly detection jobs.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").describe_anomaly_detection_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/describe_anomaly_detection_executions.html)

```python
# describe_anomaly_detection_executions method definition

await def describe_anomaly_detection_executions(
    self,
    *,
    AnomalyDetectorArn: str,
    Timestamp: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeAnomalyDetectionExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAnomalyDetectionExecutionsResponseTypeDef](./type_defs.md#describeanomalydetectionexecutionsresponsetypedef) 


```python
# describe_anomaly_detection_executions method usage example with argument unpacking

kwargs: DescribeAnomalyDetectionExecutionsRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.describe_anomaly_detection_executions(**kwargs)
```

1. See [:material-code-braces: DescribeAnomalyDetectionExecutionsRequestTypeDef](./type_defs.md#describeanomalydetectionexecutionsrequesttypedef) 

### describe\_anomaly\_detector

Describes a detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").describe_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/describe_anomaly_detector.html)

```python
# describe_anomaly_detector method definition

await def describe_anomaly_detector(
    self,
    *,
    AnomalyDetectorArn: str,
) -> DescribeAnomalyDetectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAnomalyDetectorResponseTypeDef](./type_defs.md#describeanomalydetectorresponsetypedef) 


```python
# describe_anomaly_detector method usage example with argument unpacking

kwargs: DescribeAnomalyDetectorRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.describe_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: DescribeAnomalyDetectorRequestTypeDef](./type_defs.md#describeanomalydetectorrequesttypedef) 

### describe\_metric\_set

Describes a dataset.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").describe_metric_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/describe_metric_set.html)

```python
# describe_metric_set method definition

await def describe_metric_set(
    self,
    *,
    MetricSetArn: str,
) -> DescribeMetricSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMetricSetResponseTypeDef](./type_defs.md#describemetricsetresponsetypedef) 


```python
# describe_metric_set method usage example with argument unpacking

kwargs: DescribeMetricSetRequestTypeDef = {  # (1)
    "MetricSetArn": ...,
}

parent.describe_metric_set(**kwargs)
```

1. See [:material-code-braces: DescribeMetricSetRequestTypeDef](./type_defs.md#describemetricsetrequesttypedef) 

### detect\_metric\_set\_config

Detects an Amazon S3 dataset's file format, interval, and offset.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").detect_metric_set_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/detect_metric_set_config.html)

```python
# detect_metric_set_config method definition

await def detect_metric_set_config(
    self,
    *,
    AnomalyDetectorArn: str,
    AutoDetectionMetricSource: AutoDetectionMetricSourceTypeDef,  # (1)
) -> DetectMetricSetConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AutoDetectionMetricSourceTypeDef](./type_defs.md#autodetectionmetricsourcetypedef) 
2. See [:material-code-braces: DetectMetricSetConfigResponseTypeDef](./type_defs.md#detectmetricsetconfigresponsetypedef) 


```python
# detect_metric_set_config method usage example with argument unpacking

kwargs: DetectMetricSetConfigRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
    "AutoDetectionMetricSource": ...,
}

parent.detect_metric_set_config(**kwargs)
```

1. See [:material-code-braces: DetectMetricSetConfigRequestTypeDef](./type_defs.md#detectmetricsetconfigrequesttypedef) 

### get\_anomaly\_group

Returns details about a group of anomalous metrics.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").get_anomaly_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/get_anomaly_group.html)

```python
# get_anomaly_group method definition

await def get_anomaly_group(
    self,
    *,
    AnomalyGroupId: str,
    AnomalyDetectorArn: str,
) -> GetAnomalyGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnomalyGroupResponseTypeDef](./type_defs.md#getanomalygroupresponsetypedef) 


```python
# get_anomaly_group method usage example with argument unpacking

kwargs: GetAnomalyGroupRequestTypeDef = {  # (1)
    "AnomalyGroupId": ...,
    "AnomalyDetectorArn": ...,
}

parent.get_anomaly_group(**kwargs)
```

1. See [:material-code-braces: GetAnomalyGroupRequestTypeDef](./type_defs.md#getanomalygrouprequesttypedef) 

### get\_data\_quality\_metrics

Returns details about the requested data quality metrics.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").get_data_quality_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/get_data_quality_metrics.html)

```python
# get_data_quality_metrics method definition

await def get_data_quality_metrics(
    self,
    *,
    AnomalyDetectorArn: str,
    MetricSetArn: str = ...,
) -> GetDataQualityMetricsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataQualityMetricsResponseTypeDef](./type_defs.md#getdataqualitymetricsresponsetypedef) 


```python
# get_data_quality_metrics method usage example with argument unpacking

kwargs: GetDataQualityMetricsRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.get_data_quality_metrics(**kwargs)
```

1. See [:material-code-braces: GetDataQualityMetricsRequestTypeDef](./type_defs.md#getdataqualitymetricsrequesttypedef) 

### get\_feedback

Get feedback for an anomaly group.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").get_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/get_feedback.html)

```python
# get_feedback method definition

await def get_feedback(
    self,
    *,
    AnomalyDetectorArn: str,
    AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesTypeDef,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetFeedbackResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnomalyGroupTimeSeriesTypeDef](./type_defs.md#anomalygrouptimeseriestypedef) 
2. See [:material-code-braces: GetFeedbackResponseTypeDef](./type_defs.md#getfeedbackresponsetypedef) 


```python
# get_feedback method usage example with argument unpacking

kwargs: GetFeedbackRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
    "AnomalyGroupTimeSeriesFeedback": ...,
}

parent.get_feedback(**kwargs)
```

1. See [:material-code-braces: GetFeedbackRequestTypeDef](./type_defs.md#getfeedbackrequesttypedef) 

### get\_sample\_data

Returns a selection of sample records from an Amazon S3 datasource.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").get_sample_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/get_sample_data.html)

```python
# get_sample_data method definition

await def get_sample_data(
    self,
    *,
    S3SourceConfig: SampleDataS3SourceConfigTypeDef = ...,  # (1)
) -> GetSampleDataResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SampleDataS3SourceConfigTypeDef](./type_defs.md#sampledatas3sourceconfigtypedef) 
2. See [:material-code-braces: GetSampleDataResponseTypeDef](./type_defs.md#getsampledataresponsetypedef) 


```python
# get_sample_data method usage example with argument unpacking

kwargs: GetSampleDataRequestTypeDef = {  # (1)
    "S3SourceConfig": ...,
}

parent.get_sample_data(**kwargs)
```

1. See [:material-code-braces: GetSampleDataRequestTypeDef](./type_defs.md#getsampledatarequesttypedef) 

### list\_alerts

Lists the alerts attached to a detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").list_alerts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/list_alerts.html)

```python
# list_alerts method definition

await def list_alerts(
    self,
    *,
    AnomalyDetectorArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAlertsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAlertsResponseTypeDef](./type_defs.md#listalertsresponsetypedef) 


```python
# list_alerts method usage example with argument unpacking

kwargs: ListAlertsRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.list_alerts(**kwargs)
```

1. See [:material-code-braces: ListAlertsRequestTypeDef](./type_defs.md#listalertsrequesttypedef) 

### list\_anomaly\_detectors

Lists the detectors in the current AWS Region.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").list_anomaly_detectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/list_anomaly_detectors.html)

```python
# list_anomaly_detectors method definition

await def list_anomaly_detectors(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAnomalyDetectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAnomalyDetectorsResponseTypeDef](./type_defs.md#listanomalydetectorsresponsetypedef) 


```python
# list_anomaly_detectors method usage example with argument unpacking

kwargs: ListAnomalyDetectorsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_anomaly_detectors(**kwargs)
```

1. See [:material-code-braces: ListAnomalyDetectorsRequestTypeDef](./type_defs.md#listanomalydetectorsrequesttypedef) 

### list\_anomaly\_group\_related\_metrics

Returns a list of measures that are potential causes or effects of an anomaly
group.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").list_anomaly_group_related_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/list_anomaly_group_related_metrics.html)

```python
# list_anomaly_group_related_metrics method definition

await def list_anomaly_group_related_metrics(
    self,
    *,
    AnomalyDetectorArn: str,
    AnomalyGroupId: str,
    RelationshipTypeFilter: RelationshipTypeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAnomalyGroupRelatedMetricsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
2. See [:material-code-braces: ListAnomalyGroupRelatedMetricsResponseTypeDef](./type_defs.md#listanomalygrouprelatedmetricsresponsetypedef) 


```python
# list_anomaly_group_related_metrics method usage example with argument unpacking

kwargs: ListAnomalyGroupRelatedMetricsRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
    "AnomalyGroupId": ...,
}

parent.list_anomaly_group_related_metrics(**kwargs)
```

1. See [:material-code-braces: ListAnomalyGroupRelatedMetricsRequestTypeDef](./type_defs.md#listanomalygrouprelatedmetricsrequesttypedef) 

### list\_anomaly\_group\_summaries

Returns a list of anomaly groups.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").list_anomaly_group_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/list_anomaly_group_summaries.html)

```python
# list_anomaly_group_summaries method definition

await def list_anomaly_group_summaries(
    self,
    *,
    AnomalyDetectorArn: str,
    SensitivityThreshold: int,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAnomalyGroupSummariesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAnomalyGroupSummariesResponseTypeDef](./type_defs.md#listanomalygroupsummariesresponsetypedef) 


```python
# list_anomaly_group_summaries method usage example with argument unpacking

kwargs: ListAnomalyGroupSummariesRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
    "SensitivityThreshold": ...,
}

parent.list_anomaly_group_summaries(**kwargs)
```

1. See [:material-code-braces: ListAnomalyGroupSummariesRequestTypeDef](./type_defs.md#listanomalygroupsummariesrequesttypedef) 

### list\_anomaly\_group\_time\_series

Gets a list of anomalous metrics for a measure in an anomaly group.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").list_anomaly_group_time_series` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/list_anomaly_group_time_series.html)

```python
# list_anomaly_group_time_series method definition

await def list_anomaly_group_time_series(
    self,
    *,
    AnomalyDetectorArn: str,
    AnomalyGroupId: str,
    MetricName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAnomalyGroupTimeSeriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAnomalyGroupTimeSeriesResponseTypeDef](./type_defs.md#listanomalygrouptimeseriesresponsetypedef) 


```python
# list_anomaly_group_time_series method usage example with argument unpacking

kwargs: ListAnomalyGroupTimeSeriesRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
    "AnomalyGroupId": ...,
    "MetricName": ...,
}

parent.list_anomaly_group_time_series(**kwargs)
```

1. See [:material-code-braces: ListAnomalyGroupTimeSeriesRequestTypeDef](./type_defs.md#listanomalygrouptimeseriesrequesttypedef) 

### list\_metric\_sets

Lists the datasets in the current AWS Region.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").list_metric_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/list_metric_sets.html)

```python
# list_metric_sets method definition

await def list_metric_sets(
    self,
    *,
    AnomalyDetectorArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListMetricSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMetricSetsResponseTypeDef](./type_defs.md#listmetricsetsresponsetypedef) 


```python
# list_metric_sets method usage example with argument unpacking

kwargs: ListMetricSetsRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.list_metric_sets(**kwargs)
```

1. See [:material-code-braces: ListMetricSetsRequestTypeDef](./type_defs.md#listmetricsetsrequesttypedef) 

### list\_tags\_for\_resource

Gets a list of <a
href="https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html">tags</a>
for a detector, dataset, or alert.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### put\_feedback

Add feedback for an anomalous metric.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").put_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/put_feedback.html)

```python
# put_feedback method definition

await def put_feedback(
    self,
    *,
    AnomalyDetectorArn: str,
    AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesFeedbackTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AnomalyGroupTimeSeriesFeedbackTypeDef](./type_defs.md#anomalygrouptimeseriesfeedbacktypedef) 


```python
# put_feedback method usage example with argument unpacking

kwargs: PutFeedbackRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
    "AnomalyGroupTimeSeriesFeedback": ...,
}

parent.put_feedback(**kwargs)
```

1. See [:material-code-braces: PutFeedbackRequestTypeDef](./type_defs.md#putfeedbackrequesttypedef) 

### tag\_resource

Adds <a
href="https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html">tags</a>
to a detector, dataset, or alert.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes <a
href="https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html">tags</a>
from a detector, dataset, or alert.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_alert

Make changes to an existing alert.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").update_alert` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/update_alert.html)

```python
# update_alert method definition

await def update_alert(
    self,
    *,
    AlertArn: str,
    AlertDescription: str = ...,
    AlertSensitivityThreshold: int = ...,
    Action: ActionTypeDef = ...,  # (1)
    AlertFilters: AlertFiltersUnionTypeDef = ...,  # (2)
) -> UpdateAlertResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) [:material-code-braces: AlertFiltersOutputTypeDef](./type_defs.md#alertfiltersoutputtypedef) 
3. See [:material-code-braces: UpdateAlertResponseTypeDef](./type_defs.md#updatealertresponsetypedef) 


```python
# update_alert method usage example with argument unpacking

kwargs: UpdateAlertRequestTypeDef = {  # (1)
    "AlertArn": ...,
}

parent.update_alert(**kwargs)
```

1. See [:material-code-braces: UpdateAlertRequestTypeDef](./type_defs.md#updatealertrequesttypedef) 

### update\_anomaly\_detector

Updates a detector.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").update_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/update_anomaly_detector.html)

```python
# update_anomaly_detector method definition

await def update_anomaly_detector(
    self,
    *,
    AnomalyDetectorArn: str,
    KmsKeyArn: str = ...,
    AnomalyDetectorDescription: str = ...,
    AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef = ...,  # (1)
) -> UpdateAnomalyDetectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnomalyDetectorConfigTypeDef](./type_defs.md#anomalydetectorconfigtypedef) 
2. See [:material-code-braces: UpdateAnomalyDetectorResponseTypeDef](./type_defs.md#updateanomalydetectorresponsetypedef) 


```python
# update_anomaly_detector method usage example with argument unpacking

kwargs: UpdateAnomalyDetectorRequestTypeDef = {  # (1)
    "AnomalyDetectorArn": ...,
}

parent.update_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: UpdateAnomalyDetectorRequestTypeDef](./type_defs.md#updateanomalydetectorrequesttypedef) 

### update\_metric\_set

Updates a dataset.

Type annotations and code completion for `#!python session.create_client("lookoutmetrics").update_metric_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics/client/update_metric_set.html)

```python
# update_metric_set method definition

await def update_metric_set(
    self,
    *,
    MetricSetArn: str,
    MetricSetDescription: str = ...,
    MetricList: Sequence[MetricTypeDef] = ...,  # (1)
    Offset: int = ...,
    TimestampColumn: TimestampColumnTypeDef = ...,  # (2)
    DimensionList: Sequence[str] = ...,
    MetricSetFrequency: FrequencyType = ...,  # (3)
    MetricSource: MetricSourceUnionTypeDef = ...,  # (4)
    DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...,  # (5)
) -> UpdateMetricSetResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
3. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
4. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) [:material-code-braces: MetricSourceOutputTypeDef](./type_defs.md#metricsourceoutputtypedef) 
5. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) [:material-code-braces: MetricSetDimensionFilterOutputTypeDef](./type_defs.md#metricsetdimensionfilteroutputtypedef) 
6. See [:material-code-braces: UpdateMetricSetResponseTypeDef](./type_defs.md#updatemetricsetresponsetypedef) 


```python
# update_metric_set method usage example with argument unpacking

kwargs: UpdateMetricSetRequestTypeDef = {  # (1)
    "MetricSetArn": ...,
}

parent.update_metric_set(**kwargs)
```

1. See [:material-code-braces: UpdateMetricSetRequestTypeDef](./type_defs.md#updatemetricsetrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("lookoutmetrics").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("lookoutmetrics").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client)

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





