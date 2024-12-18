# CostExplorerClient

> [Index](../README.md) > [CostExplorer](./README.md) > CostExplorerClient

!!! note ""

    Auto-generated documentation for [CostExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#costexplorer)
    type annotations stubs module [types-aiobotocore-ce](https://pypi.org/project/types-aiobotocore-ce/).

## CostExplorerClient

Type annotations and code completion for `#!python session.create_client("ce")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client)

```python
# CostExplorerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ce.client import CostExplorerClient

session = get_session()
async with session.create_client("ce") as client:
    client: CostExplorerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ce").exceptions` structure.

```python
# CostExplorerClient.exceptions usage example

async with session.create_client("ce") as client:
    try:
        do_something(client)
    except (
            client.AnalysisNotFoundException,
        client.BackfillLimitExceededException,
        client.BillExpirationException,
        client.ClientError,
        client.DataUnavailableException,
        client.GenerationExistsException,
        client.InvalidNextTokenException,
        client.LimitExceededException,
        client.RequestChangedException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.TooManyTagsException,
        client.UnknownMonitorException,
        client.UnknownSubscriptionException,
        client.UnresolvableUsageUnitException,
    ) as e:
        print(e)
```

```python
# CostExplorerClient usage type checking example

from types_aiobotocore_ce.client import Exceptions

def handle_error(exc: Exceptions.AnalysisNotFoundException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("ce").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("ce").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("ce").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_anomaly\_monitor

Creates a new cost anomaly detection monitor with the requested type and
monitor specification.

Type annotations and code completion for `#!python session.create_client("ce").create_anomaly_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/create_anomaly_monitor.html)

```python
# create_anomaly_monitor method definition

await def create_anomaly_monitor(
    self,
    *,
    AnomalyMonitor: AnomalyMonitorTypeDef,  # (1)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
) -> CreateAnomalyMonitorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AnomalyMonitorTypeDef](./type_defs.md#anomalymonitortypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-braces: CreateAnomalyMonitorResponseTypeDef](./type_defs.md#createanomalymonitorresponsetypedef) 


```python
# create_anomaly_monitor method usage example with argument unpacking

kwargs: CreateAnomalyMonitorRequestRequestTypeDef = {  # (1)
    "AnomalyMonitor": ...,
}

parent.create_anomaly_monitor(**kwargs)
```

1. See [:material-code-braces: CreateAnomalyMonitorRequestRequestTypeDef](./type_defs.md#createanomalymonitorrequestrequesttypedef) 

### create\_anomaly\_subscription

Adds an alert subscription to a cost anomaly detection monitor.

Type annotations and code completion for `#!python session.create_client("ce").create_anomaly_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/create_anomaly_subscription.html)

```python
# create_anomaly_subscription method definition

await def create_anomaly_subscription(
    self,
    *,
    AnomalySubscription: AnomalySubscriptionTypeDef,  # (1)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
) -> CreateAnomalySubscriptionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AnomalySubscriptionTypeDef](./type_defs.md#anomalysubscriptiontypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-braces: CreateAnomalySubscriptionResponseTypeDef](./type_defs.md#createanomalysubscriptionresponsetypedef) 


```python
# create_anomaly_subscription method usage example with argument unpacking

kwargs: CreateAnomalySubscriptionRequestRequestTypeDef = {  # (1)
    "AnomalySubscription": ...,
}

parent.create_anomaly_subscription(**kwargs)
```

1. See [:material-code-braces: CreateAnomalySubscriptionRequestRequestTypeDef](./type_defs.md#createanomalysubscriptionrequestrequesttypedef) 

### create\_cost\_category\_definition

Creates a new Cost Category with the requested name and rules.

Type annotations and code completion for `#!python session.create_client("ce").create_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/create_cost_category_definition.html)

```python
# create_cost_category_definition method definition

await def create_cost_category_definition(
    self,
    *,
    Name: str,
    RuleVersion: CostCategoryRuleVersionType,  # (1)
    Rules: Sequence[CostCategoryRuleUnionTypeDef],  # (2)
    EffectiveStart: str = ...,
    DefaultValue: str = ...,
    SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...,  # (3)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (4)
) -> CreateCostCategoryDefinitionResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CostCategoryRuleVersionType](./literals.md#costcategoryruleversiontype) 
2. See [:material-code-braces: CostCategoryRuleTypeDef](./type_defs.md#costcategoryruletypedef) [:material-code-braces: CostCategoryRuleOutputTypeDef](./type_defs.md#costcategoryruleoutputtypedef) 
3. See [:material-code-braces: CostCategorySplitChargeRuleTypeDef](./type_defs.md#costcategorysplitchargeruletypedef) [:material-code-braces: CostCategorySplitChargeRuleOutputTypeDef](./type_defs.md#costcategorysplitchargeruleoutputtypedef) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
5. See [:material-code-braces: CreateCostCategoryDefinitionResponseTypeDef](./type_defs.md#createcostcategorydefinitionresponsetypedef) 


```python
# create_cost_category_definition method usage example with argument unpacking

kwargs: CreateCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RuleVersion": ...,
    "Rules": ...,
}

parent.create_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: CreateCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#createcostcategorydefinitionrequestrequesttypedef) 

### delete\_anomaly\_monitor

Deletes a cost anomaly monitor.

Type annotations and code completion for `#!python session.create_client("ce").delete_anomaly_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/delete_anomaly_monitor.html)

```python
# delete_anomaly_monitor method definition

await def delete_anomaly_monitor(
    self,
    *,
    MonitorArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_anomaly_monitor method usage example with argument unpacking

kwargs: DeleteAnomalyMonitorRequestRequestTypeDef = {  # (1)
    "MonitorArn": ...,
}

parent.delete_anomaly_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteAnomalyMonitorRequestRequestTypeDef](./type_defs.md#deleteanomalymonitorrequestrequesttypedef) 

### delete\_anomaly\_subscription

Deletes a cost anomaly subscription.

Type annotations and code completion for `#!python session.create_client("ce").delete_anomaly_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/delete_anomaly_subscription.html)

```python
# delete_anomaly_subscription method definition

await def delete_anomaly_subscription(
    self,
    *,
    SubscriptionArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_anomaly_subscription method usage example with argument unpacking

kwargs: DeleteAnomalySubscriptionRequestRequestTypeDef = {  # (1)
    "SubscriptionArn": ...,
}

parent.delete_anomaly_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteAnomalySubscriptionRequestRequestTypeDef](./type_defs.md#deleteanomalysubscriptionrequestrequesttypedef) 

### delete\_cost\_category\_definition

Deletes a Cost Category.

Type annotations and code completion for `#!python session.create_client("ce").delete_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/delete_cost_category_definition.html)

```python
# delete_cost_category_definition method definition

await def delete_cost_category_definition(
    self,
    *,
    CostCategoryArn: str,
) -> DeleteCostCategoryDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCostCategoryDefinitionResponseTypeDef](./type_defs.md#deletecostcategorydefinitionresponsetypedef) 


```python
# delete_cost_category_definition method usage example with argument unpacking

kwargs: DeleteCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "CostCategoryArn": ...,
}

parent.delete_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: DeleteCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#deletecostcategorydefinitionrequestrequesttypedef) 

### describe\_cost\_category\_definition

Returns the name, Amazon Resource Name (ARN), rules, definition, and effective
dates of a Cost Category that's defined in the account.

Type annotations and code completion for `#!python session.create_client("ce").describe_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/describe_cost_category_definition.html)

```python
# describe_cost_category_definition method definition

await def describe_cost_category_definition(
    self,
    *,
    CostCategoryArn: str,
    EffectiveOn: str = ...,
) -> DescribeCostCategoryDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCostCategoryDefinitionResponseTypeDef](./type_defs.md#describecostcategorydefinitionresponsetypedef) 


```python
# describe_cost_category_definition method usage example with argument unpacking

kwargs: DescribeCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "CostCategoryArn": ...,
}

parent.describe_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: DescribeCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#describecostcategorydefinitionrequestrequesttypedef) 

### get\_anomalies

Retrieves all of the cost anomalies detected on your account during the time
period that's specified by the <code>DateInterval</code> object.

Type annotations and code completion for `#!python session.create_client("ce").get_anomalies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_anomalies.html)

```python
# get_anomalies method definition

await def get_anomalies(
    self,
    *,
    DateInterval: AnomalyDateIntervalTypeDef,  # (1)
    MonitorArn: str = ...,
    Feedback: AnomalyFeedbackTypeType = ...,  # (2)
    TotalImpact: TotalImpactFilterTypeDef = ...,  # (3)
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetAnomaliesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AnomalyDateIntervalTypeDef](./type_defs.md#anomalydateintervaltypedef) 
2. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype) 
3. See [:material-code-braces: TotalImpactFilterTypeDef](./type_defs.md#totalimpactfiltertypedef) 
4. See [:material-code-braces: GetAnomaliesResponseTypeDef](./type_defs.md#getanomaliesresponsetypedef) 


```python
# get_anomalies method usage example with argument unpacking

kwargs: GetAnomaliesRequestRequestTypeDef = {  # (1)
    "DateInterval": ...,
}

parent.get_anomalies(**kwargs)
```

1. See [:material-code-braces: GetAnomaliesRequestRequestTypeDef](./type_defs.md#getanomaliesrequestrequesttypedef) 

### get\_anomaly\_monitors

Retrieves the cost anomaly monitor definitions for your account.

Type annotations and code completion for `#!python session.create_client("ce").get_anomaly_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_anomaly_monitors.html)

```python
# get_anomaly_monitors method definition

await def get_anomaly_monitors(
    self,
    *,
    MonitorArnList: Sequence[str] = ...,
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetAnomalyMonitorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnomalyMonitorsResponseTypeDef](./type_defs.md#getanomalymonitorsresponsetypedef) 


```python
# get_anomaly_monitors method usage example with argument unpacking

kwargs: GetAnomalyMonitorsRequestRequestTypeDef = {  # (1)
    "MonitorArnList": ...,
}

parent.get_anomaly_monitors(**kwargs)
```

1. See [:material-code-braces: GetAnomalyMonitorsRequestRequestTypeDef](./type_defs.md#getanomalymonitorsrequestrequesttypedef) 

### get\_anomaly\_subscriptions

Retrieves the cost anomaly subscription objects for your account.

Type annotations and code completion for `#!python session.create_client("ce").get_anomaly_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_anomaly_subscriptions.html)

```python
# get_anomaly_subscriptions method definition

await def get_anomaly_subscriptions(
    self,
    *,
    SubscriptionArnList: Sequence[str] = ...,
    MonitorArn: str = ...,
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetAnomalySubscriptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnomalySubscriptionsResponseTypeDef](./type_defs.md#getanomalysubscriptionsresponsetypedef) 


```python
# get_anomaly_subscriptions method usage example with argument unpacking

kwargs: GetAnomalySubscriptionsRequestRequestTypeDef = {  # (1)
    "SubscriptionArnList": ...,
}

parent.get_anomaly_subscriptions(**kwargs)
```

1. See [:material-code-braces: GetAnomalySubscriptionsRequestRequestTypeDef](./type_defs.md#getanomalysubscriptionsrequestrequesttypedef) 

### get\_approximate\_usage\_records

Retrieves estimated usage records for hourly granularity or resource-level data
at daily granularity.

Type annotations and code completion for `#!python session.create_client("ce").get_approximate_usage_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_approximate_usage_records.html)

```python
# get_approximate_usage_records method definition

await def get_approximate_usage_records(
    self,
    *,
    Granularity: GranularityType,  # (1)
    ApproximationDimension: ApproximationDimensionType,  # (2)
    Services: Sequence[str] = ...,
) -> GetApproximateUsageRecordsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
2. See [:material-code-brackets: ApproximationDimensionType](./literals.md#approximationdimensiontype) 
3. See [:material-code-braces: GetApproximateUsageRecordsResponseTypeDef](./type_defs.md#getapproximateusagerecordsresponsetypedef) 


```python
# get_approximate_usage_records method usage example with argument unpacking

kwargs: GetApproximateUsageRecordsRequestRequestTypeDef = {  # (1)
    "Granularity": ...,
    "ApproximationDimension": ...,
}

parent.get_approximate_usage_records(**kwargs)
```

1. See [:material-code-braces: GetApproximateUsageRecordsRequestRequestTypeDef](./type_defs.md#getapproximateusagerecordsrequestrequesttypedef) 

### get\_commitment\_purchase\_analysis

Retrieves a commitment purchase analysis result based on the
<code>AnalysisId</code>.

Type annotations and code completion for `#!python session.create_client("ce").get_commitment_purchase_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_commitment_purchase_analysis.html)

```python
# get_commitment_purchase_analysis method definition

await def get_commitment_purchase_analysis(
    self,
    *,
    AnalysisId: str,
) -> GetCommitmentPurchaseAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCommitmentPurchaseAnalysisResponseTypeDef](./type_defs.md#getcommitmentpurchaseanalysisresponsetypedef) 


```python
# get_commitment_purchase_analysis method usage example with argument unpacking

kwargs: GetCommitmentPurchaseAnalysisRequestRequestTypeDef = {  # (1)
    "AnalysisId": ...,
}

parent.get_commitment_purchase_analysis(**kwargs)
```

1. See [:material-code-braces: GetCommitmentPurchaseAnalysisRequestRequestTypeDef](./type_defs.md#getcommitmentpurchaseanalysisrequestrequesttypedef) 

### get\_cost\_and\_usage

Retrieves cost and usage metrics for your account.

Type annotations and code completion for `#!python session.create_client("ce").get_cost_and_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_cost_and_usage.html)

```python
# get_cost_and_usage method definition

await def get_cost_and_usage(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType,  # (2)
    Metrics: Sequence[str],
    Filter: ExpressionTypeDef = ...,  # (3)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (4)
    NextPageToken: str = ...,
) -> GetCostAndUsageResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
5. See [:material-code-braces: GetCostAndUsageResponseTypeDef](./type_defs.md#getcostandusageresponsetypedef) 


```python
# get_cost_and_usage method usage example with argument unpacking

kwargs: GetCostAndUsageRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Granularity": ...,
    "Metrics": ...,
}

parent.get_cost_and_usage(**kwargs)
```

1. See [:material-code-braces: GetCostAndUsageRequestRequestTypeDef](./type_defs.md#getcostandusagerequestrequesttypedef) 

### get\_cost\_and\_usage\_with\_resources

Retrieves cost and usage metrics with resources for your account.

Type annotations and code completion for `#!python session.create_client("ce").get_cost_and_usage_with_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_cost_and_usage_with_resources.html)

```python
# get_cost_and_usage_with_resources method definition

await def get_cost_and_usage_with_resources(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType,  # (2)
    Filter: ExpressionTypeDef,  # (3)
    Metrics: Sequence[str] = ...,
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (4)
    NextPageToken: str = ...,
) -> GetCostAndUsageWithResourcesResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
5. See [:material-code-braces: GetCostAndUsageWithResourcesResponseTypeDef](./type_defs.md#getcostandusagewithresourcesresponsetypedef) 


```python
# get_cost_and_usage_with_resources method usage example with argument unpacking

kwargs: GetCostAndUsageWithResourcesRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Granularity": ...,
    "Filter": ...,
}

parent.get_cost_and_usage_with_resources(**kwargs)
```

1. See [:material-code-braces: GetCostAndUsageWithResourcesRequestRequestTypeDef](./type_defs.md#getcostandusagewithresourcesrequestrequesttypedef) 

### get\_cost\_categories

Retrieves an array of Cost Category names and values incurred cost.

Type annotations and code completion for `#!python session.create_client("ce").get_cost_categories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_cost_categories.html)

```python
# get_cost_categories method definition

await def get_cost_categories(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    SearchString: str = ...,
    CostCategoryName: str = ...,
    Filter: ExpressionTypeDef = ...,  # (2)
    SortBy: Sequence[SortDefinitionTypeDef] = ...,  # (3)
    MaxResults: int = ...,
    NextPageToken: str = ...,
) -> GetCostCategoriesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
4. See [:material-code-braces: GetCostCategoriesResponseTypeDef](./type_defs.md#getcostcategoriesresponsetypedef) 


```python
# get_cost_categories method usage example with argument unpacking

kwargs: GetCostCategoriesRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_cost_categories(**kwargs)
```

1. See [:material-code-braces: GetCostCategoriesRequestRequestTypeDef](./type_defs.md#getcostcategoriesrequestrequesttypedef) 

### get\_cost\_forecast

Retrieves a forecast for how much Amazon Web Services predicts that you will
spend over the forecast time period that you select, based on your past costs.

Type annotations and code completion for `#!python session.create_client("ce").get_cost_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_cost_forecast.html)

```python
# get_cost_forecast method definition

await def get_cost_forecast(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Metric: MetricType,  # (2)
    Granularity: GranularityType,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    PredictionIntervalLevel: int = ...,
) -> GetCostForecastResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: GetCostForecastResponseTypeDef](./type_defs.md#getcostforecastresponsetypedef) 


```python
# get_cost_forecast method usage example with argument unpacking

kwargs: GetCostForecastRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Metric": ...,
    "Granularity": ...,
}

parent.get_cost_forecast(**kwargs)
```

1. See [:material-code-braces: GetCostForecastRequestRequestTypeDef](./type_defs.md#getcostforecastrequestrequesttypedef) 

### get\_dimension\_values

Retrieves all available filter values for a specified filter over a period of
time.

Type annotations and code completion for `#!python session.create_client("ce").get_dimension_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_dimension_values.html)

```python
# get_dimension_values method definition

await def get_dimension_values(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Dimension: DimensionType,  # (2)
    SearchString: str = ...,
    Context: ContextType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    SortBy: Sequence[SortDefinitionTypeDef] = ...,  # (5)
    MaxResults: int = ...,
    NextPageToken: str = ...,
) -> GetDimensionValuesResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
3. See [:material-code-brackets: ContextType](./literals.md#contexttype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetDimensionValuesResponseTypeDef](./type_defs.md#getdimensionvaluesresponsetypedef) 


```python
# get_dimension_values method usage example with argument unpacking

kwargs: GetDimensionValuesRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Dimension": ...,
}

parent.get_dimension_values(**kwargs)
```

1. See [:material-code-braces: GetDimensionValuesRequestRequestTypeDef](./type_defs.md#getdimensionvaluesrequestrequesttypedef) 

### get\_reservation\_coverage

Retrieves the reservation coverage for your account, which you can use to see
how much of your Amazon Elastic Compute Cloud, Amazon ElastiCache, Amazon
Relational Database Service, or Amazon Redshift usage is covered by a
reservation.

Type annotations and code completion for `#!python session.create_client("ce").get_reservation_coverage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_reservation_coverage.html)

```python
# get_reservation_coverage method definition

await def get_reservation_coverage(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (2)
    Granularity: GranularityType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    Metrics: Sequence[str] = ...,
    NextPageToken: str = ...,
    SortBy: SortDefinitionTypeDef = ...,  # (5)
    MaxResults: int = ...,
) -> GetReservationCoverageResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetReservationCoverageResponseTypeDef](./type_defs.md#getreservationcoverageresponsetypedef) 


```python
# get_reservation_coverage method usage example with argument unpacking

kwargs: GetReservationCoverageRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_reservation_coverage(**kwargs)
```

1. See [:material-code-braces: GetReservationCoverageRequestRequestTypeDef](./type_defs.md#getreservationcoveragerequestrequesttypedef) 

### get\_reservation\_purchase\_recommendation

Gets recommendations for reservation purchases.

Type annotations and code completion for `#!python session.create_client("ce").get_reservation_purchase_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_reservation_purchase_recommendation.html)

```python
# get_reservation_purchase_recommendation method definition

await def get_reservation_purchase_recommendation(
    self,
    *,
    Service: str,
    AccountId: str = ...,
    Filter: ExpressionTypeDef = ...,  # (1)
    AccountScope: AccountScopeType = ...,  # (2)
    LookbackPeriodInDays: LookbackPeriodInDaysType = ...,  # (3)
    TermInYears: TermInYearsType = ...,  # (4)
    PaymentOption: PaymentOptionType = ...,  # (5)
    ServiceSpecification: ServiceSpecificationTypeDef = ...,  # (6)
    PageSize: int = ...,
    NextPageToken: str = ...,
) -> GetReservationPurchaseRecommendationResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
3. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
4. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
5. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
6. See [:material-code-braces: ServiceSpecificationTypeDef](./type_defs.md#servicespecificationtypedef) 
7. See [:material-code-braces: GetReservationPurchaseRecommendationResponseTypeDef](./type_defs.md#getreservationpurchaserecommendationresponsetypedef) 


```python
# get_reservation_purchase_recommendation method usage example with argument unpacking

kwargs: GetReservationPurchaseRecommendationRequestRequestTypeDef = {  # (1)
    "Service": ...,
}

parent.get_reservation_purchase_recommendation(**kwargs)
```

1. See [:material-code-braces: GetReservationPurchaseRecommendationRequestRequestTypeDef](./type_defs.md#getreservationpurchaserecommendationrequestrequesttypedef) 

### get\_reservation\_utilization

Retrieves the reservation utilization for your account.

Type annotations and code completion for `#!python session.create_client("ce").get_reservation_utilization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_reservation_utilization.html)

```python
# get_reservation_utilization method definition

await def get_reservation_utilization(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (2)
    Granularity: GranularityType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    SortBy: SortDefinitionTypeDef = ...,  # (5)
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetReservationUtilizationResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetReservationUtilizationResponseTypeDef](./type_defs.md#getreservationutilizationresponsetypedef) 


```python
# get_reservation_utilization method usage example with argument unpacking

kwargs: GetReservationUtilizationRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_reservation_utilization(**kwargs)
```

1. See [:material-code-braces: GetReservationUtilizationRequestRequestTypeDef](./type_defs.md#getreservationutilizationrequestrequesttypedef) 

### get\_rightsizing\_recommendation

Creates recommendations that help you save cost by identifying idle and
underutilized Amazon EC2 instances.

Type annotations and code completion for `#!python session.create_client("ce").get_rightsizing_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_rightsizing_recommendation.html)

```python
# get_rightsizing_recommendation method definition

await def get_rightsizing_recommendation(
    self,
    *,
    Service: str,
    Filter: ExpressionTypeDef = ...,  # (1)
    Configuration: RightsizingRecommendationConfigurationTypeDef = ...,  # (2)
    PageSize: int = ...,
    NextPageToken: str = ...,
) -> GetRightsizingRecommendationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: RightsizingRecommendationConfigurationTypeDef](./type_defs.md#rightsizingrecommendationconfigurationtypedef) 
3. See [:material-code-braces: GetRightsizingRecommendationResponseTypeDef](./type_defs.md#getrightsizingrecommendationresponsetypedef) 


```python
# get_rightsizing_recommendation method usage example with argument unpacking

kwargs: GetRightsizingRecommendationRequestRequestTypeDef = {  # (1)
    "Service": ...,
}

parent.get_rightsizing_recommendation(**kwargs)
```

1. See [:material-code-braces: GetRightsizingRecommendationRequestRequestTypeDef](./type_defs.md#getrightsizingrecommendationrequestrequesttypedef) 

### get\_savings\_plan\_purchase\_recommendation\_details

Retrieves the details for a Savings Plan recommendation.

Type annotations and code completion for `#!python session.create_client("ce").get_savings_plan_purchase_recommendation_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_savings_plan_purchase_recommendation_details.html)

```python
# get_savings_plan_purchase_recommendation_details method definition

await def get_savings_plan_purchase_recommendation_details(
    self,
    *,
    RecommendationDetailId: str,
) -> GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef](./type_defs.md#getsavingsplanpurchaserecommendationdetailsresponsetypedef) 


```python
# get_savings_plan_purchase_recommendation_details method usage example with argument unpacking

kwargs: GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef = {  # (1)
    "RecommendationDetailId": ...,
}

parent.get_savings_plan_purchase_recommendation_details(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef](./type_defs.md#getsavingsplanpurchaserecommendationdetailsrequestrequesttypedef) 

### get\_savings\_plans\_coverage

Retrieves the Savings Plans covered for your account.

Type annotations and code completion for `#!python session.create_client("ce").get_savings_plans_coverage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_savings_plans_coverage.html)

```python
# get_savings_plans_coverage method definition

await def get_savings_plans_coverage(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (2)
    Granularity: GranularityType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    Metrics: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortBy: SortDefinitionTypeDef = ...,  # (5)
) -> GetSavingsPlansCoverageResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetSavingsPlansCoverageResponseTypeDef](./type_defs.md#getsavingsplanscoverageresponsetypedef) 


```python
# get_savings_plans_coverage method usage example with argument unpacking

kwargs: GetSavingsPlansCoverageRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_savings_plans_coverage(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansCoverageRequestRequestTypeDef](./type_defs.md#getsavingsplanscoveragerequestrequesttypedef) 

### get\_savings\_plans\_purchase\_recommendation

Retrieves the Savings Plans recommendations for your account.

Type annotations and code completion for `#!python session.create_client("ce").get_savings_plans_purchase_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_savings_plans_purchase_recommendation.html)

```python
# get_savings_plans_purchase_recommendation method definition

await def get_savings_plans_purchase_recommendation(
    self,
    *,
    SavingsPlansType: SupportedSavingsPlansTypeType,  # (1)
    TermInYears: TermInYearsType,  # (2)
    PaymentOption: PaymentOptionType,  # (3)
    LookbackPeriodInDays: LookbackPeriodInDaysType,  # (4)
    AccountScope: AccountScopeType = ...,  # (5)
    NextPageToken: str = ...,
    PageSize: int = ...,
    Filter: ExpressionTypeDef = ...,  # (6)
) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: SupportedSavingsPlansTypeType](./literals.md#supportedsavingsplanstypetype) 
2. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
3. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
4. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
5. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
6. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
7. See [:material-code-braces: GetSavingsPlansPurchaseRecommendationResponseTypeDef](./type_defs.md#getsavingsplanspurchaserecommendationresponsetypedef) 


```python
# get_savings_plans_purchase_recommendation method usage example with argument unpacking

kwargs: GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef = {  # (1)
    "SavingsPlansType": ...,
    "TermInYears": ...,
    "PaymentOption": ...,
    "LookbackPeriodInDays": ...,
}

parent.get_savings_plans_purchase_recommendation(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef](./type_defs.md#getsavingsplanspurchaserecommendationrequestrequesttypedef) 

### get\_savings\_plans\_utilization

Retrieves the Savings Plans utilization for your account across date ranges
with daily or monthly granularity.

Type annotations and code completion for `#!python session.create_client("ce").get_savings_plans_utilization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_savings_plans_utilization.html)

```python
# get_savings_plans_utilization method definition

await def get_savings_plans_utilization(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType = ...,  # (2)
    Filter: ExpressionTypeDef = ...,  # (3)
    SortBy: SortDefinitionTypeDef = ...,  # (4)
) -> GetSavingsPlansUtilizationResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
5. See [:material-code-braces: GetSavingsPlansUtilizationResponseTypeDef](./type_defs.md#getsavingsplansutilizationresponsetypedef) 


```python
# get_savings_plans_utilization method usage example with argument unpacking

kwargs: GetSavingsPlansUtilizationRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_savings_plans_utilization(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansUtilizationRequestRequestTypeDef](./type_defs.md#getsavingsplansutilizationrequestrequesttypedef) 

### get\_savings\_plans\_utilization\_details

Retrieves attribute data along with aggregate utilization and savings data for
a given time period.

Type annotations and code completion for `#!python session.create_client("ce").get_savings_plans_utilization_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_savings_plans_utilization_details.html)

```python
# get_savings_plans_utilization_details method definition

await def get_savings_plans_utilization_details(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Filter: ExpressionTypeDef = ...,  # (2)
    DataType: Sequence[SavingsPlansDataTypeType] = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
    SortBy: SortDefinitionTypeDef = ...,  # (4)
) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-brackets: SavingsPlansDataTypeType](./literals.md#savingsplansdatatypetype) 
4. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
5. See [:material-code-braces: GetSavingsPlansUtilizationDetailsResponseTypeDef](./type_defs.md#getsavingsplansutilizationdetailsresponsetypedef) 


```python
# get_savings_plans_utilization_details method usage example with argument unpacking

kwargs: GetSavingsPlansUtilizationDetailsRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_savings_plans_utilization_details(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansUtilizationDetailsRequestRequestTypeDef](./type_defs.md#getsavingsplansutilizationdetailsrequestrequesttypedef) 

### get\_tags

Queries for available tag keys and tag values for a specified period.

Type annotations and code completion for `#!python session.create_client("ce").get_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_tags.html)

```python
# get_tags method definition

await def get_tags(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    SearchString: str = ...,
    TagKey: str = ...,
    Filter: ExpressionTypeDef = ...,  # (2)
    SortBy: Sequence[SortDefinitionTypeDef] = ...,  # (3)
    MaxResults: int = ...,
    NextPageToken: str = ...,
) -> GetTagsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
4. See [:material-code-braces: GetTagsResponseTypeDef](./type_defs.md#gettagsresponsetypedef) 


```python
# get_tags method usage example with argument unpacking

kwargs: GetTagsRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_tags(**kwargs)
```

1. See [:material-code-braces: GetTagsRequestRequestTypeDef](./type_defs.md#gettagsrequestrequesttypedef) 

### get\_usage\_forecast

Retrieves a forecast for how much Amazon Web Services predicts that you will
use over the forecast time period that you select, based on your past usage.

Type annotations and code completion for `#!python session.create_client("ce").get_usage_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/get_usage_forecast.html)

```python
# get_usage_forecast method definition

await def get_usage_forecast(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Metric: MetricType,  # (2)
    Granularity: GranularityType,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    PredictionIntervalLevel: int = ...,
) -> GetUsageForecastResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: GetUsageForecastResponseTypeDef](./type_defs.md#getusageforecastresponsetypedef) 


```python
# get_usage_forecast method usage example with argument unpacking

kwargs: GetUsageForecastRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Metric": ...,
    "Granularity": ...,
}

parent.get_usage_forecast(**kwargs)
```

1. See [:material-code-braces: GetUsageForecastRequestRequestTypeDef](./type_defs.md#getusageforecastrequestrequesttypedef) 

### list\_commitment\_purchase\_analyses

Lists the commitment purchase analyses for your account.

Type annotations and code completion for `#!python session.create_client("ce").list_commitment_purchase_analyses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/list_commitment_purchase_analyses.html)

```python
# list_commitment_purchase_analyses method definition

await def list_commitment_purchase_analyses(
    self,
    *,
    AnalysisStatus: AnalysisStatusType = ...,  # (1)
    NextPageToken: str = ...,
    PageSize: int = ...,
    AnalysisIds: Sequence[str] = ...,
) -> ListCommitmentPurchaseAnalysesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AnalysisStatusType](./literals.md#analysisstatustype) 
2. See [:material-code-braces: ListCommitmentPurchaseAnalysesResponseTypeDef](./type_defs.md#listcommitmentpurchaseanalysesresponsetypedef) 


```python
# list_commitment_purchase_analyses method usage example with argument unpacking

kwargs: ListCommitmentPurchaseAnalysesRequestRequestTypeDef = {  # (1)
    "AnalysisStatus": ...,
}

parent.list_commitment_purchase_analyses(**kwargs)
```

1. See [:material-code-braces: ListCommitmentPurchaseAnalysesRequestRequestTypeDef](./type_defs.md#listcommitmentpurchaseanalysesrequestrequesttypedef) 

### list\_cost\_allocation\_tag\_backfill\_history

Retrieves a list of your historical cost allocation tag backfill requests.

Type annotations and code completion for `#!python session.create_client("ce").list_cost_allocation_tag_backfill_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/list_cost_allocation_tag_backfill_history.html)

```python
# list_cost_allocation_tag_backfill_history method definition

await def list_cost_allocation_tag_backfill_history(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCostAllocationTagBackfillHistoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCostAllocationTagBackfillHistoryResponseTypeDef](./type_defs.md#listcostallocationtagbackfillhistoryresponsetypedef) 


```python
# list_cost_allocation_tag_backfill_history method usage example with argument unpacking

kwargs: ListCostAllocationTagBackfillHistoryRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_cost_allocation_tag_backfill_history(**kwargs)
```

1. See [:material-code-braces: ListCostAllocationTagBackfillHistoryRequestRequestTypeDef](./type_defs.md#listcostallocationtagbackfillhistoryrequestrequesttypedef) 

### list\_cost\_allocation\_tags

Get a list of cost allocation tags.

Type annotations and code completion for `#!python session.create_client("ce").list_cost_allocation_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/list_cost_allocation_tags.html)

```python
# list_cost_allocation_tags method definition

await def list_cost_allocation_tags(
    self,
    *,
    Status: CostAllocationTagStatusType = ...,  # (1)
    TagKeys: Sequence[str] = ...,
    Type: CostAllocationTagTypeType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCostAllocationTagsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CostAllocationTagStatusType](./literals.md#costallocationtagstatustype) 
2. See [:material-code-brackets: CostAllocationTagTypeType](./literals.md#costallocationtagtypetype) 
3. See [:material-code-braces: ListCostAllocationTagsResponseTypeDef](./type_defs.md#listcostallocationtagsresponsetypedef) 


```python
# list_cost_allocation_tags method usage example with argument unpacking

kwargs: ListCostAllocationTagsRequestRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_cost_allocation_tags(**kwargs)
```

1. See [:material-code-braces: ListCostAllocationTagsRequestRequestTypeDef](./type_defs.md#listcostallocationtagsrequestrequesttypedef) 

### list\_cost\_category\_definitions

Returns the name, Amazon Resource Name (ARN), <code>NumberOfRules</code> and
effective dates of all Cost Categories defined in the account.

Type annotations and code completion for `#!python session.create_client("ce").list_cost_category_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/list_cost_category_definitions.html)

```python
# list_cost_category_definitions method definition

await def list_cost_category_definitions(
    self,
    *,
    EffectiveOn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCostCategoryDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCostCategoryDefinitionsResponseTypeDef](./type_defs.md#listcostcategorydefinitionsresponsetypedef) 


```python
# list_cost_category_definitions method usage example with argument unpacking

kwargs: ListCostCategoryDefinitionsRequestRequestTypeDef = {  # (1)
    "EffectiveOn": ...,
}

parent.list_cost_category_definitions(**kwargs)
```

1. See [:material-code-braces: ListCostCategoryDefinitionsRequestRequestTypeDef](./type_defs.md#listcostcategorydefinitionsrequestrequesttypedef) 

### list\_savings\_plans\_purchase\_recommendation\_generation

Retrieves a list of your historical recommendation generations within the past
30 days.

Type annotations and code completion for `#!python session.create_client("ce").list_savings_plans_purchase_recommendation_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/list_savings_plans_purchase_recommendation_generation.html)

```python
# list_savings_plans_purchase_recommendation_generation method definition

await def list_savings_plans_purchase_recommendation_generation(
    self,
    *,
    GenerationStatus: GenerationStatusType = ...,  # (1)
    RecommendationIds: Sequence[str] = ...,
    PageSize: int = ...,
    NextPageToken: str = ...,
) -> ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GenerationStatusType](./literals.md#generationstatustype) 
2. See [:material-code-braces: ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef](./type_defs.md#listsavingsplanspurchaserecommendationgenerationresponsetypedef) 


```python
# list_savings_plans_purchase_recommendation_generation method usage example with argument unpacking

kwargs: ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef = {  # (1)
    "GenerationStatus": ...,
}

parent.list_savings_plans_purchase_recommendation_generation(**kwargs)
```

1. See [:material-code-braces: ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef](./type_defs.md#listsavingsplanspurchaserecommendationgenerationrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of resource tags associated with the resource specified by the
Amazon Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("ce").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### provide\_anomaly\_feedback

Modifies the feedback property of a given cost anomaly.

Type annotations and code completion for `#!python session.create_client("ce").provide_anomaly_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/provide_anomaly_feedback.html)

```python
# provide_anomaly_feedback method definition

await def provide_anomaly_feedback(
    self,
    *,
    AnomalyId: str,
    Feedback: AnomalyFeedbackTypeType,  # (1)
) -> ProvideAnomalyFeedbackResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype) 
2. See [:material-code-braces: ProvideAnomalyFeedbackResponseTypeDef](./type_defs.md#provideanomalyfeedbackresponsetypedef) 


```python
# provide_anomaly_feedback method usage example with argument unpacking

kwargs: ProvideAnomalyFeedbackRequestRequestTypeDef = {  # (1)
    "AnomalyId": ...,
    "Feedback": ...,
}

parent.provide_anomaly_feedback(**kwargs)
```

1. See [:material-code-braces: ProvideAnomalyFeedbackRequestRequestTypeDef](./type_defs.md#provideanomalyfeedbackrequestrequesttypedef) 

### start\_commitment\_purchase\_analysis

Specifies the parameters of a planned commitment purchase and starts the
generation of the analysis.

Type annotations and code completion for `#!python session.create_client("ce").start_commitment_purchase_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/start_commitment_purchase_analysis.html)

```python
# start_commitment_purchase_analysis method definition

await def start_commitment_purchase_analysis(
    self,
    *,
    CommitmentPurchaseAnalysisConfiguration: CommitmentPurchaseAnalysisConfigurationTypeDef,  # (1)
) -> StartCommitmentPurchaseAnalysisResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CommitmentPurchaseAnalysisConfigurationTypeDef](./type_defs.md#commitmentpurchaseanalysisconfigurationtypedef) 
2. See [:material-code-braces: StartCommitmentPurchaseAnalysisResponseTypeDef](./type_defs.md#startcommitmentpurchaseanalysisresponsetypedef) 


```python
# start_commitment_purchase_analysis method usage example with argument unpacking

kwargs: StartCommitmentPurchaseAnalysisRequestRequestTypeDef = {  # (1)
    "CommitmentPurchaseAnalysisConfiguration": ...,
}

parent.start_commitment_purchase_analysis(**kwargs)
```

1. See [:material-code-braces: StartCommitmentPurchaseAnalysisRequestRequestTypeDef](./type_defs.md#startcommitmentpurchaseanalysisrequestrequesttypedef) 

### start\_cost\_allocation\_tag\_backfill

Request a cost allocation tag backfill.

Type annotations and code completion for `#!python session.create_client("ce").start_cost_allocation_tag_backfill` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/start_cost_allocation_tag_backfill.html)

```python
# start_cost_allocation_tag_backfill method definition

await def start_cost_allocation_tag_backfill(
    self,
    *,
    BackfillFrom: str,
) -> StartCostAllocationTagBackfillResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartCostAllocationTagBackfillResponseTypeDef](./type_defs.md#startcostallocationtagbackfillresponsetypedef) 


```python
# start_cost_allocation_tag_backfill method usage example with argument unpacking

kwargs: StartCostAllocationTagBackfillRequestRequestTypeDef = {  # (1)
    "BackfillFrom": ...,
}

parent.start_cost_allocation_tag_backfill(**kwargs)
```

1. See [:material-code-braces: StartCostAllocationTagBackfillRequestRequestTypeDef](./type_defs.md#startcostallocationtagbackfillrequestrequesttypedef) 

### start\_savings\_plans\_purchase\_recommendation\_generation

Requests a Savings Plans recommendation generation.

Type annotations and code completion for `#!python session.create_client("ce").start_savings_plans_purchase_recommendation_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/start_savings_plans_purchase_recommendation_generation.html)

```python
# start_savings_plans_purchase_recommendation_generation method definition

await def start_savings_plans_purchase_recommendation_generation(
    self,
) -> StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef](./type_defs.md#startsavingsplanspurchaserecommendationgenerationresponsetypedef) 

### tag\_resource

An API operation for adding one or more tags (key-value pairs) to a resource.

Type annotations and code completion for `#!python session.create_client("ce").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    ResourceTags: Sequence[ResourceTagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "ResourceTags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from a resource.

Type annotations and code completion for `#!python session.create_client("ce").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    ResourceTagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "ResourceTagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_anomaly\_monitor

Updates an existing cost anomaly monitor.

Type annotations and code completion for `#!python session.create_client("ce").update_anomaly_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/update_anomaly_monitor.html)

```python
# update_anomaly_monitor method definition

await def update_anomaly_monitor(
    self,
    *,
    MonitorArn: str,
    MonitorName: str = ...,
) -> UpdateAnomalyMonitorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAnomalyMonitorResponseTypeDef](./type_defs.md#updateanomalymonitorresponsetypedef) 


```python
# update_anomaly_monitor method usage example with argument unpacking

kwargs: UpdateAnomalyMonitorRequestRequestTypeDef = {  # (1)
    "MonitorArn": ...,
}

parent.update_anomaly_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateAnomalyMonitorRequestRequestTypeDef](./type_defs.md#updateanomalymonitorrequestrequesttypedef) 

### update\_anomaly\_subscription

Updates an existing cost anomaly subscription.

Type annotations and code completion for `#!python session.create_client("ce").update_anomaly_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/update_anomaly_subscription.html)

```python
# update_anomaly_subscription method definition

await def update_anomaly_subscription(
    self,
    *,
    SubscriptionArn: str,
    Threshold: float = ...,
    Frequency: AnomalySubscriptionFrequencyType = ...,  # (1)
    MonitorArnList: Sequence[str] = ...,
    Subscribers: Sequence[SubscriberTypeDef] = ...,  # (2)
    SubscriptionName: str = ...,
    ThresholdExpression: ExpressionTypeDef = ...,  # (3)
) -> UpdateAnomalySubscriptionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AnomalySubscriptionFrequencyType](./literals.md#anomalysubscriptionfrequencytype) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: UpdateAnomalySubscriptionResponseTypeDef](./type_defs.md#updateanomalysubscriptionresponsetypedef) 


```python
# update_anomaly_subscription method usage example with argument unpacking

kwargs: UpdateAnomalySubscriptionRequestRequestTypeDef = {  # (1)
    "SubscriptionArn": ...,
}

parent.update_anomaly_subscription(**kwargs)
```

1. See [:material-code-braces: UpdateAnomalySubscriptionRequestRequestTypeDef](./type_defs.md#updateanomalysubscriptionrequestrequesttypedef) 

### update\_cost\_allocation\_tags\_status

Updates status for cost allocation tags in bulk, with maximum batch size of 20.

Type annotations and code completion for `#!python session.create_client("ce").update_cost_allocation_tags_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/update_cost_allocation_tags_status.html)

```python
# update_cost_allocation_tags_status method definition

await def update_cost_allocation_tags_status(
    self,
    *,
    CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef],  # (1)
) -> UpdateCostAllocationTagsStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CostAllocationTagStatusEntryTypeDef](./type_defs.md#costallocationtagstatusentrytypedef) 
2. See [:material-code-braces: UpdateCostAllocationTagsStatusResponseTypeDef](./type_defs.md#updatecostallocationtagsstatusresponsetypedef) 


```python
# update_cost_allocation_tags_status method usage example with argument unpacking

kwargs: UpdateCostAllocationTagsStatusRequestRequestTypeDef = {  # (1)
    "CostAllocationTagsStatus": ...,
}

parent.update_cost_allocation_tags_status(**kwargs)
```

1. See [:material-code-braces: UpdateCostAllocationTagsStatusRequestRequestTypeDef](./type_defs.md#updatecostallocationtagsstatusrequestrequesttypedef) 

### update\_cost\_category\_definition

Updates an existing Cost Category.

Type annotations and code completion for `#!python session.create_client("ce").update_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce/client/update_cost_category_definition.html)

```python
# update_cost_category_definition method definition

await def update_cost_category_definition(
    self,
    *,
    CostCategoryArn: str,
    RuleVersion: CostCategoryRuleVersionType,  # (1)
    Rules: Sequence[CostCategoryRuleTypeDef],  # (2)
    EffectiveStart: str = ...,
    DefaultValue: str = ...,
    SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,  # (3)
) -> UpdateCostCategoryDefinitionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CostCategoryRuleVersionType](./literals.md#costcategoryruleversiontype) 
2. See [:material-code-braces: CostCategoryRuleTypeDef](./type_defs.md#costcategoryruletypedef) 
3. See [:material-code-braces: CostCategorySplitChargeRuleTypeDef](./type_defs.md#costcategorysplitchargeruletypedef) 
4. See [:material-code-braces: UpdateCostCategoryDefinitionResponseTypeDef](./type_defs.md#updatecostcategorydefinitionresponsetypedef) 


```python
# update_cost_category_definition method usage example with argument unpacking

kwargs: UpdateCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "CostCategoryArn": ...,
    "RuleVersion": ...,
    "Rules": ...,
}

parent.update_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: UpdateCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#updatecostcategorydefinitionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ce").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CostExplorerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ce").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client)

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





