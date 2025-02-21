# CloudWatchEvidentlyClient

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > CloudWatchEvidentlyClient

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## CloudWatchEvidentlyClient

Type annotations and code completion for `#!python session.create_client("evidently")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client)

```python
# CloudWatchEvidentlyClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_evidently.client import CloudWatchEvidentlyClient

session = get_session()
async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("evidently").exceptions` structure.

```python
# CloudWatchEvidentlyClient.exceptions usage example

async with session.create_client("evidently") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CloudWatchEvidentlyClient usage type checking example

from types_aiobotocore_evidently.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("evidently").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("evidently").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/generate_presigned_url.html)

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


### batch\_evaluate\_feature

This operation assigns feature variation to user sessions.

Type annotations and code completion for `#!python session.create_client("evidently").batch_evaluate_feature` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/batch_evaluate_feature.html)

```python
# batch_evaluate_feature method definition

await def batch_evaluate_feature(
    self,
    *,
    project: str,
    requests: Sequence[EvaluationRequestTypeDef],  # (1)
) -> BatchEvaluateFeatureResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EvaluationRequestTypeDef](./type_defs.md#evaluationrequesttypedef) 
2. See [:material-code-braces: BatchEvaluateFeatureResponseTypeDef](./type_defs.md#batchevaluatefeatureresponsetypedef) 


```python
# batch_evaluate_feature method usage example with argument unpacking

kwargs: BatchEvaluateFeatureRequestTypeDef = {  # (1)
    "project": ...,
    "requests": ...,
}

parent.batch_evaluate_feature(**kwargs)
```

1. See [:material-code-braces: BatchEvaluateFeatureRequestTypeDef](./type_defs.md#batchevaluatefeaturerequesttypedef) 

### create\_experiment

Creates an Evidently <i>experiment</i>.

Type annotations and code completion for `#!python session.create_client("evidently").create_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/create_experiment.html)

```python
# create_experiment method definition

await def create_experiment(
    self,
    *,
    metricGoals: Sequence[MetricGoalConfigTypeDef],  # (1)
    name: str,
    project: str,
    treatments: Sequence[TreatmentConfigTypeDef],  # (2)
    description: str = ...,
    onlineAbConfig: OnlineAbConfigTypeDef = ...,  # (3)
    randomizationSalt: str = ...,
    samplingRate: int = ...,
    segment: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateExperimentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MetricGoalConfigTypeDef](./type_defs.md#metricgoalconfigtypedef) 
2. See [:material-code-braces: TreatmentConfigTypeDef](./type_defs.md#treatmentconfigtypedef) 
3. See [:material-code-braces: OnlineAbConfigTypeDef](./type_defs.md#onlineabconfigtypedef) 
4. See [:material-code-braces: CreateExperimentResponseTypeDef](./type_defs.md#createexperimentresponsetypedef) 


```python
# create_experiment method usage example with argument unpacking

kwargs: CreateExperimentRequestTypeDef = {  # (1)
    "metricGoals": ...,
    "name": ...,
    "project": ...,
    "treatments": ...,
}

parent.create_experiment(**kwargs)
```

1. See [:material-code-braces: CreateExperimentRequestTypeDef](./type_defs.md#createexperimentrequesttypedef) 

### create\_feature

Creates an Evidently <i>feature</i> that you want to launch or test.

Type annotations and code completion for `#!python session.create_client("evidently").create_feature` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/create_feature.html)

```python
# create_feature method definition

await def create_feature(
    self,
    *,
    name: str,
    project: str,
    variations: Sequence[VariationConfigTypeDef],  # (1)
    defaultVariation: str = ...,
    description: str = ...,
    entityOverrides: Mapping[str, str] = ...,
    evaluationStrategy: FeatureEvaluationStrategyType = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateFeatureResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VariationConfigTypeDef](./type_defs.md#variationconfigtypedef) 
2. See [:material-code-brackets: FeatureEvaluationStrategyType](./literals.md#featureevaluationstrategytype) 
3. See [:material-code-braces: CreateFeatureResponseTypeDef](./type_defs.md#createfeatureresponsetypedef) 


```python
# create_feature method usage example with argument unpacking

