# ApplicationInsightsClient

> [Index](../README.md) > [ApplicationInsights](./README.md) > ApplicationInsightsClient

!!! note ""

    Auto-generated documentation for [ApplicationInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
    type annotations stubs module [types-aiobotocore-application-insights](https://pypi.org/project/types-aiobotocore-application-insights/).

## ApplicationInsightsClient

Type annotations and code completion for `#!python session.create_client("application-insights")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client)

```python
# ApplicationInsightsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_application_insights.client import ApplicationInsightsClient

session = get_session()
async with session.create_client("application-insights") as client:
    client: ApplicationInsightsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("application-insights").exceptions` structure.

```python
# ApplicationInsightsClient.exceptions usage example

async with session.create_client("application-insights") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.TagsAlreadyExistException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# ApplicationInsightsClient usage type checking example

from types_aiobotocore_application_insights.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### add\_workload

Adds a workload to a component.

Type annotations and code completion for `#!python session.create_client("application-insights").add_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.add_workload)

```python
# add_workload method definition

await def add_workload(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadConfiguration: WorkloadConfigurationTypeDef,  # (1)
) -> AddWorkloadResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: WorkloadConfigurationTypeDef](./type_defs.md#workloadconfigurationtypedef) 
2. See [:material-code-braces: AddWorkloadResponseTypeDef](./type_defs.md#addworkloadresponsetypedef) 


```python
# add_workload method usage example with argument unpacking

kwargs: AddWorkloadRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
    "WorkloadConfiguration": ...,
}

parent.add_workload(**kwargs)
```

1. See [:material-code-braces: AddWorkloadRequestRequestTypeDef](./type_defs.md#addworkloadrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("application-insights").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("application-insights").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_application

Adds an application that is created from a resource group.

Type annotations and code completion for `#!python session.create_client("application-insights").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_application)

```python
# create_application method definition

await def create_application(
    self,
    *,
    ResourceGroupName: str = ...,
    OpsCenterEnabled: bool = ...,
    CWEMonitorEnabled: bool = ...,
    OpsItemSNSTopicArn: str = ...,
    SNSNotificationArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    AutoConfigEnabled: bool = ...,
    AutoCreate: bool = ...,
    GroupingType: GroupingTypeType = ...,  # (2)
    AttachMissingPermission: bool = ...,
) -> CreateApplicationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: GroupingTypeType](./literals.md#groupingtypetype) 
3. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### create\_component

Creates a custom component by grouping similar standalone instances to monitor.

Type annotations and code completion for `#!python session.create_client("application-insights").create_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_component)

```python
# create_component method definition

await def create_component(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    ResourceList: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# create_component method usage example with argument unpacking

kwargs: CreateComponentRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
    "ResourceList": ...,
}

parent.create_component(**kwargs)
```

1. See [:material-code-braces: CreateComponentRequestRequestTypeDef](./type_defs.md#createcomponentrequestrequesttypedef) 

### create\_log\_pattern

Adds an log pattern to a `LogPatternSet`.

Type annotations and code completion for `#!python session.create_client("application-insights").create_log_pattern` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_log_pattern)

```python
# create_log_pattern method definition

await def create_log_pattern(
    self,
    *,
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
    Pattern: str,
    Rank: int,
) -> CreateLogPatternResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLogPatternResponseTypeDef](./type_defs.md#createlogpatternresponsetypedef) 


```python
# create_log_pattern method usage example with argument unpacking

kwargs: CreateLogPatternRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "PatternSetName": ...,
    "PatternName": ...,
    "Pattern": ...,
    "Rank": ...,
}

parent.create_log_pattern(**kwargs)
```

1. See [:material-code-braces: CreateLogPatternRequestRequestTypeDef](./type_defs.md#createlogpatternrequestrequesttypedef) 

### delete\_application

Removes the specified application from monitoring.

Type annotations and code completion for `#!python session.create_client("application-insights").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_application)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    ResourceGroupName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef) 

### delete\_component

Ungroups a custom component.

Type annotations and code completion for `#!python session.create_client("application-insights").delete_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_component)

```python
# delete_component method definition

await def delete_component(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_component method usage example with argument unpacking

kwargs: DeleteComponentRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
}

parent.delete_component(**kwargs)
```

1. See [:material-code-braces: DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef) 

### delete\_log\_pattern

Removes the specified log pattern from a `LogPatternSet`.

Type annotations and code completion for `#!python session.create_client("application-insights").delete_log_pattern` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_log_pattern)

```python
# delete_log_pattern method definition

await def delete_log_pattern(
    self,
    *,
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_log_pattern method usage example with argument unpacking

kwargs: DeleteLogPatternRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "PatternSetName": ...,
    "PatternName": ...,
}

parent.delete_log_pattern(**kwargs)
```

1. See [:material-code-braces: DeleteLogPatternRequestRequestTypeDef](./type_defs.md#deletelogpatternrequestrequesttypedef) 

### describe\_application

Describes the application.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_application)

```python
# describe_application method definition

await def describe_application(
    self,
    *,
    ResourceGroupName: str,
    AccountId: str = ...,
) -> DescribeApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationResponseTypeDef](./type_defs.md#describeapplicationresponsetypedef) 


```python
# describe_application method usage example with argument unpacking

kwargs: DescribeApplicationRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.describe_application(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationRequestRequestTypeDef](./type_defs.md#describeapplicationrequestrequesttypedef) 

### describe\_component

Describes a component and lists the resources that are grouped together in a
component.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component)

```python
# describe_component method definition

await def describe_component(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    AccountId: str = ...,
) -> DescribeComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeComponentResponseTypeDef](./type_defs.md#describecomponentresponsetypedef) 


```python
# describe_component method usage example with argument unpacking

kwargs: DescribeComponentRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
}

parent.describe_component(**kwargs)
```

1. See [:material-code-braces: DescribeComponentRequestRequestTypeDef](./type_defs.md#describecomponentrequestrequesttypedef) 

### describe\_component\_configuration

Describes the monitoring configuration of the component.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_component_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration)

```python
# describe_component_configuration method definition

await def describe_component_configuration(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    AccountId: str = ...,
) -> DescribeComponentConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeComponentConfigurationResponseTypeDef](./type_defs.md#describecomponentconfigurationresponsetypedef) 


```python
# describe_component_configuration method usage example with argument unpacking

kwargs: DescribeComponentConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
}

parent.describe_component_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeComponentConfigurationRequestRequestTypeDef](./type_defs.md#describecomponentconfigurationrequestrequesttypedef) 

### describe\_component\_configuration\_recommendation

Describes the recommended monitoring configuration of the component.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_component_configuration_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)

```python
# describe_component_configuration_recommendation method definition

await def describe_component_configuration_recommendation(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    Tier: TierType,  # (1)
    WorkloadName: str = ...,
    RecommendationType: RecommendationTypeType = ...,  # (2)
) -> DescribeComponentConfigurationRecommendationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 
2. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
3. See [:material-code-braces: DescribeComponentConfigurationRecommendationResponseTypeDef](./type_defs.md#describecomponentconfigurationrecommendationresponsetypedef) 


```python
# describe_component_configuration_recommendation method usage example with argument unpacking

kwargs: DescribeComponentConfigurationRecommendationRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
    "Tier": ...,
}

parent.describe_component_configuration_recommendation(**kwargs)
```

1. See [:material-code-braces: DescribeComponentConfigurationRecommendationRequestRequestTypeDef](./type_defs.md#describecomponentconfigurationrecommendationrequestrequesttypedef) 

### describe\_log\_pattern

Describe a specific log pattern from a `LogPatternSet`.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_log_pattern` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_log_pattern)

```python
# describe_log_pattern method definition

await def describe_log_pattern(
    self,
    *,
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
    AccountId: str = ...,
) -> DescribeLogPatternResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLogPatternResponseTypeDef](./type_defs.md#describelogpatternresponsetypedef) 


```python
# describe_log_pattern method usage example with argument unpacking

kwargs: DescribeLogPatternRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "PatternSetName": ...,
    "PatternName": ...,
}

parent.describe_log_pattern(**kwargs)
```

1. See [:material-code-braces: DescribeLogPatternRequestRequestTypeDef](./type_defs.md#describelogpatternrequestrequesttypedef) 

### describe\_observation

Describes an anomaly or error with the application.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_observation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_observation)

```python
# describe_observation method definition

await def describe_observation(
    self,
    *,
    ObservationId: str,
    AccountId: str = ...,
) -> DescribeObservationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeObservationResponseTypeDef](./type_defs.md#describeobservationresponsetypedef) 


```python
# describe_observation method usage example with argument unpacking

kwargs: DescribeObservationRequestRequestTypeDef = {  # (1)
    "ObservationId": ...,
}

parent.describe_observation(**kwargs)
```

1. See [:material-code-braces: DescribeObservationRequestRequestTypeDef](./type_defs.md#describeobservationrequestrequesttypedef) 

### describe\_problem

Describes an application problem.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_problem` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem)

```python
# describe_problem method definition

await def describe_problem(
    self,
    *,
    ProblemId: str,
    AccountId: str = ...,
) -> DescribeProblemResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProblemResponseTypeDef](./type_defs.md#describeproblemresponsetypedef) 


```python
# describe_problem method usage example with argument unpacking

kwargs: DescribeProblemRequestRequestTypeDef = {  # (1)
    "ProblemId": ...,
}

parent.describe_problem(**kwargs)
```

1. See [:material-code-braces: DescribeProblemRequestRequestTypeDef](./type_defs.md#describeproblemrequestrequesttypedef) 

### describe\_problem\_observations

Describes the anomalies or errors associated with the problem.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_problem_observations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem_observations)

```python
# describe_problem_observations method definition

await def describe_problem_observations(
    self,
    *,
    ProblemId: str,
    AccountId: str = ...,
) -> DescribeProblemObservationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProblemObservationsResponseTypeDef](./type_defs.md#describeproblemobservationsresponsetypedef) 


```python
# describe_problem_observations method usage example with argument unpacking

kwargs: DescribeProblemObservationsRequestRequestTypeDef = {  # (1)
    "ProblemId": ...,
}

parent.describe_problem_observations(**kwargs)
```

1. See [:material-code-braces: DescribeProblemObservationsRequestRequestTypeDef](./type_defs.md#describeproblemobservationsrequestrequesttypedef) 

### describe\_workload

Describes a workload and its configuration.

Type annotations and code completion for `#!python session.create_client("application-insights").describe_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_workload)

```python
# describe_workload method definition

await def describe_workload(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadId: str,
    AccountId: str = ...,
) -> DescribeWorkloadResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkloadResponseTypeDef](./type_defs.md#describeworkloadresponsetypedef) 


```python
# describe_workload method usage example with argument unpacking

kwargs: DescribeWorkloadRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
    "WorkloadId": ...,
}

parent.describe_workload(**kwargs)
```

1. See [:material-code-braces: DescribeWorkloadRequestRequestTypeDef](./type_defs.md#describeworkloadrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("application-insights").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.generate_presigned_url)

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


### list\_applications

Lists the IDs of the applications that you are monitoring.

Type annotations and code completion for `#!python session.create_client("application-insights").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_applications)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    AccountId: str = ...,
) -> ListApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef) 

### list\_components

Lists the auto-grouped, standalone, and custom components of the application.

Type annotations and code completion for `#!python session.create_client("application-insights").list_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)

```python
# list_components method definition

await def list_components(
    self,
    *,
    ResourceGroupName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    AccountId: str = ...,
) -> ListComponentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python
# list_components method usage example with argument unpacking

kwargs: ListComponentsRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.list_components(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef) 

### list\_configuration\_history

Lists the INFO, WARN, and ERROR events for periodic configuration updates
performed by Application
Insights.

Type annotations and code completion for `#!python session.create_client("application-insights").list_configuration_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_configuration_history)

```python
# list_configuration_history method definition

await def list_configuration_history(
    self,
    *,
    ResourceGroupName: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    EventStatus: ConfigurationEventStatusType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
    AccountId: str = ...,
) -> ListConfigurationHistoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConfigurationEventStatusType](./literals.md#configurationeventstatustype) 
2. See [:material-code-braces: ListConfigurationHistoryResponseTypeDef](./type_defs.md#listconfigurationhistoryresponsetypedef) 


```python
# list_configuration_history method usage example with argument unpacking

kwargs: ListConfigurationHistoryRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.list_configuration_history(**kwargs)
```

1. See [:material-code-braces: ListConfigurationHistoryRequestRequestTypeDef](./type_defs.md#listconfigurationhistoryrequestrequesttypedef) 

### list\_log\_pattern\_sets

Lists the log pattern sets in the specific application.

Type annotations and code completion for `#!python session.create_client("application-insights").list_log_pattern_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_pattern_sets)

```python
# list_log_pattern_sets method definition

await def list_log_pattern_sets(
    self,
    *,
    ResourceGroupName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    AccountId: str = ...,
) -> ListLogPatternSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLogPatternSetsResponseTypeDef](./type_defs.md#listlogpatternsetsresponsetypedef) 


```python
# list_log_pattern_sets method usage example with argument unpacking

kwargs: ListLogPatternSetsRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.list_log_pattern_sets(**kwargs)
```

1. See [:material-code-braces: ListLogPatternSetsRequestRequestTypeDef](./type_defs.md#listlogpatternsetsrequestrequesttypedef) 

### list\_log\_patterns

Lists the log patterns in the specific log `LogPatternSet`.

Type annotations and code completion for `#!python session.create_client("application-insights").list_log_patterns` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)

```python
# list_log_patterns method definition

await def list_log_patterns(
    self,
    *,
    ResourceGroupName: str,
    PatternSetName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    AccountId: str = ...,
) -> ListLogPatternsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLogPatternsResponseTypeDef](./type_defs.md#listlogpatternsresponsetypedef) 


```python
# list_log_patterns method usage example with argument unpacking

kwargs: ListLogPatternsRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.list_log_patterns(**kwargs)
```

1. See [:material-code-braces: ListLogPatternsRequestRequestTypeDef](./type_defs.md#listlogpatternsrequestrequesttypedef) 

### list\_problems

Lists the problems with your application.

Type annotations and code completion for `#!python session.create_client("application-insights").list_problems` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_problems)

```python
# list_problems method definition

await def list_problems(
    self,
    *,
    AccountId: str = ...,
    ResourceGroupName: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ComponentName: str = ...,
    Visibility: VisibilityType = ...,  # (1)
) -> ListProblemsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
2. See [:material-code-braces: ListProblemsResponseTypeDef](./type_defs.md#listproblemsresponsetypedef) 


```python
# list_problems method usage example with argument unpacking

kwargs: ListProblemsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_problems(**kwargs)
```

1. See [:material-code-braces: ListProblemsRequestRequestTypeDef](./type_defs.md#listproblemsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieve a list of the tags (keys and values) that are associated with a
specified
application.

Type annotations and code completion for `#!python session.create_client("application-insights").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_workloads

Lists the workloads that are configured on a given component.

Type annotations and code completion for `#!python session.create_client("application-insights").list_workloads` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_workloads)

```python
# list_workloads method definition

await def list_workloads(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    AccountId: str = ...,
) -> ListWorkloadsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkloadsResponseTypeDef](./type_defs.md#listworkloadsresponsetypedef) 


```python
# list_workloads method usage example with argument unpacking

kwargs: ListWorkloadsRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
}

parent.list_workloads(**kwargs)
```

1. See [:material-code-braces: ListWorkloadsRequestRequestTypeDef](./type_defs.md#listworkloadsrequestrequesttypedef) 

### remove\_workload

Remove workload from a component.

Type annotations and code completion for `#!python session.create_client("application-insights").remove_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.remove_workload)

```python
# remove_workload method definition

await def remove_workload(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadId: str,
) -> Dict[str, Any]:
    ...
```



```python
# remove_workload method usage example with argument unpacking

kwargs: RemoveWorkloadRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
    "WorkloadId": ...,
}

parent.remove_workload(**kwargs)
```

1. See [:material-code-braces: RemoveWorkloadRequestRequestTypeDef](./type_defs.md#removeworkloadrequestrequesttypedef) 

### tag\_resource

Add one or more tags (keys and values) to a specified application.

Type annotations and code completion for `#!python session.create_client("application-insights").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Remove one or more tags (keys and values) from a specified application.

Type annotations and code completion for `#!python session.create_client("application-insights").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_application

Updates the application.

Type annotations and code completion for `#!python session.create_client("application-insights").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_application)

```python
# update_application method definition

await def update_application(
    self,
    *,
    ResourceGroupName: str,
    OpsCenterEnabled: bool = ...,
    CWEMonitorEnabled: bool = ...,
    OpsItemSNSTopicArn: str = ...,
    SNSNotificationArn: str = ...,
    RemoveSNSTopic: bool = ...,
    AutoConfigEnabled: bool = ...,
    AttachMissingPermission: bool = ...,
) -> UpdateApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef) 


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### update\_component

Updates the custom component name and/or the list of resources that make up the
component.

Type annotations and code completion for `#!python session.create_client("application-insights").update_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_component)

```python
# update_component method definition

await def update_component(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    NewComponentName: str = ...,
    ResourceList: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_component method usage example with argument unpacking

kwargs: UpdateComponentRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
}

parent.update_component(**kwargs)
```

1. See [:material-code-braces: UpdateComponentRequestRequestTypeDef](./type_defs.md#updatecomponentrequestrequesttypedef) 

### update\_component\_configuration

Updates the monitoring configurations for the component.

Type annotations and code completion for `#!python session.create_client("application-insights").update_component_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_component_configuration)

```python
# update_component_configuration method definition

await def update_component_configuration(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    Monitor: bool = ...,
    Tier: TierType = ...,  # (1)
    ComponentConfiguration: str = ...,
    AutoConfigEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 


```python
# update_component_configuration method usage example with argument unpacking

kwargs: UpdateComponentConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
}

parent.update_component_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateComponentConfigurationRequestRequestTypeDef](./type_defs.md#updatecomponentconfigurationrequestrequesttypedef) 

### update\_log\_pattern

Adds a log pattern to a `LogPatternSet`.

Type annotations and code completion for `#!python session.create_client("application-insights").update_log_pattern` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)

```python
# update_log_pattern method definition

await def update_log_pattern(
    self,
    *,
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
    Pattern: str = ...,
    Rank: int = ...,
) -> UpdateLogPatternResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateLogPatternResponseTypeDef](./type_defs.md#updatelogpatternresponsetypedef) 


```python
# update_log_pattern method usage example with argument unpacking

kwargs: UpdateLogPatternRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "PatternSetName": ...,
    "PatternName": ...,
}

