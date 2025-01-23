# MainframeModernizationApplicationTestingClient

> [Index](../README.md) > [MainframeModernizationApplicationTesting](./README.md) > MainframeModernizationApplicationTestingClient

!!! note ""

    Auto-generated documentation for [MainframeModernizationApplicationTesting](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#mainframemodernizationapplicationtesting)
    type annotations stubs module [types-aiobotocore-apptest](https://pypi.org/project/types-aiobotocore-apptest/).

## MainframeModernizationApplicationTestingClient

Type annotations and code completion for `#!python session.create_client("apptest")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#MainframeModernizationApplicationTesting.Client)

```python
# MainframeModernizationApplicationTestingClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_apptest.client import MainframeModernizationApplicationTestingClient

session = get_session()
async with session.create_client("apptest") as client:
    client: MainframeModernizationApplicationTestingClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("apptest").exceptions` structure.

```python
# MainframeModernizationApplicationTestingClient.exceptions usage example

async with session.create_client("apptest") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# MainframeModernizationApplicationTestingClient usage type checking example

from types_aiobotocore_apptest.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("apptest").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("apptest").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/generate_presigned_url.html)

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


### create\_test\_case

Creates a test case.

Type annotations and code completion for `#!python session.create_client("apptest").create_test_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/create_test_case.html)

```python
# create_test_case method definition

await def create_test_case(
    self,
    *,
    name: str,
    steps: Sequence[StepUnionTypeDef],  # (1)
    description: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateTestCaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) [:material-code-braces: StepOutputTypeDef](./type_defs.md#stepoutputtypedef) 
2. See [:material-code-braces: CreateTestCaseResponseTypeDef](./type_defs.md#createtestcaseresponsetypedef) 


```python
# create_test_case method usage example with argument unpacking

kwargs: CreateTestCaseRequestRequestTypeDef = {  # (1)
    "name": ...,
    "steps": ...,
}

parent.create_test_case(**kwargs)
```

1. See [:material-code-braces: CreateTestCaseRequestRequestTypeDef](./type_defs.md#createtestcaserequestrequesttypedef) 

### create\_test\_configuration

Creates a test configuration.

Type annotations and code completion for `#!python session.create_client("apptest").create_test_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/create_test_configuration.html)

```python
# create_test_configuration method definition

await def create_test_configuration(
    self,
    *,
    name: str,
    resources: Sequence[ResourceUnionTypeDef],  # (1)
    description: str = ...,
    properties: Mapping[str, str] = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
    serviceSettings: ServiceSettingsTypeDef = ...,  # (2)
) -> CreateTestConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef) 
3. See [:material-code-braces: CreateTestConfigurationResponseTypeDef](./type_defs.md#createtestconfigurationresponsetypedef) 


```python
# create_test_configuration method usage example with argument unpacking

kwargs: CreateTestConfigurationRequestRequestTypeDef = {  # (1)
    "name": ...,
    "resources": ...,
}

parent.create_test_configuration(**kwargs)
```

1. See [:material-code-braces: CreateTestConfigurationRequestRequestTypeDef](./type_defs.md#createtestconfigurationrequestrequesttypedef) 

### create\_test\_suite

Creates a test suite.

Type annotations and code completion for `#!python session.create_client("apptest").create_test_suite` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/create_test_suite.html)

```python
# create_test_suite method definition

await def create_test_suite(
    self,
    *,
    name: str,
    testCases: TestCasesTypeDef,  # (1)
    description: str = ...,
    beforeSteps: Sequence[StepTypeDef] = ...,  # (2)
    afterSteps: Sequence[StepTypeDef] = ...,  # (2)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateTestSuiteResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TestCasesTypeDef](./type_defs.md#testcasestypedef) 
2. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
3. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
4. See [:material-code-braces: CreateTestSuiteResponseTypeDef](./type_defs.md#createtestsuiteresponsetypedef) 


```python
# create_test_suite method usage example with argument unpacking

kwargs: CreateTestSuiteRequestRequestTypeDef = {  # (1)
    "name": ...,
    "testCases": ...,
}

parent.create_test_suite(**kwargs)
```

1. See [:material-code-braces: CreateTestSuiteRequestRequestTypeDef](./type_defs.md#createtestsuiterequestrequesttypedef) 

### delete\_test\_case

Deletes a test case.

Type annotations and code completion for `#!python session.create_client("apptest").delete_test_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/delete_test_case.html)

```python
# delete_test_case method definition

await def delete_test_case(
    self,
    *,
    testCaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_test_case method usage example with argument unpacking

kwargs: DeleteTestCaseRequestRequestTypeDef = {  # (1)
    "testCaseId": ...,
}

parent.delete_test_case(**kwargs)
```

1. See [:material-code-braces: DeleteTestCaseRequestRequestTypeDef](./type_defs.md#deletetestcaserequestrequesttypedef) 

### delete\_test\_configuration

Deletes a test configuration.

Type annotations and code completion for `#!python session.create_client("apptest").delete_test_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/delete_test_configuration.html)

```python
# delete_test_configuration method definition

await def delete_test_configuration(
    self,
    *,
    testConfigurationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_test_configuration method usage example with argument unpacking

kwargs: DeleteTestConfigurationRequestRequestTypeDef = {  # (1)
    "testConfigurationId": ...,
}

parent.delete_test_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteTestConfigurationRequestRequestTypeDef](./type_defs.md#deletetestconfigurationrequestrequesttypedef) 

### delete\_test\_run

Deletes a test run.

Type annotations and code completion for `#!python session.create_client("apptest").delete_test_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/delete_test_run.html)

```python
# delete_test_run method definition

await def delete_test_run(
    self,
    *,
    testRunId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_test_run method usage example with argument unpacking

kwargs: DeleteTestRunRequestRequestTypeDef = {  # (1)
    "testRunId": ...,
}

parent.delete_test_run(**kwargs)
```

1. See [:material-code-braces: DeleteTestRunRequestRequestTypeDef](./type_defs.md#deletetestrunrequestrequesttypedef) 

### delete\_test\_suite

Deletes a test suite.

Type annotations and code completion for `#!python session.create_client("apptest").delete_test_suite` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/delete_test_suite.html)

```python
# delete_test_suite method definition

await def delete_test_suite(
    self,
    *,
    testSuiteId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_test_suite method usage example with argument unpacking

kwargs: DeleteTestSuiteRequestRequestTypeDef = {  # (1)
    "testSuiteId": ...,
}

parent.delete_test_suite(**kwargs)
```

1. See [:material-code-braces: DeleteTestSuiteRequestRequestTypeDef](./type_defs.md#deletetestsuiterequestrequesttypedef) 

### get\_test\_case

Gets a test case.

Type annotations and code completion for `#!python session.create_client("apptest").get_test_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/get_test_case.html)

```python
# get_test_case method definition

await def get_test_case(
    self,
    *,
    testCaseId: str,
    testCaseVersion: int = ...,
) -> GetTestCaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestCaseResponseTypeDef](./type_defs.md#gettestcaseresponsetypedef) 


```python
# get_test_case method usage example with argument unpacking

kwargs: GetTestCaseRequestRequestTypeDef = {  # (1)
    "testCaseId": ...,
}

parent.get_test_case(**kwargs)
```

1. See [:material-code-braces: GetTestCaseRequestRequestTypeDef](./type_defs.md#gettestcaserequestrequesttypedef) 

### get\_test\_configuration

Gets a test configuration.

Type annotations and code completion for `#!python session.create_client("apptest").get_test_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/get_test_configuration.html)

```python
# get_test_configuration method definition

await def get_test_configuration(
    self,
    *,
    testConfigurationId: str,
    testConfigurationVersion: int = ...,
) -> GetTestConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestConfigurationResponseTypeDef](./type_defs.md#gettestconfigurationresponsetypedef) 


```python
# get_test_configuration method usage example with argument unpacking

kwargs: GetTestConfigurationRequestRequestTypeDef = {  # (1)
    "testConfigurationId": ...,
}

parent.get_test_configuration(**kwargs)
```

1. See [:material-code-braces: GetTestConfigurationRequestRequestTypeDef](./type_defs.md#gettestconfigurationrequestrequesttypedef) 

### get\_test\_run\_step

Gets a test run step.

Type annotations and code completion for `#!python session.create_client("apptest").get_test_run_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/get_test_run_step.html)

```python
# get_test_run_step method definition

await def get_test_run_step(
    self,
    *,
    testRunId: str,
    stepName: str,
    testCaseId: str = ...,
    testSuiteId: str = ...,
) -> GetTestRunStepResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestRunStepResponseTypeDef](./type_defs.md#gettestrunstepresponsetypedef) 


```python
# get_test_run_step method usage example with argument unpacking

kwargs: GetTestRunStepRequestRequestTypeDef = {  # (1)
    "testRunId": ...,
    "stepName": ...,
}

parent.get_test_run_step(**kwargs)
```

1. See [:material-code-braces: GetTestRunStepRequestRequestTypeDef](./type_defs.md#gettestrunsteprequestrequesttypedef) 

### get\_test\_suite

Gets a test suite.

Type annotations and code completion for `#!python session.create_client("apptest").get_test_suite` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/get_test_suite.html)

```python
# get_test_suite method definition

await def get_test_suite(
    self,
    *,
    testSuiteId: str,
    testSuiteVersion: int = ...,
) -> GetTestSuiteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestSuiteResponseTypeDef](./type_defs.md#gettestsuiteresponsetypedef) 


```python
# get_test_suite method usage example with argument unpacking

kwargs: GetTestSuiteRequestRequestTypeDef = {  # (1)
    "testSuiteId": ...,
}

parent.get_test_suite(**kwargs)
```

1. See [:material-code-braces: GetTestSuiteRequestRequestTypeDef](./type_defs.md#gettestsuiterequestrequesttypedef) 

### list\_tags\_for\_resource

Lists tags for a resource.

Type annotations and code completion for `#!python session.create_client("apptest").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/list_tags_for_resource.html)

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

### list\_test\_cases

Lists test cases.

Type annotations and code completion for `#!python session.create_client("apptest").list_test_cases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/list_test_cases.html)

```python
# list_test_cases method definition

await def list_test_cases(
    self,
    *,
    testCaseIds: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTestCasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestCasesResponseTypeDef](./type_defs.md#listtestcasesresponsetypedef) 


```python
# list_test_cases method usage example with argument unpacking

kwargs: ListTestCasesRequestRequestTypeDef = {  # (1)
    "testCaseIds": ...,
}

parent.list_test_cases(**kwargs)
```

1. See [:material-code-braces: ListTestCasesRequestRequestTypeDef](./type_defs.md#listtestcasesrequestrequesttypedef) 

### list\_test\_configurations

Lists test configurations.

Type annotations and code completion for `#!python session.create_client("apptest").list_test_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/list_test_configurations.html)

```python
# list_test_configurations method definition

await def list_test_configurations(
    self,
    *,
    testConfigurationIds: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTestConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestConfigurationsResponseTypeDef](./type_defs.md#listtestconfigurationsresponsetypedef) 


```python
# list_test_configurations method usage example with argument unpacking

kwargs: ListTestConfigurationsRequestRequestTypeDef = {  # (1)
    "testConfigurationIds": ...,
}

parent.list_test_configurations(**kwargs)
```

1. See [:material-code-braces: ListTestConfigurationsRequestRequestTypeDef](./type_defs.md#listtestconfigurationsrequestrequesttypedef) 

### list\_test\_run\_steps

Lists test run steps.

Type annotations and code completion for `#!python session.create_client("apptest").list_test_run_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/list_test_run_steps.html)

```python
# list_test_run_steps method definition

await def list_test_run_steps(
    self,
    *,
    testRunId: str,
    testCaseId: str = ...,
    testSuiteId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTestRunStepsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestRunStepsResponseTypeDef](./type_defs.md#listtestrunstepsresponsetypedef) 


```python
# list_test_run_steps method usage example with argument unpacking

kwargs: ListTestRunStepsRequestRequestTypeDef = {  # (1)
    "testRunId": ...,
}

parent.list_test_run_steps(**kwargs)
```

1. See [:material-code-braces: ListTestRunStepsRequestRequestTypeDef](./type_defs.md#listtestrunstepsrequestrequesttypedef) 

### list\_test\_run\_test\_cases

Lists test run test cases.

Type annotations and code completion for `#!python session.create_client("apptest").list_test_run_test_cases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/list_test_run_test_cases.html)

```python
# list_test_run_test_cases method definition

await def list_test_run_test_cases(
    self,
    *,
    testRunId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTestRunTestCasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestRunTestCasesResponseTypeDef](./type_defs.md#listtestruntestcasesresponsetypedef) 


```python
# list_test_run_test_cases method usage example with argument unpacking

kwargs: ListTestRunTestCasesRequestRequestTypeDef = {  # (1)
    "testRunId": ...,
}

parent.list_test_run_test_cases(**kwargs)
```

1. See [:material-code-braces: ListTestRunTestCasesRequestRequestTypeDef](./type_defs.md#listtestruntestcasesrequestrequesttypedef) 

### list\_test\_runs

Lists test runs.

Type annotations and code completion for `#!python session.create_client("apptest").list_test_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/list_test_runs.html)

```python
# list_test_runs method definition

await def list_test_runs(
    self,
    *,
    testSuiteId: str = ...,
    testRunIds: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTestRunsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestRunsResponseTypeDef](./type_defs.md#listtestrunsresponsetypedef) 


```python
# list_test_runs method usage example with argument unpacking

kwargs: ListTestRunsRequestRequestTypeDef = {  # (1)
    "testSuiteId": ...,
}

parent.list_test_runs(**kwargs)
```

1. See [:material-code-braces: ListTestRunsRequestRequestTypeDef](./type_defs.md#listtestrunsrequestrequesttypedef) 

### list\_test\_suites

Lists test suites.

Type annotations and code completion for `#!python session.create_client("apptest").list_test_suites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/list_test_suites.html)

```python
# list_test_suites method definition

await def list_test_suites(
    self,
    *,
    testSuiteIds: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTestSuitesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestSuitesResponseTypeDef](./type_defs.md#listtestsuitesresponsetypedef) 


```python
# list_test_suites method usage example with argument unpacking

kwargs: ListTestSuitesRequestRequestTypeDef = {  # (1)
    "testSuiteIds": ...,
}

parent.list_test_suites(**kwargs)
```

1. See [:material-code-braces: ListTestSuitesRequestRequestTypeDef](./type_defs.md#listtestsuitesrequestrequesttypedef) 

### start\_test\_run

Starts a test run.

Type annotations and code completion for `#!python session.create_client("apptest").start_test_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/start_test_run.html)

```python
# start_test_run method definition

await def start_test_run(
    self,
    *,
    testSuiteId: str,
    testConfigurationId: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> StartTestRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartTestRunResponseTypeDef](./type_defs.md#starttestrunresponsetypedef) 


```python
# start_test_run method usage example with argument unpacking

kwargs: StartTestRunRequestRequestTypeDef = {  # (1)
    "testSuiteId": ...,
}

parent.start_test_run(**kwargs)
```

1. See [:material-code-braces: StartTestRunRequestRequestTypeDef](./type_defs.md#starttestrunrequestrequesttypedef) 

### tag\_resource

Specifies tags of a resource.

Type annotations and code completion for `#!python session.create_client("apptest").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/tag_resource.html)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Untags a resource.

Type annotations and code completion for `#!python session.create_client("apptest").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/untag_resource.html)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_test\_case

Updates a test case.

Type annotations and code completion for `#!python session.create_client("apptest").update_test_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/update_test_case.html)

```python
# update_test_case method definition

await def update_test_case(
    self,
    *,
    testCaseId: str,
    description: str = ...,
    steps: Sequence[StepTypeDef] = ...,  # (1)
) -> UpdateTestCaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
2. See [:material-code-braces: UpdateTestCaseResponseTypeDef](./type_defs.md#updatetestcaseresponsetypedef) 


```python
# update_test_case method usage example with argument unpacking

kwargs: UpdateTestCaseRequestRequestTypeDef = {  # (1)
    "testCaseId": ...,
}

parent.update_test_case(**kwargs)
```

1. See [:material-code-braces: UpdateTestCaseRequestRequestTypeDef](./type_defs.md#updatetestcaserequestrequesttypedef) 

### update\_test\_configuration

Updates a test configuration.

Type annotations and code completion for `#!python session.create_client("apptest").update_test_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/update_test_configuration.html)

```python
# update_test_configuration method definition

await def update_test_configuration(
    self,
    *,
    testConfigurationId: str,
    description: str = ...,
    resources: Sequence[ResourceTypeDef] = ...,  # (1)
    properties: Mapping[str, str] = ...,
    serviceSettings: ServiceSettingsTypeDef = ...,  # (2)
) -> UpdateTestConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef) 
3. See [:material-code-braces: UpdateTestConfigurationResponseTypeDef](./type_defs.md#updatetestconfigurationresponsetypedef) 


```python
# update_test_configuration method usage example with argument unpacking

kwargs: UpdateTestConfigurationRequestRequestTypeDef = {  # (1)
    "testConfigurationId": ...,
}

parent.update_test_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateTestConfigurationRequestRequestTypeDef](./type_defs.md#updatetestconfigurationrequestrequesttypedef) 

### update\_test\_suite

Updates a test suite.

Type annotations and code completion for `#!python session.create_client("apptest").update_test_suite` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest/client/update_test_suite.html)

```python
# update_test_suite method definition

await def update_test_suite(
    self,
    *,
    testSuiteId: str,
    description: str = ...,
    beforeSteps: Sequence[StepTypeDef] = ...,  # (1)
    afterSteps: Sequence[StepTypeDef] = ...,  # (1)
    testCases: TestCasesTypeDef = ...,  # (3)
) -> UpdateTestSuiteResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
2. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
3. See [:material-code-braces: TestCasesTypeDef](./type_defs.md#testcasestypedef) 
4. See [:material-code-braces: UpdateTestSuiteResponseTypeDef](./type_defs.md#updatetestsuiteresponsetypedef) 


```python
# update_test_suite method usage example with argument unpacking

kwargs: UpdateTestSuiteRequestRequestTypeDef = {  # (1)
    "testSuiteId": ...,
}

parent.update_test_suite(**kwargs)
```

1. See [:material-code-braces: UpdateTestSuiteRequestRequestTypeDef](./type_defs.md#updatetestsuiterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("apptest").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#MainframeModernizationApplicationTesting.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("apptest").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#MainframeModernizationApplicationTesting.Client)

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

Type annotations and code completion for `#!python session.create_client("apptest").get_paginator` method with overloads.

- `client.get_paginator("list_test_cases")` -> [ListTestCasesPaginator](./paginators.md#listtestcasespaginator)
- `client.get_paginator("list_test_configurations")` -> [ListTestConfigurationsPaginator](./paginators.md#listtestconfigurationspaginator)
- `client.get_paginator("list_test_run_steps")` -> [ListTestRunStepsPaginator](./paginators.md#listtestrunstepspaginator)
- `client.get_paginator("list_test_run_test_cases")` -> [ListTestRunTestCasesPaginator](./paginators.md#listtestruntestcasespaginator)
- `client.get_paginator("list_test_runs")` -> [ListTestRunsPaginator](./paginators.md#listtestrunspaginator)
- `client.get_paginator("list_test_suites")` -> [ListTestSuitesPaginator](./paginators.md#listtestsuitespaginator)



