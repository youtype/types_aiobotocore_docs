# CloudWatchObservabilityAdminServiceClient

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > CloudWatchObservabilityAdminServiceClient

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).

## CloudWatchObservabilityAdminServiceClient

Type annotations and code completion for `#!python session.create_client("observabilityadmin")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#CloudWatchObservabilityAdminService.Client)

```python
# CloudWatchObservabilityAdminServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_observabilityadmin.client import CloudWatchObservabilityAdminServiceClient

session = get_session()
async with session.create_client("observabilityadmin") as client:
    client: CloudWatchObservabilityAdminServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("observabilityadmin").exceptions` structure.

```python
# CloudWatchObservabilityAdminServiceClient.exceptions usage example

async with session.create_client("observabilityadmin") as client:
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
# CloudWatchObservabilityAdminServiceClient usage type checking example

from types_aiobotocore_observabilityadmin.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("observabilityadmin").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("observabilityadmin").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/generate_presigned_url.html)

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


### create\_telemetry\_rule

Creates a telemetry rule that defines how telemetry should be configured for
Amazon Web Services resources in your account.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").create_telemetry_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/create_telemetry_rule.html)

```python
# create_telemetry_rule method definition

await def create_telemetry_rule(
    self,
    *,
    RuleName: str,
    Rule: TelemetryRuleTypeDef,  # (1)
    Tags: Mapping[str, str] = ...,
) -> CreateTelemetryRuleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)
2. See [:material-code-braces: CreateTelemetryRuleOutputTypeDef](./type_defs.md#createtelemetryruleoutputtypedef)


```python
# create_telemetry_rule method usage example with argument unpacking

kwargs: CreateTelemetryRuleInputTypeDef = {  # (1)
    "RuleName": ...,
    "Rule": ...,
}

parent.create_telemetry_rule(**kwargs)
```

1. See [:material-code-braces: CreateTelemetryRuleInputTypeDef](./type_defs.md#createtelemetryruleinputtypedef)

### create\_telemetry\_rule\_for\_organization

Creates a telemetry rule that applies across an Amazon Web Services
Organization.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").create_telemetry_rule_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/create_telemetry_rule_for_organization.html)

```python
# create_telemetry_rule_for_organization method definition

