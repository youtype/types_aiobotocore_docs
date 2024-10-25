# SecurityHubClient

> [Index](../README.md) > [SecurityHub](./README.md) > SecurityHubClient

!!! note ""

    Auto-generated documentation for [SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
    type annotations stubs module [types-aiobotocore-securityhub](https://pypi.org/project/types-aiobotocore-securityhub/).

## SecurityHubClient

Type annotations and code completion for `#!python session.create_client("securityhub")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client)

```python
# SecurityHubClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_securityhub.client import SecurityHubClient

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("securityhub").exceptions` structure.

```python
# SecurityHubClient.exceptions usage example

async with session.create_client("securityhub") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalException,
        client.InvalidAccessException,
        client.InvalidInputException,
        client.LimitExceededException,
        client.ResourceConflictException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# SecurityHubClient usage type checking example

from types_aiobotocore_securityhub.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### accept\_administrator\_invitation

.

Type annotations and code completion for `#!python session.create_client("securityhub").accept_administrator_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.accept_administrator_invitation)

```python
# accept_administrator_invitation method definition

await def accept_administrator_invitation(
    self,
    *,
    AdministratorId: str,
    InvitationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# accept_administrator_invitation method usage example with argument unpacking

kwargs: AcceptAdministratorInvitationRequestRequestTypeDef = {  # (1)
    "AdministratorId": ...,
    "InvitationId": ...,
}

parent.accept_administrator_invitation(**kwargs)
```

1. See [:material-code-braces: AcceptAdministratorInvitationRequestRequestTypeDef](./type_defs.md#acceptadministratorinvitationrequestrequesttypedef) 

### accept\_invitation

This method is deprecated.

Type annotations and code completion for `#!python session.create_client("securityhub").accept_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.accept_invitation)

```python
# accept_invitation method definition

await def accept_invitation(
    self,
    *,
    MasterId: str,
    InvitationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# accept_invitation method usage example with argument unpacking

kwargs: AcceptInvitationRequestRequestTypeDef = {  # (1)
    "MasterId": ...,
    "InvitationId": ...,
}

parent.accept_invitation(**kwargs)
```

1. See [:material-code-braces: AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef) 

### batch\_delete\_automation\_rules

Deletes one or more automation rules.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_delete_automation_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_delete_automation_rules)

```python
# batch_delete_automation_rules method definition

await def batch_delete_automation_rules(
    self,
    *,
    AutomationRulesArns: Sequence[str],
) -> BatchDeleteAutomationRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteAutomationRulesResponseTypeDef](./type_defs.md#batchdeleteautomationrulesresponsetypedef) 


```python
# batch_delete_automation_rules method usage example with argument unpacking

kwargs: BatchDeleteAutomationRulesRequestRequestTypeDef = {  # (1)
    "AutomationRulesArns": ...,
}

parent.batch_delete_automation_rules(**kwargs)
```

1. See [:material-code-braces: BatchDeleteAutomationRulesRequestRequestTypeDef](./type_defs.md#batchdeleteautomationrulesrequestrequesttypedef) 

### batch\_disable\_standards

Disables the standards specified by the provided `StandardsSubscriptionArns`.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_disable_standards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_disable_standards)

```python
# batch_disable_standards method definition

await def batch_disable_standards(
    self,
    *,
    StandardsSubscriptionArns: Sequence[str],
) -> BatchDisableStandardsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDisableStandardsResponseTypeDef](./type_defs.md#batchdisablestandardsresponsetypedef) 


```python
# batch_disable_standards method usage example with argument unpacking

kwargs: BatchDisableStandardsRequestRequestTypeDef = {  # (1)
    "StandardsSubscriptionArns": ...,
}

parent.batch_disable_standards(**kwargs)
```

1. See [:material-code-braces: BatchDisableStandardsRequestRequestTypeDef](./type_defs.md#batchdisablestandardsrequestrequesttypedef) 

### batch\_enable\_standards

Enables the standards specified by the provided `StandardsArn`.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_enable_standards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_enable_standards)

```python
# batch_enable_standards method definition

await def batch_enable_standards(
    self,
    *,
    StandardsSubscriptionRequests: Sequence[StandardsSubscriptionRequestTypeDef],  # (1)
) -> BatchEnableStandardsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StandardsSubscriptionRequestTypeDef](./type_defs.md#standardssubscriptionrequesttypedef) 
2. See [:material-code-braces: BatchEnableStandardsResponseTypeDef](./type_defs.md#batchenablestandardsresponsetypedef) 


```python
# batch_enable_standards method usage example with argument unpacking

kwargs: BatchEnableStandardsRequestRequestTypeDef = {  # (1)
    "StandardsSubscriptionRequests": ...,
}

parent.batch_enable_standards(**kwargs)
```

1. See [:material-code-braces: BatchEnableStandardsRequestRequestTypeDef](./type_defs.md#batchenablestandardsrequestrequesttypedef) 

### batch\_get\_automation\_rules

Retrieves a list of details for automation rules based on rule Amazon Resource
Names
(ARNs).

Type annotations and code completion for `#!python session.create_client("securityhub").batch_get_automation_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_automation_rules)

```python
# batch_get_automation_rules method definition

await def batch_get_automation_rules(
    self,
    *,
    AutomationRulesArns: Sequence[str],
) -> BatchGetAutomationRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetAutomationRulesResponseTypeDef](./type_defs.md#batchgetautomationrulesresponsetypedef) 


```python
# batch_get_automation_rules method usage example with argument unpacking

kwargs: BatchGetAutomationRulesRequestRequestTypeDef = {  # (1)
    "AutomationRulesArns": ...,
}

parent.batch_get_automation_rules(**kwargs)
```

1. See [:material-code-braces: BatchGetAutomationRulesRequestRequestTypeDef](./type_defs.md#batchgetautomationrulesrequestrequesttypedef) 

### batch\_get\_configuration\_policy\_associations

Returns associations between an Security Hub configuration and a batch of
target accounts, organizational units, or the
root.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_get_configuration_policy_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_configuration_policy_associations)

```python
# batch_get_configuration_policy_associations method definition

await def batch_get_configuration_policy_associations(
    self,
    *,
    ConfigurationPolicyAssociationIdentifiers: Sequence[ConfigurationPolicyAssociationTypeDef],  # (1)
) -> BatchGetConfigurationPolicyAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationPolicyAssociationTypeDef](./type_defs.md#configurationpolicyassociationtypedef) 
2. See [:material-code-braces: BatchGetConfigurationPolicyAssociationsResponseTypeDef](./type_defs.md#batchgetconfigurationpolicyassociationsresponsetypedef) 


```python
# batch_get_configuration_policy_associations method usage example with argument unpacking

kwargs: BatchGetConfigurationPolicyAssociationsRequestRequestTypeDef = {  # (1)
    "ConfigurationPolicyAssociationIdentifiers": ...,
}

parent.batch_get_configuration_policy_associations(**kwargs)
```

1. See [:material-code-braces: BatchGetConfigurationPolicyAssociationsRequestRequestTypeDef](./type_defs.md#batchgetconfigurationpolicyassociationsrequestrequesttypedef) 

### batch\_get\_security\_controls

Provides details about a batch of security controls for the current Amazon Web
Services account and Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_get_security_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_security_controls)

```python
# batch_get_security_controls method definition

await def batch_get_security_controls(
    self,
    *,
    SecurityControlIds: Sequence[str],
) -> BatchGetSecurityControlsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetSecurityControlsResponseTypeDef](./type_defs.md#batchgetsecuritycontrolsresponsetypedef) 


```python
# batch_get_security_controls method usage example with argument unpacking

kwargs: BatchGetSecurityControlsRequestRequestTypeDef = {  # (1)
    "SecurityControlIds": ...,
}

parent.batch_get_security_controls(**kwargs)
```

1. See [:material-code-braces: BatchGetSecurityControlsRequestRequestTypeDef](./type_defs.md#batchgetsecuritycontrolsrequestrequesttypedef) 

### batch\_get\_standards\_control\_associations

For a batch of security controls and standards, identifies whether each control
is currently enabled or disabled in a
standard.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_get_standards_control_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)

```python
# batch_get_standards_control_associations method definition

await def batch_get_standards_control_associations(
    self,
    *,
    StandardsControlAssociationIds: Sequence[StandardsControlAssociationIdTypeDef],  # (1)
) -> BatchGetStandardsControlAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StandardsControlAssociationIdTypeDef](./type_defs.md#standardscontrolassociationidtypedef) 
2. See [:material-code-braces: BatchGetStandardsControlAssociationsResponseTypeDef](./type_defs.md#batchgetstandardscontrolassociationsresponsetypedef) 


```python
# batch_get_standards_control_associations method usage example with argument unpacking

kwargs: BatchGetStandardsControlAssociationsRequestRequestTypeDef = {  # (1)
    "StandardsControlAssociationIds": ...,
}

parent.batch_get_standards_control_associations(**kwargs)
```

1. See [:material-code-braces: BatchGetStandardsControlAssociationsRequestRequestTypeDef](./type_defs.md#batchgetstandardscontrolassociationsrequestrequesttypedef) 

### batch\_import\_findings

Imports security findings generated by a finding provider into Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_import_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)

```python
# batch_import_findings method definition

await def batch_import_findings(
    self,
    *,
    Findings: Sequence[AwsSecurityFindingUnionTypeDef],  # (1)
) -> BatchImportFindingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingTypeDef](./type_defs.md#awssecurityfindingtypedef) [:material-code-braces: AwsSecurityFindingOutputTypeDef](./type_defs.md#awssecurityfindingoutputtypedef) 
2. See [:material-code-braces: BatchImportFindingsResponseTypeDef](./type_defs.md#batchimportfindingsresponsetypedef) 


```python
# batch_import_findings method usage example with argument unpacking

kwargs: BatchImportFindingsRequestRequestTypeDef = {  # (1)
    "Findings": ...,
}

parent.batch_import_findings(**kwargs)
```

1. See [:material-code-braces: BatchImportFindingsRequestRequestTypeDef](./type_defs.md#batchimportfindingsrequestrequesttypedef) 

### batch\_update\_automation\_rules

Updates one or more automation rules based on rule Amazon Resource Names (ARNs)
and input
parameters.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_update_automation_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_automation_rules)

```python
# batch_update_automation_rules method definition

await def batch_update_automation_rules(
    self,
    *,
    UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef],  # (1)
) -> BatchUpdateAutomationRulesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateAutomationRulesRequestItemTypeDef](./type_defs.md#updateautomationrulesrequestitemtypedef) 
2. See [:material-code-braces: BatchUpdateAutomationRulesResponseTypeDef](./type_defs.md#batchupdateautomationrulesresponsetypedef) 


```python
# batch_update_automation_rules method usage example with argument unpacking

kwargs: BatchUpdateAutomationRulesRequestRequestTypeDef = {  # (1)
    "UpdateAutomationRulesRequestItems": ...,
}

parent.batch_update_automation_rules(**kwargs)
```

1. See [:material-code-braces: BatchUpdateAutomationRulesRequestRequestTypeDef](./type_defs.md#batchupdateautomationrulesrequestrequesttypedef) 

### batch\_update\_findings

Used by Security Hub customers to update information about their investigation
into a
finding.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_update_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_findings)

```python
# batch_update_findings method definition

await def batch_update_findings(
    self,
    *,
    FindingIdentifiers: Sequence[AwsSecurityFindingIdentifierTypeDef],  # (1)
    Note: NoteUpdateTypeDef = ...,  # (2)
    Severity: SeverityUpdateTypeDef = ...,  # (3)
    VerificationState: VerificationStateType = ...,  # (4)
    Confidence: int = ...,
    Criticality: int = ...,
    Types: Sequence[str] = ...,
    UserDefinedFields: Mapping[str, str] = ...,
    Workflow: WorkflowUpdateTypeDef = ...,  # (5)
    RelatedFindings: Sequence[RelatedFindingTypeDef] = ...,  # (6)
) -> BatchUpdateFindingsResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
2. See [:material-code-braces: NoteUpdateTypeDef](./type_defs.md#noteupdatetypedef) 
3. See [:material-code-braces: SeverityUpdateTypeDef](./type_defs.md#severityupdatetypedef) 
4. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
5. See [:material-code-braces: WorkflowUpdateTypeDef](./type_defs.md#workflowupdatetypedef) 
6. See [:material-code-braces: RelatedFindingTypeDef](./type_defs.md#relatedfindingtypedef) 
7. See [:material-code-braces: BatchUpdateFindingsResponseTypeDef](./type_defs.md#batchupdatefindingsresponsetypedef) 


```python
# batch_update_findings method usage example with argument unpacking

kwargs: BatchUpdateFindingsRequestRequestTypeDef = {  # (1)
    "FindingIdentifiers": ...,
}

parent.batch_update_findings(**kwargs)
```

1. See [:material-code-braces: BatchUpdateFindingsRequestRequestTypeDef](./type_defs.md#batchupdatefindingsrequestrequesttypedef) 

### batch\_update\_standards\_control\_associations

For a batch of security controls and standards, this operation updates the
enablement status of a control in a
standard.

Type annotations and code completion for `#!python session.create_client("securityhub").batch_update_standards_control_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_standards_control_associations)

```python
# batch_update_standards_control_associations method definition

await def batch_update_standards_control_associations(
    self,
    *,
    StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef],  # (1)
) -> BatchUpdateStandardsControlAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StandardsControlAssociationUpdateTypeDef](./type_defs.md#standardscontrolassociationupdatetypedef) 
2. See [:material-code-braces: BatchUpdateStandardsControlAssociationsResponseTypeDef](./type_defs.md#batchupdatestandardscontrolassociationsresponsetypedef) 


```python
# batch_update_standards_control_associations method usage example with argument unpacking

kwargs: BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = {  # (1)
    "StandardsControlAssociationUpdates": ...,
}

parent.batch_update_standards_control_associations(**kwargs)
```

1. See [:material-code-braces: BatchUpdateStandardsControlAssociationsRequestRequestTypeDef](./type_defs.md#batchupdatestandardscontrolassociationsrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("securityhub").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("securityhub").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_action\_target

Creates a custom action target in Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").create_action_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_action_target)

```python
# create_action_target method definition

await def create_action_target(
    self,
    *,
    Name: str,
    Description: str,
    Id: str,
) -> CreateActionTargetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateActionTargetResponseTypeDef](./type_defs.md#createactiontargetresponsetypedef) 


```python
# create_action_target method usage example with argument unpacking

kwargs: CreateActionTargetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Description": ...,
    "Id": ...,
}

parent.create_action_target(**kwargs)
```

1. See [:material-code-braces: CreateActionTargetRequestRequestTypeDef](./type_defs.md#createactiontargetrequestrequesttypedef) 

### create\_automation\_rule

Creates an automation rule based on input parameters.

Type annotations and code completion for `#!python session.create_client("securityhub").create_automation_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_automation_rule)

```python
# create_automation_rule method definition

await def create_automation_rule(
    self,
    *,
    RuleOrder: int,
    RuleName: str,
    Description: str,
    Criteria: AutomationRulesFindingFiltersTypeDef,  # (1)
    Actions: Sequence[AutomationRulesActionUnionTypeDef],  # (2)
    Tags: Mapping[str, str] = ...,
    RuleStatus: RuleStatusType = ...,  # (3)
    IsTerminal: bool = ...,
) -> CreateAutomationRuleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AutomationRulesFindingFiltersTypeDef](./type_defs.md#automationrulesfindingfilterstypedef) 
2. See [:material-code-braces: AutomationRulesActionTypeDef](./type_defs.md#automationrulesactiontypedef) [:material-code-braces: AutomationRulesActionOutputTypeDef](./type_defs.md#automationrulesactionoutputtypedef) 
3. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
4. See [:material-code-braces: CreateAutomationRuleResponseTypeDef](./type_defs.md#createautomationruleresponsetypedef) 


```python
# create_automation_rule method usage example with argument unpacking

kwargs: CreateAutomationRuleRequestRequestTypeDef = {  # (1)
    "RuleOrder": ...,
    "RuleName": ...,
    "Description": ...,
    "Criteria": ...,
    "Actions": ...,
}

parent.create_automation_rule(**kwargs)
```

1. See [:material-code-braces: CreateAutomationRuleRequestRequestTypeDef](./type_defs.md#createautomationrulerequestrequesttypedef) 

### create\_configuration\_policy

Creates a configuration policy with the defined configuration.

Type annotations and code completion for `#!python session.create_client("securityhub").create_configuration_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_configuration_policy)

```python
# create_configuration_policy method definition

await def create_configuration_policy(
    self,
    *,
    Name: str,
    ConfigurationPolicy: PolicyTypeDef,  # (1)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateConfigurationPolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: CreateConfigurationPolicyResponseTypeDef](./type_defs.md#createconfigurationpolicyresponsetypedef) 


```python
# create_configuration_policy method usage example with argument unpacking

kwargs: CreateConfigurationPolicyRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ConfigurationPolicy": ...,
}

parent.create_configuration_policy(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationPolicyRequestRequestTypeDef](./type_defs.md#createconfigurationpolicyrequestrequesttypedef) 

### create\_finding\_aggregator

.

Type annotations and code completion for `#!python session.create_client("securityhub").create_finding_aggregator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)

```python
# create_finding_aggregator method definition

await def create_finding_aggregator(
    self,
    *,
    RegionLinkingMode: str,
    Regions: Sequence[str] = ...,
) -> CreateFindingAggregatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateFindingAggregatorResponseTypeDef](./type_defs.md#createfindingaggregatorresponsetypedef) 


```python
# create_finding_aggregator method usage example with argument unpacking

kwargs: CreateFindingAggregatorRequestRequestTypeDef = {  # (1)
    "RegionLinkingMode": ...,
}

parent.create_finding_aggregator(**kwargs)
```

1. See [:material-code-braces: CreateFindingAggregatorRequestRequestTypeDef](./type_defs.md#createfindingaggregatorrequestrequesttypedef) 

### create\_insight

Creates a custom insight in Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").create_insight` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)

```python
# create_insight method definition

await def create_insight(
    self,
    *,
    Name: str,
    Filters: AwsSecurityFindingFiltersTypeDef,  # (1)
    GroupByAttribute: str,
) -> CreateInsightResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
2. See [:material-code-braces: CreateInsightResponseTypeDef](./type_defs.md#createinsightresponsetypedef) 


```python
# create_insight method usage example with argument unpacking

kwargs: CreateInsightRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Filters": ...,
    "GroupByAttribute": ...,
}

parent.create_insight(**kwargs)
```

1. See [:material-code-braces: CreateInsightRequestRequestTypeDef](./type_defs.md#createinsightrequestrequesttypedef) 

### create\_members

Creates a member association in Security Hub between the specified accounts and
the account used to make the request, which is the administrator
account.

Type annotations and code completion for `#!python session.create_client("securityhub").create_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_members)

```python
# create_members method definition

await def create_members(
    self,
    *,
    AccountDetails: Sequence[AccountDetailsTypeDef],  # (1)
) -> CreateMembersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AccountDetailsTypeDef](./type_defs.md#accountdetailstypedef) 
2. See [:material-code-braces: CreateMembersResponseTypeDef](./type_defs.md#createmembersresponsetypedef) 


```python
# create_members method usage example with argument unpacking

kwargs: CreateMembersRequestRequestTypeDef = {  # (1)
    "AccountDetails": ...,
}

parent.create_members(**kwargs)
```

1. See [:material-code-braces: CreateMembersRequestRequestTypeDef](./type_defs.md#createmembersrequestrequesttypedef) 

### decline\_invitations

.

Type annotations and code completion for `#!python session.create_client("securityhub").decline_invitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.decline_invitations)

```python
# decline_invitations method definition

await def decline_invitations(
    self,
    *,
    AccountIds: Sequence[str],
) -> DeclineInvitationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeclineInvitationsResponseTypeDef](./type_defs.md#declineinvitationsresponsetypedef) 


```python
# decline_invitations method usage example with argument unpacking

kwargs: DeclineInvitationsRequestRequestTypeDef = {  # (1)
    "AccountIds": ...,
}

parent.decline_invitations(**kwargs)
```

1. See [:material-code-braces: DeclineInvitationsRequestRequestTypeDef](./type_defs.md#declineinvitationsrequestrequesttypedef) 

### delete\_action\_target

Deletes a custom action target from Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").delete_action_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_action_target)

```python
# delete_action_target method definition

await def delete_action_target(
    self,
    *,
    ActionTargetArn: str,
) -> DeleteActionTargetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteActionTargetResponseTypeDef](./type_defs.md#deleteactiontargetresponsetypedef) 


```python
# delete_action_target method usage example with argument unpacking

kwargs: DeleteActionTargetRequestRequestTypeDef = {  # (1)
    "ActionTargetArn": ...,
}

parent.delete_action_target(**kwargs)
```

1. See [:material-code-braces: DeleteActionTargetRequestRequestTypeDef](./type_defs.md#deleteactiontargetrequestrequesttypedef) 

### delete\_configuration\_policy

Deletes a configuration policy.

Type annotations and code completion for `#!python session.create_client("securityhub").delete_configuration_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_configuration_policy)

```python
# delete_configuration_policy method definition

await def delete_configuration_policy(
    self,
    *,
    Identifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_configuration_policy method usage example with argument unpacking

kwargs: DeleteConfigurationPolicyRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_configuration_policy(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationPolicyRequestRequestTypeDef](./type_defs.md#deleteconfigurationpolicyrequestrequesttypedef) 

### delete\_finding\_aggregator

.

Type annotations and code completion for `#!python session.create_client("securityhub").delete_finding_aggregator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_finding_aggregator)

```python
# delete_finding_aggregator method definition

await def delete_finding_aggregator(
    self,
    *,
    FindingAggregatorArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_finding_aggregator method usage example with argument unpacking

kwargs: DeleteFindingAggregatorRequestRequestTypeDef = {  # (1)
    "FindingAggregatorArn": ...,
}

parent.delete_finding_aggregator(**kwargs)
```

1. See [:material-code-braces: DeleteFindingAggregatorRequestRequestTypeDef](./type_defs.md#deletefindingaggregatorrequestrequesttypedef) 

### delete\_insight

Deletes the insight specified by the `InsightArn`.

Type annotations and code completion for `#!python session.create_client("securityhub").delete_insight` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_insight)

```python
# delete_insight method definition

await def delete_insight(
    self,
    *,
    InsightArn: str,
) -> DeleteInsightResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInsightResponseTypeDef](./type_defs.md#deleteinsightresponsetypedef) 


```python
# delete_insight method usage example with argument unpacking

kwargs: DeleteInsightRequestRequestTypeDef = {  # (1)
    "InsightArn": ...,
}

parent.delete_insight(**kwargs)
```

1. See [:material-code-braces: DeleteInsightRequestRequestTypeDef](./type_defs.md#deleteinsightrequestrequesttypedef) 

### delete\_invitations

.

Type annotations and code completion for `#!python session.create_client("securityhub").delete_invitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_invitations)

```python
# delete_invitations method definition

await def delete_invitations(
    self,
    *,
    AccountIds: Sequence[str],
) -> DeleteInvitationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInvitationsResponseTypeDef](./type_defs.md#deleteinvitationsresponsetypedef) 


```python
# delete_invitations method usage example with argument unpacking

kwargs: DeleteInvitationsRequestRequestTypeDef = {  # (1)
    "AccountIds": ...,
}

parent.delete_invitations(**kwargs)
```

1. See [:material-code-braces: DeleteInvitationsRequestRequestTypeDef](./type_defs.md#deleteinvitationsrequestrequesttypedef) 

### delete\_members

Deletes the specified member accounts from Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").delete_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_members)

```python
# delete_members method definition

await def delete_members(
    self,
    *,
    AccountIds: Sequence[str],
) -> DeleteMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMembersResponseTypeDef](./type_defs.md#deletemembersresponsetypedef) 


```python
# delete_members method usage example with argument unpacking

kwargs: DeleteMembersRequestRequestTypeDef = {  # (1)
    "AccountIds": ...,
}

parent.delete_members(**kwargs)
```

1. See [:material-code-braces: DeleteMembersRequestRequestTypeDef](./type_defs.md#deletemembersrequestrequesttypedef) 

### describe\_action\_targets

Returns a list of the custom action targets in Security Hub in your account.

Type annotations and code completion for `#!python session.create_client("securityhub").describe_action_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.describe_action_targets)

```python
# describe_action_targets method definition

await def describe_action_targets(
    self,
    *,
    ActionTargetArns: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeActionTargetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef) 


```python
# describe_action_targets method usage example with argument unpacking

kwargs: DescribeActionTargetsRequestRequestTypeDef = {  # (1)
    "ActionTargetArns": ...,
}

parent.describe_action_targets(**kwargs)
```

1. See [:material-code-braces: DescribeActionTargetsRequestRequestTypeDef](./type_defs.md#describeactiontargetsrequestrequesttypedef) 

### describe\_hub

Returns details about the Hub resource in your account, including the `HubArn`
and the time when you enabled Security
Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").describe_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.describe_hub)

```python
# describe_hub method definition

await def describe_hub(
    self,
    *,
    HubArn: str = ...,
) -> DescribeHubResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHubResponseTypeDef](./type_defs.md#describehubresponsetypedef) 


```python
# describe_hub method usage example with argument unpacking

kwargs: DescribeHubRequestRequestTypeDef = {  # (1)
    "HubArn": ...,
}

parent.describe_hub(**kwargs)
```

1. See [:material-code-braces: DescribeHubRequestRequestTypeDef](./type_defs.md#describehubrequestrequesttypedef) 

### describe\_organization\_configuration

Returns information about the way your organization is configured in Security
Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").describe_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.describe_organization_configuration)

```python
# describe_organization_configuration method definition

await def describe_organization_configuration(
    self,
) -> DescribeOrganizationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef) 

### describe\_products

Returns information about product integrations in Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").describe_products` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.describe_products)

```python
# describe_products method definition

await def describe_products(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    ProductArn: str = ...,
) -> DescribeProductsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProductsResponseTypeDef](./type_defs.md#describeproductsresponsetypedef) 


```python
# describe_products method usage example with argument unpacking

kwargs: DescribeProductsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_products(**kwargs)
```

1. See [:material-code-braces: DescribeProductsRequestRequestTypeDef](./type_defs.md#describeproductsrequestrequesttypedef) 

### describe\_standards

Returns a list of the available standards in Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").describe_standards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.describe_standards)

```python
# describe_standards method definition

await def describe_standards(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeStandardsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStandardsResponseTypeDef](./type_defs.md#describestandardsresponsetypedef) 


```python
# describe_standards method usage example with argument unpacking

kwargs: DescribeStandardsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_standards(**kwargs)
```

1. See [:material-code-braces: DescribeStandardsRequestRequestTypeDef](./type_defs.md#describestandardsrequestrequesttypedef) 

### describe\_standards\_controls

Returns a list of security standards controls.

Type annotations and code completion for `#!python session.create_client("securityhub").describe_standards_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.describe_standards_controls)

```python
# describe_standards_controls method definition

await def describe_standards_controls(
    self,
    *,
    StandardsSubscriptionArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeStandardsControlsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStandardsControlsResponseTypeDef](./type_defs.md#describestandardscontrolsresponsetypedef) 


```python
# describe_standards_controls method usage example with argument unpacking

kwargs: DescribeStandardsControlsRequestRequestTypeDef = {  # (1)
    "StandardsSubscriptionArn": ...,
}

parent.describe_standards_controls(**kwargs)
```

1. See [:material-code-braces: DescribeStandardsControlsRequestRequestTypeDef](./type_defs.md#describestandardscontrolsrequestrequesttypedef) 

### disable\_import\_findings\_for\_product

Disables the integration of the specified product with Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").disable_import_findings_for_product` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.disable_import_findings_for_product)

```python
# disable_import_findings_for_product method definition

await def disable_import_findings_for_product(
    self,
    *,
    ProductSubscriptionArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disable_import_findings_for_product method usage example with argument unpacking

kwargs: DisableImportFindingsForProductRequestRequestTypeDef = {  # (1)
    "ProductSubscriptionArn": ...,
}

parent.disable_import_findings_for_product(**kwargs)
```

1. See [:material-code-braces: DisableImportFindingsForProductRequestRequestTypeDef](./type_defs.md#disableimportfindingsforproductrequestrequesttypedef) 

### disable\_organization\_admin\_account

Disables a Security Hub administrator account.

Type annotations and code completion for `#!python session.create_client("securityhub").disable_organization_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.disable_organization_admin_account)

```python
# disable_organization_admin_account method definition

await def disable_organization_admin_account(
    self,
    *,
    AdminAccountId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disable_organization_admin_account method usage example with argument unpacking

kwargs: DisableOrganizationAdminAccountRequestRequestTypeDef = {  # (1)
    "AdminAccountId": ...,
}

parent.disable_organization_admin_account(**kwargs)
```

1. See [:material-code-braces: DisableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#disableorganizationadminaccountrequestrequesttypedef) 

### disable\_security\_hub

Disables Security Hub in your account only in the current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("securityhub").disable_security_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.disable_security_hub)

```python
# disable_security_hub method definition

await def disable_security_hub(
    self,
) -> Dict[str, Any]:
    ...
```


### disassociate\_from\_administrator\_account

Disassociates the current Security Hub member account from the associated
administrator
account.

Type annotations and code completion for `#!python session.create_client("securityhub").disassociate_from_administrator_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.disassociate_from_administrator_account)

```python
# disassociate_from_administrator_account method definition

await def disassociate_from_administrator_account(
    self,
) -> Dict[str, Any]:
    ...
```


### disassociate\_from\_master\_account

This method is deprecated.

Type annotations and code completion for `#!python session.create_client("securityhub").disassociate_from_master_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.disassociate_from_master_account)

```python
# disassociate_from_master_account method definition

await def disassociate_from_master_account(
    self,
) -> Dict[str, Any]:
    ...
```


### disassociate\_members

Disassociates the specified member accounts from the associated administrator
account.

Type annotations and code completion for `#!python session.create_client("securityhub").disassociate_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.disassociate_members)

```python
# disassociate_members method definition

await def disassociate_members(
    self,
    *,
    AccountIds: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_members method usage example with argument unpacking

kwargs: DisassociateMembersRequestRequestTypeDef = {  # (1)
    "AccountIds": ...,
}

parent.disassociate_members(**kwargs)
```

1. See [:material-code-braces: DisassociateMembersRequestRequestTypeDef](./type_defs.md#disassociatemembersrequestrequesttypedef) 

### enable\_import\_findings\_for\_product

Enables the integration of a partner product with Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").enable_import_findings_for_product` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_import_findings_for_product)

```python
# enable_import_findings_for_product method definition

await def enable_import_findings_for_product(
    self,
    *,
    ProductArn: str,
) -> EnableImportFindingsForProductResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnableImportFindingsForProductResponseTypeDef](./type_defs.md#enableimportfindingsforproductresponsetypedef) 


```python
# enable_import_findings_for_product method usage example with argument unpacking

kwargs: EnableImportFindingsForProductRequestRequestTypeDef = {  # (1)
    "ProductArn": ...,
}

parent.enable_import_findings_for_product(**kwargs)
```

1. See [:material-code-braces: EnableImportFindingsForProductRequestRequestTypeDef](./type_defs.md#enableimportfindingsforproductrequestrequesttypedef) 

### enable\_organization\_admin\_account

Designates the Security Hub administrator account for an organization.

Type annotations and code completion for `#!python session.create_client("securityhub").enable_organization_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_organization_admin_account)

```python
# enable_organization_admin_account method definition

await def enable_organization_admin_account(
    self,
    *,
    AdminAccountId: str,
) -> Dict[str, Any]:
    ...
```



```python
# enable_organization_admin_account method usage example with argument unpacking

kwargs: EnableOrganizationAdminAccountRequestRequestTypeDef = {  # (1)
    "AdminAccountId": ...,
}

parent.enable_organization_admin_account(**kwargs)
```

1. See [:material-code-braces: EnableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#enableorganizationadminaccountrequestrequesttypedef) 

### enable\_security\_hub

Enables Security Hub for your account in the current Region or the Region you
specify in the
request.

Type annotations and code completion for `#!python session.create_client("securityhub").enable_security_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_security_hub)

```python
# enable_security_hub method definition

await def enable_security_hub(
    self,
    *,
    Tags: Mapping[str, str] = ...,
    EnableDefaultStandards: bool = ...,
    ControlFindingGenerator: ControlFindingGeneratorType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ControlFindingGeneratorType](./literals.md#controlfindinggeneratortype) 


```python
# enable_security_hub method usage example with argument unpacking

kwargs: EnableSecurityHubRequestRequestTypeDef = {  # (1)
    "Tags": ...,
}

parent.enable_security_hub(**kwargs)
```

1. See [:material-code-braces: EnableSecurityHubRequestRequestTypeDef](./type_defs.md#enablesecurityhubrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("securityhub").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.generate_presigned_url)

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


### get\_administrator\_account

Provides the details for the Security Hub administrator account for the current
member
account.

Type annotations and code completion for `#!python session.create_client("securityhub").get_administrator_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_administrator_account)

```python
# get_administrator_account method definition

await def get_administrator_account(
    self,
) -> GetAdministratorAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAdministratorAccountResponseTypeDef](./type_defs.md#getadministratoraccountresponsetypedef) 

### get\_configuration\_policy

Provides information about a configuration policy.

Type annotations and code completion for `#!python session.create_client("securityhub").get_configuration_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_configuration_policy)

```python
# get_configuration_policy method definition

await def get_configuration_policy(
    self,
    *,
    Identifier: str,
) -> GetConfigurationPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfigurationPolicyResponseTypeDef](./type_defs.md#getconfigurationpolicyresponsetypedef) 


```python
# get_configuration_policy method usage example with argument unpacking

kwargs: GetConfigurationPolicyRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_configuration_policy(**kwargs)
```

1. See [:material-code-braces: GetConfigurationPolicyRequestRequestTypeDef](./type_defs.md#getconfigurationpolicyrequestrequesttypedef) 

### get\_configuration\_policy\_association

Returns the association between a configuration and a target account,
organizational unit, or the
root.

Type annotations and code completion for `#!python session.create_client("securityhub").get_configuration_policy_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_configuration_policy_association)

```python
# get_configuration_policy_association method definition

await def get_configuration_policy_association(
    self,
    *,
    Target: TargetTypeDef,  # (1)
) -> GetConfigurationPolicyAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: GetConfigurationPolicyAssociationResponseTypeDef](./type_defs.md#getconfigurationpolicyassociationresponsetypedef) 


```python
# get_configuration_policy_association method usage example with argument unpacking

kwargs: GetConfigurationPolicyAssociationRequestRequestTypeDef = {  # (1)
    "Target": ...,
}

parent.get_configuration_policy_association(**kwargs)
```

1. See [:material-code-braces: GetConfigurationPolicyAssociationRequestRequestTypeDef](./type_defs.md#getconfigurationpolicyassociationrequestrequesttypedef) 

### get\_enabled\_standards

Returns a list of the standards that are currently enabled.

Type annotations and code completion for `#!python session.create_client("securityhub").get_enabled_standards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_enabled_standards)

```python
# get_enabled_standards method definition

await def get_enabled_standards(
    self,
    *,
    StandardsSubscriptionArns: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetEnabledStandardsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnabledStandardsResponseTypeDef](./type_defs.md#getenabledstandardsresponsetypedef) 


```python
# get_enabled_standards method usage example with argument unpacking

kwargs: GetEnabledStandardsRequestRequestTypeDef = {  # (1)
    "StandardsSubscriptionArns": ...,
}

parent.get_enabled_standards(**kwargs)
```

1. See [:material-code-braces: GetEnabledStandardsRequestRequestTypeDef](./type_defs.md#getenabledstandardsrequestrequesttypedef) 

### get\_finding\_aggregator

.

Type annotations and code completion for `#!python session.create_client("securityhub").get_finding_aggregator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_aggregator)

```python
# get_finding_aggregator method definition

await def get_finding_aggregator(
    self,
    *,
    FindingAggregatorArn: str,
) -> GetFindingAggregatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFindingAggregatorResponseTypeDef](./type_defs.md#getfindingaggregatorresponsetypedef) 


```python
# get_finding_aggregator method usage example with argument unpacking

kwargs: GetFindingAggregatorRequestRequestTypeDef = {  # (1)
    "FindingAggregatorArn": ...,
}

parent.get_finding_aggregator(**kwargs)
```

1. See [:material-code-braces: GetFindingAggregatorRequestRequestTypeDef](./type_defs.md#getfindingaggregatorrequestrequesttypedef) 

### get\_finding\_history

Returns history for a Security Hub finding in the last 90 days.

Type annotations and code completion for `#!python session.create_client("securityhub").get_finding_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)

```python
# get_finding_history method definition

await def get_finding_history(
    self,
    *,
    FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetFindingHistoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
2. See [:material-code-braces: GetFindingHistoryResponseTypeDef](./type_defs.md#getfindinghistoryresponsetypedef) 


```python
# get_finding_history method usage example with argument unpacking

kwargs: GetFindingHistoryRequestRequestTypeDef = {  # (1)
    "FindingIdentifier": ...,
}

parent.get_finding_history(**kwargs)
```

1. See [:material-code-braces: GetFindingHistoryRequestRequestTypeDef](./type_defs.md#getfindinghistoryrequestrequesttypedef) 

### get\_findings

Returns a list of findings that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("securityhub").get_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_findings)

```python
# get_findings method definition

await def get_findings(
    self,
    *,
    Filters: AwsSecurityFindingFiltersTypeDef = ...,  # (1)
    SortCriteria: Sequence[SortCriterionTypeDef] = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetFindingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
3. See [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


```python
# get_findings method usage example with argument unpacking

kwargs: GetFindingsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.get_findings(**kwargs)
```

1. See [:material-code-braces: GetFindingsRequestRequestTypeDef](./type_defs.md#getfindingsrequestrequesttypedef) 

### get\_insight\_results

Lists the results of the Security Hub insight specified by the insight ARN.

Type annotations and code completion for `#!python session.create_client("securityhub").get_insight_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_insight_results)

```python
# get_insight_results method definition

await def get_insight_results(
    self,
    *,
    InsightArn: str,
) -> GetInsightResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightResultsResponseTypeDef](./type_defs.md#getinsightresultsresponsetypedef) 


```python
# get_insight_results method usage example with argument unpacking

kwargs: GetInsightResultsRequestRequestTypeDef = {  # (1)
    "InsightArn": ...,
}

parent.get_insight_results(**kwargs)
```

1. See [:material-code-braces: GetInsightResultsRequestRequestTypeDef](./type_defs.md#getinsightresultsrequestrequesttypedef) 

### get\_insights

Lists and describes insights for the specified insight ARNs.

Type annotations and code completion for `#!python session.create_client("securityhub").get_insights` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_insights)

```python
# get_insights method definition

await def get_insights(
    self,
    *,
    InsightArns: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetInsightsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightsResponseTypeDef](./type_defs.md#getinsightsresponsetypedef) 


```python
# get_insights method usage example with argument unpacking

kwargs: GetInsightsRequestRequestTypeDef = {  # (1)
    "InsightArns": ...,
}

parent.get_insights(**kwargs)
```

1. See [:material-code-braces: GetInsightsRequestRequestTypeDef](./type_defs.md#getinsightsrequestrequesttypedef) 

### get\_invitations\_count

.

Type annotations and code completion for `#!python session.create_client("securityhub").get_invitations_count` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_invitations_count)

```python
# get_invitations_count method definition

await def get_invitations_count(
    self,
) -> GetInvitationsCountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInvitationsCountResponseTypeDef](./type_defs.md#getinvitationscountresponsetypedef) 

### get\_master\_account

This method is deprecated.

Type annotations and code completion for `#!python session.create_client("securityhub").get_master_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_master_account)

```python
# get_master_account method definition

await def get_master_account(
    self,
) -> GetMasterAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMasterAccountResponseTypeDef](./type_defs.md#getmasteraccountresponsetypedef) 

### get\_members

Returns the details for the Security Hub member accounts for the specified
account
IDs.

Type annotations and code completion for `#!python session.create_client("securityhub").get_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_members)

```python
# get_members method definition

await def get_members(
    self,
    *,
    AccountIds: Sequence[str],
) -> GetMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMembersResponseTypeDef](./type_defs.md#getmembersresponsetypedef) 


```python
# get_members method usage example with argument unpacking

kwargs: GetMembersRequestRequestTypeDef = {  # (1)
    "AccountIds": ...,
}

parent.get_members(**kwargs)
```

1. See [:material-code-braces: GetMembersRequestRequestTypeDef](./type_defs.md#getmembersrequestrequesttypedef) 

### get\_security\_control\_definition

Retrieves the definition of a security control.

Type annotations and code completion for `#!python session.create_client("securityhub").get_security_control_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_security_control_definition)

```python
# get_security_control_definition method definition

await def get_security_control_definition(
    self,
    *,
    SecurityControlId: str,
) -> GetSecurityControlDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSecurityControlDefinitionResponseTypeDef](./type_defs.md#getsecuritycontroldefinitionresponsetypedef) 


```python
# get_security_control_definition method usage example with argument unpacking

kwargs: GetSecurityControlDefinitionRequestRequestTypeDef = {  # (1)
    "SecurityControlId": ...,
}

parent.get_security_control_definition(**kwargs)
```

1. See [:material-code-braces: GetSecurityControlDefinitionRequestRequestTypeDef](./type_defs.md#getsecuritycontroldefinitionrequestrequesttypedef) 

### invite\_members

.

Type annotations and code completion for `#!python session.create_client("securityhub").invite_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.invite_members)

```python
# invite_members method definition

await def invite_members(
    self,
    *,
    AccountIds: Sequence[str],
) -> InviteMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InviteMembersResponseTypeDef](./type_defs.md#invitemembersresponsetypedef) 


```python
# invite_members method usage example with argument unpacking

kwargs: InviteMembersRequestRequestTypeDef = {  # (1)
    "AccountIds": ...,
}

parent.invite_members(**kwargs)
```

1. See [:material-code-braces: InviteMembersRequestRequestTypeDef](./type_defs.md#invitemembersrequestrequesttypedef) 

### list\_automation\_rules

A list of automation rules and their metadata for the calling account.

Type annotations and code completion for `#!python session.create_client("securityhub").list_automation_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_automation_rules)

```python
# list_automation_rules method definition

await def list_automation_rules(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAutomationRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAutomationRulesResponseTypeDef](./type_defs.md#listautomationrulesresponsetypedef) 


```python
# list_automation_rules method usage example with argument unpacking

kwargs: ListAutomationRulesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_automation_rules(**kwargs)
```

1. See [:material-code-braces: ListAutomationRulesRequestRequestTypeDef](./type_defs.md#listautomationrulesrequestrequesttypedef) 

### list\_configuration\_policies

Lists the configuration policies that the Security Hub delegated administrator
has created for your
organization.

Type annotations and code completion for `#!python session.create_client("securityhub").list_configuration_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_configuration_policies)

```python
# list_configuration_policies method definition

await def list_configuration_policies(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListConfigurationPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfigurationPoliciesResponseTypeDef](./type_defs.md#listconfigurationpoliciesresponsetypedef) 


```python
# list_configuration_policies method usage example with argument unpacking

kwargs: ListConfigurationPoliciesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_configuration_policies(**kwargs)
```

1. See [:material-code-braces: ListConfigurationPoliciesRequestRequestTypeDef](./type_defs.md#listconfigurationpoliciesrequestrequesttypedef) 

### list\_configuration\_policy\_associations

Provides information about the associations for your configuration policies and
self-managed
behavior.

Type annotations and code completion for `#!python session.create_client("securityhub").list_configuration_policy_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_configuration_policy_associations)

```python
# list_configuration_policy_associations method definition

await def list_configuration_policy_associations(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: AssociationFiltersTypeDef = ...,  # (1)
) -> ListConfigurationPolicyAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssociationFiltersTypeDef](./type_defs.md#associationfilterstypedef) 
2. See [:material-code-braces: ListConfigurationPolicyAssociationsResponseTypeDef](./type_defs.md#listconfigurationpolicyassociationsresponsetypedef) 


```python
# list_configuration_policy_associations method usage example with argument unpacking

kwargs: ListConfigurationPolicyAssociationsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_configuration_policy_associations(**kwargs)
```

1. See [:material-code-braces: ListConfigurationPolicyAssociationsRequestRequestTypeDef](./type_defs.md#listconfigurationpolicyassociationsrequestrequesttypedef) 

### list\_enabled\_products\_for\_import

Lists all findings-generating solutions (products) that you are subscribed to
receive findings from in Security
Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").list_enabled_products_for_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_enabled_products_for_import)

```python
# list_enabled_products_for_import method definition

await def list_enabled_products_for_import(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEnabledProductsForImportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnabledProductsForImportResponseTypeDef](./type_defs.md#listenabledproductsforimportresponsetypedef) 


```python
# list_enabled_products_for_import method usage example with argument unpacking

kwargs: ListEnabledProductsForImportRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_enabled_products_for_import(**kwargs)
```

1. See [:material-code-braces: ListEnabledProductsForImportRequestRequestTypeDef](./type_defs.md#listenabledproductsforimportrequestrequesttypedef) 

### list\_finding\_aggregators

If cross-Region aggregation is enabled, then `ListFindingAggregators` returns
the Amazon Resource Name (ARN) of the finding
aggregator.

Type annotations and code completion for `#!python session.create_client("securityhub").list_finding_aggregators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_finding_aggregators)

```python
# list_finding_aggregators method definition

await def list_finding_aggregators(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFindingAggregatorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFindingAggregatorsResponseTypeDef](./type_defs.md#listfindingaggregatorsresponsetypedef) 


```python
# list_finding_aggregators method usage example with argument unpacking

kwargs: ListFindingAggregatorsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_finding_aggregators(**kwargs)
```

1. See [:material-code-braces: ListFindingAggregatorsRequestRequestTypeDef](./type_defs.md#listfindingaggregatorsrequestrequesttypedef) 

### list\_invitations

.

Type annotations and code completion for `#!python session.create_client("securityhub").list_invitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_invitations)

```python
# list_invitations method definition

await def list_invitations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInvitationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


```python
# list_invitations method usage example with argument unpacking

kwargs: ListInvitationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_invitations(**kwargs)
```

1. See [:material-code-braces: ListInvitationsRequestRequestTypeDef](./type_defs.md#listinvitationsrequestrequesttypedef) 

### list\_members

Lists details about all member accounts for the current Security Hub
administrator
account.

Type annotations and code completion for `#!python session.create_client("securityhub").list_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_members)

```python
# list_members method definition

await def list_members(
    self,
    *,
    OnlyAssociated: bool = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python
# list_members method usage example with argument unpacking

kwargs: ListMembersRequestRequestTypeDef = {  # (1)
    "OnlyAssociated": ...,
}

parent.list_members(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef) 

### list\_organization\_admin\_accounts

Lists the Security Hub administrator accounts.

Type annotations and code completion for `#!python session.create_client("securityhub").list_organization_admin_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_organization_admin_accounts)

```python
# list_organization_admin_accounts method definition

await def list_organization_admin_accounts(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOrganizationAdminAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


```python
# list_organization_admin_accounts method usage example with argument unpacking

kwargs: ListOrganizationAdminAccountsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_organization_admin_accounts(**kwargs)
```

1. See [:material-code-braces: ListOrganizationAdminAccountsRequestRequestTypeDef](./type_defs.md#listorganizationadminaccountsrequestrequesttypedef) 

### list\_security\_control\_definitions

Lists all of the security controls that apply to a specified standard.

Type annotations and code completion for `#!python session.create_client("securityhub").list_security_control_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_security_control_definitions)

```python
# list_security_control_definitions method definition

await def list_security_control_definitions(
    self,
    *,
    StandardsArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSecurityControlDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityControlDefinitionsResponseTypeDef](./type_defs.md#listsecuritycontroldefinitionsresponsetypedef) 


```python
# list_security_control_definitions method usage example with argument unpacking

kwargs: ListSecurityControlDefinitionsRequestRequestTypeDef = {  # (1)
    "StandardsArn": ...,
}

parent.list_security_control_definitions(**kwargs)
```

1. See [:material-code-braces: ListSecurityControlDefinitionsRequestRequestTypeDef](./type_defs.md#listsecuritycontroldefinitionsrequestrequesttypedef) 

### list\_standards\_control\_associations

Specifies whether a control is currently enabled or disabled in each enabled
standard in the calling
account.

Type annotations and code completion for `#!python session.create_client("securityhub").list_standards_control_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_standards_control_associations)

```python
# list_standards_control_associations method definition

await def list_standards_control_associations(
    self,
    *,
    SecurityControlId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListStandardsControlAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStandardsControlAssociationsResponseTypeDef](./type_defs.md#liststandardscontrolassociationsresponsetypedef) 


```python
# list_standards_control_associations method usage example with argument unpacking

kwargs: ListStandardsControlAssociationsRequestRequestTypeDef = {  # (1)
    "SecurityControlId": ...,
}

parent.list_standards_control_associations(**kwargs)
```

1. See [:material-code-braces: ListStandardsControlAssociationsRequestRequestTypeDef](./type_defs.md#liststandardscontrolassociationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags associated with a resource.

Type annotations and code completion for `#!python session.create_client("securityhub").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_tags_for_resource)

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

### start\_configuration\_policy\_association

Associates a target account, organizational unit, or the root with a specified
configuration.

Type annotations and code completion for `#!python session.create_client("securityhub").start_configuration_policy_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.start_configuration_policy_association)

```python
# start_configuration_policy_association method definition

await def start_configuration_policy_association(
    self,
    *,
    ConfigurationPolicyIdentifier: str,
    Target: TargetTypeDef,  # (1)
) -> StartConfigurationPolicyAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: StartConfigurationPolicyAssociationResponseTypeDef](./type_defs.md#startconfigurationpolicyassociationresponsetypedef) 


```python
# start_configuration_policy_association method usage example with argument unpacking

kwargs: StartConfigurationPolicyAssociationRequestRequestTypeDef = {  # (1)
    "ConfigurationPolicyIdentifier": ...,
    "Target": ...,
}

parent.start_configuration_policy_association(**kwargs)
```

1. See [:material-code-braces: StartConfigurationPolicyAssociationRequestRequestTypeDef](./type_defs.md#startconfigurationpolicyassociationrequestrequesttypedef) 

### start\_configuration\_policy\_disassociation

Disassociates a target account, organizational unit, or the root from a
specified
configuration.

Type annotations and code completion for `#!python session.create_client("securityhub").start_configuration_policy_disassociation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.start_configuration_policy_disassociation)

```python
# start_configuration_policy_disassociation method definition

await def start_configuration_policy_disassociation(
    self,
    *,
    ConfigurationPolicyIdentifier: str,
    Target: TargetTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 


```python
# start_configuration_policy_disassociation method usage example with argument unpacking

kwargs: StartConfigurationPolicyDisassociationRequestRequestTypeDef = {  # (1)
    "ConfigurationPolicyIdentifier": ...,
}

parent.start_configuration_policy_disassociation(**kwargs)
```

1. See [:material-code-braces: StartConfigurationPolicyDisassociationRequestRequestTypeDef](./type_defs.md#startconfigurationpolicydisassociationrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to a resource.

Type annotations and code completion for `#!python session.create_client("securityhub").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from a resource.

Type annotations and code completion for `#!python session.create_client("securityhub").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_action\_target

Updates the name and description of a custom action target in Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").update_action_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_action_target)

```python
# update_action_target method definition

await def update_action_target(
    self,
    *,
    ActionTargetArn: str,
    Name: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_action_target method usage example with argument unpacking

kwargs: UpdateActionTargetRequestRequestTypeDef = {  # (1)
    "ActionTargetArn": ...,
}

parent.update_action_target(**kwargs)
```

1. See [:material-code-braces: UpdateActionTargetRequestRequestTypeDef](./type_defs.md#updateactiontargetrequestrequesttypedef) 

### update\_configuration\_policy

Updates a configuration policy.

Type annotations and code completion for `#!python session.create_client("securityhub").update_configuration_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_configuration_policy)

```python
# update_configuration_policy method definition

await def update_configuration_policy(
    self,
    *,
    Identifier: str,
    Name: str = ...,
    Description: str = ...,
    UpdatedReason: str = ...,
    ConfigurationPolicy: PolicyTypeDef = ...,  # (1)
) -> UpdateConfigurationPolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: UpdateConfigurationPolicyResponseTypeDef](./type_defs.md#updateconfigurationpolicyresponsetypedef) 


```python
# update_configuration_policy method usage example with argument unpacking

kwargs: UpdateConfigurationPolicyRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_configuration_policy(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationPolicyRequestRequestTypeDef](./type_defs.md#updateconfigurationpolicyrequestrequesttypedef) 

### update\_finding\_aggregator

.

Type annotations and code completion for `#!python session.create_client("securityhub").update_finding_aggregator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)

```python
# update_finding_aggregator method definition

await def update_finding_aggregator(
    self,
    *,
    FindingAggregatorArn: str,
    RegionLinkingMode: str,
    Regions: Sequence[str] = ...,
) -> UpdateFindingAggregatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateFindingAggregatorResponseTypeDef](./type_defs.md#updatefindingaggregatorresponsetypedef) 


```python
# update_finding_aggregator method usage example with argument unpacking

kwargs: UpdateFindingAggregatorRequestRequestTypeDef = {  # (1)
    "FindingAggregatorArn": ...,
    "RegionLinkingMode": ...,
}

parent.update_finding_aggregator(**kwargs)
```

1. See [:material-code-braces: UpdateFindingAggregatorRequestRequestTypeDef](./type_defs.md#updatefindingaggregatorrequestrequesttypedef) 

### update\_findings

`UpdateFindings` is a deprecated operation.

Type annotations and code completion for `#!python session.create_client("securityhub").update_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)

```python
# update_findings method definition

await def update_findings(
    self,
    *,
    Filters: AwsSecurityFindingFiltersTypeDef,  # (1)
    Note: NoteUpdateTypeDef = ...,  # (2)
    RecordState: RecordStateType = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
2. See [:material-code-braces: NoteUpdateTypeDef](./type_defs.md#noteupdatetypedef) 
3. See [:material-code-brackets: RecordStateType](./literals.md#recordstatetype) 


```python
# update_findings method usage example with argument unpacking

kwargs: UpdateFindingsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.update_findings(**kwargs)
```

1. See [:material-code-braces: UpdateFindingsRequestRequestTypeDef](./type_defs.md#updatefindingsrequestrequesttypedef) 

### update\_insight

Updates the Security Hub insight identified by the specified insight ARN.

Type annotations and code completion for `#!python session.create_client("securityhub").update_insight` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)

```python
# update_insight method definition

await def update_insight(
    self,
    *,
    InsightArn: str,
    Name: str = ...,
    Filters: AwsSecurityFindingFiltersTypeDef = ...,  # (1)
    GroupByAttribute: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 


```python
# update_insight method usage example with argument unpacking

kwargs: UpdateInsightRequestRequestTypeDef = {  # (1)
    "InsightArn": ...,
}

parent.update_insight(**kwargs)
```

1. See [:material-code-braces: UpdateInsightRequestRequestTypeDef](./type_defs.md#updateinsightrequestrequesttypedef) 

### update\_organization\_configuration

Updates the configuration of your organization in Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").update_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_organization_configuration)

```python
# update_organization_configuration method definition

await def update_organization_configuration(
    self,
    *,
    AutoEnable: bool,
    AutoEnableStandards: AutoEnableStandardsType = ...,  # (1)
    OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AutoEnableStandardsType](./literals.md#autoenablestandardstype) 
2. See [:material-code-braces: OrganizationConfigurationTypeDef](./type_defs.md#organizationconfigurationtypedef) 


```python
# update_organization_configuration method usage example with argument unpacking

kwargs: UpdateOrganizationConfigurationRequestRequestTypeDef = {  # (1)
    "AutoEnable": ...,
}

parent.update_organization_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef) 

### update\_security\_control

Updates the properties of a security control.

Type annotations and code completion for `#!python session.create_client("securityhub").update_security_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_control)

```python
# update_security_control method definition

await def update_security_control(
    self,
    *,
    SecurityControlId: str,
    Parameters: Mapping[str, ParameterConfigurationUnionTypeDef],  # (1)
    LastUpdateReason: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ParameterConfigurationTypeDef](./type_defs.md#parameterconfigurationtypedef) [:material-code-braces: ParameterConfigurationOutputTypeDef](./type_defs.md#parameterconfigurationoutputtypedef) 


```python
# update_security_control method usage example with argument unpacking

kwargs: UpdateSecurityControlRequestRequestTypeDef = {  # (1)
    "SecurityControlId": ...,
    "Parameters": ...,
}

parent.update_security_control(**kwargs)
```

1. See [:material-code-braces: UpdateSecurityControlRequestRequestTypeDef](./type_defs.md#updatesecuritycontrolrequestrequesttypedef) 

### update\_security\_hub\_configuration

Updates configuration options for Security Hub.

Type annotations and code completion for `#!python session.create_client("securityhub").update_security_hub_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_hub_configuration)

```python
# update_security_hub_configuration method definition

await def update_security_hub_configuration(
    self,
    *,
    AutoEnableControls: bool = ...,
    ControlFindingGenerator: ControlFindingGeneratorType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ControlFindingGeneratorType](./literals.md#controlfindinggeneratortype) 


```python
# update_security_hub_configuration method usage example with argument unpacking

kwargs: UpdateSecurityHubConfigurationRequestRequestTypeDef = {  # (1)
    "AutoEnableControls": ...,
}

parent.update_security_hub_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateSecurityHubConfigurationRequestRequestTypeDef](./type_defs.md#updatesecurityhubconfigurationrequestrequesttypedef) 

### update\_standards\_control

Used to control whether an individual security standard control is enabled or
disabled.

Type annotations and code completion for `#!python session.create_client("securityhub").update_standards_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_standards_control)

```python
# update_standards_control method definition

await def update_standards_control(
    self,
    *,
    StandardsControlArn: str,
    ControlStatus: ControlStatusType = ...,  # (1)
    DisabledReason: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ControlStatusType](./literals.md#controlstatustype) 


```python
# update_standards_control method usage example with argument unpacking

kwargs: UpdateStandardsControlRequestRequestTypeDef = {  # (1)
    "StandardsControlArn": ...,
}

parent.update_standards_control(**kwargs)
```

1. See [:material-code-braces: UpdateStandardsControlRequestRequestTypeDef](./type_defs.md#updatestandardscontrolrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("securityhub").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SecurityHubClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("securityhub").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator` method with overloads.

- `client.get_paginator("describe_action_targets")` -> [DescribeActionTargetsPaginator](./paginators.md#describeactiontargetspaginator)
- `client.get_paginator("describe_products")` -> [DescribeProductsPaginator](./paginators.md#describeproductspaginator)
- `client.get_paginator("describe_standards")` -> [DescribeStandardsPaginator](./paginators.md#describestandardspaginator)
- `client.get_paginator("describe_standards_controls")` -> [DescribeStandardsControlsPaginator](./paginators.md#describestandardscontrolspaginator)
- `client.get_paginator("get_enabled_standards")` -> [GetEnabledStandardsPaginator](./paginators.md#getenabledstandardspaginator)
- `client.get_paginator("get_finding_history")` -> [GetFindingHistoryPaginator](./paginators.md#getfindinghistorypaginator)
- `client.get_paginator("get_findings")` -> [GetFindingsPaginator](./paginators.md#getfindingspaginator)
- `client.get_paginator("get_insights")` -> [GetInsightsPaginator](./paginators.md#getinsightspaginator)
- `client.get_paginator("list_configuration_policies")` -> [ListConfigurationPoliciesPaginator](./paginators.md#listconfigurationpoliciespaginator)
- `client.get_paginator("list_configuration_policy_associations")` -> [ListConfigurationPolicyAssociationsPaginator](./paginators.md#listconfigurationpolicyassociationspaginator)
- `client.get_paginator("list_enabled_products_for_import")` -> [ListEnabledProductsForImportPaginator](./paginators.md#listenabledproductsforimportpaginator)
- `client.get_paginator("list_finding_aggregators")` -> [ListFindingAggregatorsPaginator](./paginators.md#listfindingaggregatorspaginator)
- `client.get_paginator("list_invitations")` -> [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
- `client.get_paginator("list_members")` -> [ListMembersPaginator](./paginators.md#listmemberspaginator)
- `client.get_paginator("list_organization_admin_accounts")` -> [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
- `client.get_paginator("list_security_control_definitions")` -> [ListSecurityControlDefinitionsPaginator](./paginators.md#listsecuritycontroldefinitionspaginator)
- `client.get_paginator("list_standards_control_associations")` -> [ListStandardsControlAssociationsPaginator](./paginators.md#liststandardscontrolassociationspaginator)