kwargs: CreateFeatureRequestTypeDef = {  # (1)
    "name": ...,
    "project": ...,
    "variations": ...,
}

parent.create_feature(**kwargs)
```

1. See [:material-code-braces: CreateFeatureRequestTypeDef](./type_defs.md#createfeaturerequesttypedef) 

### create\_launch

Creates a <i>launch</i> of a given feature.

Type annotations and code completion for `#!python session.create_client("evidently").create_launch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/create_launch.html)

```python
# create_launch method definition

await def create_launch(
    self,
    *,
    groups: Sequence[LaunchGroupConfigTypeDef],  # (1)
    name: str,
    project: str,
    description: str = ...,
    metricMonitors: Sequence[MetricMonitorConfigTypeDef] = ...,  # (2)
    randomizationSalt: str = ...,
    scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...,  # (3)
    tags: Mapping[str, str] = ...,
) -> CreateLaunchResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LaunchGroupConfigTypeDef](./type_defs.md#launchgroupconfigtypedef) 
2. See [:material-code-braces: MetricMonitorConfigTypeDef](./type_defs.md#metricmonitorconfigtypedef) 
3. See [:material-code-braces: ScheduledSplitsLaunchConfigTypeDef](./type_defs.md#scheduledsplitslaunchconfigtypedef) 
4. See [:material-code-braces: CreateLaunchResponseTypeDef](./type_defs.md#createlaunchresponsetypedef) 


```python
# create_launch method usage example with argument unpacking

kwargs: CreateLaunchRequestTypeDef = {  # (1)
    "groups": ...,
    "name": ...,
    "project": ...,
}

parent.create_launch(**kwargs)
```

1. See [:material-code-braces: CreateLaunchRequestTypeDef](./type_defs.md#createlaunchrequesttypedef) 

### create\_project

Creates a project, which is the logical object in Evidently that can contain
features, launches, and experiments.

Type annotations and code completion for `#!python session.create_client("evidently").create_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/create_project.html)

```python
# create_project method definition

await def create_project(
    self,
    *,
    name: str,
    appConfigResource: ProjectAppConfigResourceConfigTypeDef = ...,  # (1)
    dataDelivery: ProjectDataDeliveryConfigTypeDef = ...,  # (2)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateProjectResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ProjectAppConfigResourceConfigTypeDef](./type_defs.md#projectappconfigresourceconfigtypedef) 
2. See [:material-code-braces: ProjectDataDeliveryConfigTypeDef](./type_defs.md#projectdatadeliveryconfigtypedef) 
3. See [:material-code-braces: CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef) 


```python
# create_project method usage example with argument unpacking

kwargs: CreateProjectRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_project(**kwargs)
```

1. See [:material-code-braces: CreateProjectRequestTypeDef](./type_defs.md#createprojectrequesttypedef) 

### create\_segment

Use this operation to define a <i>segment</i> of your audience.

Type annotations and code completion for `#!python session.create_client("evidently").create_segment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/create_segment.html)

```python
# create_segment method definition

await def create_segment(
    self,
    *,
    name: str,
    pattern: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateSegmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSegmentResponseTypeDef](./type_defs.md#createsegmentresponsetypedef) 


```python
# create_segment method usage example with argument unpacking

kwargs: CreateSegmentRequestTypeDef = {  # (1)
    "name": ...,
    "pattern": ...,
}

parent.create_segment(**kwargs)
```

1. See [:material-code-braces: CreateSegmentRequestTypeDef](./type_defs.md#createsegmentrequesttypedef) 

### delete\_experiment

Deletes an Evidently experiment.

Type annotations and code completion for `#!python session.create_client("evidently").delete_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/delete_experiment.html)

```python
# delete_experiment method definition

await def delete_experiment(
    self,
    *,
    experiment: str,
    project: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_experiment method usage example with argument unpacking

kwargs: DeleteExperimentRequestTypeDef = {  # (1)
    "experiment": ...,
    "project": ...,
}

parent.delete_experiment(**kwargs)
```