await def create_telemetry_rule_for_organization(
    self,
    *,
    RuleName: str,
    Rule: TelemetryRuleTypeDef,  # (1)
    Tags: Mapping[str, str] = ...,
) -> CreateTelemetryRuleForOrganizationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)
2. See [:material-code-braces: CreateTelemetryRuleForOrganizationOutputTypeDef](./type_defs.md#createtelemetryrulefororganizationoutputtypedef)


```python
# create_telemetry_rule_for_organization method usage example with argument unpacking

kwargs: CreateTelemetryRuleForOrganizationInputTypeDef = {  # (1)
    "RuleName": ...,
    "Rule": ...,
}

parent.create_telemetry_rule_for_organization(**kwargs)
```

1. See [:material-code-braces: CreateTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#createtelemetryrulefororganizationinputtypedef)

### delete\_telemetry\_rule

Deletes a telemetry rule from your account.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").delete_telemetry_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/delete_telemetry_rule.html)

```python
# delete_telemetry_rule method definition

await def delete_telemetry_rule(
    self,
    *,
    RuleIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_telemetry_rule method usage example with argument unpacking

kwargs: DeleteTelemetryRuleInputTypeDef = {  # (1)
    "RuleIdentifier": ...,
}

parent.delete_telemetry_rule(**kwargs)
```

1. See [:material-code-braces: DeleteTelemetryRuleInputTypeDef](./type_defs.md#deletetelemetryruleinputtypedef)

### delete\_telemetry\_rule\_for\_organization

Deletes an organization-wide telemetry rule.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").delete_telemetry_rule_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/delete_telemetry_rule_for_organization.html)

```python
# delete_telemetry_rule_for_organization method definition

await def delete_telemetry_rule_for_organization(
    self,
    *,
    RuleIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_telemetry_rule_for_organization method usage example with argument unpacking

kwargs: DeleteTelemetryRuleForOrganizationInputTypeDef = {  # (1)
    "RuleIdentifier": ...,
}

parent.delete_telemetry_rule_for_organization(**kwargs)
```

1. See [:material-code-braces: DeleteTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#deletetelemetryrulefororganizationinputtypedef)

### get\_telemetry\_evaluation\_status

Returns the current onboarding status of the telemetry config feature,
including the status of the feature and reason the feature failed to start or
stop.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_telemetry_evaluation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/get_telemetry_evaluation_status.html)

```python
# get_telemetry_evaluation_status method definition

await def get_telemetry_evaluation_status(
    self,
) -> GetTelemetryEvaluationStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTelemetryEvaluationStatusOutputTypeDef](./type_defs.md#gettelemetryevaluationstatusoutputtypedef)



### get\_telemetry\_evaluation\_status\_for\_organization

This returns the onboarding status of the telemetry configuration feature for
the organization.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_telemetry_evaluation_status_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/get_telemetry_evaluation_status_for_organization.html)

```python
# get_telemetry_evaluation_status_for_organization method definition

await def get_telemetry_evaluation_status_for_organization(
    self,
) -> GetTelemetryEvaluationStatusForOrganizationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTelemetryEvaluationStatusForOrganizationOutputTypeDef](./type_defs.md#gettelemetryevaluationstatusfororganizationoutputtypedef)



### get\_telemetry\_rule

Retrieves the details of a specific telemetry rule in your account.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_telemetry_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/get_telemetry_rule.html)

```python
# get_telemetry_rule method definition

await def get_telemetry_rule(
    self,
    *,
    RuleIdentifier: str,
) -> GetTelemetryRuleOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTelemetryRuleOutputTypeDef](./type_defs.md#gettelemetryruleoutputtypedef)


```python
# get_telemetry_rule method usage example with argument unpacking

kwargs: GetTelemetryRuleInputTypeDef = {  # (1)
    "RuleIdentifier": ...,
}

parent.get_telemetry_rule(**kwargs)
```

1. See [:material-code-braces: GetTelemetryRuleInputTypeDef](./type_defs.md#gettelemetryruleinputtypedef)

### get\_telemetry\_rule\_for\_organization

Retrieves the details of a specific organization telemetry rule.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_telemetry_rule_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/get_telemetry_rule_for_organization.html)

```python
# get_telemetry_rule_for_organization method definition

await def get_telemetry_rule_for_organization(
    self,
    *,
    RuleIdentifier: str,
) -> GetTelemetryRuleForOrganizationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTelemetryRuleForOrganizationOutputTypeDef](./type_defs.md#gettelemetryrulefororganizationoutputtypedef)


```python
# get_telemetry_rule_for_organization method usage example with argument unpacking

kwargs: GetTelemetryRuleForOrganizationInputTypeDef = {  # (1)
    "RuleIdentifier": ...,
}

parent.get_telemetry_rule_for_organization(**kwargs)
```

1. See [:material-code-braces: GetTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#gettelemetryrulefororganizationinputtypedef)

### list\_resource\_telemetry

Returns a list of telemetry configurations for Amazon Web Services resources
supported by telemetry config.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").list_resource_telemetry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/list_resource_telemetry.html)

```python
# list_resource_telemetry method definition

await def list_resource_telemetry(
    self,
    *,
    ResourceIdentifierPrefix: str = ...,
    ResourceTypes: Sequence[ResourceTypeType] = ...,  # (1)
    TelemetryConfigurationState: Mapping[TelemetryTypeType, TelemetryStateType] = ...,  # (2)
    ResourceTags: Mapping[str, str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourceTelemetryOutputTypeDef:  # (3)
    ...
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`
3. See [:material-code-braces: ListResourceTelemetryOutputTypeDef](./type_defs.md#listresourcetelemetryoutputtypedef)


```python
# list_resource_telemetry method usage example with argument unpacking

kwargs: ListResourceTelemetryInputTypeDef = {  # (1)
    "ResourceIdentifierPrefix": ...,
}

parent.list_resource_telemetry(**kwargs)
```

1. See [:material-code-braces: ListResourceTelemetryInputTypeDef](./type_defs.md#listresourcetelemetryinputtypedef)

### list\_resource\_telemetry\_for\_organization

Returns a list of telemetry configurations for Amazon Web Services resources
supported by telemetry config in the organization.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").list_resource_telemetry_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/list_resource_telemetry_for_organization.html)

```python
# list_resource_telemetry_for_organization method definition

await def list_resource_telemetry_for_organization(
    self,
    *,
    AccountIdentifiers: Sequence[str] = ...,
    ResourceIdentifierPrefix: str = ...,
    ResourceTypes: Sequence[ResourceTypeType] = ...,  # (1)
    TelemetryConfigurationState: Mapping[TelemetryTypeType, TelemetryStateType] = ...,  # (2)
    ResourceTags: Mapping[str, str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourceTelemetryForOrganizationOutputTypeDef:  # (3)
    ...
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`
3. See [:material-code-braces: ListResourceTelemetryForOrganizationOutputTypeDef](./type_defs.md#listresourcetelemetryfororganizationoutputtypedef)


```python
# list_resource_telemetry_for_organization method usage example with argument unpacking

kwargs: ListResourceTelemetryForOrganizationInputTypeDef = {  # (1)
    "AccountIdentifiers": ...,
}

parent.list_resource_telemetry_for_organization(**kwargs)
```

1. See [:material-code-braces: ListResourceTelemetryForOrganizationInputTypeDef](./type_defs.md#listresourcetelemetryfororganizationinputtypedef)

### list\_tags\_for\_resource

Lists all tags attached to the specified telemetry rule resource.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)

### list\_telemetry\_rules

Lists all telemetry rules in your account.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").list_telemetry_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/list_telemetry_rules.html)

```python
# list_telemetry_rules method definition

await def list_telemetry_rules(
    self,
    *,
    RuleNamePrefix: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTelemetryRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTelemetryRulesOutputTypeDef](./type_defs.md#listtelemetryrulesoutputtypedef)


```python
# list_telemetry_rules method usage example with argument unpacking

kwargs: ListTelemetryRulesInputTypeDef = {  # (1)
    "RuleNamePrefix": ...,
}

parent.list_telemetry_rules(**kwargs)
```

1. See [:material-code-braces: ListTelemetryRulesInputTypeDef](./type_defs.md#listtelemetryrulesinputtypedef)

### list\_telemetry\_rules\_for\_organization

Lists all telemetry rules in your organization.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").list_telemetry_rules_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/list_telemetry_rules_for_organization.html)

```python
# list_telemetry_rules_for_organization method definition

await def list_telemetry_rules_for_organization(
    self,
    *,
    RuleNamePrefix: str = ...,
    SourceAccountIds: Sequence[str] = ...,
    SourceOrganizationUnitIds: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTelemetryRulesForOrganizationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTelemetryRulesForOrganizationOutputTypeDef](./type_defs.md#listtelemetryrulesfororganizationoutputtypedef)


```python
# list_telemetry_rules_for_organization method usage example with argument unpacking

kwargs: ListTelemetryRulesForOrganizationInputTypeDef = {  # (1)
    "RuleNamePrefix": ...,
}

parent.list_telemetry_rules_for_organization(**kwargs)
```

1. See [:material-code-braces: ListTelemetryRulesForOrganizationInputTypeDef](./type_defs.md#listtelemetryrulesfororganizationinputtypedef)

### start\_telemetry\_evaluation

This action begins onboarding the caller Amazon Web Services account to the
telemetry config feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").start_telemetry_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/start_telemetry_evaluation.html)

```python
# start_telemetry_evaluation method definition

await def start_telemetry_evaluation(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



### start\_telemetry\_evaluation\_for\_organization

This actions begins onboarding the organization and all member accounts to the
telemetry config feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").start_telemetry_evaluation_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/start_telemetry_evaluation_for_organization.html)

```python
# start_telemetry_evaluation_for_organization method definition

await def start_telemetry_evaluation_for_organization(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



### stop\_telemetry\_evaluation

This action begins offboarding the caller Amazon Web Services account from the
telemetry config feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").stop_telemetry_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/stop_telemetry_evaluation.html)

```python
# stop_telemetry_evaluation method definition

await def stop_telemetry_evaluation(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



### stop\_telemetry\_evaluation\_for\_organization

This action offboards the Organization of the caller Amazon Web Services
account from the telemetry config feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").stop_telemetry_evaluation_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/stop_telemetry_evaluation_for_organization.html)

```python
# stop_telemetry_evaluation_for_organization method definition

await def stop_telemetry_evaluation_for_organization(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



### tag\_resource

Adds or updates tags for a telemetry rule resource.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)

### untag\_resource

Removes tags from a telemetry rule resource.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)

### update\_telemetry\_rule

Updates an existing telemetry rule in your account.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").update_telemetry_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/update_telemetry_rule.html)

```python
# update_telemetry_rule method definition

await def update_telemetry_rule(
    self,
    *,
    RuleIdentifier: str,
    Rule: TelemetryRuleTypeDef,  # (1)
) -> UpdateTelemetryRuleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)
2. See [:material-code-braces: UpdateTelemetryRuleOutputTypeDef](./type_defs.md#updatetelemetryruleoutputtypedef)


```python
# update_telemetry_rule method usage example with argument unpacking

kwargs: UpdateTelemetryRuleInputTypeDef = {  # (1)
    "RuleIdentifier": ...,
    "Rule": ...,
}

parent.update_telemetry_rule(**kwargs)
```

1. See [:material-code-braces: UpdateTelemetryRuleInputTypeDef](./type_defs.md#updatetelemetryruleinputtypedef)

### update\_telemetry\_rule\_for\_organization

Updates an existing telemetry rule that applies across an Amazon Web Services
Organization.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").update_telemetry_rule_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/update_telemetry_rule_for_organization.html)

```python
# update_telemetry_rule_for_organization method definition

await def update_telemetry_rule_for_organization(
    self,
    *,
    RuleIdentifier: str,
    Rule: TelemetryRuleTypeDef,  # (1)
) -> UpdateTelemetryRuleForOrganizationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TelemetryRuleTypeDef](./type_defs.md#telemetryruletypedef)
2. See [:material-code-braces: UpdateTelemetryRuleForOrganizationOutputTypeDef](./type_defs.md#updatetelemetryrulefororganizationoutputtypedef)


```python
# update_telemetry_rule_for_organization method usage example with argument unpacking

kwargs: UpdateTelemetryRuleForOrganizationInputTypeDef = {  # (1)
    "RuleIdentifier": ...,
    "Rule": ...,
}

parent.update_telemetry_rule_for_organization(**kwargs)
```

1. See [:material-code-braces: UpdateTelemetryRuleForOrganizationInputTypeDef](./type_defs.md#updatetelemetryrulefororganizationinputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("observabilityadmin").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#CloudWatchObservabilityAdminService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("observabilityadmin").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#CloudWatchObservabilityAdminService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator` method with overloads.

- `client.get_paginator("list_resource_telemetry_for_organization")` -> [ListResourceTelemetryForOrganizationPaginator](./paginators.md#listresourcetelemetryfororganizationpaginator)
- `client.get_paginator("list_resource_telemetry")` -> [ListResourceTelemetryPaginator](./paginators.md#listresourcetelemetrypaginator)
- `client.get_paginator("list_telemetry_rules_for_organization")` -> [ListTelemetryRulesForOrganizationPaginator](./paginators.md#listtelemetryrulesfororganizationpaginator)
- `client.get_paginator("list_telemetry_rules")` -> [ListTelemetryRulesPaginator](./paginators.md#listtelemetryrulespaginator)