parent.update_log_pattern(**kwargs)
```

1. See [:material-code-braces: UpdateLogPatternRequestRequestTypeDef](./type_defs.md#updatelogpatternrequestrequesttypedef) 

### update\_problem

Updates the visibility of the problem or specifies the problem as `RESOLVED`.

Type annotations and code completion for `#!python session.create_client("application-insights").update_problem` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_problem)

```python
# update_problem method definition

await def update_problem(
    self,
    *,
    ProblemId: str,
    UpdateStatus: UpdateStatusType = ...,  # (1)
    Visibility: VisibilityType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: UpdateStatusType](./literals.md#updatestatustype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 


```python
# update_problem method usage example with argument unpacking

kwargs: UpdateProblemRequestRequestTypeDef = {  # (1)
    "ProblemId": ...,
}

parent.update_problem(**kwargs)
```

1. See [:material-code-braces: UpdateProblemRequestRequestTypeDef](./type_defs.md#updateproblemrequestrequesttypedef) 

### update\_workload

Adds a workload to a component.

Type annotations and code completion for `#!python session.create_client("application-insights").update_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_workload)

```python
# update_workload method definition

await def update_workload(
    self,
    *,
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadConfiguration: WorkloadConfigurationTypeDef,  # (1)
    WorkloadId: str = ...,
) -> UpdateWorkloadResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: WorkloadConfigurationTypeDef](./type_defs.md#workloadconfigurationtypedef) 
2. See [:material-code-braces: UpdateWorkloadResponseTypeDef](./type_defs.md#updateworkloadresponsetypedef) 


```python
# update_workload method usage example with argument unpacking

kwargs: UpdateWorkloadRequestRequestTypeDef = {  # (1)
    "ResourceGroupName": ...,
    "ComponentName": ...,
    "WorkloadConfiguration": ...,
}

parent.update_workload(**kwargs)
```

1. See [:material-code-braces: UpdateWorkloadRequestRequestTypeDef](./type_defs.md#updateworkloadrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("application-insights").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ApplicationInsightsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("application-insights").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.__aexit__)

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