1. See [:material-code-braces: DeleteExperimentRequestTypeDef](./type_defs.md#deleteexperimentrequesttypedef) 

### delete\_feature

Deletes an Evidently feature.

Type annotations and code completion for `#!python session.create_client("evidently").delete_feature` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/delete_feature.html)

```python
# delete_feature method definition

await def delete_feature(
    self,
    *,
    feature: str,
    project: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_feature method usage example with argument unpacking

kwargs: DeleteFeatureRequestTypeDef = {  # (1)
    "feature": ...,
    "project": ...,
}

parent.delete_feature(**kwargs)
```

1. See [:material-code-braces: DeleteFeatureRequestTypeDef](./type_defs.md#deletefeaturerequesttypedef) 

### delete\_launch

Deletes an Evidently launch.

Type annotations and code completion for `#!python session.create_client("evidently").delete_launch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/delete_launch.html)

```python
# delete_launch method definition

await def delete_launch(
    self,
    *,
    launch: str,
    project: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_launch method usage example with argument unpacking

kwargs: DeleteLaunchRequestTypeDef = {  # (1)
    "launch": ...,
    "project": ...,
}

parent.delete_launch(**kwargs)
```

1. See [:material-code-braces: DeleteLaunchRequestTypeDef](./type_defs.md#deletelaunchrequesttypedef) 

### delete\_project

Deletes an Evidently project.

Type annotations and code completion for `#!python session.create_client("evidently").delete_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/delete_project.html)

```python
# delete_project method definition

await def delete_project(
    self,
    *,
    project: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_project method usage example with argument unpacking

kwargs: DeleteProjectRequestTypeDef = {  # (1)
    "project": ...,
}

parent.delete_project(**kwargs)
```

1. See [:material-code-braces: DeleteProjectRequestTypeDef](./type_defs.md#deleteprojectrequesttypedef) 

### delete\_segment

Deletes a segment.

Type annotations and code completion for `#!python session.create_client("evidently").delete_segment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/delete_segment.html)

```python
# delete_segment method definition

await def delete_segment(
    self,
    *,
    segment: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_segment method usage example with argument unpacking

kwargs: DeleteSegmentRequestTypeDef = {  # (1)
    "segment": ...,
}

parent.delete_segment(**kwargs)
```

1. See [:material-code-braces: DeleteSegmentRequestTypeDef](./type_defs.md#deletesegmentrequesttypedef) 

### evaluate\_feature

This operation assigns a feature variation to one given user session.

Type annotations and code completion for `#!python session.create_client("evidently").evaluate_feature` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/evaluate_feature.html)

```python
# evaluate_feature method definition

await def evaluate_feature(
    self,
    *,
    entityId: str,
    feature: str,
    project: str,
    evaluationContext: str = ...,
) -> EvaluateFeatureResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EvaluateFeatureResponseTypeDef](./type_defs.md#evaluatefeatureresponsetypedef) 


```python
# evaluate_feature method usage example with argument unpacking

kwargs: EvaluateFeatureRequestTypeDef = {  # (1)
    "entityId": ...,
    "feature": ...,
    "project": ...,
}

parent.evaluate_feature(**kwargs)
```

1. See [:material-code-braces: EvaluateFeatureRequestTypeDef](./type_defs.md#evaluatefeaturerequesttypedef) 

### get\_experiment

Returns the details about one experiment.

Type annotations and code completion for `#!python session.create_client("evidently").get_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/get_experiment.html)

```python
# get_experiment method definition

await def get_experiment(
    self,
    *,
    experiment: str,
    project: str,
) -> GetExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExperimentResponseTypeDef](./type_defs.md#getexperimentresponsetypedef) 


```python
# get_experiment method usage example with argument unpacking

kwargs: GetExperimentRequestTypeDef = {  # (1)
    "experiment": ...,
    "project": ...,
}

parent.get_experiment(**kwargs)
```

1. See [:material-code-braces: GetExperimentRequestTypeDef](./type_defs.md#getexperimentrequesttypedef) 

### get\_experiment\_results

Retrieves the results of a running or completed experiment.

Type annotations and code completion for `#!python session.create_client("evidently").get_experiment_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/get_experiment_results.html)

```python
# get_experiment_results method definition

await def get_experiment_results(
    self,
    *,
    experiment: str,
    metricNames: Sequence[str],
    project: str,
    treatmentNames: Sequence[str],
    baseStat: ExperimentBaseStatType = ...,  # (1)
    endTime: TimestampTypeDef = ...,
    period: int = ...,
    reportNames: Sequence[ExperimentReportNameType] = ...,  # (2)
    resultStats: Sequence[ExperimentResultRequestTypeType] = ...,  # (3)
    startTime: TimestampTypeDef = ...,
) -> GetExperimentResultsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ExperimentBaseStatType](./literals.md#experimentbasestattype) 
2. See [:material-code-brackets: ExperimentReportNameType](./literals.md#experimentreportnametype) 
3. See [:material-code-brackets: ExperimentResultRequestTypeType](./literals.md#experimentresultrequesttypetype) 
4. See [:material-code-braces: GetExperimentResultsResponseTypeDef](./type_defs.md#getexperimentresultsresponsetypedef) 


```python
# get_experiment_results method usage example with argument unpacking

kwargs: GetExperimentResultsRequestTypeDef = {  # (1)
    "experiment": ...,
    "metricNames": ...,
    "project": ...,
    "treatmentNames": ...,
}

parent.get_experiment_results(**kwargs)
```

1. See [:material-code-braces: GetExperimentResultsRequestTypeDef](./type_defs.md#getexperimentresultsrequesttypedef) 

### get\_feature

Returns the details about one feature.

Type annotations and code completion for `#!python session.create_client("evidently").get_feature` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/get_feature.html)

```python
# get_feature method definition

await def get_feature(
    self,
    *,
    feature: str,
    project: str,
) -> GetFeatureResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFeatureResponseTypeDef](./type_defs.md#getfeatureresponsetypedef) 


```python
# get_feature method usage example with argument unpacking

kwargs: GetFeatureRequestTypeDef = {  # (1)
    "feature": ...,
    "project": ...,
}

parent.get_feature(**kwargs)
```

1. See [:material-code-braces: GetFeatureRequestTypeDef](./type_defs.md#getfeaturerequesttypedef) 

### get\_launch

Returns the details about one launch.

Type annotations and code completion for `#!python session.create_client("evidently").get_launch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/get_launch.html)

```python
# get_launch method definition

await def get_launch(
    self,
    *,
    launch: str,
    project: str,
) -> GetLaunchResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLaunchResponseTypeDef](./type_defs.md#getlaunchresponsetypedef) 


```python
# get_launch method usage example with argument unpacking

kwargs: GetLaunchRequestTypeDef = {  # (1)
    "launch": ...,
    "project": ...,
}

parent.get_launch(**kwargs)
```

1. See [:material-code-braces: GetLaunchRequestTypeDef](./type_defs.md#getlaunchrequesttypedef) 

### get\_project

Returns the details about one launch.

Type annotations and code completion for `#!python session.create_client("evidently").get_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/get_project.html)

```python
# get_project method definition

await def get_project(
    self,
    *,
    project: str,
) -> GetProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProjectResponseTypeDef](./type_defs.md#getprojectresponsetypedef) 


```python
# get_project method usage example with argument unpacking

kwargs: GetProjectRequestTypeDef = {  # (1)
    "project": ...,
}

parent.get_project(**kwargs)
```

1. See [:material-code-braces: GetProjectRequestTypeDef](./type_defs.md#getprojectrequesttypedef) 

### get\_segment

Returns information about the specified segment.

Type annotations and code completion for `#!python session.create_client("evidently").get_segment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/get_segment.html)

```python
# get_segment method definition

await def get_segment(
    self,
    *,
    segment: str,
) -> GetSegmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSegmentResponseTypeDef](./type_defs.md#getsegmentresponsetypedef) 


```python
# get_segment method usage example with argument unpacking

kwargs: GetSegmentRequestTypeDef = {  # (1)
    "segment": ...,
}

parent.get_segment(**kwargs)
```

1. See [:material-code-braces: GetSegmentRequestTypeDef](./type_defs.md#getsegmentrequesttypedef) 

### list\_experiments

Returns configuration details about all the experiments in the specified
project.

Type annotations and code completion for `#!python session.create_client("evidently").list_experiments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/list_experiments.html)

```python
# list_experiments method definition

await def list_experiments(
    self,
    *,
    project: str,
    maxResults: int = ...,
    nextToken: str = ...,
    status: ExperimentStatusType = ...,  # (1)
) -> ListExperimentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
2. See [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 


```python
# list_experiments method usage example with argument unpacking

kwargs: ListExperimentsRequestTypeDef = {  # (1)
    "project": ...,
}

parent.list_experiments(**kwargs)
```

1. See [:material-code-braces: ListExperimentsRequestTypeDef](./type_defs.md#listexperimentsrequesttypedef) 

### list\_features

Returns configuration details about all the features in the specified project.

Type annotations and code completion for `#!python session.create_client("evidently").list_features` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/list_features.html)

```python
# list_features method definition

await def list_features(
    self,
    *,
    project: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFeaturesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFeaturesResponseTypeDef](./type_defs.md#listfeaturesresponsetypedef) 


```python
# list_features method usage example with argument unpacking

kwargs: ListFeaturesRequestTypeDef = {  # (1)
    "project": ...,
}

parent.list_features(**kwargs)
```

1. See [:material-code-braces: ListFeaturesRequestTypeDef](./type_defs.md#listfeaturesrequesttypedef) 

### list\_launches

Returns configuration details about all the launches in the specified project.

Type annotations and code completion for `#!python session.create_client("evidently").list_launches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/list_launches.html)

```python
# list_launches method definition

await def list_launches(
    self,
    *,
    project: str,
    maxResults: int = ...,
    nextToken: str = ...,
    status: LaunchStatusType = ...,  # (1)
) -> ListLaunchesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: ListLaunchesResponseTypeDef](./type_defs.md#listlaunchesresponsetypedef) 


```python
# list_launches method usage example with argument unpacking

kwargs: ListLaunchesRequestTypeDef = {  # (1)
    "project": ...,
}

parent.list_launches(**kwargs)
```

1. See [:material-code-braces: ListLaunchesRequestTypeDef](./type_defs.md#listlaunchesrequesttypedef) 

### list\_projects

Returns configuration details about all the projects in the current Region in
your account.

Type annotations and code completion for `#!python session.create_client("evidently").list_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/list_projects.html)

```python
# list_projects method definition

await def list_projects(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListProjectsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# list_projects method usage example with argument unpacking

kwargs: ListProjectsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_projects(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestTypeDef](./type_defs.md#listprojectsrequesttypedef) 

### list\_segment\_references

Use this operation to find which experiments or launches are using a specified
segment.

Type annotations and code completion for `#!python session.create_client("evidently").list_segment_references` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/list_segment_references.html)

```python
# list_segment_references method definition

await def list_segment_references(
    self,
    *,
    segment: str,
    type: SegmentReferenceResourceTypeType,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSegmentReferencesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SegmentReferenceResourceTypeType](./literals.md#segmentreferenceresourcetypetype) 
2. See [:material-code-braces: ListSegmentReferencesResponseTypeDef](./type_defs.md#listsegmentreferencesresponsetypedef) 


```python
# list_segment_references method usage example with argument unpacking

kwargs: ListSegmentReferencesRequestTypeDef = {  # (1)
    "segment": ...,
    "type": ...,
}

parent.list_segment_references(**kwargs)
```

1. See [:material-code-braces: ListSegmentReferencesRequestTypeDef](./type_defs.md#listsegmentreferencesrequesttypedef) 

### list\_segments

Returns a list of audience segments that you have created in your account in
this Region.

Type annotations and code completion for `#!python session.create_client("evidently").list_segments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/list_segments.html)

```python
# list_segments method definition

await def list_segments(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSegmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSegmentsResponseTypeDef](./type_defs.md#listsegmentsresponsetypedef) 


```python
# list_segments method usage example with argument unpacking

kwargs: ListSegmentsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_segments(**kwargs)
```

1. See [:material-code-braces: ListSegmentsRequestTypeDef](./type_defs.md#listsegmentsrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with an Evidently resource.

Type annotations and code completion for `#!python session.create_client("evidently").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/list_tags_for_resource.html)

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

### put\_project\_events

Sends performance events to Evidently.

Type annotations and code completion for `#!python session.create_client("evidently").put_project_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/put_project_events.html)

```python
# put_project_events method definition

await def put_project_events(
    self,
    *,
    events: Sequence[EventTypeDef],  # (1)
    project: str,
) -> PutProjectEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: PutProjectEventsResponseTypeDef](./type_defs.md#putprojecteventsresponsetypedef) 


```python
# put_project_events method usage example with argument unpacking

kwargs: PutProjectEventsRequestTypeDef = {  # (1)
    "events": ...,
    "project": ...,
}

parent.put_project_events(**kwargs)
```

1. See [:material-code-braces: PutProjectEventsRequestTypeDef](./type_defs.md#putprojecteventsrequesttypedef) 

### start\_experiment

Starts an existing experiment.

Type annotations and code completion for `#!python session.create_client("evidently").start_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/start_experiment.html)

```python
# start_experiment method definition

await def start_experiment(
    self,
    *,
    analysisCompleteTime: TimestampTypeDef,
    experiment: str,
    project: str,
) -> StartExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartExperimentResponseTypeDef](./type_defs.md#startexperimentresponsetypedef) 


```python
# start_experiment method usage example with argument unpacking

kwargs: StartExperimentRequestTypeDef = {  # (1)
    "analysisCompleteTime": ...,
    "experiment": ...,
    "project": ...,
}

parent.start_experiment(**kwargs)
```

1. See [:material-code-braces: StartExperimentRequestTypeDef](./type_defs.md#startexperimentrequesttypedef) 

### start\_launch

Starts an existing launch.

Type annotations and code completion for `#!python session.create_client("evidently").start_launch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/start_launch.html)

```python
# start_launch method definition

await def start_launch(
    self,
    *,
    launch: str,
    project: str,
) -> StartLaunchResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartLaunchResponseTypeDef](./type_defs.md#startlaunchresponsetypedef) 


```python
# start_launch method usage example with argument unpacking

kwargs: StartLaunchRequestTypeDef = {  # (1)
    "launch": ...,
    "project": ...,
}

parent.start_launch(**kwargs)
```

1. See [:material-code-braces: StartLaunchRequestTypeDef](./type_defs.md#startlaunchrequesttypedef) 

### stop\_experiment

Stops an experiment that is currently running.

Type annotations and code completion for `#!python session.create_client("evidently").stop_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/stop_experiment.html)

```python
# stop_experiment method definition

await def stop_experiment(
    self,
    *,
    experiment: str,
    project: str,
    desiredState: ExperimentStopDesiredStateType = ...,  # (1)
    reason: str = ...,
) -> StopExperimentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ExperimentStopDesiredStateType](./literals.md#experimentstopdesiredstatetype) 
2. See [:material-code-braces: StopExperimentResponseTypeDef](./type_defs.md#stopexperimentresponsetypedef) 


```python
# stop_experiment method usage example with argument unpacking

kwargs: StopExperimentRequestTypeDef = {  # (1)
    "experiment": ...,
    "project": ...,
}

parent.stop_experiment(**kwargs)
```

1. See [:material-code-braces: StopExperimentRequestTypeDef](./type_defs.md#stopexperimentrequesttypedef) 

### stop\_launch

Stops a launch that is currently running.

Type annotations and code completion for `#!python session.create_client("evidently").stop_launch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/stop_launch.html)

```python
# stop_launch method definition

await def stop_launch(
    self,
    *,
    launch: str,
    project: str,
    desiredState: LaunchStopDesiredStateType = ...,  # (1)
    reason: str = ...,
) -> StopLaunchResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LaunchStopDesiredStateType](./literals.md#launchstopdesiredstatetype) 
2. See [:material-code-braces: StopLaunchResponseTypeDef](./type_defs.md#stoplaunchresponsetypedef) 


```python
# stop_launch method usage example with argument unpacking

kwargs: StopLaunchRequestTypeDef = {  # (1)
    "launch": ...,
    "project": ...,
}

parent.stop_launch(**kwargs)
```

1. See [:material-code-braces: StopLaunchRequestTypeDef](./type_defs.md#stoplaunchrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified CloudWatch
Evidently resource.

Type annotations and code completion for `#!python session.create_client("evidently").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### test\_segment\_pattern

Use this operation to test a rules pattern that you plan to use to create an
audience segment.

Type annotations and code completion for `#!python session.create_client("evidently").test_segment_pattern` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/test_segment_pattern.html)

```python
# test_segment_pattern method definition

await def test_segment_pattern(
    self,
    *,
    pattern: str,
    payload: str,
) -> TestSegmentPatternResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestSegmentPatternResponseTypeDef](./type_defs.md#testsegmentpatternresponsetypedef) 


```python
# test_segment_pattern method usage example with argument unpacking

kwargs: TestSegmentPatternRequestTypeDef = {  # (1)
    "pattern": ...,
    "payload": ...,
}

parent.test_segment_pattern(**kwargs)
```

1. See [:material-code-braces: TestSegmentPatternRequestTypeDef](./type_defs.md#testsegmentpatternrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("evidently").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/untag_resource.html)

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

### update\_experiment

Updates an Evidently experiment.

Type annotations and code completion for `#!python session.create_client("evidently").update_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/update_experiment.html)

```python
# update_experiment method definition

await def update_experiment(
    self,
    *,
    experiment: str,
    project: str,
    description: str = ...,
    metricGoals: Sequence[MetricGoalConfigTypeDef] = ...,  # (1)
    onlineAbConfig: OnlineAbConfigTypeDef = ...,  # (2)
    randomizationSalt: str = ...,
    removeSegment: bool = ...,
    samplingRate: int = ...,
    segment: str = ...,
    treatments: Sequence[TreatmentConfigTypeDef] = ...,  # (3)
) -> UpdateExperimentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MetricGoalConfigTypeDef](./type_defs.md#metricgoalconfigtypedef) 
2. See [:material-code-braces: OnlineAbConfigTypeDef](./type_defs.md#onlineabconfigtypedef) 
3. See [:material-code-braces: TreatmentConfigTypeDef](./type_defs.md#treatmentconfigtypedef) 
4. See [:material-code-braces: UpdateExperimentResponseTypeDef](./type_defs.md#updateexperimentresponsetypedef) 


```python
# update_experiment method usage example with argument unpacking

kwargs: UpdateExperimentRequestTypeDef = {  # (1)
    "experiment": ...,
    "project": ...,
}

parent.update_experiment(**kwargs)
```

1. See [:material-code-braces: UpdateExperimentRequestTypeDef](./type_defs.md#updateexperimentrequesttypedef) 

### update\_feature

Updates an existing feature.

Type annotations and code completion for `#!python session.create_client("evidently").update_feature` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/update_feature.html)

```python
# update_feature method definition

await def update_feature(
    self,
    *,
    feature: str,
    project: str,
    addOrUpdateVariations: Sequence[VariationConfigTypeDef] = ...,  # (1)
    defaultVariation: str = ...,
    description: str = ...,
    entityOverrides: Mapping[str, str] = ...,
    evaluationStrategy: FeatureEvaluationStrategyType = ...,  # (2)
    removeVariations: Sequence[str] = ...,
) -> UpdateFeatureResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VariationConfigTypeDef](./type_defs.md#variationconfigtypedef) 
2. See [:material-code-brackets: FeatureEvaluationStrategyType](./literals.md#featureevaluationstrategytype) 
3. See [:material-code-braces: UpdateFeatureResponseTypeDef](./type_defs.md#updatefeatureresponsetypedef) 


```python
# update_feature method usage example with argument unpacking

kwargs: UpdateFeatureRequestTypeDef = {  # (1)
    "feature": ...,
    "project": ...,
}

parent.update_feature(**kwargs)
```

1. See [:material-code-braces: UpdateFeatureRequestTypeDef](./type_defs.md#updatefeaturerequesttypedef) 

### update\_launch

Updates a launch of a given feature.

Type annotations and code completion for `#!python session.create_client("evidently").update_launch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/update_launch.html)

```python
# update_launch method definition

await def update_launch(
    self,
    *,
    launch: str,
    project: str,
    description: str = ...,
    groups: Sequence[LaunchGroupConfigTypeDef] = ...,  # (1)
    metricMonitors: Sequence[MetricMonitorConfigTypeDef] = ...,  # (2)
    randomizationSalt: str = ...,
    scheduledSplitsConfig: ScheduledSplitsLaunchConfigTypeDef = ...,  # (3)
) -> UpdateLaunchResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LaunchGroupConfigTypeDef](./type_defs.md#launchgroupconfigtypedef) 
2. See [:material-code-braces: MetricMonitorConfigTypeDef](./type_defs.md#metricmonitorconfigtypedef) 
3. See [:material-code-braces: ScheduledSplitsLaunchConfigTypeDef](./type_defs.md#scheduledsplitslaunchconfigtypedef) 
4. See [:material-code-braces: UpdateLaunchResponseTypeDef](./type_defs.md#updatelaunchresponsetypedef) 


```python
# update_launch method usage example with argument unpacking

kwargs: UpdateLaunchRequestTypeDef = {  # (1)
    "launch": ...,
    "project": ...,
}

parent.update_launch(**kwargs)
```

1. See [:material-code-braces: UpdateLaunchRequestTypeDef](./type_defs.md#updatelaunchrequesttypedef) 

### update\_project

Updates the description of an existing project.

Type annotations and code completion for `#!python session.create_client("evidently").update_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/update_project.html)

```python
# update_project method definition

await def update_project(
    self,
    *,
    project: str,
    appConfigResource: ProjectAppConfigResourceConfigTypeDef = ...,  # (1)
    description: str = ...,
) -> UpdateProjectResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ProjectAppConfigResourceConfigTypeDef](./type_defs.md#projectappconfigresourceconfigtypedef) 
2. See [:material-code-braces: UpdateProjectResponseTypeDef](./type_defs.md#updateprojectresponsetypedef) 


```python
# update_project method usage example with argument unpacking

kwargs: UpdateProjectRequestTypeDef = {  # (1)
    "project": ...,
}

parent.update_project(**kwargs)
```

1. See [:material-code-braces: UpdateProjectRequestTypeDef](./type_defs.md#updateprojectrequesttypedef) 

### update\_project\_data\_delivery

Updates the data storage options for this project.

Type annotations and code completion for `#!python session.create_client("evidently").update_project_data_delivery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/client/update_project_data_delivery.html)

```python
# update_project_data_delivery method definition

await def update_project_data_delivery(
    self,
    *,
    project: str,
    cloudWatchLogs: CloudWatchLogsDestinationConfigTypeDef = ...,  # (1)
    s3Destination: S3DestinationConfigTypeDef = ...,  # (2)
) -> UpdateProjectDataDeliveryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CloudWatchLogsDestinationConfigTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigtypedef) 
2. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
3. See [:material-code-braces: UpdateProjectDataDeliveryResponseTypeDef](./type_defs.md#updateprojectdatadeliveryresponsetypedef) 


```python
# update_project_data_delivery method usage example with argument unpacking

kwargs: UpdateProjectDataDeliveryRequestTypeDef = {  # (1)
    "project": ...,
}

parent.update_project_data_delivery(**kwargs)
```

1. See [:material-code-braces: UpdateProjectDataDeliveryRequestTypeDef](./type_defs.md#updateprojectdatadeliveryrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("evidently").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("evidently").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("evidently").get_paginator` method with overloads.

- `client.get_paginator("list_experiments")` -> [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
- `client.get_paginator("list_features")` -> [ListFeaturesPaginator](./paginators.md#listfeaturespaginator)
- `client.get_paginator("list_launches")` -> [ListLaunchesPaginator](./paginators.md#listlaunchespaginator)
- `client.get_paginator("list_projects")` -> [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- `client.get_paginator("list_segment_references")` -> [ListSegmentReferencesPaginator](./paginators.md#listsegmentreferencespaginator)
- `client.get_paginator("list_segments")` -> [ListSegmentsPaginator](./paginators.md#listsegmentspaginator)



