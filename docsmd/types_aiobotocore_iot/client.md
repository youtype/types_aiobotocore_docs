# IoTClient

> [Index](../README.md) > [IoT](./README.md) > IoTClient

!!! note ""

    Auto-generated documentation for [IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#iot)
    type annotations stubs module [types-aiobotocore-iot](https://pypi.org/project/types-aiobotocore-iot/).

## IoTClient

Type annotations and code completion for `#!python session.create_client("iot")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client)

```python
# IoTClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iot.client import IoTClient

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iot").exceptions` structure.

```python
# IoTClient.exceptions usage example

async with session.create_client("iot") as client:
    try:
        do_something(client)
    except (
            client.CertificateConflictException,
        client.CertificateStateException,
        client.CertificateValidationException,
        client.ClientError,
        client.ConflictException,
        client.ConflictingResourceUpdateException,
        client.DeleteConflictException,
        client.IndexNotReadyException,
        client.InternalException,
        client.InternalFailureException,
        client.InternalServerException,
        client.InvalidAggregationException,
        client.InvalidQueryException,
        client.InvalidRequestException,
        client.InvalidResponseException,
        client.InvalidStateTransitionException,
        client.LimitExceededException,
        client.MalformedPolicyException,
        client.NotConfiguredException,
        client.RegistrationCodeValidationException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ResourceRegistrationFailureException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
        client.SqlParseException,
        client.TaskAlreadyExistsException,
        client.ThrottlingException,
        client.TransferAlreadyCompletedException,
        client.TransferConflictException,
        client.UnauthorizedException,
        client.ValidationException,
        client.VersionConflictException,
        client.VersionsLimitExceededException,
    ) as e:
        print(e)
```

```python
# IoTClient usage type checking example

from types_aiobotocore_iot.client import Exceptions

def handle_error(exc: Exceptions.CertificateConflictException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iot").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iot").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/generate_presigned_url.html)

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


### accept\_certificate\_transfer

Accepts a pending certificate transfer.

Type annotations and code completion for `#!python session.create_client("iot").accept_certificate_transfer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/accept_certificate_transfer.html)

```python
# accept_certificate_transfer method definition

await def accept_certificate_transfer(
    self,
    *,
    certificateId: str,
    setAsActive: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# accept_certificate_transfer method usage example with argument unpacking

kwargs: AcceptCertificateTransferRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.accept_certificate_transfer(**kwargs)
```

1. See [:material-code-braces: AcceptCertificateTransferRequestRequestTypeDef](./type_defs.md#acceptcertificatetransferrequestrequesttypedef) 

### add\_thing\_to\_billing\_group

Adds a thing to a billing group.

Type annotations and code completion for `#!python session.create_client("iot").add_thing_to_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/add_thing_to_billing_group.html)

```python
# add_thing_to_billing_group method definition

await def add_thing_to_billing_group(
    self,
    *,
    billingGroupName: str = ...,
    billingGroupArn: str = ...,
    thingName: str = ...,
    thingArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# add_thing_to_billing_group method usage example with argument unpacking

kwargs: AddThingToBillingGroupRequestRequestTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.add_thing_to_billing_group(**kwargs)
```

1. See [:material-code-braces: AddThingToBillingGroupRequestRequestTypeDef](./type_defs.md#addthingtobillinggrouprequestrequesttypedef) 

### add\_thing\_to\_thing\_group

Adds a thing to a thing group.

Type annotations and code completion for `#!python session.create_client("iot").add_thing_to_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/add_thing_to_thing_group.html)

```python
# add_thing_to_thing_group method definition

await def add_thing_to_thing_group(
    self,
    *,
    thingGroupName: str = ...,
    thingGroupArn: str = ...,
    thingName: str = ...,
    thingArn: str = ...,
    overrideDynamicGroups: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# add_thing_to_thing_group method usage example with argument unpacking

kwargs: AddThingToThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.add_thing_to_thing_group(**kwargs)
```

1. See [:material-code-braces: AddThingToThingGroupRequestRequestTypeDef](./type_defs.md#addthingtothinggrouprequestrequesttypedef) 

### associate\_sbom\_with\_package\_version

Associates the selected software bill of materials (SBOM) with a specific
software package version.

Type annotations and code completion for `#!python session.create_client("iot").associate_sbom_with_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/associate_sbom_with_package_version.html)

```python
# associate_sbom_with_package_version method definition

await def associate_sbom_with_package_version(
    self,
    *,
    packageName: str,
    versionName: str,
    sbom: SbomTypeDef,  # (1)
    clientToken: str = ...,
) -> AssociateSbomWithPackageVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SbomTypeDef](./type_defs.md#sbomtypedef) 
2. See [:material-code-braces: AssociateSbomWithPackageVersionResponseTypeDef](./type_defs.md#associatesbomwithpackageversionresponsetypedef) 


```python
# associate_sbom_with_package_version method usage example with argument unpacking

kwargs: AssociateSbomWithPackageVersionRequestRequestTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
    "sbom": ...,
}

parent.associate_sbom_with_package_version(**kwargs)
```

1. See [:material-code-braces: AssociateSbomWithPackageVersionRequestRequestTypeDef](./type_defs.md#associatesbomwithpackageversionrequestrequesttypedef) 

### associate\_targets\_with\_job

Associates a group with a continuous job.

Type annotations and code completion for `#!python session.create_client("iot").associate_targets_with_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/associate_targets_with_job.html)

```python
# associate_targets_with_job method definition

await def associate_targets_with_job(
    self,
    *,
    targets: Sequence[str],
    jobId: str,
    comment: str = ...,
    namespaceId: str = ...,
) -> AssociateTargetsWithJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateTargetsWithJobResponseTypeDef](./type_defs.md#associatetargetswithjobresponsetypedef) 


```python
# associate_targets_with_job method usage example with argument unpacking

kwargs: AssociateTargetsWithJobRequestRequestTypeDef = {  # (1)
    "targets": ...,
    "jobId": ...,
}

parent.associate_targets_with_job(**kwargs)
```

1. See [:material-code-braces: AssociateTargetsWithJobRequestRequestTypeDef](./type_defs.md#associatetargetswithjobrequestrequesttypedef) 

### attach\_policy

Attaches the specified policy to the specified principal (certificate or other
credential).

Type annotations and code completion for `#!python session.create_client("iot").attach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/attach_policy.html)

```python
# attach_policy method definition

await def attach_policy(
    self,
    *,
    policyName: str,
    target: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# attach_policy method usage example with argument unpacking

kwargs: AttachPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "target": ...,
}

parent.attach_policy(**kwargs)
```

1. See [:material-code-braces: AttachPolicyRequestRequestTypeDef](./type_defs.md#attachpolicyrequestrequesttypedef) 

### attach\_principal\_policy

Attaches the specified policy to the specified principal (certificate or other
credential).

Type annotations and code completion for `#!python session.create_client("iot").attach_principal_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/attach_principal_policy.html)

```python
# attach_principal_policy method definition

await def attach_principal_policy(
    self,
    *,
    policyName: str,
    principal: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# attach_principal_policy method usage example with argument unpacking

kwargs: AttachPrincipalPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "principal": ...,
}

parent.attach_principal_policy(**kwargs)
```

1. See [:material-code-braces: AttachPrincipalPolicyRequestRequestTypeDef](./type_defs.md#attachprincipalpolicyrequestrequesttypedef) 

### attach\_security\_profile

Associates a Device Defender security profile with a thing group or this
account.

Type annotations and code completion for `#!python session.create_client("iot").attach_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/attach_security_profile.html)

```python
# attach_security_profile method definition

await def attach_security_profile(
    self,
    *,
    securityProfileName: str,
    securityProfileTargetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# attach_security_profile method usage example with argument unpacking

kwargs: AttachSecurityProfileRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
    "securityProfileTargetArn": ...,
}

parent.attach_security_profile(**kwargs)
```

1. See [:material-code-braces: AttachSecurityProfileRequestRequestTypeDef](./type_defs.md#attachsecurityprofilerequestrequesttypedef) 

### attach\_thing\_principal

Attaches the specified principal to the specified thing.

Type annotations and code completion for `#!python session.create_client("iot").attach_thing_principal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/attach_thing_principal.html)

```python
# attach_thing_principal method definition

await def attach_thing_principal(
    self,
    *,
    thingName: str,
    principal: str,
    thingPrincipalType: ThingPrincipalTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 


```python
# attach_thing_principal method usage example with argument unpacking

kwargs: AttachThingPrincipalRequestRequestTypeDef = {  # (1)
    "thingName": ...,
    "principal": ...,
}

parent.attach_thing_principal(**kwargs)
```

1. See [:material-code-braces: AttachThingPrincipalRequestRequestTypeDef](./type_defs.md#attachthingprincipalrequestrequesttypedef) 

### cancel\_audit\_mitigation\_actions\_task

Cancels a mitigation action task that is in progress.

Type annotations and code completion for `#!python session.create_client("iot").cancel_audit_mitigation_actions_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/cancel_audit_mitigation_actions_task.html)

```python
# cancel_audit_mitigation_actions_task method definition

await def cancel_audit_mitigation_actions_task(
    self,
    *,
    taskId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_audit_mitigation_actions_task method usage example with argument unpacking

kwargs: CancelAuditMitigationActionsTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.cancel_audit_mitigation_actions_task(**kwargs)
```

1. See [:material-code-braces: CancelAuditMitigationActionsTaskRequestRequestTypeDef](./type_defs.md#cancelauditmitigationactionstaskrequestrequesttypedef) 

### cancel\_audit\_task

Cancels an audit that is in progress.

Type annotations and code completion for `#!python session.create_client("iot").cancel_audit_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/cancel_audit_task.html)

```python
# cancel_audit_task method definition

await def cancel_audit_task(
    self,
    *,
    taskId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_audit_task method usage example with argument unpacking

kwargs: CancelAuditTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.cancel_audit_task(**kwargs)
```

1. See [:material-code-braces: CancelAuditTaskRequestRequestTypeDef](./type_defs.md#cancelaudittaskrequestrequesttypedef) 

### cancel\_certificate\_transfer

Cancels a pending transfer for the specified certificate.

Type annotations and code completion for `#!python session.create_client("iot").cancel_certificate_transfer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/cancel_certificate_transfer.html)

```python
# cancel_certificate_transfer method definition

await def cancel_certificate_transfer(
    self,
    *,
    certificateId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_certificate_transfer method usage example with argument unpacking

kwargs: CancelCertificateTransferRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.cancel_certificate_transfer(**kwargs)
```

1. See [:material-code-braces: CancelCertificateTransferRequestRequestTypeDef](./type_defs.md#cancelcertificatetransferrequestrequesttypedef) 

### cancel\_detect\_mitigation\_actions\_task

Cancels a Device Defender ML Detect mitigation action.

Type annotations and code completion for `#!python session.create_client("iot").cancel_detect_mitigation_actions_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/cancel_detect_mitigation_actions_task.html)

```python
# cancel_detect_mitigation_actions_task method definition

await def cancel_detect_mitigation_actions_task(
    self,
    *,
    taskId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_detect_mitigation_actions_task method usage example with argument unpacking

kwargs: CancelDetectMitigationActionsTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.cancel_detect_mitigation_actions_task(**kwargs)
```

1. See [:material-code-braces: CancelDetectMitigationActionsTaskRequestRequestTypeDef](./type_defs.md#canceldetectmitigationactionstaskrequestrequesttypedef) 

### cancel\_job

Cancels a job.

Type annotations and code completion for `#!python session.create_client("iot").cancel_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/cancel_job.html)

```python
# cancel_job method definition

await def cancel_job(
    self,
    *,
    jobId: str,
    reasonCode: str = ...,
    comment: str = ...,
    force: bool = ...,
) -> CancelJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJobResponseTypeDef](./type_defs.md#canceljobresponsetypedef) 


```python
# cancel_job method usage example with argument unpacking

kwargs: CancelJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef) 

### cancel\_job\_execution

Cancels the execution of a job for a given thing.

Type annotations and code completion for `#!python session.create_client("iot").cancel_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/cancel_job_execution.html)

```python
# cancel_job_execution method definition

await def cancel_job_execution(
    self,
    *,
    jobId: str,
    thingName: str,
    force: bool = ...,
    expectedVersion: int = ...,
    statusDetails: Mapping[str, str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_job_execution method usage example with argument unpacking

kwargs: CancelJobExecutionRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "thingName": ...,
}

parent.cancel_job_execution(**kwargs)
```

1. See [:material-code-braces: CancelJobExecutionRequestRequestTypeDef](./type_defs.md#canceljobexecutionrequestrequesttypedef) 

### clear\_default\_authorizer

Clears the default authorizer.

Type annotations and code completion for `#!python session.create_client("iot").clear_default_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/clear_default_authorizer.html)

```python
# clear_default_authorizer method definition

await def clear_default_authorizer(
    self,
) -> Dict[str, Any]:
    ...
```


### confirm\_topic\_rule\_destination

Confirms a topic rule destination.

Type annotations and code completion for `#!python session.create_client("iot").confirm_topic_rule_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/confirm_topic_rule_destination.html)

```python
# confirm_topic_rule_destination method definition

await def confirm_topic_rule_destination(
    self,
    *,
    confirmationToken: str,
) -> Dict[str, Any]:
    ...
```



```python
# confirm_topic_rule_destination method usage example with argument unpacking

kwargs: ConfirmTopicRuleDestinationRequestRequestTypeDef = {  # (1)
    "confirmationToken": ...,
}

parent.confirm_topic_rule_destination(**kwargs)
```

1. See [:material-code-braces: ConfirmTopicRuleDestinationRequestRequestTypeDef](./type_defs.md#confirmtopicruledestinationrequestrequesttypedef) 

### create\_audit\_suppression

Creates a Device Defender audit suppression.

Type annotations and code completion for `#!python session.create_client("iot").create_audit_suppression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_audit_suppression.html)

```python
# create_audit_suppression method definition

await def create_audit_suppression(
    self,
    *,
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
    clientRequestToken: str,
    expirationDate: TimestampTypeDef = ...,
    suppressIndefinitely: bool = ...,
    description: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 


```python
# create_audit_suppression method usage example with argument unpacking

kwargs: CreateAuditSuppressionRequestRequestTypeDef = {  # (1)
    "checkName": ...,
    "resourceIdentifier": ...,
    "clientRequestToken": ...,
}

parent.create_audit_suppression(**kwargs)
```

1. See [:material-code-braces: CreateAuditSuppressionRequestRequestTypeDef](./type_defs.md#createauditsuppressionrequestrequesttypedef) 

### create\_authorizer

Creates an authorizer.

Type annotations and code completion for `#!python session.create_client("iot").create_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_authorizer.html)

```python
# create_authorizer method definition

await def create_authorizer(
    self,
    *,
    authorizerName: str,
    authorizerFunctionArn: str,
    tokenKeyName: str = ...,
    tokenSigningPublicKeys: Mapping[str, str] = ...,
    status: AuthorizerStatusType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
    signingDisabled: bool = ...,
    enableCachingForHttp: bool = ...,
) -> CreateAuthorizerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateAuthorizerResponseTypeDef](./type_defs.md#createauthorizerresponsetypedef) 


```python
# create_authorizer method usage example with argument unpacking

kwargs: CreateAuthorizerRequestRequestTypeDef = {  # (1)
    "authorizerName": ...,
    "authorizerFunctionArn": ...,
}

parent.create_authorizer(**kwargs)
```

1. See [:material-code-braces: CreateAuthorizerRequestRequestTypeDef](./type_defs.md#createauthorizerrequestrequesttypedef) 

### create\_billing\_group

Creates a billing group.

Type annotations and code completion for `#!python session.create_client("iot").create_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_billing_group.html)

```python
# create_billing_group method definition

await def create_billing_group(
    self,
    *,
    billingGroupName: str,
    billingGroupProperties: BillingGroupPropertiesTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateBillingGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BillingGroupPropertiesTypeDef](./type_defs.md#billinggrouppropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateBillingGroupResponseTypeDef](./type_defs.md#createbillinggroupresponsetypedef) 


```python
# create_billing_group method usage example with argument unpacking

kwargs: CreateBillingGroupRequestRequestTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.create_billing_group(**kwargs)
```

1. See [:material-code-braces: CreateBillingGroupRequestRequestTypeDef](./type_defs.md#createbillinggrouprequestrequesttypedef) 

### create\_certificate\_from\_csr

Creates an X.509 certificate using the specified certificate signing request.

Type annotations and code completion for `#!python session.create_client("iot").create_certificate_from_csr` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_certificate_from_csr.html)

```python
# create_certificate_from_csr method definition

await def create_certificate_from_csr(
    self,
    *,
    certificateSigningRequest: str,
    setAsActive: bool = ...,
) -> CreateCertificateFromCsrResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateCertificateFromCsrResponseTypeDef](./type_defs.md#createcertificatefromcsrresponsetypedef) 


```python
# create_certificate_from_csr method usage example with argument unpacking

kwargs: CreateCertificateFromCsrRequestRequestTypeDef = {  # (1)
    "certificateSigningRequest": ...,
}

parent.create_certificate_from_csr(**kwargs)
```

1. See [:material-code-braces: CreateCertificateFromCsrRequestRequestTypeDef](./type_defs.md#createcertificatefromcsrrequestrequesttypedef) 

### create\_certificate\_provider

Creates an Amazon Web Services IoT Core certificate provider.

Type annotations and code completion for `#!python session.create_client("iot").create_certificate_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_certificate_provider.html)

```python
# create_certificate_provider method definition

await def create_certificate_provider(
    self,
    *,
    certificateProviderName: str,
    lambdaFunctionArn: str,
    accountDefaultForOperations: Sequence[CertificateProviderOperationType],  # (1)
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateCertificateProviderResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CertificateProviderOperationType](./literals.md#certificateprovideroperationtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateCertificateProviderResponseTypeDef](./type_defs.md#createcertificateproviderresponsetypedef) 


```python
# create_certificate_provider method usage example with argument unpacking

kwargs: CreateCertificateProviderRequestRequestTypeDef = {  # (1)
    "certificateProviderName": ...,
    "lambdaFunctionArn": ...,
    "accountDefaultForOperations": ...,
}

parent.create_certificate_provider(**kwargs)
```

1. See [:material-code-braces: CreateCertificateProviderRequestRequestTypeDef](./type_defs.md#createcertificateproviderrequestrequesttypedef) 

### create\_command

Creates a command.

Type annotations and code completion for `#!python session.create_client("iot").create_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_command.html)

```python
# create_command method definition

await def create_command(
    self,
    *,
    commandId: str,
    namespace: CommandNamespaceType = ...,  # (1)
    displayName: str = ...,
    description: str = ...,
    payload: CommandPayloadTypeDef = ...,  # (2)
    mandatoryParameters: Sequence[CommandParameterUnionTypeDef] = ...,  # (3)
    roleArn: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateCommandResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-braces: CommandPayloadTypeDef](./type_defs.md#commandpayloadtypedef) 
3. See [:material-code-braces: CommandParameterTypeDef](./type_defs.md#commandparametertypedef) [:material-code-braces: CommandParameterOutputTypeDef](./type_defs.md#commandparameteroutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateCommandResponseTypeDef](./type_defs.md#createcommandresponsetypedef) 


```python
# create_command method usage example with argument unpacking

kwargs: CreateCommandRequestRequestTypeDef = {  # (1)
    "commandId": ...,
}

parent.create_command(**kwargs)
```

1. See [:material-code-braces: CreateCommandRequestRequestTypeDef](./type_defs.md#createcommandrequestrequesttypedef) 

### create\_custom\_metric

Use this API to define a Custom Metric published by your devices to Device
Defender.

Type annotations and code completion for `#!python session.create_client("iot").create_custom_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_custom_metric.html)

```python
# create_custom_metric method definition

await def create_custom_metric(
    self,
    *,
    metricName: str,
    metricType: CustomMetricTypeType,  # (1)
    clientRequestToken: str,
    displayName: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateCustomMetricResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CustomMetricTypeType](./literals.md#custommetrictypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateCustomMetricResponseTypeDef](./type_defs.md#createcustommetricresponsetypedef) 


```python
# create_custom_metric method usage example with argument unpacking

kwargs: CreateCustomMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
    "metricType": ...,
    "clientRequestToken": ...,
}

parent.create_custom_metric(**kwargs)
```

1. See [:material-code-braces: CreateCustomMetricRequestRequestTypeDef](./type_defs.md#createcustommetricrequestrequesttypedef) 

### create\_dimension

Create a dimension that you can use to limit the scope of a metric used in a
security profile for IoT Device Defender.

Type annotations and code completion for `#!python session.create_client("iot").create_dimension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_dimension.html)

```python
# create_dimension method definition

await def create_dimension(
    self,
    *,
    name: str,
    type: DimensionTypeType,  # (1)
    stringValues: Sequence[str],
    clientRequestToken: str,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDimensionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DimensionTypeType](./literals.md#dimensiontypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDimensionResponseTypeDef](./type_defs.md#createdimensionresponsetypedef) 


```python
# create_dimension method usage example with argument unpacking

kwargs: CreateDimensionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "type": ...,
    "stringValues": ...,
    "clientRequestToken": ...,
}

parent.create_dimension(**kwargs)
```

1. See [:material-code-braces: CreateDimensionRequestRequestTypeDef](./type_defs.md#createdimensionrequestrequesttypedef) 

### create\_domain\_configuration

Creates a domain configuration.

Type annotations and code completion for `#!python session.create_client("iot").create_domain_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_domain_configuration.html)

```python
# create_domain_configuration method definition

await def create_domain_configuration(
    self,
    *,
    domainConfigurationName: str,
    domainName: str = ...,
    serverCertificateArns: Sequence[str] = ...,
    validationCertificateArn: str = ...,
    authorizerConfig: AuthorizerConfigTypeDef = ...,  # (1)
    serviceType: ServiceTypeType = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
    tlsConfig: TlsConfigTypeDef = ...,  # (4)
    serverCertificateConfig: ServerCertificateConfigTypeDef = ...,  # (5)
    authenticationType: AuthenticationTypeType = ...,  # (6)
    applicationProtocol: ApplicationProtocolType = ...,  # (7)
    clientCertificateConfig: ClientCertificateConfigTypeDef = ...,  # (8)
) -> CreateDomainConfigurationResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: AuthorizerConfigTypeDef](./type_defs.md#authorizerconfigtypedef) 
2. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
5. See [:material-code-braces: ServerCertificateConfigTypeDef](./type_defs.md#servercertificateconfigtypedef) 
6. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
7. See [:material-code-brackets: ApplicationProtocolType](./literals.md#applicationprotocoltype) 
8. See [:material-code-braces: ClientCertificateConfigTypeDef](./type_defs.md#clientcertificateconfigtypedef) 
9. See [:material-code-braces: CreateDomainConfigurationResponseTypeDef](./type_defs.md#createdomainconfigurationresponsetypedef) 


```python
# create_domain_configuration method usage example with argument unpacking

kwargs: CreateDomainConfigurationRequestRequestTypeDef = {  # (1)
    "domainConfigurationName": ...,
}

parent.create_domain_configuration(**kwargs)
```

1. See [:material-code-braces: CreateDomainConfigurationRequestRequestTypeDef](./type_defs.md#createdomainconfigurationrequestrequesttypedef) 

### create\_dynamic\_thing\_group

Creates a dynamic thing group.

Type annotations and code completion for `#!python session.create_client("iot").create_dynamic_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_dynamic_thing_group.html)

```python
# create_dynamic_thing_group method definition

await def create_dynamic_thing_group(
    self,
    *,
    thingGroupName: str,
    queryString: str,
    thingGroupProperties: ThingGroupPropertiesTypeDef = ...,  # (1)
    indexName: str = ...,
    queryVersion: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDynamicThingGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDynamicThingGroupResponseTypeDef](./type_defs.md#createdynamicthinggroupresponsetypedef) 


```python
# create_dynamic_thing_group method usage example with argument unpacking

kwargs: CreateDynamicThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
    "queryString": ...,
}

parent.create_dynamic_thing_group(**kwargs)
```

1. See [:material-code-braces: CreateDynamicThingGroupRequestRequestTypeDef](./type_defs.md#createdynamicthinggrouprequestrequesttypedef) 

### create\_fleet\_metric

Creates a fleet metric.

Type annotations and code completion for `#!python session.create_client("iot").create_fleet_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_fleet_metric.html)

```python
# create_fleet_metric method definition

await def create_fleet_metric(
    self,
    *,
    metricName: str,
    queryString: str,
    aggregationType: AggregationTypeTypeDef,  # (1)
    period: int,
    aggregationField: str,
    description: str = ...,
    queryVersion: str = ...,
    indexName: str = ...,
    unit: FleetMetricUnitType = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateFleetMetricResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AggregationTypeTypeDef](./type_defs.md#aggregationtypetypedef) 
2. See [:material-code-brackets: FleetMetricUnitType](./literals.md#fleetmetricunittype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateFleetMetricResponseTypeDef](./type_defs.md#createfleetmetricresponsetypedef) 


```python
# create_fleet_metric method usage example with argument unpacking

kwargs: CreateFleetMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
    "queryString": ...,
    "aggregationType": ...,
    "period": ...,
    "aggregationField": ...,
}

parent.create_fleet_metric(**kwargs)
```

1. See [:material-code-braces: CreateFleetMetricRequestRequestTypeDef](./type_defs.md#createfleetmetricrequestrequesttypedef) 

### create\_job

Creates a job.

Type annotations and code completion for `#!python session.create_client("iot").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_job.html)

```python
# create_job method definition

await def create_job(
    self,
    *,
    jobId: str,
    targets: Sequence[str],
    documentSource: str = ...,
    document: str = ...,
    description: str = ...,
    presignedUrlConfig: PresignedUrlConfigTypeDef = ...,  # (1)
    targetSelection: TargetSelectionType = ...,  # (2)
    jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,  # (3)
    abortConfig: AbortConfigTypeDef = ...,  # (4)
    timeoutConfig: TimeoutConfigTypeDef = ...,  # (5)
    tags: Sequence[TagTypeDef] = ...,  # (6)
    namespaceId: str = ...,
    jobTemplateArn: str = ...,
    jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,  # (7)
    documentParameters: Mapping[str, str] = ...,
    schedulingConfig: SchedulingConfigTypeDef = ...,  # (8)
    destinationPackageVersions: Sequence[str] = ...,
) -> CreateJobResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
2. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
3. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
4. See [:material-code-braces: AbortConfigTypeDef](./type_defs.md#abortconfigtypedef) 
5. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: JobExecutionsRetryConfigTypeDef](./type_defs.md#jobexecutionsretryconfigtypedef) 
8. See [:material-code-braces: SchedulingConfigTypeDef](./type_defs.md#schedulingconfigtypedef) 
9. See [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef) 


```python
# create_job method usage example with argument unpacking

kwargs: CreateJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "targets": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef) 

### create\_job\_template

Creates a job template.

Type annotations and code completion for `#!python session.create_client("iot").create_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_job_template.html)

```python
# create_job_template method definition

await def create_job_template(
    self,
    *,
    jobTemplateId: str,
    description: str,
    jobArn: str = ...,
    documentSource: str = ...,
    document: str = ...,
    presignedUrlConfig: PresignedUrlConfigTypeDef = ...,  # (1)
    jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,  # (2)
    abortConfig: AbortConfigTypeDef = ...,  # (3)
    timeoutConfig: TimeoutConfigTypeDef = ...,  # (4)
    tags: Sequence[TagTypeDef] = ...,  # (5)
    jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,  # (6)
    maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,  # (7)
    destinationPackageVersions: Sequence[str] = ...,
) -> CreateJobTemplateResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
2. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
3. See [:material-code-braces: AbortConfigTypeDef](./type_defs.md#abortconfigtypedef) 
4. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: JobExecutionsRetryConfigTypeDef](./type_defs.md#jobexecutionsretryconfigtypedef) 
7. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
8. See [:material-code-braces: CreateJobTemplateResponseTypeDef](./type_defs.md#createjobtemplateresponsetypedef) 


```python
# create_job_template method usage example with argument unpacking

kwargs: CreateJobTemplateRequestRequestTypeDef = {  # (1)
    "jobTemplateId": ...,
    "description": ...,
}

parent.create_job_template(**kwargs)
```

1. See [:material-code-braces: CreateJobTemplateRequestRequestTypeDef](./type_defs.md#createjobtemplaterequestrequesttypedef) 

### create\_keys\_and\_certificate

Creates a 2048-bit RSA key pair and issues an X.509 certificate using the
issued public key.

Type annotations and code completion for `#!python session.create_client("iot").create_keys_and_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_keys_and_certificate.html)

```python
# create_keys_and_certificate method definition

await def create_keys_and_certificate(
    self,
    *,
    setAsActive: bool = ...,
) -> CreateKeysAndCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateKeysAndCertificateResponseTypeDef](./type_defs.md#createkeysandcertificateresponsetypedef) 


```python
# create_keys_and_certificate method usage example with argument unpacking

kwargs: CreateKeysAndCertificateRequestRequestTypeDef = {  # (1)
    "setAsActive": ...,
}

parent.create_keys_and_certificate(**kwargs)
```

1. See [:material-code-braces: CreateKeysAndCertificateRequestRequestTypeDef](./type_defs.md#createkeysandcertificaterequestrequesttypedef) 

### create\_mitigation\_action

Defines an action that can be applied to audit findings by using
StartAuditMitigationActionsTask.

Type annotations and code completion for `#!python session.create_client("iot").create_mitigation_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_mitigation_action.html)

```python
# create_mitigation_action method definition

await def create_mitigation_action(
    self,
    *,
    actionName: str,
    roleArn: str,
    actionParams: MitigationActionParamsTypeDef,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateMitigationActionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MitigationActionParamsTypeDef](./type_defs.md#mitigationactionparamstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateMitigationActionResponseTypeDef](./type_defs.md#createmitigationactionresponsetypedef) 


```python
# create_mitigation_action method usage example with argument unpacking

kwargs: CreateMitigationActionRequestRequestTypeDef = {  # (1)
    "actionName": ...,
    "roleArn": ...,
    "actionParams": ...,
}

parent.create_mitigation_action(**kwargs)
```

1. See [:material-code-braces: CreateMitigationActionRequestRequestTypeDef](./type_defs.md#createmitigationactionrequestrequesttypedef) 

### create\_ota\_update

Creates an IoT OTA update on a target group of things or groups.

Type annotations and code completion for `#!python session.create_client("iot").create_ota_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_ota_update.html)

```python
# create_ota_update method definition

await def create_ota_update(
    self,
    *,
    otaUpdateId: str,
    targets: Sequence[str],
    files: Sequence[OTAUpdateFileUnionTypeDef],  # (1)
    roleArn: str,
    description: str = ...,
    protocols: Sequence[ProtocolType] = ...,  # (2)
    targetSelection: TargetSelectionType = ...,  # (3)
    awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,  # (4)
    awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,  # (5)
    awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,  # (6)
    awsJobTimeoutConfig: AwsJobTimeoutConfigTypeDef = ...,  # (7)
    additionalParameters: Mapping[str, str] = ...,
    tags: Sequence[TagTypeDef] = ...,  # (8)
) -> CreateOTAUpdateResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: OTAUpdateFileTypeDef](./type_defs.md#otaupdatefiletypedef) [:material-code-braces: OTAUpdateFileOutputTypeDef](./type_defs.md#otaupdatefileoutputtypedef) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
3. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
4. See [:material-code-braces: AwsJobExecutionsRolloutConfigTypeDef](./type_defs.md#awsjobexecutionsrolloutconfigtypedef) 
5. See [:material-code-braces: AwsJobPresignedUrlConfigTypeDef](./type_defs.md#awsjobpresignedurlconfigtypedef) 
6. See [:material-code-braces: AwsJobAbortConfigTypeDef](./type_defs.md#awsjobabortconfigtypedef) 
7. See [:material-code-braces: AwsJobTimeoutConfigTypeDef](./type_defs.md#awsjobtimeoutconfigtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: CreateOTAUpdateResponseTypeDef](./type_defs.md#createotaupdateresponsetypedef) 


```python
# create_ota_update method usage example with argument unpacking

kwargs: CreateOTAUpdateRequestRequestTypeDef = {  # (1)
    "otaUpdateId": ...,
    "targets": ...,
    "files": ...,
    "roleArn": ...,
}

parent.create_ota_update(**kwargs)
```

1. See [:material-code-braces: CreateOTAUpdateRequestRequestTypeDef](./type_defs.md#createotaupdaterequestrequesttypedef) 

### create\_package

Creates an IoT software package that can be deployed to your fleet.

Type annotations and code completion for `#!python session.create_client("iot").create_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_package.html)

```python
# create_package method definition

await def create_package(
    self,
    *,
    packageName: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreatePackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePackageResponseTypeDef](./type_defs.md#createpackageresponsetypedef) 


```python
# create_package method usage example with argument unpacking

kwargs: CreatePackageRequestRequestTypeDef = {  # (1)
    "packageName": ...,
}

parent.create_package(**kwargs)
```

1. See [:material-code-braces: CreatePackageRequestRequestTypeDef](./type_defs.md#createpackagerequestrequesttypedef) 

### create\_package\_version

Creates a new version for an existing IoT software package.

Type annotations and code completion for `#!python session.create_client("iot").create_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_package_version.html)

```python
# create_package_version method definition

await def create_package_version(
    self,
    *,
    packageName: str,
    versionName: str,
    description: str = ...,
    attributes: Mapping[str, str] = ...,
    artifact: PackageVersionArtifactTypeDef = ...,  # (1)
    recipe: str = ...,
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreatePackageVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PackageVersionArtifactTypeDef](./type_defs.md#packageversionartifacttypedef) 
2. See [:material-code-braces: CreatePackageVersionResponseTypeDef](./type_defs.md#createpackageversionresponsetypedef) 


```python
# create_package_version method usage example with argument unpacking

kwargs: CreatePackageVersionRequestRequestTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
}

parent.create_package_version(**kwargs)
```

1. See [:material-code-braces: CreatePackageVersionRequestRequestTypeDef](./type_defs.md#createpackageversionrequestrequesttypedef) 

### create\_policy

Creates an IoT policy.

Type annotations and code completion for `#!python session.create_client("iot").create_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_policy.html)

```python
# create_policy method definition

await def create_policy(
    self,
    *,
    policyName: str,
    policyDocument: str,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreatePolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreatePolicyResponseTypeDef](./type_defs.md#createpolicyresponsetypedef) 


```python
# create_policy method usage example with argument unpacking

kwargs: CreatePolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "policyDocument": ...,
}

parent.create_policy(**kwargs)
```

1. See [:material-code-braces: CreatePolicyRequestRequestTypeDef](./type_defs.md#createpolicyrequestrequesttypedef) 

### create\_policy\_version

Creates a new version of the specified IoT policy.

Type annotations and code completion for `#!python session.create_client("iot").create_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_policy_version.html)

```python
# create_policy_version method definition

await def create_policy_version(
    self,
    *,
    policyName: str,
    policyDocument: str,
    setAsDefault: bool = ...,
) -> CreatePolicyVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePolicyVersionResponseTypeDef](./type_defs.md#createpolicyversionresponsetypedef) 


```python
# create_policy_version method usage example with argument unpacking

kwargs: CreatePolicyVersionRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "policyDocument": ...,
}

parent.create_policy_version(**kwargs)
```

1. See [:material-code-braces: CreatePolicyVersionRequestRequestTypeDef](./type_defs.md#createpolicyversionrequestrequesttypedef) 

### create\_provisioning\_claim

Creates a provisioning claim.

Type annotations and code completion for `#!python session.create_client("iot").create_provisioning_claim` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_provisioning_claim.html)

```python
# create_provisioning_claim method definition

await def create_provisioning_claim(
    self,
    *,
    templateName: str,
) -> CreateProvisioningClaimResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateProvisioningClaimResponseTypeDef](./type_defs.md#createprovisioningclaimresponsetypedef) 


```python
# create_provisioning_claim method usage example with argument unpacking

kwargs: CreateProvisioningClaimRequestRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.create_provisioning_claim(**kwargs)
```

1. See [:material-code-braces: CreateProvisioningClaimRequestRequestTypeDef](./type_defs.md#createprovisioningclaimrequestrequesttypedef) 

### create\_provisioning\_template

Creates a provisioning template.

Type annotations and code completion for `#!python session.create_client("iot").create_provisioning_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_provisioning_template.html)

```python
# create_provisioning_template method definition

await def create_provisioning_template(
    self,
    *,
    templateName: str,
    templateBody: str,
    provisioningRoleArn: str,
    description: str = ...,
    enabled: bool = ...,
    preProvisioningHook: ProvisioningHookTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
    type: TemplateTypeType = ...,  # (3)
) -> CreateProvisioningTemplateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ProvisioningHookTypeDef](./type_defs.md#provisioninghooktypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
4. See [:material-code-braces: CreateProvisioningTemplateResponseTypeDef](./type_defs.md#createprovisioningtemplateresponsetypedef) 


```python
# create_provisioning_template method usage example with argument unpacking

kwargs: CreateProvisioningTemplateRequestRequestTypeDef = {  # (1)
    "templateName": ...,
    "templateBody": ...,
    "provisioningRoleArn": ...,
}

parent.create_provisioning_template(**kwargs)
```

1. See [:material-code-braces: CreateProvisioningTemplateRequestRequestTypeDef](./type_defs.md#createprovisioningtemplaterequestrequesttypedef) 

### create\_provisioning\_template\_version

Creates a new version of a provisioning template.

Type annotations and code completion for `#!python session.create_client("iot").create_provisioning_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_provisioning_template_version.html)

```python
# create_provisioning_template_version method definition

await def create_provisioning_template_version(
    self,
    *,
    templateName: str,
    templateBody: str,
    setAsDefault: bool = ...,
) -> CreateProvisioningTemplateVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateProvisioningTemplateVersionResponseTypeDef](./type_defs.md#createprovisioningtemplateversionresponsetypedef) 


```python
# create_provisioning_template_version method usage example with argument unpacking

kwargs: CreateProvisioningTemplateVersionRequestRequestTypeDef = {  # (1)
    "templateName": ...,
    "templateBody": ...,
}

parent.create_provisioning_template_version(**kwargs)
```

1. See [:material-code-braces: CreateProvisioningTemplateVersionRequestRequestTypeDef](./type_defs.md#createprovisioningtemplateversionrequestrequesttypedef) 

### create\_role\_alias

Creates a role alias.

Type annotations and code completion for `#!python session.create_client("iot").create_role_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_role_alias.html)

```python
# create_role_alias method definition

await def create_role_alias(
    self,
    *,
    roleAlias: str,
    roleArn: str,
    credentialDurationSeconds: int = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateRoleAliasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateRoleAliasResponseTypeDef](./type_defs.md#createrolealiasresponsetypedef) 


```python
# create_role_alias method usage example with argument unpacking

kwargs: CreateRoleAliasRequestRequestTypeDef = {  # (1)
    "roleAlias": ...,
    "roleArn": ...,
}

parent.create_role_alias(**kwargs)
```

1. See [:material-code-braces: CreateRoleAliasRequestRequestTypeDef](./type_defs.md#createrolealiasrequestrequesttypedef) 

### create\_scheduled\_audit

Creates a scheduled audit that is run at a specified time interval.

Type annotations and code completion for `#!python session.create_client("iot").create_scheduled_audit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_scheduled_audit.html)

```python
# create_scheduled_audit method definition

await def create_scheduled_audit(
    self,
    *,
    frequency: AuditFrequencyType,  # (1)
    targetCheckNames: Sequence[str],
    scheduledAuditName: str,
    dayOfMonth: str = ...,
    dayOfWeek: DayOfWeekType = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateScheduledAuditResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AuditFrequencyType](./literals.md#auditfrequencytype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateScheduledAuditResponseTypeDef](./type_defs.md#createscheduledauditresponsetypedef) 


```python
# create_scheduled_audit method usage example with argument unpacking

kwargs: CreateScheduledAuditRequestRequestTypeDef = {  # (1)
    "frequency": ...,
    "targetCheckNames": ...,
    "scheduledAuditName": ...,
}

parent.create_scheduled_audit(**kwargs)
```

1. See [:material-code-braces: CreateScheduledAuditRequestRequestTypeDef](./type_defs.md#createscheduledauditrequestrequesttypedef) 

### create\_security\_profile

Creates a Device Defender security profile.

Type annotations and code completion for `#!python session.create_client("iot").create_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_security_profile.html)

```python
# create_security_profile method definition

await def create_security_profile(
    self,
    *,
    securityProfileName: str,
    securityProfileDescription: str = ...,
    behaviors: Sequence[BehaviorUnionTypeDef] = ...,  # (1)
    alertTargets: Mapping[AlertTargetTypeType, AlertTargetTypeDef] = ...,  # (2)
    additionalMetricsToRetain: Sequence[str] = ...,
    additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,  # (3)
    tags: Sequence[TagTypeDef] = ...,  # (4)
    metricsExportConfig: MetricsExportConfigTypeDef = ...,  # (5)
) -> CreateSecurityProfileResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: BehaviorTypeDef](./type_defs.md#behaviortypedef) [:material-code-braces: BehaviorOutputTypeDef](./type_defs.md#behavioroutputtypedef) 
2. See [:material-code-brackets: AlertTargetTypeType](./literals.md#alerttargettypetype) [:material-code-braces: AlertTargetTypeDef](./type_defs.md#alerttargettypedef) 
3. See [:material-code-braces: MetricToRetainTypeDef](./type_defs.md#metrictoretaintypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MetricsExportConfigTypeDef](./type_defs.md#metricsexportconfigtypedef) 
6. See [:material-code-braces: CreateSecurityProfileResponseTypeDef](./type_defs.md#createsecurityprofileresponsetypedef) 


```python
# create_security_profile method usage example with argument unpacking

kwargs: CreateSecurityProfileRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.create_security_profile(**kwargs)
```

1. See [:material-code-braces: CreateSecurityProfileRequestRequestTypeDef](./type_defs.md#createsecurityprofilerequestrequesttypedef) 

### create\_stream

Creates a stream for delivering one or more large files in chunks over MQTT.

Type annotations and code completion for `#!python session.create_client("iot").create_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_stream.html)

```python
# create_stream method definition

await def create_stream(
    self,
    *,
    streamId: str,
    files: Sequence[StreamFileTypeDef],  # (1)
    roleArn: str,
    description: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateStreamResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: StreamFileTypeDef](./type_defs.md#streamfiletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateStreamResponseTypeDef](./type_defs.md#createstreamresponsetypedef) 


```python
# create_stream method usage example with argument unpacking

kwargs: CreateStreamRequestRequestTypeDef = {  # (1)
    "streamId": ...,
    "files": ...,
    "roleArn": ...,
}

parent.create_stream(**kwargs)
```

1. See [:material-code-braces: CreateStreamRequestRequestTypeDef](./type_defs.md#createstreamrequestrequesttypedef) 

### create\_thing

Creates a thing record in the registry.

Type annotations and code completion for `#!python session.create_client("iot").create_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_thing.html)

```python
# create_thing method definition

await def create_thing(
    self,
    *,
    thingName: str,
    thingTypeName: str = ...,
    attributePayload: AttributePayloadTypeDef = ...,  # (1)
    billingGroupName: str = ...,
) -> CreateThingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttributePayloadTypeDef](./type_defs.md#attributepayloadtypedef) 
2. See [:material-code-braces: CreateThingResponseTypeDef](./type_defs.md#createthingresponsetypedef) 


```python
# create_thing method usage example with argument unpacking

kwargs: CreateThingRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.create_thing(**kwargs)
```

1. See [:material-code-braces: CreateThingRequestRequestTypeDef](./type_defs.md#createthingrequestrequesttypedef) 

### create\_thing\_group

Create a thing group.

Type annotations and code completion for `#!python session.create_client("iot").create_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_thing_group.html)

```python
# create_thing_group method definition

await def create_thing_group(
    self,
    *,
    thingGroupName: str,
    parentGroupName: str = ...,
    thingGroupProperties: ThingGroupPropertiesTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateThingGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateThingGroupResponseTypeDef](./type_defs.md#createthinggroupresponsetypedef) 


```python
# create_thing_group method usage example with argument unpacking

kwargs: CreateThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.create_thing_group(**kwargs)
```

1. See [:material-code-braces: CreateThingGroupRequestRequestTypeDef](./type_defs.md#createthinggrouprequestrequesttypedef) 

### create\_thing\_type

Creates a new thing type.

Type annotations and code completion for `#!python session.create_client("iot").create_thing_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_thing_type.html)

```python
# create_thing_type method definition

await def create_thing_type(
    self,
    *,
    thingTypeName: str,
    thingTypeProperties: ThingTypePropertiesTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateThingTypeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ThingTypePropertiesTypeDef](./type_defs.md#thingtypepropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateThingTypeResponseTypeDef](./type_defs.md#createthingtyperesponsetypedef) 


```python
# create_thing_type method usage example with argument unpacking

kwargs: CreateThingTypeRequestRequestTypeDef = {  # (1)
    "thingTypeName": ...,
}

parent.create_thing_type(**kwargs)
```

1. See [:material-code-braces: CreateThingTypeRequestRequestTypeDef](./type_defs.md#createthingtyperequestrequesttypedef) 

### create\_topic\_rule

Creates a rule.

Type annotations and code completion for `#!python session.create_client("iot").create_topic_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_topic_rule.html)

```python
# create_topic_rule method definition

await def create_topic_rule(
    self,
    *,
    ruleName: str,
    topicRulePayload: TopicRulePayloadTypeDef,  # (1)
    tags: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicRulePayloadTypeDef](./type_defs.md#topicrulepayloadtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_topic_rule method usage example with argument unpacking

kwargs: CreateTopicRuleRequestRequestTypeDef = {  # (1)
    "ruleName": ...,
    "topicRulePayload": ...,
}

parent.create_topic_rule(**kwargs)
```

1. See [:material-code-braces: CreateTopicRuleRequestRequestTypeDef](./type_defs.md#createtopicrulerequestrequesttypedef) 

### create\_topic\_rule\_destination

Creates a topic rule destination.

Type annotations and code completion for `#!python session.create_client("iot").create_topic_rule_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/create_topic_rule_destination.html)

```python
# create_topic_rule_destination method definition

await def create_topic_rule_destination(
    self,
    *,
    destinationConfiguration: TopicRuleDestinationConfigurationTypeDef,  # (1)
) -> CreateTopicRuleDestinationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicRuleDestinationConfigurationTypeDef](./type_defs.md#topicruledestinationconfigurationtypedef) 
2. See [:material-code-braces: CreateTopicRuleDestinationResponseTypeDef](./type_defs.md#createtopicruledestinationresponsetypedef) 


```python
# create_topic_rule_destination method usage example with argument unpacking

kwargs: CreateTopicRuleDestinationRequestRequestTypeDef = {  # (1)
    "destinationConfiguration": ...,
}

parent.create_topic_rule_destination(**kwargs)
```

1. See [:material-code-braces: CreateTopicRuleDestinationRequestRequestTypeDef](./type_defs.md#createtopicruledestinationrequestrequesttypedef) 

### delete\_account\_audit\_configuration

Restores the default settings for Device Defender audits for this account.

Type annotations and code completion for `#!python session.create_client("iot").delete_account_audit_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_account_audit_configuration.html)

```python
# delete_account_audit_configuration method definition

await def delete_account_audit_configuration(
    self,
    *,
    deleteScheduledAudits: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_account_audit_configuration method usage example with argument unpacking

kwargs: DeleteAccountAuditConfigurationRequestRequestTypeDef = {  # (1)
    "deleteScheduledAudits": ...,
}

parent.delete_account_audit_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteAccountAuditConfigurationRequestRequestTypeDef](./type_defs.md#deleteaccountauditconfigurationrequestrequesttypedef) 

### delete\_audit\_suppression

Deletes a Device Defender audit suppression.

Type annotations and code completion for `#!python session.create_client("iot").delete_audit_suppression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_audit_suppression.html)

```python
# delete_audit_suppression method definition

await def delete_audit_suppression(
    self,
    *,
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 


```python
# delete_audit_suppression method usage example with argument unpacking

kwargs: DeleteAuditSuppressionRequestRequestTypeDef = {  # (1)
    "checkName": ...,
    "resourceIdentifier": ...,
}

parent.delete_audit_suppression(**kwargs)
```

1. See [:material-code-braces: DeleteAuditSuppressionRequestRequestTypeDef](./type_defs.md#deleteauditsuppressionrequestrequesttypedef) 

### delete\_authorizer

Deletes an authorizer.

Type annotations and code completion for `#!python session.create_client("iot").delete_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_authorizer.html)

```python
# delete_authorizer method definition

await def delete_authorizer(
    self,
    *,
    authorizerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_authorizer method usage example with argument unpacking

kwargs: DeleteAuthorizerRequestRequestTypeDef = {  # (1)
    "authorizerName": ...,
}

parent.delete_authorizer(**kwargs)
```

1. See [:material-code-braces: DeleteAuthorizerRequestRequestTypeDef](./type_defs.md#deleteauthorizerrequestrequesttypedef) 

### delete\_billing\_group

Deletes the billing group.

Type annotations and code completion for `#!python session.create_client("iot").delete_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_billing_group.html)

```python
# delete_billing_group method definition

await def delete_billing_group(
    self,
    *,
    billingGroupName: str,
    expectedVersion: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_billing_group method usage example with argument unpacking

kwargs: DeleteBillingGroupRequestRequestTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.delete_billing_group(**kwargs)
```

1. See [:material-code-braces: DeleteBillingGroupRequestRequestTypeDef](./type_defs.md#deletebillinggrouprequestrequesttypedef) 

### delete\_ca\_certificate

Deletes a registered CA certificate.

Type annotations and code completion for `#!python session.create_client("iot").delete_ca_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_ca_certificate.html)

```python
# delete_ca_certificate method definition

await def delete_ca_certificate(
    self,
    *,
    certificateId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ca_certificate method usage example with argument unpacking

kwargs: DeleteCACertificateRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.delete_ca_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteCACertificateRequestRequestTypeDef](./type_defs.md#deletecacertificaterequestrequesttypedef) 

### delete\_certificate

Deletes the specified certificate.

Type annotations and code completion for `#!python session.create_client("iot").delete_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_certificate.html)

```python
# delete_certificate method definition

await def delete_certificate(
    self,
    *,
    certificateId: str,
    forceDelete: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_certificate method usage example with argument unpacking

kwargs: DeleteCertificateRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.delete_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteCertificateRequestRequestTypeDef](./type_defs.md#deletecertificaterequestrequesttypedef) 

### delete\_certificate\_provider

Deletes a certificate provider.

Type annotations and code completion for `#!python session.create_client("iot").delete_certificate_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_certificate_provider.html)

```python
# delete_certificate_provider method definition

await def delete_certificate_provider(
    self,
    *,
    certificateProviderName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_certificate_provider method usage example with argument unpacking

kwargs: DeleteCertificateProviderRequestRequestTypeDef = {  # (1)
    "certificateProviderName": ...,
}

parent.delete_certificate_provider(**kwargs)
```

1. See [:material-code-braces: DeleteCertificateProviderRequestRequestTypeDef](./type_defs.md#deletecertificateproviderrequestrequesttypedef) 

### delete\_command

Delete a command resource.

Type annotations and code completion for `#!python session.create_client("iot").delete_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_command.html)

```python
# delete_command method definition

await def delete_command(
    self,
    *,
    commandId: str,
) -> DeleteCommandResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCommandResponseTypeDef](./type_defs.md#deletecommandresponsetypedef) 


```python
# delete_command method usage example with argument unpacking

kwargs: DeleteCommandRequestRequestTypeDef = {  # (1)
    "commandId": ...,
}

parent.delete_command(**kwargs)
```

1. See [:material-code-braces: DeleteCommandRequestRequestTypeDef](./type_defs.md#deletecommandrequestrequesttypedef) 

### delete\_command\_execution

Delete a command execution.

Type annotations and code completion for `#!python session.create_client("iot").delete_command_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_command_execution.html)

```python
# delete_command_execution method definition

await def delete_command_execution(
    self,
    *,
    executionId: str,
    targetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_command_execution method usage example with argument unpacking

kwargs: DeleteCommandExecutionRequestRequestTypeDef = {  # (1)
    "executionId": ...,
    "targetArn": ...,
}

parent.delete_command_execution(**kwargs)
```

1. See [:material-code-braces: DeleteCommandExecutionRequestRequestTypeDef](./type_defs.md#deletecommandexecutionrequestrequesttypedef) 

### delete\_custom\_metric

Deletes a Device Defender detect custom metric.

Type annotations and code completion for `#!python session.create_client("iot").delete_custom_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_custom_metric.html)

```python
# delete_custom_metric method definition

await def delete_custom_metric(
    self,
    *,
    metricName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_custom_metric method usage example with argument unpacking

kwargs: DeleteCustomMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
}

parent.delete_custom_metric(**kwargs)
```

1. See [:material-code-braces: DeleteCustomMetricRequestRequestTypeDef](./type_defs.md#deletecustommetricrequestrequesttypedef) 

### delete\_dimension

Removes the specified dimension from your Amazon Web Services accounts.

Type annotations and code completion for `#!python session.create_client("iot").delete_dimension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_dimension.html)

```python
# delete_dimension method definition

await def delete_dimension(
    self,
    *,
    name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_dimension method usage example with argument unpacking

kwargs: DeleteDimensionRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_dimension(**kwargs)
```

1. See [:material-code-braces: DeleteDimensionRequestRequestTypeDef](./type_defs.md#deletedimensionrequestrequesttypedef) 

### delete\_domain\_configuration

Deletes the specified domain configuration.

Type annotations and code completion for `#!python session.create_client("iot").delete_domain_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_domain_configuration.html)

```python
# delete_domain_configuration method definition

await def delete_domain_configuration(
    self,
    *,
    domainConfigurationName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_domain_configuration method usage example with argument unpacking

kwargs: DeleteDomainConfigurationRequestRequestTypeDef = {  # (1)
    "domainConfigurationName": ...,
}

parent.delete_domain_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteDomainConfigurationRequestRequestTypeDef](./type_defs.md#deletedomainconfigurationrequestrequesttypedef) 

### delete\_dynamic\_thing\_group

Deletes a dynamic thing group.

Type annotations and code completion for `#!python session.create_client("iot").delete_dynamic_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_dynamic_thing_group.html)

```python
# delete_dynamic_thing_group method definition

await def delete_dynamic_thing_group(
    self,
    *,
    thingGroupName: str,
    expectedVersion: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_dynamic_thing_group method usage example with argument unpacking

kwargs: DeleteDynamicThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.delete_dynamic_thing_group(**kwargs)
```

1. See [:material-code-braces: DeleteDynamicThingGroupRequestRequestTypeDef](./type_defs.md#deletedynamicthinggrouprequestrequesttypedef) 

### delete\_fleet\_metric

Deletes the specified fleet metric.

Type annotations and code completion for `#!python session.create_client("iot").delete_fleet_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_fleet_metric.html)

```python
# delete_fleet_metric method definition

await def delete_fleet_metric(
    self,
    *,
    metricName: str,
    expectedVersion: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_fleet_metric method usage example with argument unpacking

kwargs: DeleteFleetMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
}

parent.delete_fleet_metric(**kwargs)
```

1. See [:material-code-braces: DeleteFleetMetricRequestRequestTypeDef](./type_defs.md#deletefleetmetricrequestrequesttypedef) 

### delete\_job

Deletes a job and its related job executions.

Type annotations and code completion for `#!python session.create_client("iot").delete_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_job.html)

```python
# delete_job method definition

await def delete_job(
    self,
    *,
    jobId: str,
    force: bool = ...,
    namespaceId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_job method usage example with argument unpacking

kwargs: DeleteJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.delete_job(**kwargs)
```

1. See [:material-code-braces: DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef) 

### delete\_job\_execution

Deletes a job execution.

Type annotations and code completion for `#!python session.create_client("iot").delete_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_job_execution.html)

```python
# delete_job_execution method definition

await def delete_job_execution(
    self,
    *,
    jobId: str,
    thingName: str,
    executionNumber: int,
    force: bool = ...,
    namespaceId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_job_execution method usage example with argument unpacking

kwargs: DeleteJobExecutionRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "thingName": ...,
    "executionNumber": ...,
}

parent.delete_job_execution(**kwargs)
```

1. See [:material-code-braces: DeleteJobExecutionRequestRequestTypeDef](./type_defs.md#deletejobexecutionrequestrequesttypedef) 

### delete\_job\_template

Deletes the specified job template.

Type annotations and code completion for `#!python session.create_client("iot").delete_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_job_template.html)

```python
# delete_job_template method definition

await def delete_job_template(
    self,
    *,
    jobTemplateId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_job_template method usage example with argument unpacking

kwargs: DeleteJobTemplateRequestRequestTypeDef = {  # (1)
    "jobTemplateId": ...,
}

parent.delete_job_template(**kwargs)
```

1. See [:material-code-braces: DeleteJobTemplateRequestRequestTypeDef](./type_defs.md#deletejobtemplaterequestrequesttypedef) 

### delete\_mitigation\_action

Deletes a defined mitigation action from your Amazon Web Services accounts.

Type annotations and code completion for `#!python session.create_client("iot").delete_mitigation_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_mitigation_action.html)

```python
# delete_mitigation_action method definition

await def delete_mitigation_action(
    self,
    *,
    actionName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_mitigation_action method usage example with argument unpacking

kwargs: DeleteMitigationActionRequestRequestTypeDef = {  # (1)
    "actionName": ...,
}

parent.delete_mitigation_action(**kwargs)
```

1. See [:material-code-braces: DeleteMitigationActionRequestRequestTypeDef](./type_defs.md#deletemitigationactionrequestrequesttypedef) 

### delete\_ota\_update

Delete an OTA update.

Type annotations and code completion for `#!python session.create_client("iot").delete_ota_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_ota_update.html)

```python
# delete_ota_update method definition

await def delete_ota_update(
    self,
    *,
    otaUpdateId: str,
    deleteStream: bool = ...,
    forceDeleteAWSJob: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ota_update method usage example with argument unpacking

kwargs: DeleteOTAUpdateRequestRequestTypeDef = {  # (1)
    "otaUpdateId": ...,
}

parent.delete_ota_update(**kwargs)
```

1. See [:material-code-braces: DeleteOTAUpdateRequestRequestTypeDef](./type_defs.md#deleteotaupdaterequestrequesttypedef) 

### delete\_package

Deletes a specific version from a software package.

Type annotations and code completion for `#!python session.create_client("iot").delete_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_package.html)

```python
# delete_package method definition

await def delete_package(
    self,
    *,
    packageName: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_package method usage example with argument unpacking

kwargs: DeletePackageRequestRequestTypeDef = {  # (1)
    "packageName": ...,
}

parent.delete_package(**kwargs)
```

1. See [:material-code-braces: DeletePackageRequestRequestTypeDef](./type_defs.md#deletepackagerequestrequesttypedef) 

### delete\_package\_version

Deletes a specific version from a software package.

Type annotations and code completion for `#!python session.create_client("iot").delete_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_package_version.html)

```python
# delete_package_version method definition

await def delete_package_version(
    self,
    *,
    packageName: str,
    versionName: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_package_version method usage example with argument unpacking

kwargs: DeletePackageVersionRequestRequestTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
}

parent.delete_package_version(**kwargs)
```

1. See [:material-code-braces: DeletePackageVersionRequestRequestTypeDef](./type_defs.md#deletepackageversionrequestrequesttypedef) 

### delete\_policy

Deletes the specified policy.

Type annotations and code completion for `#!python session.create_client("iot").delete_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_policy.html)

```python
# delete_policy method definition

await def delete_policy(
    self,
    *,
    policyName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_policy method usage example with argument unpacking

kwargs: DeletePolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
}

parent.delete_policy(**kwargs)
```

1. See [:material-code-braces: DeletePolicyRequestRequestTypeDef](./type_defs.md#deletepolicyrequestrequesttypedef) 

### delete\_policy\_version

Deletes the specified version of the specified policy.

Type annotations and code completion for `#!python session.create_client("iot").delete_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_policy_version.html)

```python
# delete_policy_version method definition

await def delete_policy_version(
    self,
    *,
    policyName: str,
    policyVersionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_policy_version method usage example with argument unpacking

kwargs: DeletePolicyVersionRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "policyVersionId": ...,
}

parent.delete_policy_version(**kwargs)
```

1. See [:material-code-braces: DeletePolicyVersionRequestRequestTypeDef](./type_defs.md#deletepolicyversionrequestrequesttypedef) 

### delete\_provisioning\_template

Deletes a provisioning template.

Type annotations and code completion for `#!python session.create_client("iot").delete_provisioning_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_provisioning_template.html)

```python
# delete_provisioning_template method definition

await def delete_provisioning_template(
    self,
    *,
    templateName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_provisioning_template method usage example with argument unpacking

kwargs: DeleteProvisioningTemplateRequestRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.delete_provisioning_template(**kwargs)
```

1. See [:material-code-braces: DeleteProvisioningTemplateRequestRequestTypeDef](./type_defs.md#deleteprovisioningtemplaterequestrequesttypedef) 

### delete\_provisioning\_template\_version

Deletes a provisioning template version.

Type annotations and code completion for `#!python session.create_client("iot").delete_provisioning_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_provisioning_template_version.html)

```python
# delete_provisioning_template_version method definition

await def delete_provisioning_template_version(
    self,
    *,
    templateName: str,
    versionId: int,
) -> Dict[str, Any]:
    ...
```



```python
# delete_provisioning_template_version method usage example with argument unpacking

kwargs: DeleteProvisioningTemplateVersionRequestRequestTypeDef = {  # (1)
    "templateName": ...,
    "versionId": ...,
}

parent.delete_provisioning_template_version(**kwargs)
```

1. See [:material-code-braces: DeleteProvisioningTemplateVersionRequestRequestTypeDef](./type_defs.md#deleteprovisioningtemplateversionrequestrequesttypedef) 

### delete\_registration\_code

Deletes a CA certificate registration code.

Type annotations and code completion for `#!python session.create_client("iot").delete_registration_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_registration_code.html)

```python
# delete_registration_code method definition

await def delete_registration_code(
    self,
) -> Dict[str, Any]:
    ...
```


### delete\_role\_alias

Deletes a role alias.

Type annotations and code completion for `#!python session.create_client("iot").delete_role_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_role_alias.html)

```python
# delete_role_alias method definition

await def delete_role_alias(
    self,
    *,
    roleAlias: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_role_alias method usage example with argument unpacking

kwargs: DeleteRoleAliasRequestRequestTypeDef = {  # (1)
    "roleAlias": ...,
}

parent.delete_role_alias(**kwargs)
```

1. See [:material-code-braces: DeleteRoleAliasRequestRequestTypeDef](./type_defs.md#deleterolealiasrequestrequesttypedef) 

### delete\_scheduled\_audit

Deletes a scheduled audit.

Type annotations and code completion for `#!python session.create_client("iot").delete_scheduled_audit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_scheduled_audit.html)

```python
# delete_scheduled_audit method definition

await def delete_scheduled_audit(
    self,
    *,
    scheduledAuditName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_scheduled_audit method usage example with argument unpacking

kwargs: DeleteScheduledAuditRequestRequestTypeDef = {  # (1)
    "scheduledAuditName": ...,
}

parent.delete_scheduled_audit(**kwargs)
```

1. See [:material-code-braces: DeleteScheduledAuditRequestRequestTypeDef](./type_defs.md#deletescheduledauditrequestrequesttypedef) 

### delete\_security\_profile

Deletes a Device Defender security profile.

Type annotations and code completion for `#!python session.create_client("iot").delete_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_security_profile.html)

```python
# delete_security_profile method definition

await def delete_security_profile(
    self,
    *,
    securityProfileName: str,
    expectedVersion: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_security_profile method usage example with argument unpacking

kwargs: DeleteSecurityProfileRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.delete_security_profile(**kwargs)
```

1. See [:material-code-braces: DeleteSecurityProfileRequestRequestTypeDef](./type_defs.md#deletesecurityprofilerequestrequesttypedef) 

### delete\_stream

Deletes a stream.

Type annotations and code completion for `#!python session.create_client("iot").delete_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_stream.html)

```python
# delete_stream method definition

await def delete_stream(
    self,
    *,
    streamId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_stream method usage example with argument unpacking

kwargs: DeleteStreamRequestRequestTypeDef = {  # (1)
    "streamId": ...,
}

parent.delete_stream(**kwargs)
```

1. See [:material-code-braces: DeleteStreamRequestRequestTypeDef](./type_defs.md#deletestreamrequestrequesttypedef) 

### delete\_thing

Deletes the specified thing.

Type annotations and code completion for `#!python session.create_client("iot").delete_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_thing.html)

```python
# delete_thing method definition

await def delete_thing(
    self,
    *,
    thingName: str,
    expectedVersion: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_thing method usage example with argument unpacking

kwargs: DeleteThingRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.delete_thing(**kwargs)
```

1. See [:material-code-braces: DeleteThingRequestRequestTypeDef](./type_defs.md#deletethingrequestrequesttypedef) 

### delete\_thing\_group

Deletes a thing group.

Type annotations and code completion for `#!python session.create_client("iot").delete_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_thing_group.html)

```python
# delete_thing_group method definition

await def delete_thing_group(
    self,
    *,
    thingGroupName: str,
    expectedVersion: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_thing_group method usage example with argument unpacking

kwargs: DeleteThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.delete_thing_group(**kwargs)
```

1. See [:material-code-braces: DeleteThingGroupRequestRequestTypeDef](./type_defs.md#deletethinggrouprequestrequesttypedef) 

### delete\_thing\_type

Deletes the specified thing type.

Type annotations and code completion for `#!python session.create_client("iot").delete_thing_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_thing_type.html)

```python
# delete_thing_type method definition

await def delete_thing_type(
    self,
    *,
    thingTypeName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_thing_type method usage example with argument unpacking

kwargs: DeleteThingTypeRequestRequestTypeDef = {  # (1)
    "thingTypeName": ...,
}

parent.delete_thing_type(**kwargs)
```

1. See [:material-code-braces: DeleteThingTypeRequestRequestTypeDef](./type_defs.md#deletethingtyperequestrequesttypedef) 

### delete\_topic\_rule

Deletes the rule.

Type annotations and code completion for `#!python session.create_client("iot").delete_topic_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_topic_rule.html)

```python
# delete_topic_rule method definition

await def delete_topic_rule(
    self,
    *,
    ruleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_topic_rule method usage example with argument unpacking

kwargs: DeleteTopicRuleRequestRequestTypeDef = {  # (1)
    "ruleName": ...,
}

parent.delete_topic_rule(**kwargs)
```

1. See [:material-code-braces: DeleteTopicRuleRequestRequestTypeDef](./type_defs.md#deletetopicrulerequestrequesttypedef) 

### delete\_topic\_rule\_destination

Deletes a topic rule destination.

Type annotations and code completion for `#!python session.create_client("iot").delete_topic_rule_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_topic_rule_destination.html)

```python
# delete_topic_rule_destination method definition

await def delete_topic_rule_destination(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_topic_rule_destination method usage example with argument unpacking

kwargs: DeleteTopicRuleDestinationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_topic_rule_destination(**kwargs)
```

1. See [:material-code-braces: DeleteTopicRuleDestinationRequestRequestTypeDef](./type_defs.md#deletetopicruledestinationrequestrequesttypedef) 

### delete\_v2\_logging\_level

Deletes a logging level.

Type annotations and code completion for `#!python session.create_client("iot").delete_v2_logging_level` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/delete_v2_logging_level.html)

```python
# delete_v2_logging_level method definition

await def delete_v2_logging_level(
    self,
    *,
    targetType: LogTargetTypeType,  # (1)
    targetName: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_v2_logging_level method usage example with argument unpacking

kwargs: DeleteV2LoggingLevelRequestRequestTypeDef = {  # (1)
    "targetType": ...,
    "targetName": ...,
}

parent.delete_v2_logging_level(**kwargs)
```

1. See [:material-code-braces: DeleteV2LoggingLevelRequestRequestTypeDef](./type_defs.md#deletev2logginglevelrequestrequesttypedef) 

### deprecate\_thing\_type

Deprecates a thing type.

Type annotations and code completion for `#!python session.create_client("iot").deprecate_thing_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/deprecate_thing_type.html)

```python
# deprecate_thing_type method definition

await def deprecate_thing_type(
    self,
    *,
    thingTypeName: str,
    undoDeprecate: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# deprecate_thing_type method usage example with argument unpacking

kwargs: DeprecateThingTypeRequestRequestTypeDef = {  # (1)
    "thingTypeName": ...,
}

parent.deprecate_thing_type(**kwargs)
```

1. See [:material-code-braces: DeprecateThingTypeRequestRequestTypeDef](./type_defs.md#deprecatethingtyperequestrequesttypedef) 

### describe\_account\_audit\_configuration

Gets information about the Device Defender audit settings for this account.

Type annotations and code completion for `#!python session.create_client("iot").describe_account_audit_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_account_audit_configuration.html)

```python
# describe_account_audit_configuration method definition

await def describe_account_audit_configuration(
    self,
) -> DescribeAccountAuditConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountAuditConfigurationResponseTypeDef](./type_defs.md#describeaccountauditconfigurationresponsetypedef) 

### describe\_audit\_finding

Gets information about a single audit finding.

Type annotations and code completion for `#!python session.create_client("iot").describe_audit_finding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_audit_finding.html)

```python
# describe_audit_finding method definition

await def describe_audit_finding(
    self,
    *,
    findingId: str,
) -> DescribeAuditFindingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAuditFindingResponseTypeDef](./type_defs.md#describeauditfindingresponsetypedef) 


```python
# describe_audit_finding method usage example with argument unpacking

kwargs: DescribeAuditFindingRequestRequestTypeDef = {  # (1)
    "findingId": ...,
}

parent.describe_audit_finding(**kwargs)
```

1. See [:material-code-braces: DescribeAuditFindingRequestRequestTypeDef](./type_defs.md#describeauditfindingrequestrequesttypedef) 

### describe\_audit\_mitigation\_actions\_task

Gets information about an audit mitigation task that is used to apply
mitigation actions to a set of audit findings.

Type annotations and code completion for `#!python session.create_client("iot").describe_audit_mitigation_actions_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_audit_mitigation_actions_task.html)

```python
# describe_audit_mitigation_actions_task method definition

await def describe_audit_mitigation_actions_task(
    self,
    *,
    taskId: str,
) -> DescribeAuditMitigationActionsTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAuditMitigationActionsTaskResponseTypeDef](./type_defs.md#describeauditmitigationactionstaskresponsetypedef) 


```python
# describe_audit_mitigation_actions_task method usage example with argument unpacking

kwargs: DescribeAuditMitigationActionsTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.describe_audit_mitigation_actions_task(**kwargs)
```

1. See [:material-code-braces: DescribeAuditMitigationActionsTaskRequestRequestTypeDef](./type_defs.md#describeauditmitigationactionstaskrequestrequesttypedef) 

### describe\_audit\_suppression

Gets information about a Device Defender audit suppression.

Type annotations and code completion for `#!python session.create_client("iot").describe_audit_suppression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_audit_suppression.html)

```python
# describe_audit_suppression method definition

await def describe_audit_suppression(
    self,
    *,
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
) -> DescribeAuditSuppressionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: DescribeAuditSuppressionResponseTypeDef](./type_defs.md#describeauditsuppressionresponsetypedef) 


```python
# describe_audit_suppression method usage example with argument unpacking

kwargs: DescribeAuditSuppressionRequestRequestTypeDef = {  # (1)
    "checkName": ...,
    "resourceIdentifier": ...,
}

parent.describe_audit_suppression(**kwargs)
```

1. See [:material-code-braces: DescribeAuditSuppressionRequestRequestTypeDef](./type_defs.md#describeauditsuppressionrequestrequesttypedef) 

### describe\_audit\_task

Gets information about a Device Defender audit.

Type annotations and code completion for `#!python session.create_client("iot").describe_audit_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_audit_task.html)

```python
# describe_audit_task method definition

await def describe_audit_task(
    self,
    *,
    taskId: str,
) -> DescribeAuditTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAuditTaskResponseTypeDef](./type_defs.md#describeaudittaskresponsetypedef) 


```python
# describe_audit_task method usage example with argument unpacking

kwargs: DescribeAuditTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.describe_audit_task(**kwargs)
```

1. See [:material-code-braces: DescribeAuditTaskRequestRequestTypeDef](./type_defs.md#describeaudittaskrequestrequesttypedef) 

### describe\_authorizer

Describes an authorizer.

Type annotations and code completion for `#!python session.create_client("iot").describe_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_authorizer.html)

```python
# describe_authorizer method definition

await def describe_authorizer(
    self,
    *,
    authorizerName: str,
) -> DescribeAuthorizerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAuthorizerResponseTypeDef](./type_defs.md#describeauthorizerresponsetypedef) 


```python
# describe_authorizer method usage example with argument unpacking

kwargs: DescribeAuthorizerRequestRequestTypeDef = {  # (1)
    "authorizerName": ...,
}

parent.describe_authorizer(**kwargs)
```

1. See [:material-code-braces: DescribeAuthorizerRequestRequestTypeDef](./type_defs.md#describeauthorizerrequestrequesttypedef) 

### describe\_billing\_group

Returns information about a billing group.

Type annotations and code completion for `#!python session.create_client("iot").describe_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_billing_group.html)

```python
# describe_billing_group method definition

await def describe_billing_group(
    self,
    *,
    billingGroupName: str,
) -> DescribeBillingGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBillingGroupResponseTypeDef](./type_defs.md#describebillinggroupresponsetypedef) 


```python
# describe_billing_group method usage example with argument unpacking

kwargs: DescribeBillingGroupRequestRequestTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.describe_billing_group(**kwargs)
```

1. See [:material-code-braces: DescribeBillingGroupRequestRequestTypeDef](./type_defs.md#describebillinggrouprequestrequesttypedef) 

### describe\_ca\_certificate

Describes a registered CA certificate.

Type annotations and code completion for `#!python session.create_client("iot").describe_ca_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_ca_certificate.html)

```python
# describe_ca_certificate method definition

await def describe_ca_certificate(
    self,
    *,
    certificateId: str,
) -> DescribeCACertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCACertificateResponseTypeDef](./type_defs.md#describecacertificateresponsetypedef) 


```python
# describe_ca_certificate method usage example with argument unpacking

kwargs: DescribeCACertificateRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.describe_ca_certificate(**kwargs)
```

1. See [:material-code-braces: DescribeCACertificateRequestRequestTypeDef](./type_defs.md#describecacertificaterequestrequesttypedef) 

### describe\_certificate

Gets information about the specified certificate.

Type annotations and code completion for `#!python session.create_client("iot").describe_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_certificate.html)

```python
# describe_certificate method definition

await def describe_certificate(
    self,
    *,
    certificateId: str,
) -> DescribeCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef) 


```python
# describe_certificate method usage example with argument unpacking

kwargs: DescribeCertificateRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.describe_certificate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificateRequestRequestTypeDef](./type_defs.md#describecertificaterequestrequesttypedef) 

### describe\_certificate\_provider

Describes a certificate provider.

Type annotations and code completion for `#!python session.create_client("iot").describe_certificate_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_certificate_provider.html)

```python
# describe_certificate_provider method definition

await def describe_certificate_provider(
    self,
    *,
    certificateProviderName: str,
) -> DescribeCertificateProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCertificateProviderResponseTypeDef](./type_defs.md#describecertificateproviderresponsetypedef) 


```python
# describe_certificate_provider method usage example with argument unpacking

kwargs: DescribeCertificateProviderRequestRequestTypeDef = {  # (1)
    "certificateProviderName": ...,
}

parent.describe_certificate_provider(**kwargs)
```

1. See [:material-code-braces: DescribeCertificateProviderRequestRequestTypeDef](./type_defs.md#describecertificateproviderrequestrequesttypedef) 

### describe\_custom\_metric

Gets information about a Device Defender detect custom metric.

Type annotations and code completion for `#!python session.create_client("iot").describe_custom_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_custom_metric.html)

```python
# describe_custom_metric method definition

await def describe_custom_metric(
    self,
    *,
    metricName: str,
) -> DescribeCustomMetricResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCustomMetricResponseTypeDef](./type_defs.md#describecustommetricresponsetypedef) 


```python
# describe_custom_metric method usage example with argument unpacking

kwargs: DescribeCustomMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
}

parent.describe_custom_metric(**kwargs)
```

1. See [:material-code-braces: DescribeCustomMetricRequestRequestTypeDef](./type_defs.md#describecustommetricrequestrequesttypedef) 

### describe\_default\_authorizer

Describes the default authorizer.

Type annotations and code completion for `#!python session.create_client("iot").describe_default_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_default_authorizer.html)

```python
# describe_default_authorizer method definition

await def describe_default_authorizer(
    self,
) -> DescribeDefaultAuthorizerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDefaultAuthorizerResponseTypeDef](./type_defs.md#describedefaultauthorizerresponsetypedef) 

### describe\_detect\_mitigation\_actions\_task

Gets information about a Device Defender ML Detect mitigation action.

Type annotations and code completion for `#!python session.create_client("iot").describe_detect_mitigation_actions_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_detect_mitigation_actions_task.html)

```python
# describe_detect_mitigation_actions_task method definition

await def describe_detect_mitigation_actions_task(
    self,
    *,
    taskId: str,
) -> DescribeDetectMitigationActionsTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDetectMitigationActionsTaskResponseTypeDef](./type_defs.md#describedetectmitigationactionstaskresponsetypedef) 


```python
# describe_detect_mitigation_actions_task method usage example with argument unpacking

kwargs: DescribeDetectMitigationActionsTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.describe_detect_mitigation_actions_task(**kwargs)
```

1. See [:material-code-braces: DescribeDetectMitigationActionsTaskRequestRequestTypeDef](./type_defs.md#describedetectmitigationactionstaskrequestrequesttypedef) 

### describe\_dimension

Provides details about a dimension that is defined in your Amazon Web Services
accounts.

Type annotations and code completion for `#!python session.create_client("iot").describe_dimension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_dimension.html)

```python
# describe_dimension method definition

await def describe_dimension(
    self,
    *,
    name: str,
) -> DescribeDimensionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDimensionResponseTypeDef](./type_defs.md#describedimensionresponsetypedef) 


```python
# describe_dimension method usage example with argument unpacking

kwargs: DescribeDimensionRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.describe_dimension(**kwargs)
```

1. See [:material-code-braces: DescribeDimensionRequestRequestTypeDef](./type_defs.md#describedimensionrequestrequesttypedef) 

### describe\_domain\_configuration

Gets summary information about a domain configuration.

Type annotations and code completion for `#!python session.create_client("iot").describe_domain_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_domain_configuration.html)

```python
# describe_domain_configuration method definition

await def describe_domain_configuration(
    self,
    *,
    domainConfigurationName: str,
) -> DescribeDomainConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainConfigurationResponseTypeDef](./type_defs.md#describedomainconfigurationresponsetypedef) 


```python
# describe_domain_configuration method usage example with argument unpacking

kwargs: DescribeDomainConfigurationRequestRequestTypeDef = {  # (1)
    "domainConfigurationName": ...,
}

parent.describe_domain_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeDomainConfigurationRequestRequestTypeDef](./type_defs.md#describedomainconfigurationrequestrequesttypedef) 

### describe\_endpoint

Returns or creates a unique endpoint specific to the Amazon Web Services
account making the call.

Type annotations and code completion for `#!python session.create_client("iot").describe_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_endpoint.html)

```python
# describe_endpoint method definition

await def describe_endpoint(
    self,
    *,
    endpointType: str = ...,
) -> DescribeEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEndpointResponseTypeDef](./type_defs.md#describeendpointresponsetypedef) 


```python
# describe_endpoint method usage example with argument unpacking

kwargs: DescribeEndpointRequestRequestTypeDef = {  # (1)
    "endpointType": ...,
}

parent.describe_endpoint(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointRequestRequestTypeDef](./type_defs.md#describeendpointrequestrequesttypedef) 

### describe\_event\_configurations

Describes event configurations.

Type annotations and code completion for `#!python session.create_client("iot").describe_event_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_event_configurations.html)

```python
# describe_event_configurations method definition

await def describe_event_configurations(
    self,
) -> DescribeEventConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEventConfigurationsResponseTypeDef](./type_defs.md#describeeventconfigurationsresponsetypedef) 

### describe\_fleet\_metric

Gets information about the specified fleet metric.

Type annotations and code completion for `#!python session.create_client("iot").describe_fleet_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_fleet_metric.html)

```python
# describe_fleet_metric method definition

await def describe_fleet_metric(
    self,
    *,
    metricName: str,
) -> DescribeFleetMetricResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetMetricResponseTypeDef](./type_defs.md#describefleetmetricresponsetypedef) 


```python
# describe_fleet_metric method usage example with argument unpacking

kwargs: DescribeFleetMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
}

parent.describe_fleet_metric(**kwargs)
```

1. See [:material-code-braces: DescribeFleetMetricRequestRequestTypeDef](./type_defs.md#describefleetmetricrequestrequesttypedef) 

### describe\_index

Describes a search index.

Type annotations and code completion for `#!python session.create_client("iot").describe_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_index.html)

```python
# describe_index method definition

await def describe_index(
    self,
    *,
    indexName: str,
) -> DescribeIndexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIndexResponseTypeDef](./type_defs.md#describeindexresponsetypedef) 


```python
# describe_index method usage example with argument unpacking

kwargs: DescribeIndexRequestRequestTypeDef = {  # (1)
    "indexName": ...,
}

parent.describe_index(**kwargs)
```

1. See [:material-code-braces: DescribeIndexRequestRequestTypeDef](./type_defs.md#describeindexrequestrequesttypedef) 

### describe\_job

Describes a job.

Type annotations and code completion for `#!python session.create_client("iot").describe_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_job.html)

```python
# describe_job method definition

await def describe_job(
    self,
    *,
    jobId: str,
    beforeSubstitution: bool = ...,
) -> DescribeJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobResponseTypeDef](./type_defs.md#describejobresponsetypedef) 


```python
# describe_job method usage example with argument unpacking

kwargs: DescribeJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.describe_job(**kwargs)
```

1. See [:material-code-braces: DescribeJobRequestRequestTypeDef](./type_defs.md#describejobrequestrequesttypedef) 

### describe\_job\_execution

Describes a job execution.

Type annotations and code completion for `#!python session.create_client("iot").describe_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_job_execution.html)

```python
# describe_job_execution method definition

await def describe_job_execution(
    self,
    *,
    jobId: str,
    thingName: str,
    executionNumber: int = ...,
) -> DescribeJobExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobExecutionResponseTypeDef](./type_defs.md#describejobexecutionresponsetypedef) 


```python
# describe_job_execution method usage example with argument unpacking

kwargs: DescribeJobExecutionRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "thingName": ...,
}

parent.describe_job_execution(**kwargs)
```

1. See [:material-code-braces: DescribeJobExecutionRequestRequestTypeDef](./type_defs.md#describejobexecutionrequestrequesttypedef) 

### describe\_job\_template

Returns information about a job template.

Type annotations and code completion for `#!python session.create_client("iot").describe_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_job_template.html)

```python
# describe_job_template method definition

await def describe_job_template(
    self,
    *,
    jobTemplateId: str,
) -> DescribeJobTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobTemplateResponseTypeDef](./type_defs.md#describejobtemplateresponsetypedef) 


```python
# describe_job_template method usage example with argument unpacking

kwargs: DescribeJobTemplateRequestRequestTypeDef = {  # (1)
    "jobTemplateId": ...,
}

parent.describe_job_template(**kwargs)
```

1. See [:material-code-braces: DescribeJobTemplateRequestRequestTypeDef](./type_defs.md#describejobtemplaterequestrequesttypedef) 

### describe\_managed\_job\_template

View details of a managed job template.

Type annotations and code completion for `#!python session.create_client("iot").describe_managed_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_managed_job_template.html)

```python
# describe_managed_job_template method definition

await def describe_managed_job_template(
    self,
    *,
    templateName: str,
    templateVersion: str = ...,
) -> DescribeManagedJobTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeManagedJobTemplateResponseTypeDef](./type_defs.md#describemanagedjobtemplateresponsetypedef) 


```python
# describe_managed_job_template method usage example with argument unpacking

kwargs: DescribeManagedJobTemplateRequestRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.describe_managed_job_template(**kwargs)
```

1. See [:material-code-braces: DescribeManagedJobTemplateRequestRequestTypeDef](./type_defs.md#describemanagedjobtemplaterequestrequesttypedef) 

### describe\_mitigation\_action

Gets information about a mitigation action.

Type annotations and code completion for `#!python session.create_client("iot").describe_mitigation_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_mitigation_action.html)

```python
# describe_mitigation_action method definition

await def describe_mitigation_action(
    self,
    *,
    actionName: str,
) -> DescribeMitigationActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMitigationActionResponseTypeDef](./type_defs.md#describemitigationactionresponsetypedef) 


```python
# describe_mitigation_action method usage example with argument unpacking

kwargs: DescribeMitigationActionRequestRequestTypeDef = {  # (1)
    "actionName": ...,
}

parent.describe_mitigation_action(**kwargs)
```

1. See [:material-code-braces: DescribeMitigationActionRequestRequestTypeDef](./type_defs.md#describemitigationactionrequestrequesttypedef) 

### describe\_provisioning\_template

Returns information about a provisioning template.

Type annotations and code completion for `#!python session.create_client("iot").describe_provisioning_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_provisioning_template.html)

```python
# describe_provisioning_template method definition

await def describe_provisioning_template(
    self,
    *,
    templateName: str,
) -> DescribeProvisioningTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProvisioningTemplateResponseTypeDef](./type_defs.md#describeprovisioningtemplateresponsetypedef) 


```python
# describe_provisioning_template method usage example with argument unpacking

kwargs: DescribeProvisioningTemplateRequestRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.describe_provisioning_template(**kwargs)
```

1. See [:material-code-braces: DescribeProvisioningTemplateRequestRequestTypeDef](./type_defs.md#describeprovisioningtemplaterequestrequesttypedef) 

### describe\_provisioning\_template\_version

Returns information about a provisioning template version.

Type annotations and code completion for `#!python session.create_client("iot").describe_provisioning_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_provisioning_template_version.html)

```python
# describe_provisioning_template_version method definition

await def describe_provisioning_template_version(
    self,
    *,
    templateName: str,
    versionId: int,
) -> DescribeProvisioningTemplateVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProvisioningTemplateVersionResponseTypeDef](./type_defs.md#describeprovisioningtemplateversionresponsetypedef) 


```python
# describe_provisioning_template_version method usage example with argument unpacking

kwargs: DescribeProvisioningTemplateVersionRequestRequestTypeDef = {  # (1)
    "templateName": ...,
    "versionId": ...,
}

parent.describe_provisioning_template_version(**kwargs)
```

1. See [:material-code-braces: DescribeProvisioningTemplateVersionRequestRequestTypeDef](./type_defs.md#describeprovisioningtemplateversionrequestrequesttypedef) 

### describe\_role\_alias

Describes a role alias.

Type annotations and code completion for `#!python session.create_client("iot").describe_role_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_role_alias.html)

```python
# describe_role_alias method definition

await def describe_role_alias(
    self,
    *,
    roleAlias: str,
) -> DescribeRoleAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRoleAliasResponseTypeDef](./type_defs.md#describerolealiasresponsetypedef) 


```python
# describe_role_alias method usage example with argument unpacking

kwargs: DescribeRoleAliasRequestRequestTypeDef = {  # (1)
    "roleAlias": ...,
}

parent.describe_role_alias(**kwargs)
```

1. See [:material-code-braces: DescribeRoleAliasRequestRequestTypeDef](./type_defs.md#describerolealiasrequestrequesttypedef) 

### describe\_scheduled\_audit

Gets information about a scheduled audit.

Type annotations and code completion for `#!python session.create_client("iot").describe_scheduled_audit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_scheduled_audit.html)

```python
# describe_scheduled_audit method definition

await def describe_scheduled_audit(
    self,
    *,
    scheduledAuditName: str,
) -> DescribeScheduledAuditResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeScheduledAuditResponseTypeDef](./type_defs.md#describescheduledauditresponsetypedef) 


```python
# describe_scheduled_audit method usage example with argument unpacking

kwargs: DescribeScheduledAuditRequestRequestTypeDef = {  # (1)
    "scheduledAuditName": ...,
}

parent.describe_scheduled_audit(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledAuditRequestRequestTypeDef](./type_defs.md#describescheduledauditrequestrequesttypedef) 

### describe\_security\_profile

Gets information about a Device Defender security profile.

Type annotations and code completion for `#!python session.create_client("iot").describe_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_security_profile.html)

```python
# describe_security_profile method definition

await def describe_security_profile(
    self,
    *,
    securityProfileName: str,
) -> DescribeSecurityProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSecurityProfileResponseTypeDef](./type_defs.md#describesecurityprofileresponsetypedef) 


```python
# describe_security_profile method usage example with argument unpacking

kwargs: DescribeSecurityProfileRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.describe_security_profile(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityProfileRequestRequestTypeDef](./type_defs.md#describesecurityprofilerequestrequesttypedef) 

### describe\_stream

Gets information about a stream.

Type annotations and code completion for `#!python session.create_client("iot").describe_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_stream.html)

```python
# describe_stream method definition

await def describe_stream(
    self,
    *,
    streamId: str,
) -> DescribeStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStreamResponseTypeDef](./type_defs.md#describestreamresponsetypedef) 


```python
# describe_stream method usage example with argument unpacking

kwargs: DescribeStreamRequestRequestTypeDef = {  # (1)
    "streamId": ...,
}

parent.describe_stream(**kwargs)
```

1. See [:material-code-braces: DescribeStreamRequestRequestTypeDef](./type_defs.md#describestreamrequestrequesttypedef) 

### describe\_thing

Gets information about the specified thing.

Type annotations and code completion for `#!python session.create_client("iot").describe_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_thing.html)

```python
# describe_thing method definition

await def describe_thing(
    self,
    *,
    thingName: str,
) -> DescribeThingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThingResponseTypeDef](./type_defs.md#describethingresponsetypedef) 


```python
# describe_thing method usage example with argument unpacking

kwargs: DescribeThingRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.describe_thing(**kwargs)
```

1. See [:material-code-braces: DescribeThingRequestRequestTypeDef](./type_defs.md#describethingrequestrequesttypedef) 

### describe\_thing\_group

Describe a thing group.

Type annotations and code completion for `#!python session.create_client("iot").describe_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_thing_group.html)

```python
# describe_thing_group method definition

await def describe_thing_group(
    self,
    *,
    thingGroupName: str,
) -> DescribeThingGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThingGroupResponseTypeDef](./type_defs.md#describethinggroupresponsetypedef) 


```python
# describe_thing_group method usage example with argument unpacking

kwargs: DescribeThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.describe_thing_group(**kwargs)
```

1. See [:material-code-braces: DescribeThingGroupRequestRequestTypeDef](./type_defs.md#describethinggrouprequestrequesttypedef) 

### describe\_thing\_registration\_task

Describes a bulk thing provisioning task.

Type annotations and code completion for `#!python session.create_client("iot").describe_thing_registration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_thing_registration_task.html)

```python
# describe_thing_registration_task method definition

await def describe_thing_registration_task(
    self,
    *,
    taskId: str,
) -> DescribeThingRegistrationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThingRegistrationTaskResponseTypeDef](./type_defs.md#describethingregistrationtaskresponsetypedef) 


```python
# describe_thing_registration_task method usage example with argument unpacking

kwargs: DescribeThingRegistrationTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.describe_thing_registration_task(**kwargs)
```

1. See [:material-code-braces: DescribeThingRegistrationTaskRequestRequestTypeDef](./type_defs.md#describethingregistrationtaskrequestrequesttypedef) 

### describe\_thing\_type

Gets information about the specified thing type.

Type annotations and code completion for `#!python session.create_client("iot").describe_thing_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/describe_thing_type.html)

```python
# describe_thing_type method definition

await def describe_thing_type(
    self,
    *,
    thingTypeName: str,
) -> DescribeThingTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThingTypeResponseTypeDef](./type_defs.md#describethingtyperesponsetypedef) 


```python
# describe_thing_type method usage example with argument unpacking

kwargs: DescribeThingTypeRequestRequestTypeDef = {  # (1)
    "thingTypeName": ...,
}

parent.describe_thing_type(**kwargs)
```

1. See [:material-code-braces: DescribeThingTypeRequestRequestTypeDef](./type_defs.md#describethingtyperequestrequesttypedef) 

### detach\_policy

Detaches a policy from the specified target.

Type annotations and code completion for `#!python session.create_client("iot").detach_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/detach_policy.html)

```python
# detach_policy method definition

await def detach_policy(
    self,
    *,
    policyName: str,
    target: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# detach_policy method usage example with argument unpacking

kwargs: DetachPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "target": ...,
}

parent.detach_policy(**kwargs)
```

1. See [:material-code-braces: DetachPolicyRequestRequestTypeDef](./type_defs.md#detachpolicyrequestrequesttypedef) 

### detach\_principal\_policy

Removes the specified policy from the specified certificate.

Type annotations and code completion for `#!python session.create_client("iot").detach_principal_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/detach_principal_policy.html)

```python
# detach_principal_policy method definition

await def detach_principal_policy(
    self,
    *,
    policyName: str,
    principal: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# detach_principal_policy method usage example with argument unpacking

kwargs: DetachPrincipalPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "principal": ...,
}

parent.detach_principal_policy(**kwargs)
```

1. See [:material-code-braces: DetachPrincipalPolicyRequestRequestTypeDef](./type_defs.md#detachprincipalpolicyrequestrequesttypedef) 

### detach\_security\_profile

Disassociates a Device Defender security profile from a thing group or from
this account.

Type annotations and code completion for `#!python session.create_client("iot").detach_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/detach_security_profile.html)

```python
# detach_security_profile method definition

await def detach_security_profile(
    self,
    *,
    securityProfileName: str,
    securityProfileTargetArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# detach_security_profile method usage example with argument unpacking

kwargs: DetachSecurityProfileRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
    "securityProfileTargetArn": ...,
}

parent.detach_security_profile(**kwargs)
```

1. See [:material-code-braces: DetachSecurityProfileRequestRequestTypeDef](./type_defs.md#detachsecurityprofilerequestrequesttypedef) 

### detach\_thing\_principal

Detaches the specified principal from the specified thing.

Type annotations and code completion for `#!python session.create_client("iot").detach_thing_principal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/detach_thing_principal.html)

```python
# detach_thing_principal method definition

await def detach_thing_principal(
    self,
    *,
    thingName: str,
    principal: str,
) -> Dict[str, Any]:
    ...
```



```python
# detach_thing_principal method usage example with argument unpacking

kwargs: DetachThingPrincipalRequestRequestTypeDef = {  # (1)
    "thingName": ...,
    "principal": ...,
}

parent.detach_thing_principal(**kwargs)
```

1. See [:material-code-braces: DetachThingPrincipalRequestRequestTypeDef](./type_defs.md#detachthingprincipalrequestrequesttypedef) 

### disable\_topic\_rule

Disables the rule.

Type annotations and code completion for `#!python session.create_client("iot").disable_topic_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/disable_topic_rule.html)

```python
# disable_topic_rule method definition

await def disable_topic_rule(
    self,
    *,
    ruleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disable_topic_rule method usage example with argument unpacking

kwargs: DisableTopicRuleRequestRequestTypeDef = {  # (1)
    "ruleName": ...,
}

parent.disable_topic_rule(**kwargs)
```

1. See [:material-code-braces: DisableTopicRuleRequestRequestTypeDef](./type_defs.md#disabletopicrulerequestrequesttypedef) 

### disassociate\_sbom\_from\_package\_version

Disassociates the selected software bill of materials (SBOM) from a specific
software package version.

Type annotations and code completion for `#!python session.create_client("iot").disassociate_sbom_from_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/disassociate_sbom_from_package_version.html)

```python
# disassociate_sbom_from_package_version method definition

await def disassociate_sbom_from_package_version(
    self,
    *,
    packageName: str,
    versionName: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_sbom_from_package_version method usage example with argument unpacking

kwargs: DisassociateSbomFromPackageVersionRequestRequestTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
}

parent.disassociate_sbom_from_package_version(**kwargs)
```

1. See [:material-code-braces: DisassociateSbomFromPackageVersionRequestRequestTypeDef](./type_defs.md#disassociatesbomfrompackageversionrequestrequesttypedef) 

### enable\_topic\_rule

Enables the rule.

Type annotations and code completion for `#!python session.create_client("iot").enable_topic_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/enable_topic_rule.html)

```python
# enable_topic_rule method definition

await def enable_topic_rule(
    self,
    *,
    ruleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_topic_rule method usage example with argument unpacking

kwargs: EnableTopicRuleRequestRequestTypeDef = {  # (1)
    "ruleName": ...,
}

parent.enable_topic_rule(**kwargs)
```

1. See [:material-code-braces: EnableTopicRuleRequestRequestTypeDef](./type_defs.md#enabletopicrulerequestrequesttypedef) 

### get\_behavior\_model\_training\_summaries

Returns a Device Defender's ML Detect Security Profile training model's status.

Type annotations and code completion for `#!python session.create_client("iot").get_behavior_model_training_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_behavior_model_training_summaries.html)

```python
# get_behavior_model_training_summaries method definition

await def get_behavior_model_training_summaries(
    self,
    *,
    securityProfileName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetBehaviorModelTrainingSummariesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBehaviorModelTrainingSummariesResponseTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesresponsetypedef) 


```python
# get_behavior_model_training_summaries method usage example with argument unpacking

kwargs: GetBehaviorModelTrainingSummariesRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.get_behavior_model_training_summaries(**kwargs)
```

1. See [:material-code-braces: GetBehaviorModelTrainingSummariesRequestRequestTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesrequestrequesttypedef) 

### get\_buckets\_aggregation

Aggregates on indexed data with search queries pertaining to particular fields.

Type annotations and code completion for `#!python session.create_client("iot").get_buckets_aggregation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_buckets_aggregation.html)

```python
# get_buckets_aggregation method definition

await def get_buckets_aggregation(
    self,
    *,
    queryString: str,
    aggregationField: str,
    bucketsAggregationType: BucketsAggregationTypeTypeDef,  # (1)
    indexName: str = ...,
    queryVersion: str = ...,
) -> GetBucketsAggregationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BucketsAggregationTypeTypeDef](./type_defs.md#bucketsaggregationtypetypedef) 
2. See [:material-code-braces: GetBucketsAggregationResponseTypeDef](./type_defs.md#getbucketsaggregationresponsetypedef) 


```python
# get_buckets_aggregation method usage example with argument unpacking

kwargs: GetBucketsAggregationRequestRequestTypeDef = {  # (1)
    "queryString": ...,
    "aggregationField": ...,
    "bucketsAggregationType": ...,
}

parent.get_buckets_aggregation(**kwargs)
```

1. See [:material-code-braces: GetBucketsAggregationRequestRequestTypeDef](./type_defs.md#getbucketsaggregationrequestrequesttypedef) 

### get\_cardinality

Returns the approximate count of unique values that match the query.

Type annotations and code completion for `#!python session.create_client("iot").get_cardinality` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_cardinality.html)

```python
# get_cardinality method definition

await def get_cardinality(
    self,
    *,
    queryString: str,
    indexName: str = ...,
    aggregationField: str = ...,
    queryVersion: str = ...,
) -> GetCardinalityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCardinalityResponseTypeDef](./type_defs.md#getcardinalityresponsetypedef) 


```python
# get_cardinality method usage example with argument unpacking

kwargs: GetCardinalityRequestRequestTypeDef = {  # (1)
    "queryString": ...,
}

parent.get_cardinality(**kwargs)
```

1. See [:material-code-braces: GetCardinalityRequestRequestTypeDef](./type_defs.md#getcardinalityrequestrequesttypedef) 

### get\_command

Gets information about the specified command.

Type annotations and code completion for `#!python session.create_client("iot").get_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_command.html)

```python
# get_command method definition

await def get_command(
    self,
    *,
    commandId: str,
) -> GetCommandResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCommandResponseTypeDef](./type_defs.md#getcommandresponsetypedef) 


```python
# get_command method usage example with argument unpacking

kwargs: GetCommandRequestRequestTypeDef = {  # (1)
    "commandId": ...,
}

parent.get_command(**kwargs)
```

1. See [:material-code-braces: GetCommandRequestRequestTypeDef](./type_defs.md#getcommandrequestrequesttypedef) 

### get\_command\_execution

Gets information about the specific command execution on a single device.

Type annotations and code completion for `#!python session.create_client("iot").get_command_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_command_execution.html)

```python
# get_command_execution method definition

await def get_command_execution(
    self,
    *,
    executionId: str,
    targetArn: str,
    includeResult: bool = ...,
) -> GetCommandExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCommandExecutionResponseTypeDef](./type_defs.md#getcommandexecutionresponsetypedef) 


```python
# get_command_execution method usage example with argument unpacking

kwargs: GetCommandExecutionRequestRequestTypeDef = {  # (1)
    "executionId": ...,
    "targetArn": ...,
}

parent.get_command_execution(**kwargs)
```

1. See [:material-code-braces: GetCommandExecutionRequestRequestTypeDef](./type_defs.md#getcommandexecutionrequestrequesttypedef) 

### get\_effective\_policies

Gets a list of the policies that have an effect on the authorization behavior
of the specified device when it connects to the IoT device gateway.

Type annotations and code completion for `#!python session.create_client("iot").get_effective_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_effective_policies.html)

```python
# get_effective_policies method definition

await def get_effective_policies(
    self,
    *,
    principal: str = ...,
    cognitoIdentityPoolId: str = ...,
    thingName: str = ...,
) -> GetEffectivePoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEffectivePoliciesResponseTypeDef](./type_defs.md#geteffectivepoliciesresponsetypedef) 


```python
# get_effective_policies method usage example with argument unpacking

kwargs: GetEffectivePoliciesRequestRequestTypeDef = {  # (1)
    "principal": ...,
}

parent.get_effective_policies(**kwargs)
```

1. See [:material-code-braces: GetEffectivePoliciesRequestRequestTypeDef](./type_defs.md#geteffectivepoliciesrequestrequesttypedef) 

### get\_indexing\_configuration

Gets the indexing configuration.

Type annotations and code completion for `#!python session.create_client("iot").get_indexing_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_indexing_configuration.html)

```python
# get_indexing_configuration method definition

await def get_indexing_configuration(
    self,
) -> GetIndexingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIndexingConfigurationResponseTypeDef](./type_defs.md#getindexingconfigurationresponsetypedef) 

### get\_job\_document

Gets a job document.

Type annotations and code completion for `#!python session.create_client("iot").get_job_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_job_document.html)

```python
# get_job_document method definition

await def get_job_document(
    self,
    *,
    jobId: str,
    beforeSubstitution: bool = ...,
) -> GetJobDocumentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobDocumentResponseTypeDef](./type_defs.md#getjobdocumentresponsetypedef) 


```python
# get_job_document method usage example with argument unpacking

kwargs: GetJobDocumentRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.get_job_document(**kwargs)
```

1. See [:material-code-braces: GetJobDocumentRequestRequestTypeDef](./type_defs.md#getjobdocumentrequestrequesttypedef) 

### get\_logging\_options

Gets the logging options.

Type annotations and code completion for `#!python session.create_client("iot").get_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_logging_options.html)

```python
# get_logging_options method definition

await def get_logging_options(
    self,
) -> GetLoggingOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLoggingOptionsResponseTypeDef](./type_defs.md#getloggingoptionsresponsetypedef) 

### get\_ota\_update

Gets an OTA update.

Type annotations and code completion for `#!python session.create_client("iot").get_ota_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_ota_update.html)

```python
# get_ota_update method definition

await def get_ota_update(
    self,
    *,
    otaUpdateId: str,
) -> GetOTAUpdateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOTAUpdateResponseTypeDef](./type_defs.md#getotaupdateresponsetypedef) 


```python
# get_ota_update method usage example with argument unpacking

kwargs: GetOTAUpdateRequestRequestTypeDef = {  # (1)
    "otaUpdateId": ...,
}

parent.get_ota_update(**kwargs)
```

1. See [:material-code-braces: GetOTAUpdateRequestRequestTypeDef](./type_defs.md#getotaupdaterequestrequesttypedef) 

### get\_package

Gets information about the specified software package.

Type annotations and code completion for `#!python session.create_client("iot").get_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_package.html)

```python
# get_package method definition

await def get_package(
    self,
    *,
    packageName: str,
) -> GetPackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPackageResponseTypeDef](./type_defs.md#getpackageresponsetypedef) 


```python
# get_package method usage example with argument unpacking

kwargs: GetPackageRequestRequestTypeDef = {  # (1)
    "packageName": ...,
}

parent.get_package(**kwargs)
```

1. See [:material-code-braces: GetPackageRequestRequestTypeDef](./type_defs.md#getpackagerequestrequesttypedef) 

### get\_package\_configuration

Gets information about the specified software package's configuration.

Type annotations and code completion for `#!python session.create_client("iot").get_package_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_package_configuration.html)

```python
# get_package_configuration method definition

await def get_package_configuration(
    self,
) -> GetPackageConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPackageConfigurationResponseTypeDef](./type_defs.md#getpackageconfigurationresponsetypedef) 

### get\_package\_version

Gets information about the specified package version.

Type annotations and code completion for `#!python session.create_client("iot").get_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_package_version.html)

```python
# get_package_version method definition

await def get_package_version(
    self,
    *,
    packageName: str,
    versionName: str,
) -> GetPackageVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPackageVersionResponseTypeDef](./type_defs.md#getpackageversionresponsetypedef) 


```python
# get_package_version method usage example with argument unpacking

kwargs: GetPackageVersionRequestRequestTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
}

parent.get_package_version(**kwargs)
```

1. See [:material-code-braces: GetPackageVersionRequestRequestTypeDef](./type_defs.md#getpackageversionrequestrequesttypedef) 

### get\_percentiles

Groups the aggregated values that match the query into percentile groupings.

Type annotations and code completion for `#!python session.create_client("iot").get_percentiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_percentiles.html)

```python
# get_percentiles method definition

await def get_percentiles(
    self,
    *,
    queryString: str,
    indexName: str = ...,
    aggregationField: str = ...,
    queryVersion: str = ...,
    percents: Sequence[float] = ...,
) -> GetPercentilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPercentilesResponseTypeDef](./type_defs.md#getpercentilesresponsetypedef) 


```python
# get_percentiles method usage example with argument unpacking

kwargs: GetPercentilesRequestRequestTypeDef = {  # (1)
    "queryString": ...,
}

parent.get_percentiles(**kwargs)
```

1. See [:material-code-braces: GetPercentilesRequestRequestTypeDef](./type_defs.md#getpercentilesrequestrequesttypedef) 

### get\_policy

Gets information about the specified policy with the policy document of the
default version.

Type annotations and code completion for `#!python session.create_client("iot").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_policy.html)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    policyName: str,
) -> GetPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef) 

### get\_policy\_version

Gets information about the specified policy version.

Type annotations and code completion for `#!python session.create_client("iot").get_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_policy_version.html)

```python
# get_policy_version method definition

await def get_policy_version(
    self,
    *,
    policyName: str,
    policyVersionId: str,
) -> GetPolicyVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyVersionResponseTypeDef](./type_defs.md#getpolicyversionresponsetypedef) 


```python
# get_policy_version method usage example with argument unpacking

kwargs: GetPolicyVersionRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "policyVersionId": ...,
}

parent.get_policy_version(**kwargs)
```

1. See [:material-code-braces: GetPolicyVersionRequestRequestTypeDef](./type_defs.md#getpolicyversionrequestrequesttypedef) 

### get\_registration\_code

Gets a registration code used to register a CA certificate with IoT.

Type annotations and code completion for `#!python session.create_client("iot").get_registration_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_registration_code.html)

```python
# get_registration_code method definition

await def get_registration_code(
    self,
) -> GetRegistrationCodeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRegistrationCodeResponseTypeDef](./type_defs.md#getregistrationcoderesponsetypedef) 

### get\_statistics

Returns the count, average, sum, minimum, maximum, sum of squares, variance,
and standard deviation for the specified aggregated field.

Type annotations and code completion for `#!python session.create_client("iot").get_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_statistics.html)

```python
# get_statistics method definition

await def get_statistics(
    self,
    *,
    queryString: str,
    indexName: str = ...,
    aggregationField: str = ...,
    queryVersion: str = ...,
) -> GetStatisticsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStatisticsResponseTypeDef](./type_defs.md#getstatisticsresponsetypedef) 


```python
# get_statistics method usage example with argument unpacking

kwargs: GetStatisticsRequestRequestTypeDef = {  # (1)
    "queryString": ...,
}

parent.get_statistics(**kwargs)
```

1. See [:material-code-braces: GetStatisticsRequestRequestTypeDef](./type_defs.md#getstatisticsrequestrequesttypedef) 

### get\_thing\_connectivity\_data

Retrieves the live connectivity status per device.

Type annotations and code completion for `#!python session.create_client("iot").get_thing_connectivity_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_thing_connectivity_data.html)

```python
# get_thing_connectivity_data method definition

await def get_thing_connectivity_data(
    self,
    *,
    thingName: str,
) -> GetThingConnectivityDataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetThingConnectivityDataResponseTypeDef](./type_defs.md#getthingconnectivitydataresponsetypedef) 


```python
# get_thing_connectivity_data method usage example with argument unpacking

kwargs: GetThingConnectivityDataRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.get_thing_connectivity_data(**kwargs)
```

1. See [:material-code-braces: GetThingConnectivityDataRequestRequestTypeDef](./type_defs.md#getthingconnectivitydatarequestrequesttypedef) 

### get\_topic\_rule

Gets information about the rule.

Type annotations and code completion for `#!python session.create_client("iot").get_topic_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_topic_rule.html)

```python
# get_topic_rule method definition

await def get_topic_rule(
    self,
    *,
    ruleName: str,
) -> GetTopicRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTopicRuleResponseTypeDef](./type_defs.md#gettopicruleresponsetypedef) 


```python
# get_topic_rule method usage example with argument unpacking

kwargs: GetTopicRuleRequestRequestTypeDef = {  # (1)
    "ruleName": ...,
}

parent.get_topic_rule(**kwargs)
```

1. See [:material-code-braces: GetTopicRuleRequestRequestTypeDef](./type_defs.md#gettopicrulerequestrequesttypedef) 

### get\_topic\_rule\_destination

Gets information about a topic rule destination.

Type annotations and code completion for `#!python session.create_client("iot").get_topic_rule_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_topic_rule_destination.html)

```python
# get_topic_rule_destination method definition

await def get_topic_rule_destination(
    self,
    *,
    arn: str,
) -> GetTopicRuleDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTopicRuleDestinationResponseTypeDef](./type_defs.md#gettopicruledestinationresponsetypedef) 


```python
# get_topic_rule_destination method usage example with argument unpacking

kwargs: GetTopicRuleDestinationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_topic_rule_destination(**kwargs)
```

1. See [:material-code-braces: GetTopicRuleDestinationRequestRequestTypeDef](./type_defs.md#gettopicruledestinationrequestrequesttypedef) 

### get\_v2\_logging\_options

Gets the fine grained logging options.

Type annotations and code completion for `#!python session.create_client("iot").get_v2_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/get_v2_logging_options.html)

```python
# get_v2_logging_options method definition

await def get_v2_logging_options(
    self,
) -> GetV2LoggingOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetV2LoggingOptionsResponseTypeDef](./type_defs.md#getv2loggingoptionsresponsetypedef) 

### list\_active\_violations

Lists the active violations for a given Device Defender security profile.

Type annotations and code completion for `#!python session.create_client("iot").list_active_violations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_active_violations.html)

```python
# list_active_violations method definition

await def list_active_violations(
    self,
    *,
    thingName: str = ...,
    securityProfileName: str = ...,
    behaviorCriteriaType: BehaviorCriteriaTypeType = ...,  # (1)
    listSuppressedAlerts: bool = ...,
    verificationState: VerificationStateType = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListActiveViolationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
3. See [:material-code-braces: ListActiveViolationsResponseTypeDef](./type_defs.md#listactiveviolationsresponsetypedef) 


```python
# list_active_violations method usage example with argument unpacking

kwargs: ListActiveViolationsRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_active_violations(**kwargs)
```

1. See [:material-code-braces: ListActiveViolationsRequestRequestTypeDef](./type_defs.md#listactiveviolationsrequestrequesttypedef) 

### list\_attached\_policies

Lists the policies attached to the specified thing group.

Type annotations and code completion for `#!python session.create_client("iot").list_attached_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_attached_policies.html)

```python
# list_attached_policies method definition

await def list_attached_policies(
    self,
    *,
    target: str,
    recursive: bool = ...,
    marker: str = ...,
    pageSize: int = ...,
) -> ListAttachedPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttachedPoliciesResponseTypeDef](./type_defs.md#listattachedpoliciesresponsetypedef) 


```python
# list_attached_policies method usage example with argument unpacking

kwargs: ListAttachedPoliciesRequestRequestTypeDef = {  # (1)
    "target": ...,
}

parent.list_attached_policies(**kwargs)
```

1. See [:material-code-braces: ListAttachedPoliciesRequestRequestTypeDef](./type_defs.md#listattachedpoliciesrequestrequesttypedef) 

### list\_audit\_findings

Lists the findings (results) of a Device Defender audit or of the audits
performed during a specified time period.

Type annotations and code completion for `#!python session.create_client("iot").list_audit_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_audit_findings.html)

```python
# list_audit_findings method definition

await def list_audit_findings(
    self,
    *,
    taskId: str = ...,
    checkName: str = ...,
    resourceIdentifier: ResourceIdentifierTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    listSuppressedFindings: bool = ...,
) -> ListAuditFindingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: ListAuditFindingsResponseTypeDef](./type_defs.md#listauditfindingsresponsetypedef) 


```python
# list_audit_findings method usage example with argument unpacking

kwargs: ListAuditFindingsRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.list_audit_findings(**kwargs)
```

1. See [:material-code-braces: ListAuditFindingsRequestRequestTypeDef](./type_defs.md#listauditfindingsrequestrequesttypedef) 

### list\_audit\_mitigation\_actions\_executions

Gets the status of audit mitigation action tasks that were executed.

Type annotations and code completion for `#!python session.create_client("iot").list_audit_mitigation_actions_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_audit_mitigation_actions_executions.html)

```python
# list_audit_mitigation_actions_executions method definition

await def list_audit_mitigation_actions_executions(
    self,
    *,
    taskId: str,
    findingId: str,
    actionStatus: AuditMitigationActionsExecutionStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAuditMitigationActionsExecutionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuditMitigationActionsExecutionStatusType](./literals.md#auditmitigationactionsexecutionstatustype) 
2. See [:material-code-braces: ListAuditMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listauditmitigationactionsexecutionsresponsetypedef) 


```python
# list_audit_mitigation_actions_executions method usage example with argument unpacking

kwargs: ListAuditMitigationActionsExecutionsRequestRequestTypeDef = {  # (1)
    "taskId": ...,
    "findingId": ...,
}

parent.list_audit_mitigation_actions_executions(**kwargs)
```

1. See [:material-code-braces: ListAuditMitigationActionsExecutionsRequestRequestTypeDef](./type_defs.md#listauditmitigationactionsexecutionsrequestrequesttypedef) 

### list\_audit\_mitigation\_actions\_tasks

Gets a list of audit mitigation action tasks that match the specified filters.

Type annotations and code completion for `#!python session.create_client("iot").list_audit_mitigation_actions_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_audit_mitigation_actions_tasks.html)

```python
# list_audit_mitigation_actions_tasks method definition

await def list_audit_mitigation_actions_tasks(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    auditTaskId: str = ...,
    findingId: str = ...,
    taskStatus: AuditMitigationActionsTaskStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAuditMitigationActionsTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype) 
2. See [:material-code-braces: ListAuditMitigationActionsTasksResponseTypeDef](./type_defs.md#listauditmitigationactionstasksresponsetypedef) 


```python
# list_audit_mitigation_actions_tasks method usage example with argument unpacking

kwargs: ListAuditMitigationActionsTasksRequestRequestTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.list_audit_mitigation_actions_tasks(**kwargs)
```

1. See [:material-code-braces: ListAuditMitigationActionsTasksRequestRequestTypeDef](./type_defs.md#listauditmitigationactionstasksrequestrequesttypedef) 

### list\_audit\_suppressions

Lists your Device Defender audit listings.

Type annotations and code completion for `#!python session.create_client("iot").list_audit_suppressions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_audit_suppressions.html)

```python
# list_audit_suppressions method definition

await def list_audit_suppressions(
    self,
    *,
    checkName: str = ...,
    resourceIdentifier: ResourceIdentifierTypeDef = ...,  # (1)
    ascendingOrder: bool = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAuditSuppressionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: ListAuditSuppressionsResponseTypeDef](./type_defs.md#listauditsuppressionsresponsetypedef) 


```python
# list_audit_suppressions method usage example with argument unpacking

kwargs: ListAuditSuppressionsRequestRequestTypeDef = {  # (1)
    "checkName": ...,
}

parent.list_audit_suppressions(**kwargs)
```

1. See [:material-code-braces: ListAuditSuppressionsRequestRequestTypeDef](./type_defs.md#listauditsuppressionsrequestrequesttypedef) 

### list\_audit\_tasks

Lists the Device Defender audits that have been performed during a given time
period.

Type annotations and code completion for `#!python session.create_client("iot").list_audit_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_audit_tasks.html)

```python
# list_audit_tasks method definition

await def list_audit_tasks(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    taskType: AuditTaskTypeType = ...,  # (1)
    taskStatus: AuditTaskStatusType = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAuditTasksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuditTaskTypeType](./literals.md#audittasktypetype) 
2. See [:material-code-brackets: AuditTaskStatusType](./literals.md#audittaskstatustype) 
3. See [:material-code-braces: ListAuditTasksResponseTypeDef](./type_defs.md#listaudittasksresponsetypedef) 


```python
# list_audit_tasks method usage example with argument unpacking

kwargs: ListAuditTasksRequestRequestTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.list_audit_tasks(**kwargs)
```

1. See [:material-code-braces: ListAuditTasksRequestRequestTypeDef](./type_defs.md#listaudittasksrequestrequesttypedef) 

### list\_authorizers

Lists the authorizers registered in your account.

Type annotations and code completion for `#!python session.create_client("iot").list_authorizers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_authorizers.html)

```python
# list_authorizers method definition

await def list_authorizers(
    self,
    *,
    pageSize: int = ...,
    marker: str = ...,
    ascendingOrder: bool = ...,
    status: AuthorizerStatusType = ...,  # (1)
) -> ListAuthorizersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
2. See [:material-code-braces: ListAuthorizersResponseTypeDef](./type_defs.md#listauthorizersresponsetypedef) 


```python
# list_authorizers method usage example with argument unpacking

kwargs: ListAuthorizersRequestRequestTypeDef = {  # (1)
    "pageSize": ...,
}

parent.list_authorizers(**kwargs)
```

1. See [:material-code-braces: ListAuthorizersRequestRequestTypeDef](./type_defs.md#listauthorizersrequestrequesttypedef) 

### list\_billing\_groups

Lists the billing groups you have created.

Type annotations and code completion for `#!python session.create_client("iot").list_billing_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_billing_groups.html)

```python
# list_billing_groups method definition

await def list_billing_groups(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    namePrefixFilter: str = ...,
) -> ListBillingGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBillingGroupsResponseTypeDef](./type_defs.md#listbillinggroupsresponsetypedef) 


```python
# list_billing_groups method usage example with argument unpacking

kwargs: ListBillingGroupsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_billing_groups(**kwargs)
```

1. See [:material-code-braces: ListBillingGroupsRequestRequestTypeDef](./type_defs.md#listbillinggroupsrequestrequesttypedef) 

### list\_ca\_certificates

Lists the CA certificates registered for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iot").list_ca_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_ca_certificates.html)

```python
# list_ca_certificates method definition

await def list_ca_certificates(
    self,
    *,
    pageSize: int = ...,
    marker: str = ...,
    ascendingOrder: bool = ...,
    templateName: str = ...,
) -> ListCACertificatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCACertificatesResponseTypeDef](./type_defs.md#listcacertificatesresponsetypedef) 


```python
# list_ca_certificates method usage example with argument unpacking

kwargs: ListCACertificatesRequestRequestTypeDef = {  # (1)
    "pageSize": ...,
}

parent.list_ca_certificates(**kwargs)
```

1. See [:material-code-braces: ListCACertificatesRequestRequestTypeDef](./type_defs.md#listcacertificatesrequestrequesttypedef) 

### list\_certificate\_providers

Lists all your certificate providers in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iot").list_certificate_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_certificate_providers.html)

```python
# list_certificate_providers method definition

await def list_certificate_providers(
    self,
    *,
    nextToken: str = ...,
    ascendingOrder: bool = ...,
) -> ListCertificateProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCertificateProvidersResponseTypeDef](./type_defs.md#listcertificateprovidersresponsetypedef) 


```python
# list_certificate_providers method usage example with argument unpacking

kwargs: ListCertificateProvidersRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_certificate_providers(**kwargs)
```

1. See [:material-code-braces: ListCertificateProvidersRequestRequestTypeDef](./type_defs.md#listcertificateprovidersrequestrequesttypedef) 

### list\_certificates

Lists the certificates registered in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iot").list_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_certificates.html)

```python
# list_certificates method definition

await def list_certificates(
    self,
    *,
    pageSize: int = ...,
    marker: str = ...,
    ascendingOrder: bool = ...,
) -> ListCertificatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


```python
# list_certificates method usage example with argument unpacking

kwargs: ListCertificatesRequestRequestTypeDef = {  # (1)
    "pageSize": ...,
}

parent.list_certificates(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestRequestTypeDef](./type_defs.md#listcertificatesrequestrequesttypedef) 

### list\_certificates\_by\_ca

List the device certificates signed by the specified CA certificate.

Type annotations and code completion for `#!python session.create_client("iot").list_certificates_by_ca` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_certificates_by_ca.html)

```python
# list_certificates_by_ca method definition

await def list_certificates_by_ca(
    self,
    *,
    caCertificateId: str,
    pageSize: int = ...,
    marker: str = ...,
    ascendingOrder: bool = ...,
) -> ListCertificatesByCAResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCertificatesByCAResponseTypeDef](./type_defs.md#listcertificatesbycaresponsetypedef) 


```python
# list_certificates_by_ca method usage example with argument unpacking

kwargs: ListCertificatesByCARequestRequestTypeDef = {  # (1)
    "caCertificateId": ...,
}

parent.list_certificates_by_ca(**kwargs)
```

1. See [:material-code-braces: ListCertificatesByCARequestRequestTypeDef](./type_defs.md#listcertificatesbycarequestrequesttypedef) 

### list\_command\_executions

List all command executions.

Type annotations and code completion for `#!python session.create_client("iot").list_command_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_command_executions.html)

```python
# list_command_executions method definition

await def list_command_executions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    namespace: CommandNamespaceType = ...,  # (1)
    status: CommandExecutionStatusType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    startedTimeFilter: TimeFilterTypeDef = ...,  # (4)
    completedTimeFilter: TimeFilterTypeDef = ...,  # (4)
    targetArn: str = ...,
    commandArn: str = ...,
) -> ListCommandExecutionsResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-brackets: CommandExecutionStatusType](./literals.md#commandexecutionstatustype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
5. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
6. See [:material-code-braces: ListCommandExecutionsResponseTypeDef](./type_defs.md#listcommandexecutionsresponsetypedef) 


```python
# list_command_executions method usage example with argument unpacking

kwargs: ListCommandExecutionsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_command_executions(**kwargs)
```

1. See [:material-code-braces: ListCommandExecutionsRequestRequestTypeDef](./type_defs.md#listcommandexecutionsrequestrequesttypedef) 

### list\_commands

List all commands in your account.

Type annotations and code completion for `#!python session.create_client("iot").list_commands` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_commands.html)

```python
# list_commands method definition

await def list_commands(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    namespace: CommandNamespaceType = ...,  # (1)
    commandParameterName: str = ...,
    sortOrder: SortOrderType = ...,  # (2)
) -> ListCommandsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListCommandsResponseTypeDef](./type_defs.md#listcommandsresponsetypedef) 


```python
# list_commands method usage example with argument unpacking

kwargs: ListCommandsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_commands(**kwargs)
```

1. See [:material-code-braces: ListCommandsRequestRequestTypeDef](./type_defs.md#listcommandsrequestrequesttypedef) 

### list\_custom\_metrics

Lists your Device Defender detect custom metrics.

Type annotations and code completion for `#!python session.create_client("iot").list_custom_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_custom_metrics.html)

```python
# list_custom_metrics method definition

await def list_custom_metrics(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCustomMetricsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomMetricsResponseTypeDef](./type_defs.md#listcustommetricsresponsetypedef) 


```python
# list_custom_metrics method usage example with argument unpacking

kwargs: ListCustomMetricsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_custom_metrics(**kwargs)
```

1. See [:material-code-braces: ListCustomMetricsRequestRequestTypeDef](./type_defs.md#listcustommetricsrequestrequesttypedef) 

### list\_detect\_mitigation\_actions\_executions

Lists mitigation actions executions for a Device Defender ML Detect Security
Profile.

Type annotations and code completion for `#!python session.create_client("iot").list_detect_mitigation_actions_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_detect_mitigation_actions_executions.html)

```python
# list_detect_mitigation_actions_executions method definition

await def list_detect_mitigation_actions_executions(
    self,
    *,
    taskId: str = ...,
    violationId: str = ...,
    thingName: str = ...,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDetectMitigationActionsExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDetectMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listdetectmitigationactionsexecutionsresponsetypedef) 


```python
# list_detect_mitigation_actions_executions method usage example with argument unpacking

kwargs: ListDetectMitigationActionsExecutionsRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.list_detect_mitigation_actions_executions(**kwargs)
```

1. See [:material-code-braces: ListDetectMitigationActionsExecutionsRequestRequestTypeDef](./type_defs.md#listdetectmitigationactionsexecutionsrequestrequesttypedef) 

### list\_detect\_mitigation\_actions\_tasks

List of Device Defender ML Detect mitigation actions tasks.

Type annotations and code completion for `#!python session.create_client("iot").list_detect_mitigation_actions_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_detect_mitigation_actions_tasks.html)

```python
# list_detect_mitigation_actions_tasks method definition

await def list_detect_mitigation_actions_tasks(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDetectMitigationActionsTasksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDetectMitigationActionsTasksResponseTypeDef](./type_defs.md#listdetectmitigationactionstasksresponsetypedef) 


```python
# list_detect_mitigation_actions_tasks method usage example with argument unpacking

kwargs: ListDetectMitigationActionsTasksRequestRequestTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.list_detect_mitigation_actions_tasks(**kwargs)
```

1. See [:material-code-braces: ListDetectMitigationActionsTasksRequestRequestTypeDef](./type_defs.md#listdetectmitigationactionstasksrequestrequesttypedef) 

### list\_dimensions

List the set of dimensions that are defined for your Amazon Web Services
accounts.

Type annotations and code completion for `#!python session.create_client("iot").list_dimensions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_dimensions.html)

```python
# list_dimensions method definition

await def list_dimensions(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDimensionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDimensionsResponseTypeDef](./type_defs.md#listdimensionsresponsetypedef) 


```python
# list_dimensions method usage example with argument unpacking

kwargs: ListDimensionsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_dimensions(**kwargs)
```

1. See [:material-code-braces: ListDimensionsRequestRequestTypeDef](./type_defs.md#listdimensionsrequestrequesttypedef) 

### list\_domain\_configurations

Gets a list of domain configurations for the user.

Type annotations and code completion for `#!python session.create_client("iot").list_domain_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_domain_configurations.html)

```python
# list_domain_configurations method definition

await def list_domain_configurations(
    self,
    *,
    marker: str = ...,
    pageSize: int = ...,
    serviceType: ServiceTypeType = ...,  # (1)
) -> ListDomainConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: ListDomainConfigurationsResponseTypeDef](./type_defs.md#listdomainconfigurationsresponsetypedef) 


```python
# list_domain_configurations method usage example with argument unpacking

kwargs: ListDomainConfigurationsRequestRequestTypeDef = {  # (1)
    "marker": ...,
}

parent.list_domain_configurations(**kwargs)
```

1. See [:material-code-braces: ListDomainConfigurationsRequestRequestTypeDef](./type_defs.md#listdomainconfigurationsrequestrequesttypedef) 

### list\_fleet\_metrics

Lists all your fleet metrics.

Type annotations and code completion for `#!python session.create_client("iot").list_fleet_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_fleet_metrics.html)

```python
# list_fleet_metrics method definition

await def list_fleet_metrics(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFleetMetricsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFleetMetricsResponseTypeDef](./type_defs.md#listfleetmetricsresponsetypedef) 


```python
# list_fleet_metrics method usage example with argument unpacking

kwargs: ListFleetMetricsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_fleet_metrics(**kwargs)
```

1. See [:material-code-braces: ListFleetMetricsRequestRequestTypeDef](./type_defs.md#listfleetmetricsrequestrequesttypedef) 

### list\_indices

Lists the search indices.

Type annotations and code completion for `#!python session.create_client("iot").list_indices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_indices.html)

```python
# list_indices method definition

await def list_indices(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListIndicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef) 


```python
# list_indices method usage example with argument unpacking

kwargs: ListIndicesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_indices(**kwargs)
```

1. See [:material-code-braces: ListIndicesRequestRequestTypeDef](./type_defs.md#listindicesrequestrequesttypedef) 

### list\_job\_executions\_for\_job

Lists the job executions for a job.

Type annotations and code completion for `#!python session.create_client("iot").list_job_executions_for_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_job_executions_for_job.html)

```python
# list_job_executions_for_job method definition

await def list_job_executions_for_job(
    self,
    *,
    jobId: str,
    status: JobExecutionStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListJobExecutionsForJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: ListJobExecutionsForJobResponseTypeDef](./type_defs.md#listjobexecutionsforjobresponsetypedef) 


```python
# list_job_executions_for_job method usage example with argument unpacking

kwargs: ListJobExecutionsForJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.list_job_executions_for_job(**kwargs)
```

1. See [:material-code-braces: ListJobExecutionsForJobRequestRequestTypeDef](./type_defs.md#listjobexecutionsforjobrequestrequesttypedef) 

### list\_job\_executions\_for\_thing

Lists the job executions for the specified thing.

Type annotations and code completion for `#!python session.create_client("iot").list_job_executions_for_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_job_executions_for_thing.html)

```python
# list_job_executions_for_thing method definition

await def list_job_executions_for_thing(
    self,
    *,
    thingName: str,
    status: JobExecutionStatusType = ...,  # (1)
    namespaceId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    jobId: str = ...,
) -> ListJobExecutionsForThingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: ListJobExecutionsForThingResponseTypeDef](./type_defs.md#listjobexecutionsforthingresponsetypedef) 


```python
# list_job_executions_for_thing method usage example with argument unpacking

kwargs: ListJobExecutionsForThingRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_job_executions_for_thing(**kwargs)
```

1. See [:material-code-braces: ListJobExecutionsForThingRequestRequestTypeDef](./type_defs.md#listjobexecutionsforthingrequestrequesttypedef) 

### list\_job\_templates

Returns a list of job templates.

Type annotations and code completion for `#!python session.create_client("iot").list_job_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_job_templates.html)

```python
# list_job_templates method definition

await def list_job_templates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListJobTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef) 


```python
# list_job_templates method usage example with argument unpacking

kwargs: ListJobTemplatesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_job_templates(**kwargs)
```

1. See [:material-code-braces: ListJobTemplatesRequestRequestTypeDef](./type_defs.md#listjobtemplatesrequestrequesttypedef) 

### list\_jobs

Lists jobs.

Type annotations and code completion for `#!python session.create_client("iot").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_jobs.html)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    status: JobStatusType = ...,  # (1)
    targetSelection: TargetSelectionType = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    thingGroupName: str = ...,
    thingGroupId: str = ...,
    namespaceId: str = ...,
) -> ListJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
3. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsRequestRequestTypeDef = {  # (1)
    "status": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef) 

### list\_managed\_job\_templates

Returns a list of managed job templates.

Type annotations and code completion for `#!python session.create_client("iot").list_managed_job_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_managed_job_templates.html)

```python
# list_managed_job_templates method definition

await def list_managed_job_templates(
    self,
    *,
    templateName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListManagedJobTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListManagedJobTemplatesResponseTypeDef](./type_defs.md#listmanagedjobtemplatesresponsetypedef) 


```python
# list_managed_job_templates method usage example with argument unpacking

kwargs: ListManagedJobTemplatesRequestRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.list_managed_job_templates(**kwargs)
```

1. See [:material-code-braces: ListManagedJobTemplatesRequestRequestTypeDef](./type_defs.md#listmanagedjobtemplatesrequestrequesttypedef) 

### list\_metric\_values

Lists the values reported for an IoT Device Defender metric (device-side
metric, cloud-side metric, or custom metric) by the given thing during the
specified time period.

Type annotations and code completion for `#!python session.create_client("iot").list_metric_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_metric_values.html)

```python
# list_metric_values method definition

await def list_metric_values(
    self,
    *,
    thingName: str,
    metricName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    dimensionName: str = ...,
    dimensionValueOperator: DimensionValueOperatorType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMetricValuesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DimensionValueOperatorType](./literals.md#dimensionvalueoperatortype) 
2. See [:material-code-braces: ListMetricValuesResponseTypeDef](./type_defs.md#listmetricvaluesresponsetypedef) 


```python
# list_metric_values method usage example with argument unpacking

kwargs: ListMetricValuesRequestRequestTypeDef = {  # (1)
    "thingName": ...,
    "metricName": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.list_metric_values(**kwargs)
```

1. See [:material-code-braces: ListMetricValuesRequestRequestTypeDef](./type_defs.md#listmetricvaluesrequestrequesttypedef) 

### list\_mitigation\_actions

Gets a list of all mitigation actions that match the specified filter criteria.

Type annotations and code completion for `#!python session.create_client("iot").list_mitigation_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_mitigation_actions.html)

```python
# list_mitigation_actions method definition

await def list_mitigation_actions(
    self,
    *,
    actionType: MitigationActionTypeType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMitigationActionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MitigationActionTypeType](./literals.md#mitigationactiontypetype) 
2. See [:material-code-braces: ListMitigationActionsResponseTypeDef](./type_defs.md#listmitigationactionsresponsetypedef) 


```python
# list_mitigation_actions method usage example with argument unpacking

kwargs: ListMitigationActionsRequestRequestTypeDef = {  # (1)
    "actionType": ...,
}

parent.list_mitigation_actions(**kwargs)
```

1. See [:material-code-braces: ListMitigationActionsRequestRequestTypeDef](./type_defs.md#listmitigationactionsrequestrequesttypedef) 

### list\_ota\_updates

Lists OTA updates.

Type annotations and code completion for `#!python session.create_client("iot").list_ota_updates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_ota_updates.html)

```python
# list_ota_updates method definition

await def list_ota_updates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    otaUpdateStatus: OTAUpdateStatusType = ...,  # (1)
) -> ListOTAUpdatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OTAUpdateStatusType](./literals.md#otaupdatestatustype) 
2. See [:material-code-braces: ListOTAUpdatesResponseTypeDef](./type_defs.md#listotaupdatesresponsetypedef) 


```python
# list_ota_updates method usage example with argument unpacking

kwargs: ListOTAUpdatesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_ota_updates(**kwargs)
```

1. See [:material-code-braces: ListOTAUpdatesRequestRequestTypeDef](./type_defs.md#listotaupdatesrequestrequesttypedef) 

### list\_outgoing\_certificates

Lists certificates that are being transferred but not yet accepted.

Type annotations and code completion for `#!python session.create_client("iot").list_outgoing_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_outgoing_certificates.html)

```python
# list_outgoing_certificates method definition

await def list_outgoing_certificates(
    self,
    *,
    pageSize: int = ...,
    marker: str = ...,
    ascendingOrder: bool = ...,
) -> ListOutgoingCertificatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOutgoingCertificatesResponseTypeDef](./type_defs.md#listoutgoingcertificatesresponsetypedef) 


```python
# list_outgoing_certificates method usage example with argument unpacking

kwargs: ListOutgoingCertificatesRequestRequestTypeDef = {  # (1)
    "pageSize": ...,
}

parent.list_outgoing_certificates(**kwargs)
```

1. See [:material-code-braces: ListOutgoingCertificatesRequestRequestTypeDef](./type_defs.md#listoutgoingcertificatesrequestrequesttypedef) 

### list\_package\_versions

Lists the software package versions associated to the account.

Type annotations and code completion for `#!python session.create_client("iot").list_package_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_package_versions.html)

```python
# list_package_versions method definition

await def list_package_versions(
    self,
    *,
    packageName: str,
    status: PackageVersionStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPackageVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
2. See [:material-code-braces: ListPackageVersionsResponseTypeDef](./type_defs.md#listpackageversionsresponsetypedef) 


```python
# list_package_versions method usage example with argument unpacking

kwargs: ListPackageVersionsRequestRequestTypeDef = {  # (1)
    "packageName": ...,
}

parent.list_package_versions(**kwargs)
```

1. See [:material-code-braces: ListPackageVersionsRequestRequestTypeDef](./type_defs.md#listpackageversionsrequestrequesttypedef) 

### list\_packages

Lists the software packages associated to the account.

Type annotations and code completion for `#!python session.create_client("iot").list_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_packages.html)

```python
# list_packages method definition

await def list_packages(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPackagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPackagesResponseTypeDef](./type_defs.md#listpackagesresponsetypedef) 


```python
# list_packages method usage example with argument unpacking

kwargs: ListPackagesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_packages(**kwargs)
```

1. See [:material-code-braces: ListPackagesRequestRequestTypeDef](./type_defs.md#listpackagesrequestrequesttypedef) 

### list\_policies

Lists your policies.

Type annotations and code completion for `#!python session.create_client("iot").list_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_policies.html)

```python
# list_policies method definition

await def list_policies(
    self,
    *,
    marker: str = ...,
    pageSize: int = ...,
    ascendingOrder: bool = ...,
) -> ListPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python
# list_policies method usage example with argument unpacking

kwargs: ListPoliciesRequestRequestTypeDef = {  # (1)
    "marker": ...,
}

parent.list_policies(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestRequestTypeDef](./type_defs.md#listpoliciesrequestrequesttypedef) 

### list\_policy\_principals

Lists the principals associated with the specified policy.

Type annotations and code completion for `#!python session.create_client("iot").list_policy_principals` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_policy_principals.html)

```python
# list_policy_principals method definition

await def list_policy_principals(
    self,
    *,
    policyName: str,
    marker: str = ...,
    pageSize: int = ...,
    ascendingOrder: bool = ...,
) -> ListPolicyPrincipalsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyPrincipalsResponseTypeDef](./type_defs.md#listpolicyprincipalsresponsetypedef) 


```python
# list_policy_principals method usage example with argument unpacking

kwargs: ListPolicyPrincipalsRequestRequestTypeDef = {  # (1)
    "policyName": ...,
}

parent.list_policy_principals(**kwargs)
```

1. See [:material-code-braces: ListPolicyPrincipalsRequestRequestTypeDef](./type_defs.md#listpolicyprincipalsrequestrequesttypedef) 

### list\_policy\_versions

Lists the versions of the specified policy and identifies the default version.

Type annotations and code completion for `#!python session.create_client("iot").list_policy_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_policy_versions.html)

```python
# list_policy_versions method definition

await def list_policy_versions(
    self,
    *,
    policyName: str,
) -> ListPolicyVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyVersionsResponseTypeDef](./type_defs.md#listpolicyversionsresponsetypedef) 


```python
# list_policy_versions method usage example with argument unpacking

kwargs: ListPolicyVersionsRequestRequestTypeDef = {  # (1)
    "policyName": ...,
}

parent.list_policy_versions(**kwargs)
```

1. See [:material-code-braces: ListPolicyVersionsRequestRequestTypeDef](./type_defs.md#listpolicyversionsrequestrequesttypedef) 

### list\_principal\_policies

Lists the policies attached to the specified principal.

Type annotations and code completion for `#!python session.create_client("iot").list_principal_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_principal_policies.html)

```python
# list_principal_policies method definition

await def list_principal_policies(
    self,
    *,
    principal: str,
    marker: str = ...,
    pageSize: int = ...,
    ascendingOrder: bool = ...,
) -> ListPrincipalPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPrincipalPoliciesResponseTypeDef](./type_defs.md#listprincipalpoliciesresponsetypedef) 


```python
# list_principal_policies method usage example with argument unpacking

kwargs: ListPrincipalPoliciesRequestRequestTypeDef = {  # (1)
    "principal": ...,
}

parent.list_principal_policies(**kwargs)
```

1. See [:material-code-braces: ListPrincipalPoliciesRequestRequestTypeDef](./type_defs.md#listprincipalpoliciesrequestrequesttypedef) 

### list\_principal\_things

Lists the things associated with the specified principal.

Type annotations and code completion for `#!python session.create_client("iot").list_principal_things` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_principal_things.html)

```python
# list_principal_things method definition

await def list_principal_things(
    self,
    *,
    principal: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPrincipalThingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPrincipalThingsResponseTypeDef](./type_defs.md#listprincipalthingsresponsetypedef) 


```python
# list_principal_things method usage example with argument unpacking

kwargs: ListPrincipalThingsRequestRequestTypeDef = {  # (1)
    "principal": ...,
}

parent.list_principal_things(**kwargs)
```

1. See [:material-code-braces: ListPrincipalThingsRequestRequestTypeDef](./type_defs.md#listprincipalthingsrequestrequesttypedef) 

### list\_principal\_things\_v2

Lists the things associated with the specified principal.

Type annotations and code completion for `#!python session.create_client("iot").list_principal_things_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_principal_things_v2.html)

```python
# list_principal_things_v2 method definition

await def list_principal_things_v2(
    self,
    *,
    principal: str,
    nextToken: str = ...,
    maxResults: int = ...,
    thingPrincipalType: ThingPrincipalTypeType = ...,  # (1)
) -> ListPrincipalThingsV2ResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
2. See [:material-code-braces: ListPrincipalThingsV2ResponseTypeDef](./type_defs.md#listprincipalthingsv2responsetypedef) 


```python
# list_principal_things_v2 method usage example with argument unpacking

kwargs: ListPrincipalThingsV2RequestRequestTypeDef = {  # (1)
    "principal": ...,
}

parent.list_principal_things_v2(**kwargs)
```

1. See [:material-code-braces: ListPrincipalThingsV2RequestRequestTypeDef](./type_defs.md#listprincipalthingsv2requestrequesttypedef) 

### list\_provisioning\_template\_versions

A list of provisioning template versions.

Type annotations and code completion for `#!python session.create_client("iot").list_provisioning_template_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_provisioning_template_versions.html)

```python
# list_provisioning_template_versions method definition

await def list_provisioning_template_versions(
    self,
    *,
    templateName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListProvisioningTemplateVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProvisioningTemplateVersionsResponseTypeDef](./type_defs.md#listprovisioningtemplateversionsresponsetypedef) 


```python
# list_provisioning_template_versions method usage example with argument unpacking

kwargs: ListProvisioningTemplateVersionsRequestRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.list_provisioning_template_versions(**kwargs)
```

1. See [:material-code-braces: ListProvisioningTemplateVersionsRequestRequestTypeDef](./type_defs.md#listprovisioningtemplateversionsrequestrequesttypedef) 

### list\_provisioning\_templates

Lists the provisioning templates in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iot").list_provisioning_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_provisioning_templates.html)

```python
# list_provisioning_templates method definition

await def list_provisioning_templates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListProvisioningTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProvisioningTemplatesResponseTypeDef](./type_defs.md#listprovisioningtemplatesresponsetypedef) 


```python
# list_provisioning_templates method usage example with argument unpacking

kwargs: ListProvisioningTemplatesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_provisioning_templates(**kwargs)
```

1. See [:material-code-braces: ListProvisioningTemplatesRequestRequestTypeDef](./type_defs.md#listprovisioningtemplatesrequestrequesttypedef) 

### list\_related\_resources\_for\_audit\_finding

The related resources of an Audit finding.

Type annotations and code completion for `#!python session.create_client("iot").list_related_resources_for_audit_finding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_related_resources_for_audit_finding.html)

```python
# list_related_resources_for_audit_finding method definition

await def list_related_resources_for_audit_finding(
    self,
    *,
    findingId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListRelatedResourcesForAuditFindingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRelatedResourcesForAuditFindingResponseTypeDef](./type_defs.md#listrelatedresourcesforauditfindingresponsetypedef) 


```python
# list_related_resources_for_audit_finding method usage example with argument unpacking

kwargs: ListRelatedResourcesForAuditFindingRequestRequestTypeDef = {  # (1)
    "findingId": ...,
}

parent.list_related_resources_for_audit_finding(**kwargs)
```

1. See [:material-code-braces: ListRelatedResourcesForAuditFindingRequestRequestTypeDef](./type_defs.md#listrelatedresourcesforauditfindingrequestrequesttypedef) 

### list\_role\_aliases

Lists the role aliases registered in your account.

Type annotations and code completion for `#!python session.create_client("iot").list_role_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_role_aliases.html)

```python
# list_role_aliases method definition

await def list_role_aliases(
    self,
    *,
    pageSize: int = ...,
    marker: str = ...,
    ascendingOrder: bool = ...,
) -> ListRoleAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoleAliasesResponseTypeDef](./type_defs.md#listrolealiasesresponsetypedef) 


```python
# list_role_aliases method usage example with argument unpacking

kwargs: ListRoleAliasesRequestRequestTypeDef = {  # (1)
    "pageSize": ...,
}

parent.list_role_aliases(**kwargs)
```

1. See [:material-code-braces: ListRoleAliasesRequestRequestTypeDef](./type_defs.md#listrolealiasesrequestrequesttypedef) 

### list\_sbom\_validation\_results

The validation results for all software bill of materials (SBOM) attached to a
specific software package version.

Type annotations and code completion for `#!python session.create_client("iot").list_sbom_validation_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_sbom_validation_results.html)

```python
# list_sbom_validation_results method definition

await def list_sbom_validation_results(
    self,
    *,
    packageName: str,
    versionName: str,
    validationResult: SbomValidationResultType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSbomValidationResultsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SbomValidationResultType](./literals.md#sbomvalidationresulttype) 
2. See [:material-code-braces: ListSbomValidationResultsResponseTypeDef](./type_defs.md#listsbomvalidationresultsresponsetypedef) 


```python
# list_sbom_validation_results method usage example with argument unpacking

kwargs: ListSbomValidationResultsRequestRequestTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
}

parent.list_sbom_validation_results(**kwargs)
```

1. See [:material-code-braces: ListSbomValidationResultsRequestRequestTypeDef](./type_defs.md#listsbomvalidationresultsrequestrequesttypedef) 

### list\_scheduled\_audits

Lists all of your scheduled audits.

Type annotations and code completion for `#!python session.create_client("iot").list_scheduled_audits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_scheduled_audits.html)

```python
# list_scheduled_audits method definition

await def list_scheduled_audits(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListScheduledAuditsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScheduledAuditsResponseTypeDef](./type_defs.md#listscheduledauditsresponsetypedef) 


```python
# list_scheduled_audits method usage example with argument unpacking

kwargs: ListScheduledAuditsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_scheduled_audits(**kwargs)
```

1. See [:material-code-braces: ListScheduledAuditsRequestRequestTypeDef](./type_defs.md#listscheduledauditsrequestrequesttypedef) 

### list\_security\_profiles

Lists the Device Defender security profiles you've created.

Type annotations and code completion for `#!python session.create_client("iot").list_security_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_security_profiles.html)

```python
# list_security_profiles method definition

await def list_security_profiles(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    dimensionName: str = ...,
    metricName: str = ...,
) -> ListSecurityProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef) 


```python
# list_security_profiles method usage example with argument unpacking

kwargs: ListSecurityProfilesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_security_profiles(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesRequestRequestTypeDef](./type_defs.md#listsecurityprofilesrequestrequesttypedef) 

### list\_security\_profiles\_for\_target

Lists the Device Defender security profiles attached to a target (thing group).

Type annotations and code completion for `#!python session.create_client("iot").list_security_profiles_for_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_security_profiles_for_target.html)

```python
# list_security_profiles_for_target method definition

await def list_security_profiles_for_target(
    self,
    *,
    securityProfileTargetArn: str,
    nextToken: str = ...,
    maxResults: int = ...,
    recursive: bool = ...,
) -> ListSecurityProfilesForTargetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityProfilesForTargetResponseTypeDef](./type_defs.md#listsecurityprofilesfortargetresponsetypedef) 


```python
# list_security_profiles_for_target method usage example with argument unpacking

kwargs: ListSecurityProfilesForTargetRequestRequestTypeDef = {  # (1)
    "securityProfileTargetArn": ...,
}

parent.list_security_profiles_for_target(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesForTargetRequestRequestTypeDef](./type_defs.md#listsecurityprofilesfortargetrequestrequesttypedef) 

### list\_streams

Lists all of the streams in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iot").list_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_streams.html)

```python
# list_streams method definition

await def list_streams(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    ascendingOrder: bool = ...,
) -> ListStreamsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef) 


```python
# list_streams method usage example with argument unpacking

kwargs: ListStreamsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_streams(**kwargs)
```

1. See [:material-code-braces: ListStreamsRequestRequestTypeDef](./type_defs.md#liststreamsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags (metadata) you have assigned to the resource.

Type annotations and code completion for `#!python session.create_client("iot").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
    nextToken: str = ...,
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

### list\_targets\_for\_policy

List targets for the specified policy.

Type annotations and code completion for `#!python session.create_client("iot").list_targets_for_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_targets_for_policy.html)

```python
# list_targets_for_policy method definition

await def list_targets_for_policy(
    self,
    *,
    policyName: str,
    marker: str = ...,
    pageSize: int = ...,
) -> ListTargetsForPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef) 


```python
# list_targets_for_policy method usage example with argument unpacking

kwargs: ListTargetsForPolicyRequestRequestTypeDef = {  # (1)
    "policyName": ...,
}

parent.list_targets_for_policy(**kwargs)
```

1. See [:material-code-braces: ListTargetsForPolicyRequestRequestTypeDef](./type_defs.md#listtargetsforpolicyrequestrequesttypedef) 

### list\_targets\_for\_security\_profile

Lists the targets (thing groups) associated with a given Device Defender
security profile.

Type annotations and code completion for `#!python session.create_client("iot").list_targets_for_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_targets_for_security_profile.html)

```python
# list_targets_for_security_profile method definition

await def list_targets_for_security_profile(
    self,
    *,
    securityProfileName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTargetsForSecurityProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTargetsForSecurityProfileResponseTypeDef](./type_defs.md#listtargetsforsecurityprofileresponsetypedef) 


```python
# list_targets_for_security_profile method usage example with argument unpacking

kwargs: ListTargetsForSecurityProfileRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.list_targets_for_security_profile(**kwargs)
```

1. See [:material-code-braces: ListTargetsForSecurityProfileRequestRequestTypeDef](./type_defs.md#listtargetsforsecurityprofilerequestrequesttypedef) 

### list\_thing\_groups

List the thing groups in your account.

Type annotations and code completion for `#!python session.create_client("iot").list_thing_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_thing_groups.html)

```python
# list_thing_groups method definition

await def list_thing_groups(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    parentGroup: str = ...,
    namePrefixFilter: str = ...,
    recursive: bool = ...,
) -> ListThingGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThingGroupsResponseTypeDef](./type_defs.md#listthinggroupsresponsetypedef) 


```python
# list_thing_groups method usage example with argument unpacking

kwargs: ListThingGroupsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_thing_groups(**kwargs)
```

1. See [:material-code-braces: ListThingGroupsRequestRequestTypeDef](./type_defs.md#listthinggroupsrequestrequesttypedef) 

### list\_thing\_groups\_for\_thing

List the thing groups to which the specified thing belongs.

Type annotations and code completion for `#!python session.create_client("iot").list_thing_groups_for_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_thing_groups_for_thing.html)

```python
# list_thing_groups_for_thing method definition

await def list_thing_groups_for_thing(
    self,
    *,
    thingName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListThingGroupsForThingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThingGroupsForThingResponseTypeDef](./type_defs.md#listthinggroupsforthingresponsetypedef) 


```python
# list_thing_groups_for_thing method usage example with argument unpacking

kwargs: ListThingGroupsForThingRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_thing_groups_for_thing(**kwargs)
```

1. See [:material-code-braces: ListThingGroupsForThingRequestRequestTypeDef](./type_defs.md#listthinggroupsforthingrequestrequesttypedef) 

### list\_thing\_principals

Lists the principals associated with the specified thing.

Type annotations and code completion for `#!python session.create_client("iot").list_thing_principals` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_thing_principals.html)

```python
# list_thing_principals method definition

await def list_thing_principals(
    self,
    *,
    thingName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListThingPrincipalsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThingPrincipalsResponseTypeDef](./type_defs.md#listthingprincipalsresponsetypedef) 


```python
# list_thing_principals method usage example with argument unpacking

kwargs: ListThingPrincipalsRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_thing_principals(**kwargs)
```

1. See [:material-code-braces: ListThingPrincipalsRequestRequestTypeDef](./type_defs.md#listthingprincipalsrequestrequesttypedef) 

### list\_thing\_principals\_v2

Lists the principals associated with the specified thing.

Type annotations and code completion for `#!python session.create_client("iot").list_thing_principals_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_thing_principals_v2.html)

```python
# list_thing_principals_v2 method definition

await def list_thing_principals_v2(
    self,
    *,
    thingName: str,
    nextToken: str = ...,
    maxResults: int = ...,
    thingPrincipalType: ThingPrincipalTypeType = ...,  # (1)
) -> ListThingPrincipalsV2ResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype) 
2. See [:material-code-braces: ListThingPrincipalsV2ResponseTypeDef](./type_defs.md#listthingprincipalsv2responsetypedef) 


```python
# list_thing_principals_v2 method usage example with argument unpacking

kwargs: ListThingPrincipalsV2RequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_thing_principals_v2(**kwargs)
```

1. See [:material-code-braces: ListThingPrincipalsV2RequestRequestTypeDef](./type_defs.md#listthingprincipalsv2requestrequesttypedef) 

### list\_thing\_registration\_task\_reports

Information about the thing registration tasks.

Type annotations and code completion for `#!python session.create_client("iot").list_thing_registration_task_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_thing_registration_task_reports.html)

```python
# list_thing_registration_task_reports method definition

await def list_thing_registration_task_reports(
    self,
    *,
    taskId: str,
    reportType: ReportTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListThingRegistrationTaskReportsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ListThingRegistrationTaskReportsResponseTypeDef](./type_defs.md#listthingregistrationtaskreportsresponsetypedef) 


```python
# list_thing_registration_task_reports method usage example with argument unpacking

kwargs: ListThingRegistrationTaskReportsRequestRequestTypeDef = {  # (1)
    "taskId": ...,
    "reportType": ...,
}

parent.list_thing_registration_task_reports(**kwargs)
```

1. See [:material-code-braces: ListThingRegistrationTaskReportsRequestRequestTypeDef](./type_defs.md#listthingregistrationtaskreportsrequestrequesttypedef) 

### list\_thing\_registration\_tasks

List bulk thing provisioning tasks.

Type annotations and code completion for `#!python session.create_client("iot").list_thing_registration_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_thing_registration_tasks.html)

```python
# list_thing_registration_tasks method definition

await def list_thing_registration_tasks(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    status: StatusType = ...,  # (1)
) -> ListThingRegistrationTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ListThingRegistrationTasksResponseTypeDef](./type_defs.md#listthingregistrationtasksresponsetypedef) 


```python
# list_thing_registration_tasks method usage example with argument unpacking

kwargs: ListThingRegistrationTasksRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_thing_registration_tasks(**kwargs)
```

1. See [:material-code-braces: ListThingRegistrationTasksRequestRequestTypeDef](./type_defs.md#listthingregistrationtasksrequestrequesttypedef) 

### list\_thing\_types

Lists the existing thing types.

Type annotations and code completion for `#!python session.create_client("iot").list_thing_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_thing_types.html)

```python
# list_thing_types method definition

await def list_thing_types(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    thingTypeName: str = ...,
) -> ListThingTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThingTypesResponseTypeDef](./type_defs.md#listthingtypesresponsetypedef) 


```python
# list_thing_types method usage example with argument unpacking

kwargs: ListThingTypesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_thing_types(**kwargs)
```

1. See [:material-code-braces: ListThingTypesRequestRequestTypeDef](./type_defs.md#listthingtypesrequestrequesttypedef) 

### list\_things

Lists your things.

Type annotations and code completion for `#!python session.create_client("iot").list_things` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_things.html)

```python
# list_things method definition

await def list_things(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    attributeName: str = ...,
    attributeValue: str = ...,
    thingTypeName: str = ...,
    usePrefixAttributeValue: bool = ...,
) -> ListThingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThingsResponseTypeDef](./type_defs.md#listthingsresponsetypedef) 


```python
# list_things method usage example with argument unpacking

kwargs: ListThingsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_things(**kwargs)
```

1. See [:material-code-braces: ListThingsRequestRequestTypeDef](./type_defs.md#listthingsrequestrequesttypedef) 

### list\_things\_in\_billing\_group

Lists the things you have added to the given billing group.

Type annotations and code completion for `#!python session.create_client("iot").list_things_in_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_things_in_billing_group.html)

```python
# list_things_in_billing_group method definition

await def list_things_in_billing_group(
    self,
    *,
    billingGroupName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListThingsInBillingGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThingsInBillingGroupResponseTypeDef](./type_defs.md#listthingsinbillinggroupresponsetypedef) 


```python
# list_things_in_billing_group method usage example with argument unpacking

kwargs: ListThingsInBillingGroupRequestRequestTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.list_things_in_billing_group(**kwargs)
```

1. See [:material-code-braces: ListThingsInBillingGroupRequestRequestTypeDef](./type_defs.md#listthingsinbillinggrouprequestrequesttypedef) 

### list\_things\_in\_thing\_group

Lists the things in the specified group.

Type annotations and code completion for `#!python session.create_client("iot").list_things_in_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_things_in_thing_group.html)

```python
# list_things_in_thing_group method definition

await def list_things_in_thing_group(
    self,
    *,
    thingGroupName: str,
    recursive: bool = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListThingsInThingGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThingsInThingGroupResponseTypeDef](./type_defs.md#listthingsinthinggroupresponsetypedef) 


```python
# list_things_in_thing_group method usage example with argument unpacking

kwargs: ListThingsInThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.list_things_in_thing_group(**kwargs)
```

1. See [:material-code-braces: ListThingsInThingGroupRequestRequestTypeDef](./type_defs.md#listthingsinthinggrouprequestrequesttypedef) 

### list\_topic\_rule\_destinations

Lists all the topic rule destinations in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iot").list_topic_rule_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_topic_rule_destinations.html)

```python
# list_topic_rule_destinations method definition

await def list_topic_rule_destinations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTopicRuleDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTopicRuleDestinationsResponseTypeDef](./type_defs.md#listtopicruledestinationsresponsetypedef) 


```python
# list_topic_rule_destinations method usage example with argument unpacking

kwargs: ListTopicRuleDestinationsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_topic_rule_destinations(**kwargs)
```

1. See [:material-code-braces: ListTopicRuleDestinationsRequestRequestTypeDef](./type_defs.md#listtopicruledestinationsrequestrequesttypedef) 

### list\_topic\_rules

Lists the rules for the specific topic.

Type annotations and code completion for `#!python session.create_client("iot").list_topic_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_topic_rules.html)

```python
# list_topic_rules method definition

await def list_topic_rules(
    self,
    *,
    topic: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    ruleDisabled: bool = ...,
) -> ListTopicRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTopicRulesResponseTypeDef](./type_defs.md#listtopicrulesresponsetypedef) 


```python
# list_topic_rules method usage example with argument unpacking

kwargs: ListTopicRulesRequestRequestTypeDef = {  # (1)
    "topic": ...,
}

parent.list_topic_rules(**kwargs)
```

1. See [:material-code-braces: ListTopicRulesRequestRequestTypeDef](./type_defs.md#listtopicrulesrequestrequesttypedef) 

### list\_v2\_logging\_levels

Lists logging levels.

Type annotations and code completion for `#!python session.create_client("iot").list_v2_logging_levels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_v2_logging_levels.html)

```python
# list_v2_logging_levels method definition

await def list_v2_logging_levels(
    self,
    *,
    targetType: LogTargetTypeType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListV2LoggingLevelsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype) 
2. See [:material-code-braces: ListV2LoggingLevelsResponseTypeDef](./type_defs.md#listv2logginglevelsresponsetypedef) 


```python
# list_v2_logging_levels method usage example with argument unpacking

kwargs: ListV2LoggingLevelsRequestRequestTypeDef = {  # (1)
    "targetType": ...,
}

parent.list_v2_logging_levels(**kwargs)
```

1. See [:material-code-braces: ListV2LoggingLevelsRequestRequestTypeDef](./type_defs.md#listv2logginglevelsrequestrequesttypedef) 

### list\_violation\_events

Lists the Device Defender security profile violations discovered during the
given time period.

Type annotations and code completion for `#!python session.create_client("iot").list_violation_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/list_violation_events.html)

```python
# list_violation_events method definition

await def list_violation_events(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    thingName: str = ...,
    securityProfileName: str = ...,
    behaviorCriteriaType: BehaviorCriteriaTypeType = ...,  # (1)
    listSuppressedAlerts: bool = ...,
    verificationState: VerificationStateType = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListViolationEventsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
3. See [:material-code-braces: ListViolationEventsResponseTypeDef](./type_defs.md#listviolationeventsresponsetypedef) 


```python
# list_violation_events method usage example with argument unpacking

kwargs: ListViolationEventsRequestRequestTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.list_violation_events(**kwargs)
```

1. See [:material-code-braces: ListViolationEventsRequestRequestTypeDef](./type_defs.md#listviolationeventsrequestrequesttypedef) 

### put\_verification\_state\_on\_violation

Set a verification state and provide a description of that verification state
on a violation (detect alarm).

Type annotations and code completion for `#!python session.create_client("iot").put_verification_state_on_violation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/put_verification_state_on_violation.html)

```python
# put_verification_state_on_violation method definition

await def put_verification_state_on_violation(
    self,
    *,
    violationId: str,
    verificationState: VerificationStateType,  # (1)
    verificationStateDescription: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 


```python
# put_verification_state_on_violation method usage example with argument unpacking

kwargs: PutVerificationStateOnViolationRequestRequestTypeDef = {  # (1)
    "violationId": ...,
    "verificationState": ...,
}

parent.put_verification_state_on_violation(**kwargs)
```

1. See [:material-code-braces: PutVerificationStateOnViolationRequestRequestTypeDef](./type_defs.md#putverificationstateonviolationrequestrequesttypedef) 

### register\_ca\_certificate

Registers a CA certificate with Amazon Web Services IoT Core.

Type annotations and code completion for `#!python session.create_client("iot").register_ca_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/register_ca_certificate.html)

```python
# register_ca_certificate method definition

await def register_ca_certificate(
    self,
    *,
    caCertificate: str,
    verificationCertificate: str = ...,
    setAsActive: bool = ...,
    allowAutoRegistration: bool = ...,
    registrationConfig: RegistrationConfigTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
    certificateMode: CertificateModeType = ...,  # (3)
) -> RegisterCACertificateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RegistrationConfigTypeDef](./type_defs.md#registrationconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: CertificateModeType](./literals.md#certificatemodetype) 
4. See [:material-code-braces: RegisterCACertificateResponseTypeDef](./type_defs.md#registercacertificateresponsetypedef) 


```python
# register_ca_certificate method usage example with argument unpacking

kwargs: RegisterCACertificateRequestRequestTypeDef = {  # (1)
    "caCertificate": ...,
}

parent.register_ca_certificate(**kwargs)
```

1. See [:material-code-braces: RegisterCACertificateRequestRequestTypeDef](./type_defs.md#registercacertificaterequestrequesttypedef) 

### register\_certificate

Registers a device certificate with IoT in the same <a
href="https://docs.aws.amazon.com/iot/latest/apireference/API_CertificateDescription.html#iot-Type-CertificateDescription-certificateMode">certificate
mode</a> as the signing CA.

Type annotations and code completion for `#!python session.create_client("iot").register_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/register_certificate.html)

```python
# register_certificate method definition

await def register_certificate(
    self,
    *,
    certificatePem: str,
    caCertificatePem: str = ...,
    setAsActive: bool = ...,
    status: CertificateStatusType = ...,  # (1)
) -> RegisterCertificateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: RegisterCertificateResponseTypeDef](./type_defs.md#registercertificateresponsetypedef) 


```python
# register_certificate method usage example with argument unpacking

kwargs: RegisterCertificateRequestRequestTypeDef = {  # (1)
    "certificatePem": ...,
}

parent.register_certificate(**kwargs)
```

1. See [:material-code-braces: RegisterCertificateRequestRequestTypeDef](./type_defs.md#registercertificaterequestrequesttypedef) 

### register\_certificate\_without\_ca

Register a certificate that does not have a certificate authority (CA).

Type annotations and code completion for `#!python session.create_client("iot").register_certificate_without_ca` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/register_certificate_without_ca.html)

```python
# register_certificate_without_ca method definition

await def register_certificate_without_ca(
    self,
    *,
    certificatePem: str,
    status: CertificateStatusType = ...,  # (1)
) -> RegisterCertificateWithoutCAResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: RegisterCertificateWithoutCAResponseTypeDef](./type_defs.md#registercertificatewithoutcaresponsetypedef) 


```python
# register_certificate_without_ca method usage example with argument unpacking

kwargs: RegisterCertificateWithoutCARequestRequestTypeDef = {  # (1)
    "certificatePem": ...,
}

parent.register_certificate_without_ca(**kwargs)
```

1. See [:material-code-braces: RegisterCertificateWithoutCARequestRequestTypeDef](./type_defs.md#registercertificatewithoutcarequestrequesttypedef) 

### register\_thing

Provisions a thing in the device registry.

Type annotations and code completion for `#!python session.create_client("iot").register_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/register_thing.html)

```python
# register_thing method definition

await def register_thing(
    self,
    *,
    templateBody: str,
    parameters: Mapping[str, str] = ...,
) -> RegisterThingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterThingResponseTypeDef](./type_defs.md#registerthingresponsetypedef) 


```python
# register_thing method usage example with argument unpacking

kwargs: RegisterThingRequestRequestTypeDef = {  # (1)
    "templateBody": ...,
}

parent.register_thing(**kwargs)
```

1. See [:material-code-braces: RegisterThingRequestRequestTypeDef](./type_defs.md#registerthingrequestrequesttypedef) 

### reject\_certificate\_transfer

Rejects a pending certificate transfer.

Type annotations and code completion for `#!python session.create_client("iot").reject_certificate_transfer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/reject_certificate_transfer.html)

```python
# reject_certificate_transfer method definition

await def reject_certificate_transfer(
    self,
    *,
    certificateId: str,
    rejectReason: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# reject_certificate_transfer method usage example with argument unpacking

kwargs: RejectCertificateTransferRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.reject_certificate_transfer(**kwargs)
```

1. See [:material-code-braces: RejectCertificateTransferRequestRequestTypeDef](./type_defs.md#rejectcertificatetransferrequestrequesttypedef) 

### remove\_thing\_from\_billing\_group

Removes the given thing from the billing group.

Type annotations and code completion for `#!python session.create_client("iot").remove_thing_from_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/remove_thing_from_billing_group.html)

```python
# remove_thing_from_billing_group method definition

await def remove_thing_from_billing_group(
    self,
    *,
    billingGroupName: str = ...,
    billingGroupArn: str = ...,
    thingName: str = ...,
    thingArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# remove_thing_from_billing_group method usage example with argument unpacking

kwargs: RemoveThingFromBillingGroupRequestRequestTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.remove_thing_from_billing_group(**kwargs)
```

1. See [:material-code-braces: RemoveThingFromBillingGroupRequestRequestTypeDef](./type_defs.md#removethingfrombillinggrouprequestrequesttypedef) 

### remove\_thing\_from\_thing\_group

Remove the specified thing from the specified group.

Type annotations and code completion for `#!python session.create_client("iot").remove_thing_from_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/remove_thing_from_thing_group.html)

```python
# remove_thing_from_thing_group method definition

await def remove_thing_from_thing_group(
    self,
    *,
    thingGroupName: str = ...,
    thingGroupArn: str = ...,
    thingName: str = ...,
    thingArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# remove_thing_from_thing_group method usage example with argument unpacking

kwargs: RemoveThingFromThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.remove_thing_from_thing_group(**kwargs)
```

1. See [:material-code-braces: RemoveThingFromThingGroupRequestRequestTypeDef](./type_defs.md#removethingfromthinggrouprequestrequesttypedef) 

### replace\_topic\_rule

Replaces the rule.

Type annotations and code completion for `#!python session.create_client("iot").replace_topic_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/replace_topic_rule.html)

```python
# replace_topic_rule method definition

await def replace_topic_rule(
    self,
    *,
    ruleName: str,
    topicRulePayload: TopicRulePayloadTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicRulePayloadTypeDef](./type_defs.md#topicrulepayloadtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# replace_topic_rule method usage example with argument unpacking

kwargs: ReplaceTopicRuleRequestRequestTypeDef = {  # (1)
    "ruleName": ...,
    "topicRulePayload": ...,
}

parent.replace_topic_rule(**kwargs)
```

1. See [:material-code-braces: ReplaceTopicRuleRequestRequestTypeDef](./type_defs.md#replacetopicrulerequestrequesttypedef) 

### search\_index

The query search index.

Type annotations and code completion for `#!python session.create_client("iot").search_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/search_index.html)

```python
# search_index method definition

await def search_index(
    self,
    *,
    queryString: str,
    indexName: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    queryVersion: str = ...,
) -> SearchIndexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchIndexResponseTypeDef](./type_defs.md#searchindexresponsetypedef) 


```python
# search_index method usage example with argument unpacking

kwargs: SearchIndexRequestRequestTypeDef = {  # (1)
    "queryString": ...,
}

parent.search_index(**kwargs)
```

1. See [:material-code-braces: SearchIndexRequestRequestTypeDef](./type_defs.md#searchindexrequestrequesttypedef) 

### set\_default\_authorizer

Sets the default authorizer.

Type annotations and code completion for `#!python session.create_client("iot").set_default_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/set_default_authorizer.html)

```python
# set_default_authorizer method definition

await def set_default_authorizer(
    self,
    *,
    authorizerName: str,
) -> SetDefaultAuthorizerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SetDefaultAuthorizerResponseTypeDef](./type_defs.md#setdefaultauthorizerresponsetypedef) 


```python
# set_default_authorizer method usage example with argument unpacking

kwargs: SetDefaultAuthorizerRequestRequestTypeDef = {  # (1)
    "authorizerName": ...,
}

parent.set_default_authorizer(**kwargs)
```

1. See [:material-code-braces: SetDefaultAuthorizerRequestRequestTypeDef](./type_defs.md#setdefaultauthorizerrequestrequesttypedef) 

### set\_default\_policy\_version

Sets the specified version of the specified policy as the policy's default
(operative) version.

Type annotations and code completion for `#!python session.create_client("iot").set_default_policy_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/set_default_policy_version.html)

```python
# set_default_policy_version method definition

await def set_default_policy_version(
    self,
    *,
    policyName: str,
    policyVersionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_default_policy_version method usage example with argument unpacking

kwargs: SetDefaultPolicyVersionRequestRequestTypeDef = {  # (1)
    "policyName": ...,
    "policyVersionId": ...,
}

parent.set_default_policy_version(**kwargs)
```

1. See [:material-code-braces: SetDefaultPolicyVersionRequestRequestTypeDef](./type_defs.md#setdefaultpolicyversionrequestrequesttypedef) 

### set\_logging\_options

Sets the logging options.

Type annotations and code completion for `#!python session.create_client("iot").set_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/set_logging_options.html)

```python
# set_logging_options method definition

await def set_logging_options(
    self,
    *,
    loggingOptionsPayload: LoggingOptionsPayloadTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoggingOptionsPayloadTypeDef](./type_defs.md#loggingoptionspayloadtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_logging_options method usage example with argument unpacking

kwargs: SetLoggingOptionsRequestRequestTypeDef = {  # (1)
    "loggingOptionsPayload": ...,
}

parent.set_logging_options(**kwargs)
```

1. See [:material-code-braces: SetLoggingOptionsRequestRequestTypeDef](./type_defs.md#setloggingoptionsrequestrequesttypedef) 

### set\_v2\_logging\_level

Sets the logging level.

Type annotations and code completion for `#!python session.create_client("iot").set_v2_logging_level` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/set_v2_logging_level.html)

```python
# set_v2_logging_level method definition

await def set_v2_logging_level(
    self,
    *,
    logTarget: LogTargetTypeDef,  # (1)
    logLevel: LogLevelType,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LogTargetTypeDef](./type_defs.md#logtargettypedef) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_v2_logging_level method usage example with argument unpacking

kwargs: SetV2LoggingLevelRequestRequestTypeDef = {  # (1)
    "logTarget": ...,
    "logLevel": ...,
}

parent.set_v2_logging_level(**kwargs)
```

1. See [:material-code-braces: SetV2LoggingLevelRequestRequestTypeDef](./type_defs.md#setv2logginglevelrequestrequesttypedef) 

### set\_v2\_logging\_options

Sets the logging options for the V2 logging service.

Type annotations and code completion for `#!python session.create_client("iot").set_v2_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/set_v2_logging_options.html)

```python
# set_v2_logging_options method definition

await def set_v2_logging_options(
    self,
    *,
    roleArn: str = ...,
    defaultLogLevel: LogLevelType = ...,  # (1)
    disableAllLogs: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_v2_logging_options method usage example with argument unpacking

kwargs: SetV2LoggingOptionsRequestRequestTypeDef = {  # (1)
    "roleArn": ...,
}

parent.set_v2_logging_options(**kwargs)
```

1. See [:material-code-braces: SetV2LoggingOptionsRequestRequestTypeDef](./type_defs.md#setv2loggingoptionsrequestrequesttypedef) 

### start\_audit\_mitigation\_actions\_task

Starts a task that applies a set of mitigation actions to the specified target.

Type annotations and code completion for `#!python session.create_client("iot").start_audit_mitigation_actions_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/start_audit_mitigation_actions_task.html)

```python
# start_audit_mitigation_actions_task method definition

await def start_audit_mitigation_actions_task(
    self,
    *,
    taskId: str,
    target: AuditMitigationActionsTaskTargetTypeDef,  # (1)
    auditCheckToActionsMapping: Mapping[str, Sequence[str]],
    clientRequestToken: str,
) -> StartAuditMitigationActionsTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AuditMitigationActionsTaskTargetTypeDef](./type_defs.md#auditmitigationactionstasktargettypedef) 
2. See [:material-code-braces: StartAuditMitigationActionsTaskResponseTypeDef](./type_defs.md#startauditmitigationactionstaskresponsetypedef) 


```python
# start_audit_mitigation_actions_task method usage example with argument unpacking

kwargs: StartAuditMitigationActionsTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
    "target": ...,
    "auditCheckToActionsMapping": ...,
    "clientRequestToken": ...,
}

parent.start_audit_mitigation_actions_task(**kwargs)
```

1. See [:material-code-braces: StartAuditMitigationActionsTaskRequestRequestTypeDef](./type_defs.md#startauditmitigationactionstaskrequestrequesttypedef) 

### start\_detect\_mitigation\_actions\_task

Starts a Device Defender ML Detect mitigation actions task.

Type annotations and code completion for `#!python session.create_client("iot").start_detect_mitigation_actions_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/start_detect_mitigation_actions_task.html)

```python
# start_detect_mitigation_actions_task method definition

await def start_detect_mitigation_actions_task(
    self,
    *,
    taskId: str,
    target: DetectMitigationActionsTaskTargetTypeDef,  # (1)
    actions: Sequence[str],
    clientRequestToken: str,
    violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,  # (2)
    includeOnlyActiveViolations: bool = ...,
    includeSuppressedAlerts: bool = ...,
) -> StartDetectMitigationActionsTaskResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DetectMitigationActionsTaskTargetTypeDef](./type_defs.md#detectmitigationactionstasktargettypedef) 
2. See [:material-code-braces: ViolationEventOccurrenceRangeTypeDef](./type_defs.md#violationeventoccurrencerangetypedef) 
3. See [:material-code-braces: StartDetectMitigationActionsTaskResponseTypeDef](./type_defs.md#startdetectmitigationactionstaskresponsetypedef) 


```python
# start_detect_mitigation_actions_task method usage example with argument unpacking

kwargs: StartDetectMitigationActionsTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
    "target": ...,
    "actions": ...,
    "clientRequestToken": ...,
}

parent.start_detect_mitigation_actions_task(**kwargs)
```

1. See [:material-code-braces: StartDetectMitigationActionsTaskRequestRequestTypeDef](./type_defs.md#startdetectmitigationactionstaskrequestrequesttypedef) 

### start\_on\_demand\_audit\_task

Starts an on-demand Device Defender audit.

Type annotations and code completion for `#!python session.create_client("iot").start_on_demand_audit_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/start_on_demand_audit_task.html)

```python
# start_on_demand_audit_task method definition

await def start_on_demand_audit_task(
    self,
    *,
    targetCheckNames: Sequence[str],
) -> StartOnDemandAuditTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartOnDemandAuditTaskResponseTypeDef](./type_defs.md#startondemandaudittaskresponsetypedef) 


```python
# start_on_demand_audit_task method usage example with argument unpacking

kwargs: StartOnDemandAuditTaskRequestRequestTypeDef = {  # (1)
    "targetCheckNames": ...,
}

parent.start_on_demand_audit_task(**kwargs)
```

1. See [:material-code-braces: StartOnDemandAuditTaskRequestRequestTypeDef](./type_defs.md#startondemandaudittaskrequestrequesttypedef) 

### start\_thing\_registration\_task

Creates a bulk thing provisioning task.

Type annotations and code completion for `#!python session.create_client("iot").start_thing_registration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/start_thing_registration_task.html)

```python
# start_thing_registration_task method definition

await def start_thing_registration_task(
    self,
    *,
    templateBody: str,
    inputFileBucket: str,
    inputFileKey: str,
    roleArn: str,
) -> StartThingRegistrationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartThingRegistrationTaskResponseTypeDef](./type_defs.md#startthingregistrationtaskresponsetypedef) 


```python
# start_thing_registration_task method usage example with argument unpacking

kwargs: StartThingRegistrationTaskRequestRequestTypeDef = {  # (1)
    "templateBody": ...,
    "inputFileBucket": ...,
    "inputFileKey": ...,
    "roleArn": ...,
}

parent.start_thing_registration_task(**kwargs)
```

1. See [:material-code-braces: StartThingRegistrationTaskRequestRequestTypeDef](./type_defs.md#startthingregistrationtaskrequestrequesttypedef) 

### stop\_thing\_registration\_task

Cancels a bulk thing provisioning task.

Type annotations and code completion for `#!python session.create_client("iot").stop_thing_registration_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/stop_thing_registration_task.html)

```python
# stop_thing_registration_task method definition

await def stop_thing_registration_task(
    self,
    *,
    taskId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_thing_registration_task method usage example with argument unpacking

kwargs: StopThingRegistrationTaskRequestRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.stop_thing_registration_task(**kwargs)
```

1. See [:material-code-braces: StopThingRegistrationTaskRequestRequestTypeDef](./type_defs.md#stopthingregistrationtaskrequestrequesttypedef) 

### tag\_resource

Adds to or modifies the tags of the given resource.

Type annotations and code completion for `#!python session.create_client("iot").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/tag_resource.html)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_authorization

Tests if a specified principal is authorized to perform an IoT action on a
specified resource.

Type annotations and code completion for `#!python session.create_client("iot").test_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/test_authorization.html)

```python
# test_authorization method definition

await def test_authorization(
    self,
    *,
    authInfos: Sequence[AuthInfoUnionTypeDef],  # (1)
    principal: str = ...,
    cognitoIdentityPoolId: str = ...,
    clientId: str = ...,
    policyNamesToAdd: Sequence[str] = ...,
    policyNamesToSkip: Sequence[str] = ...,
) -> TestAuthorizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AuthInfoTypeDef](./type_defs.md#authinfotypedef) [:material-code-braces: AuthInfoOutputTypeDef](./type_defs.md#authinfooutputtypedef) 
2. See [:material-code-braces: TestAuthorizationResponseTypeDef](./type_defs.md#testauthorizationresponsetypedef) 


```python
# test_authorization method usage example with argument unpacking

kwargs: TestAuthorizationRequestRequestTypeDef = {  # (1)
    "authInfos": ...,
}

parent.test_authorization(**kwargs)
```

1. See [:material-code-braces: TestAuthorizationRequestRequestTypeDef](./type_defs.md#testauthorizationrequestrequesttypedef) 

### test\_invoke\_authorizer

Tests a custom authorization behavior by invoking a specified custom authorizer.

Type annotations and code completion for `#!python session.create_client("iot").test_invoke_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/test_invoke_authorizer.html)

```python
# test_invoke_authorizer method definition

await def test_invoke_authorizer(
    self,
    *,
    authorizerName: str,
    token: str = ...,
    tokenSignature: str = ...,
    httpContext: HttpContextTypeDef = ...,  # (1)
    mqttContext: MqttContextTypeDef = ...,  # (2)
    tlsContext: TlsContextTypeDef = ...,  # (3)
) -> TestInvokeAuthorizerResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: HttpContextTypeDef](./type_defs.md#httpcontexttypedef) 
2. See [:material-code-braces: MqttContextTypeDef](./type_defs.md#mqttcontexttypedef) 
3. See [:material-code-braces: TlsContextTypeDef](./type_defs.md#tlscontexttypedef) 
4. See [:material-code-braces: TestInvokeAuthorizerResponseTypeDef](./type_defs.md#testinvokeauthorizerresponsetypedef) 


```python
# test_invoke_authorizer method usage example with argument unpacking

kwargs: TestInvokeAuthorizerRequestRequestTypeDef = {  # (1)
    "authorizerName": ...,
}

parent.test_invoke_authorizer(**kwargs)
```

1. See [:material-code-braces: TestInvokeAuthorizerRequestRequestTypeDef](./type_defs.md#testinvokeauthorizerrequestrequesttypedef) 

### transfer\_certificate

Transfers the specified certificate to the specified Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("iot").transfer_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/transfer_certificate.html)

```python
# transfer_certificate method definition

await def transfer_certificate(
    self,
    *,
    certificateId: str,
    targetAwsAccount: str,
    transferMessage: str = ...,
) -> TransferCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TransferCertificateResponseTypeDef](./type_defs.md#transfercertificateresponsetypedef) 


```python
# transfer_certificate method usage example with argument unpacking

kwargs: TransferCertificateRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
    "targetAwsAccount": ...,
}

parent.transfer_certificate(**kwargs)
```

1. See [:material-code-braces: TransferCertificateRequestRequestTypeDef](./type_defs.md#transfercertificaterequestrequesttypedef) 

### untag\_resource

Removes the given tags (metadata) from the resource.

Type annotations and code completion for `#!python session.create_client("iot").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/untag_resource.html)

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

### update\_account\_audit\_configuration

Configures or reconfigures the Device Defender audit settings for this account.

Type annotations and code completion for `#!python session.create_client("iot").update_account_audit_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_account_audit_configuration.html)

```python
# update_account_audit_configuration method definition

await def update_account_audit_configuration(
    self,
    *,
    roleArn: str = ...,
    auditNotificationTargetConfigurations: Mapping[AuditNotificationTypeType, AuditNotificationTargetTypeDef] = ...,  # (1)
    auditCheckConfigurations: Mapping[str, AuditCheckConfigurationTypeDef] = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AuditNotificationTypeType](./literals.md#auditnotificationtypetype) [:material-code-braces: AuditNotificationTargetTypeDef](./type_defs.md#auditnotificationtargettypedef) 
2. See [:material-code-braces: AuditCheckConfigurationTypeDef](./type_defs.md#auditcheckconfigurationtypedef) 


```python
# update_account_audit_configuration method usage example with argument unpacking

kwargs: UpdateAccountAuditConfigurationRequestRequestTypeDef = {  # (1)
    "roleArn": ...,
}

parent.update_account_audit_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateAccountAuditConfigurationRequestRequestTypeDef](./type_defs.md#updateaccountauditconfigurationrequestrequesttypedef) 

### update\_audit\_suppression

Updates a Device Defender audit suppression.

Type annotations and code completion for `#!python session.create_client("iot").update_audit_suppression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_audit_suppression.html)

```python
# update_audit_suppression method definition

await def update_audit_suppression(
    self,
    *,
    checkName: str,
    resourceIdentifier: ResourceIdentifierTypeDef,  # (1)
    expirationDate: TimestampTypeDef = ...,
    suppressIndefinitely: bool = ...,
    description: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 


```python
# update_audit_suppression method usage example with argument unpacking

kwargs: UpdateAuditSuppressionRequestRequestTypeDef = {  # (1)
    "checkName": ...,
    "resourceIdentifier": ...,
}

parent.update_audit_suppression(**kwargs)
```

1. See [:material-code-braces: UpdateAuditSuppressionRequestRequestTypeDef](./type_defs.md#updateauditsuppressionrequestrequesttypedef) 

### update\_authorizer

Updates an authorizer.

Type annotations and code completion for `#!python session.create_client("iot").update_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_authorizer.html)

```python
# update_authorizer method definition

await def update_authorizer(
    self,
    *,
    authorizerName: str,
    authorizerFunctionArn: str = ...,
    tokenKeyName: str = ...,
    tokenSigningPublicKeys: Mapping[str, str] = ...,
    status: AuthorizerStatusType = ...,  # (1)
    enableCachingForHttp: bool = ...,
) -> UpdateAuthorizerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
2. See [:material-code-braces: UpdateAuthorizerResponseTypeDef](./type_defs.md#updateauthorizerresponsetypedef) 


```python
# update_authorizer method usage example with argument unpacking

kwargs: UpdateAuthorizerRequestRequestTypeDef = {  # (1)
    "authorizerName": ...,
}

parent.update_authorizer(**kwargs)
```

1. See [:material-code-braces: UpdateAuthorizerRequestRequestTypeDef](./type_defs.md#updateauthorizerrequestrequesttypedef) 

### update\_billing\_group

Updates information about the billing group.

Type annotations and code completion for `#!python session.create_client("iot").update_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_billing_group.html)

```python
# update_billing_group method definition

await def update_billing_group(
    self,
    *,
    billingGroupName: str,
    billingGroupProperties: BillingGroupPropertiesTypeDef,  # (1)
    expectedVersion: int = ...,
) -> UpdateBillingGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BillingGroupPropertiesTypeDef](./type_defs.md#billinggrouppropertiestypedef) 
2. See [:material-code-braces: UpdateBillingGroupResponseTypeDef](./type_defs.md#updatebillinggroupresponsetypedef) 


```python
# update_billing_group method usage example with argument unpacking

kwargs: UpdateBillingGroupRequestRequestTypeDef = {  # (1)
    "billingGroupName": ...,
    "billingGroupProperties": ...,
}

parent.update_billing_group(**kwargs)
```

1. See [:material-code-braces: UpdateBillingGroupRequestRequestTypeDef](./type_defs.md#updatebillinggrouprequestrequesttypedef) 

### update\_ca\_certificate

Updates a registered CA certificate.

Type annotations and code completion for `#!python session.create_client("iot").update_ca_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_ca_certificate.html)

```python
# update_ca_certificate method definition

await def update_ca_certificate(
    self,
    *,
    certificateId: str,
    newStatus: CACertificateStatusType = ...,  # (1)
    newAutoRegistrationStatus: AutoRegistrationStatusType = ...,  # (2)
    registrationConfig: RegistrationConfigTypeDef = ...,  # (3)
    removeAutoRegistration: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CACertificateStatusType](./literals.md#cacertificatestatustype) 
2. See [:material-code-brackets: AutoRegistrationStatusType](./literals.md#autoregistrationstatustype) 
3. See [:material-code-braces: RegistrationConfigTypeDef](./type_defs.md#registrationconfigtypedef) 
4. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_ca_certificate method usage example with argument unpacking

kwargs: UpdateCACertificateRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
}

parent.update_ca_certificate(**kwargs)
```

1. See [:material-code-braces: UpdateCACertificateRequestRequestTypeDef](./type_defs.md#updatecacertificaterequestrequesttypedef) 

### update\_certificate

Updates the status of the specified certificate.

Type annotations and code completion for `#!python session.create_client("iot").update_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_certificate.html)

```python
# update_certificate method definition

await def update_certificate(
    self,
    *,
    certificateId: str,
    newStatus: CertificateStatusType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_certificate method usage example with argument unpacking

kwargs: UpdateCertificateRequestRequestTypeDef = {  # (1)
    "certificateId": ...,
    "newStatus": ...,
}

parent.update_certificate(**kwargs)
```

1. See [:material-code-braces: UpdateCertificateRequestRequestTypeDef](./type_defs.md#updatecertificaterequestrequesttypedef) 

### update\_certificate\_provider

Updates a certificate provider.

Type annotations and code completion for `#!python session.create_client("iot").update_certificate_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_certificate_provider.html)

```python
# update_certificate_provider method definition

await def update_certificate_provider(
    self,
    *,
    certificateProviderName: str,
    lambdaFunctionArn: str = ...,
    accountDefaultForOperations: Sequence[CertificateProviderOperationType] = ...,  # (1)
) -> UpdateCertificateProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CertificateProviderOperationType](./literals.md#certificateprovideroperationtype) 
2. See [:material-code-braces: UpdateCertificateProviderResponseTypeDef](./type_defs.md#updatecertificateproviderresponsetypedef) 


```python
# update_certificate_provider method usage example with argument unpacking

kwargs: UpdateCertificateProviderRequestRequestTypeDef = {  # (1)
    "certificateProviderName": ...,
}

parent.update_certificate_provider(**kwargs)
```

1. See [:material-code-braces: UpdateCertificateProviderRequestRequestTypeDef](./type_defs.md#updatecertificateproviderrequestrequesttypedef) 

### update\_command

Update information about a command or mark a command for deprecation.

Type annotations and code completion for `#!python session.create_client("iot").update_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_command.html)

```python
# update_command method definition

await def update_command(
    self,
    *,
    commandId: str,
    displayName: str = ...,
    description: str = ...,
    deprecated: bool = ...,
) -> UpdateCommandResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateCommandResponseTypeDef](./type_defs.md#updatecommandresponsetypedef) 


```python
# update_command method usage example with argument unpacking

kwargs: UpdateCommandRequestRequestTypeDef = {  # (1)
    "commandId": ...,
}

parent.update_command(**kwargs)
```

1. See [:material-code-braces: UpdateCommandRequestRequestTypeDef](./type_defs.md#updatecommandrequestrequesttypedef) 

### update\_custom\_metric

Updates a Device Defender detect custom metric.

Type annotations and code completion for `#!python session.create_client("iot").update_custom_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_custom_metric.html)

```python
# update_custom_metric method definition

await def update_custom_metric(
    self,
    *,
    metricName: str,
    displayName: str,
) -> UpdateCustomMetricResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateCustomMetricResponseTypeDef](./type_defs.md#updatecustommetricresponsetypedef) 


```python
# update_custom_metric method usage example with argument unpacking

kwargs: UpdateCustomMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
    "displayName": ...,
}

parent.update_custom_metric(**kwargs)
```

1. See [:material-code-braces: UpdateCustomMetricRequestRequestTypeDef](./type_defs.md#updatecustommetricrequestrequesttypedef) 

### update\_dimension

Updates the definition for a dimension.

Type annotations and code completion for `#!python session.create_client("iot").update_dimension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_dimension.html)

```python
# update_dimension method definition

await def update_dimension(
    self,
    *,
    name: str,
    stringValues: Sequence[str],
) -> UpdateDimensionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDimensionResponseTypeDef](./type_defs.md#updatedimensionresponsetypedef) 


```python
# update_dimension method usage example with argument unpacking

kwargs: UpdateDimensionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "stringValues": ...,
}

parent.update_dimension(**kwargs)
```

1. See [:material-code-braces: UpdateDimensionRequestRequestTypeDef](./type_defs.md#updatedimensionrequestrequesttypedef) 

### update\_domain\_configuration

Updates values stored in the domain configuration.

Type annotations and code completion for `#!python session.create_client("iot").update_domain_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_domain_configuration.html)

```python
# update_domain_configuration method definition

await def update_domain_configuration(
    self,
    *,
    domainConfigurationName: str,
    authorizerConfig: AuthorizerConfigTypeDef = ...,  # (1)
    domainConfigurationStatus: DomainConfigurationStatusType = ...,  # (2)
    removeAuthorizerConfig: bool = ...,
    tlsConfig: TlsConfigTypeDef = ...,  # (3)
    serverCertificateConfig: ServerCertificateConfigTypeDef = ...,  # (4)
    authenticationType: AuthenticationTypeType = ...,  # (5)
    applicationProtocol: ApplicationProtocolType = ...,  # (6)
    clientCertificateConfig: ClientCertificateConfigTypeDef = ...,  # (7)
) -> UpdateDomainConfigurationResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: AuthorizerConfigTypeDef](./type_defs.md#authorizerconfigtypedef) 
2. See [:material-code-brackets: DomainConfigurationStatusType](./literals.md#domainconfigurationstatustype) 
3. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
4. See [:material-code-braces: ServerCertificateConfigTypeDef](./type_defs.md#servercertificateconfigtypedef) 
5. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
6. See [:material-code-brackets: ApplicationProtocolType](./literals.md#applicationprotocoltype) 
7. See [:material-code-braces: ClientCertificateConfigTypeDef](./type_defs.md#clientcertificateconfigtypedef) 
8. See [:material-code-braces: UpdateDomainConfigurationResponseTypeDef](./type_defs.md#updatedomainconfigurationresponsetypedef) 


```python
# update_domain_configuration method usage example with argument unpacking

kwargs: UpdateDomainConfigurationRequestRequestTypeDef = {  # (1)
    "domainConfigurationName": ...,
}

parent.update_domain_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateDomainConfigurationRequestRequestTypeDef](./type_defs.md#updatedomainconfigurationrequestrequesttypedef) 

### update\_dynamic\_thing\_group

Updates a dynamic thing group.

Type annotations and code completion for `#!python session.create_client("iot").update_dynamic_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_dynamic_thing_group.html)

```python
# update_dynamic_thing_group method definition

await def update_dynamic_thing_group(
    self,
    *,
    thingGroupName: str,
    thingGroupProperties: ThingGroupPropertiesTypeDef,  # (1)
    expectedVersion: int = ...,
    indexName: str = ...,
    queryString: str = ...,
    queryVersion: str = ...,
) -> UpdateDynamicThingGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
2. See [:material-code-braces: UpdateDynamicThingGroupResponseTypeDef](./type_defs.md#updatedynamicthinggroupresponsetypedef) 


```python
# update_dynamic_thing_group method usage example with argument unpacking

kwargs: UpdateDynamicThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
    "thingGroupProperties": ...,
}

parent.update_dynamic_thing_group(**kwargs)
```

1. See [:material-code-braces: UpdateDynamicThingGroupRequestRequestTypeDef](./type_defs.md#updatedynamicthinggrouprequestrequesttypedef) 

### update\_event\_configurations

Updates the event configurations.

Type annotations and code completion for `#!python session.create_client("iot").update_event_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_event_configurations.html)

```python
# update_event_configurations method definition

await def update_event_configurations(
    self,
    *,
    eventConfigurations: Mapping[EventTypeType, ConfigurationTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 


```python
# update_event_configurations method usage example with argument unpacking

kwargs: UpdateEventConfigurationsRequestRequestTypeDef = {  # (1)
    "eventConfigurations": ...,
}

parent.update_event_configurations(**kwargs)
```

1. See [:material-code-braces: UpdateEventConfigurationsRequestRequestTypeDef](./type_defs.md#updateeventconfigurationsrequestrequesttypedef) 

### update\_fleet\_metric

Updates the data for a fleet metric.

Type annotations and code completion for `#!python session.create_client("iot").update_fleet_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_fleet_metric.html)

```python
# update_fleet_metric method definition

await def update_fleet_metric(
    self,
    *,
    metricName: str,
    indexName: str,
    queryString: str = ...,
    aggregationType: AggregationTypeTypeDef = ...,  # (1)
    period: int = ...,
    aggregationField: str = ...,
    description: str = ...,
    queryVersion: str = ...,
    unit: FleetMetricUnitType = ...,  # (2)
    expectedVersion: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AggregationTypeTypeDef](./type_defs.md#aggregationtypetypedef) 
2. See [:material-code-brackets: FleetMetricUnitType](./literals.md#fleetmetricunittype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_fleet_metric method usage example with argument unpacking

kwargs: UpdateFleetMetricRequestRequestTypeDef = {  # (1)
    "metricName": ...,
    "indexName": ...,
}

parent.update_fleet_metric(**kwargs)
```

1. See [:material-code-braces: UpdateFleetMetricRequestRequestTypeDef](./type_defs.md#updatefleetmetricrequestrequesttypedef) 

### update\_indexing\_configuration

Updates the search configuration.

Type annotations and code completion for `#!python session.create_client("iot").update_indexing_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_indexing_configuration.html)

```python
# update_indexing_configuration method definition

await def update_indexing_configuration(
    self,
    *,
    thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,  # (1)
    thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ThingIndexingConfigurationTypeDef](./type_defs.md#thingindexingconfigurationtypedef) 
2. See [:material-code-braces: ThingGroupIndexingConfigurationTypeDef](./type_defs.md#thinggroupindexingconfigurationtypedef) 


```python
# update_indexing_configuration method usage example with argument unpacking

kwargs: UpdateIndexingConfigurationRequestRequestTypeDef = {  # (1)
    "thingIndexingConfiguration": ...,
}

parent.update_indexing_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateIndexingConfigurationRequestRequestTypeDef](./type_defs.md#updateindexingconfigurationrequestrequesttypedef) 

### update\_job

Updates supported fields of the specified job.

Type annotations and code completion for `#!python session.create_client("iot").update_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_job.html)

```python
# update_job method definition

await def update_job(
    self,
    *,
    jobId: str,
    description: str = ...,
    presignedUrlConfig: PresignedUrlConfigTypeDef = ...,  # (1)
    jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,  # (2)
    abortConfig: AbortConfigTypeDef = ...,  # (3)
    timeoutConfig: TimeoutConfigTypeDef = ...,  # (4)
    namespaceId: str = ...,
    jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,  # (5)
) -> EmptyResponseMetadataTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: PresignedUrlConfigTypeDef](./type_defs.md#presignedurlconfigtypedef) 
2. See [:material-code-braces: JobExecutionsRolloutConfigTypeDef](./type_defs.md#jobexecutionsrolloutconfigtypedef) 
3. See [:material-code-braces: AbortConfigTypeDef](./type_defs.md#abortconfigtypedef) 
4. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
5. See [:material-code-braces: JobExecutionsRetryConfigTypeDef](./type_defs.md#jobexecutionsretryconfigtypedef) 
6. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_job method usage example with argument unpacking

kwargs: UpdateJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.update_job(**kwargs)
```

1. See [:material-code-braces: UpdateJobRequestRequestTypeDef](./type_defs.md#updatejobrequestrequesttypedef) 

### update\_mitigation\_action

Updates the definition for the specified mitigation action.

Type annotations and code completion for `#!python session.create_client("iot").update_mitigation_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_mitigation_action.html)

```python
# update_mitigation_action method definition

await def update_mitigation_action(
    self,
    *,
    actionName: str,
    roleArn: str = ...,
    actionParams: MitigationActionParamsTypeDef = ...,  # (1)
) -> UpdateMitigationActionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MitigationActionParamsTypeDef](./type_defs.md#mitigationactionparamstypedef) 
2. See [:material-code-braces: UpdateMitigationActionResponseTypeDef](./type_defs.md#updatemitigationactionresponsetypedef) 


```python
# update_mitigation_action method usage example with argument unpacking

kwargs: UpdateMitigationActionRequestRequestTypeDef = {  # (1)
    "actionName": ...,
}

parent.update_mitigation_action(**kwargs)
```

1. See [:material-code-braces: UpdateMitigationActionRequestRequestTypeDef](./type_defs.md#updatemitigationactionrequestrequesttypedef) 

### update\_package

Updates the supported fields for a specific software package.

Type annotations and code completion for `#!python session.create_client("iot").update_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_package.html)

```python
# update_package method definition

await def update_package(
    self,
    *,
    packageName: str,
    description: str = ...,
    defaultVersionName: str = ...,
    unsetDefaultVersion: bool = ...,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_package method usage example with argument unpacking

kwargs: UpdatePackageRequestRequestTypeDef = {  # (1)
    "packageName": ...,
}

parent.update_package(**kwargs)
```

1. See [:material-code-braces: UpdatePackageRequestRequestTypeDef](./type_defs.md#updatepackagerequestrequesttypedef) 

### update\_package\_configuration

Updates the software package configuration.

Type annotations and code completion for `#!python session.create_client("iot").update_package_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_package_configuration.html)

```python
# update_package_configuration method definition

await def update_package_configuration(
    self,
    *,
    versionUpdateByJobsConfig: VersionUpdateByJobsConfigTypeDef = ...,  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: VersionUpdateByJobsConfigTypeDef](./type_defs.md#versionupdatebyjobsconfigtypedef) 


```python
# update_package_configuration method usage example with argument unpacking

kwargs: UpdatePackageConfigurationRequestRequestTypeDef = {  # (1)
    "versionUpdateByJobsConfig": ...,
}

parent.update_package_configuration(**kwargs)
```

1. See [:material-code-braces: UpdatePackageConfigurationRequestRequestTypeDef](./type_defs.md#updatepackageconfigurationrequestrequesttypedef) 

### update\_package\_version

Updates the supported fields for a specific package version.

Type annotations and code completion for `#!python session.create_client("iot").update_package_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_package_version.html)

```python
# update_package_version method definition

await def update_package_version(
    self,
    *,
    packageName: str,
    versionName: str,
    description: str = ...,
    attributes: Mapping[str, str] = ...,
    artifact: PackageVersionArtifactTypeDef = ...,  # (1)
    action: PackageVersionActionType = ...,  # (2)
    recipe: str = ...,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: PackageVersionArtifactTypeDef](./type_defs.md#packageversionartifacttypedef) 
2. See [:material-code-brackets: PackageVersionActionType](./literals.md#packageversionactiontype) 


```python
# update_package_version method usage example with argument unpacking

kwargs: UpdatePackageVersionRequestRequestTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
}

parent.update_package_version(**kwargs)
```

1. See [:material-code-braces: UpdatePackageVersionRequestRequestTypeDef](./type_defs.md#updatepackageversionrequestrequesttypedef) 

### update\_provisioning\_template

Updates a provisioning template.

Type annotations and code completion for `#!python session.create_client("iot").update_provisioning_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_provisioning_template.html)

```python
# update_provisioning_template method definition

await def update_provisioning_template(
    self,
    *,
    templateName: str,
    description: str = ...,
    enabled: bool = ...,
    defaultVersionId: int = ...,
    provisioningRoleArn: str = ...,
    preProvisioningHook: ProvisioningHookTypeDef = ...,  # (1)
    removePreProvisioningHook: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ProvisioningHookTypeDef](./type_defs.md#provisioninghooktypedef) 


```python
# update_provisioning_template method usage example with argument unpacking

kwargs: UpdateProvisioningTemplateRequestRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.update_provisioning_template(**kwargs)
```

1. See [:material-code-braces: UpdateProvisioningTemplateRequestRequestTypeDef](./type_defs.md#updateprovisioningtemplaterequestrequesttypedef) 

### update\_role\_alias

Updates a role alias.

Type annotations and code completion for `#!python session.create_client("iot").update_role_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_role_alias.html)

```python
# update_role_alias method definition

await def update_role_alias(
    self,
    *,
    roleAlias: str,
    roleArn: str = ...,
    credentialDurationSeconds: int = ...,
) -> UpdateRoleAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateRoleAliasResponseTypeDef](./type_defs.md#updaterolealiasresponsetypedef) 


```python
# update_role_alias method usage example with argument unpacking

kwargs: UpdateRoleAliasRequestRequestTypeDef = {  # (1)
    "roleAlias": ...,
}

parent.update_role_alias(**kwargs)
```

1. See [:material-code-braces: UpdateRoleAliasRequestRequestTypeDef](./type_defs.md#updaterolealiasrequestrequesttypedef) 

### update\_scheduled\_audit

Updates a scheduled audit, including which checks are performed and how often
the audit takes place.

Type annotations and code completion for `#!python session.create_client("iot").update_scheduled_audit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_scheduled_audit.html)

```python
# update_scheduled_audit method definition

await def update_scheduled_audit(
    self,
    *,
    scheduledAuditName: str,
    frequency: AuditFrequencyType = ...,  # (1)
    dayOfMonth: str = ...,
    dayOfWeek: DayOfWeekType = ...,  # (2)
    targetCheckNames: Sequence[str] = ...,
) -> UpdateScheduledAuditResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuditFrequencyType](./literals.md#auditfrequencytype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
3. See [:material-code-braces: UpdateScheduledAuditResponseTypeDef](./type_defs.md#updatescheduledauditresponsetypedef) 


```python
# update_scheduled_audit method usage example with argument unpacking

kwargs: UpdateScheduledAuditRequestRequestTypeDef = {  # (1)
    "scheduledAuditName": ...,
}

parent.update_scheduled_audit(**kwargs)
```

1. See [:material-code-braces: UpdateScheduledAuditRequestRequestTypeDef](./type_defs.md#updatescheduledauditrequestrequesttypedef) 

### update\_security\_profile

Updates a Device Defender security profile.

Type annotations and code completion for `#!python session.create_client("iot").update_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_security_profile.html)

```python
# update_security_profile method definition

await def update_security_profile(
    self,
    *,
    securityProfileName: str,
    securityProfileDescription: str = ...,
    behaviors: Sequence[BehaviorTypeDef] = ...,  # (1)
    alertTargets: Mapping[AlertTargetTypeType, AlertTargetTypeDef] = ...,  # (2)
    additionalMetricsToRetain: Sequence[str] = ...,
    additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,  # (3)
    deleteBehaviors: bool = ...,
    deleteAlertTargets: bool = ...,
    deleteAdditionalMetricsToRetain: bool = ...,
    expectedVersion: int = ...,
    metricsExportConfig: MetricsExportConfigTypeDef = ...,  # (4)
    deleteMetricsExportConfig: bool = ...,
) -> UpdateSecurityProfileResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: BehaviorTypeDef](./type_defs.md#behaviortypedef) 
2. See [:material-code-brackets: AlertTargetTypeType](./literals.md#alerttargettypetype) [:material-code-braces: AlertTargetTypeDef](./type_defs.md#alerttargettypedef) 
3. See [:material-code-braces: MetricToRetainTypeDef](./type_defs.md#metrictoretaintypedef) 
4. See [:material-code-braces: MetricsExportConfigTypeDef](./type_defs.md#metricsexportconfigtypedef) 
5. See [:material-code-braces: UpdateSecurityProfileResponseTypeDef](./type_defs.md#updatesecurityprofileresponsetypedef) 


```python
# update_security_profile method usage example with argument unpacking

kwargs: UpdateSecurityProfileRequestRequestTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.update_security_profile(**kwargs)
```

1. See [:material-code-braces: UpdateSecurityProfileRequestRequestTypeDef](./type_defs.md#updatesecurityprofilerequestrequesttypedef) 

### update\_stream

Updates an existing stream.

Type annotations and code completion for `#!python session.create_client("iot").update_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_stream.html)

```python
# update_stream method definition

await def update_stream(
    self,
    *,
    streamId: str,
    description: str = ...,
    files: Sequence[StreamFileTypeDef] = ...,  # (1)
    roleArn: str = ...,
) -> UpdateStreamResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamFileTypeDef](./type_defs.md#streamfiletypedef) 
2. See [:material-code-braces: UpdateStreamResponseTypeDef](./type_defs.md#updatestreamresponsetypedef) 


```python
# update_stream method usage example with argument unpacking

kwargs: UpdateStreamRequestRequestTypeDef = {  # (1)
    "streamId": ...,
}

parent.update_stream(**kwargs)
```

1. See [:material-code-braces: UpdateStreamRequestRequestTypeDef](./type_defs.md#updatestreamrequestrequesttypedef) 

### update\_thing

Updates the data for a thing.

Type annotations and code completion for `#!python session.create_client("iot").update_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_thing.html)

```python
# update_thing method definition

await def update_thing(
    self,
    *,
    thingName: str,
    thingTypeName: str = ...,
    attributePayload: AttributePayloadTypeDef = ...,  # (1)
    expectedVersion: int = ...,
    removeThingType: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AttributePayloadTypeDef](./type_defs.md#attributepayloadtypedef) 


```python
# update_thing method usage example with argument unpacking

kwargs: UpdateThingRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.update_thing(**kwargs)
```

1. See [:material-code-braces: UpdateThingRequestRequestTypeDef](./type_defs.md#updatethingrequestrequesttypedef) 

### update\_thing\_group

Update a thing group.

Type annotations and code completion for `#!python session.create_client("iot").update_thing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_thing_group.html)

```python
# update_thing_group method definition

await def update_thing_group(
    self,
    *,
    thingGroupName: str,
    thingGroupProperties: ThingGroupPropertiesTypeDef,  # (1)
    expectedVersion: int = ...,
) -> UpdateThingGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ThingGroupPropertiesTypeDef](./type_defs.md#thinggrouppropertiestypedef) 
2. See [:material-code-braces: UpdateThingGroupResponseTypeDef](./type_defs.md#updatethinggroupresponsetypedef) 


```python
# update_thing_group method usage example with argument unpacking

kwargs: UpdateThingGroupRequestRequestTypeDef = {  # (1)
    "thingGroupName": ...,
    "thingGroupProperties": ...,
}

parent.update_thing_group(**kwargs)
```

1. See [:material-code-braces: UpdateThingGroupRequestRequestTypeDef](./type_defs.md#updatethinggrouprequestrequesttypedef) 

### update\_thing\_groups\_for\_thing

Updates the groups to which the thing belongs.

Type annotations and code completion for `#!python session.create_client("iot").update_thing_groups_for_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_thing_groups_for_thing.html)

```python
# update_thing_groups_for_thing method definition

await def update_thing_groups_for_thing(
    self,
    *,
    thingName: str = ...,
    thingGroupsToAdd: Sequence[str] = ...,
    thingGroupsToRemove: Sequence[str] = ...,
    overrideDynamicGroups: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_thing_groups_for_thing method usage example with argument unpacking

kwargs: UpdateThingGroupsForThingRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.update_thing_groups_for_thing(**kwargs)
```

1. See [:material-code-braces: UpdateThingGroupsForThingRequestRequestTypeDef](./type_defs.md#updatethinggroupsforthingrequestrequesttypedef) 

### update\_thing\_type

Updates a thing type.

Type annotations and code completion for `#!python session.create_client("iot").update_thing_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_thing_type.html)

```python
# update_thing_type method definition

await def update_thing_type(
    self,
    *,
    thingTypeName: str,
    thingTypeProperties: ThingTypePropertiesTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ThingTypePropertiesTypeDef](./type_defs.md#thingtypepropertiestypedef) 


```python
# update_thing_type method usage example with argument unpacking

kwargs: UpdateThingTypeRequestRequestTypeDef = {  # (1)
    "thingTypeName": ...,
}

parent.update_thing_type(**kwargs)
```

1. See [:material-code-braces: UpdateThingTypeRequestRequestTypeDef](./type_defs.md#updatethingtyperequestrequesttypedef) 

### update\_topic\_rule\_destination

Updates a topic rule destination.

Type annotations and code completion for `#!python session.create_client("iot").update_topic_rule_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/update_topic_rule_destination.html)

```python
# update_topic_rule_destination method definition

await def update_topic_rule_destination(
    self,
    *,
    arn: str,
    status: TopicRuleDestinationStatusType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TopicRuleDestinationStatusType](./literals.md#topicruledestinationstatustype) 


```python
# update_topic_rule_destination method usage example with argument unpacking

kwargs: UpdateTopicRuleDestinationRequestRequestTypeDef = {  # (1)
    "arn": ...,
    "status": ...,
}

parent.update_topic_rule_destination(**kwargs)
```

1. See [:material-code-braces: UpdateTopicRuleDestinationRequestRequestTypeDef](./type_defs.md#updatetopicruledestinationrequestrequesttypedef) 

### validate\_security\_profile\_behaviors

Validates a Device Defender security profile behaviors specification.

Type annotations and code completion for `#!python session.create_client("iot").validate_security_profile_behaviors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/client/validate_security_profile_behaviors.html)

```python
# validate_security_profile_behaviors method definition

await def validate_security_profile_behaviors(
    self,
    *,
    behaviors: Sequence[BehaviorTypeDef],  # (1)
) -> ValidateSecurityProfileBehaviorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BehaviorTypeDef](./type_defs.md#behaviortypedef) 
2. See [:material-code-braces: ValidateSecurityProfileBehaviorsResponseTypeDef](./type_defs.md#validatesecurityprofilebehaviorsresponsetypedef) 


```python
# validate_security_profile_behaviors method usage example with argument unpacking

kwargs: ValidateSecurityProfileBehaviorsRequestRequestTypeDef = {  # (1)
    "behaviors": ...,
}

parent.validate_security_profile_behaviors(**kwargs)
```

1. See [:material-code-braces: ValidateSecurityProfileBehaviorsRequestRequestTypeDef](./type_defs.md#validatesecurityprofilebehaviorsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iot").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iot").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client)

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

Type annotations and code completion for `#!python session.create_client("iot").get_paginator` method with overloads.

- `client.get_paginator("get_behavior_model_training_summaries")` -> [GetBehaviorModelTrainingSummariesPaginator](./paginators.md#getbehaviormodeltrainingsummariespaginator)
- `client.get_paginator("list_active_violations")` -> [ListActiveViolationsPaginator](./paginators.md#listactiveviolationspaginator)
- `client.get_paginator("list_attached_policies")` -> [ListAttachedPoliciesPaginator](./paginators.md#listattachedpoliciespaginator)
- `client.get_paginator("list_audit_findings")` -> [ListAuditFindingsPaginator](./paginators.md#listauditfindingspaginator)
- `client.get_paginator("list_audit_mitigation_actions_executions")` -> [ListAuditMitigationActionsExecutionsPaginator](./paginators.md#listauditmitigationactionsexecutionspaginator)
- `client.get_paginator("list_audit_mitigation_actions_tasks")` -> [ListAuditMitigationActionsTasksPaginator](./paginators.md#listauditmitigationactionstaskspaginator)
- `client.get_paginator("list_audit_suppressions")` -> [ListAuditSuppressionsPaginator](./paginators.md#listauditsuppressionspaginator)
- `client.get_paginator("list_audit_tasks")` -> [ListAuditTasksPaginator](./paginators.md#listaudittaskspaginator)
- `client.get_paginator("list_authorizers")` -> [ListAuthorizersPaginator](./paginators.md#listauthorizerspaginator)
- `client.get_paginator("list_billing_groups")` -> [ListBillingGroupsPaginator](./paginators.md#listbillinggroupspaginator)
- `client.get_paginator("list_ca_certificates")` -> [ListCACertificatesPaginator](./paginators.md#listcacertificatespaginator)
- `client.get_paginator("list_certificates_by_ca")` -> [ListCertificatesByCAPaginator](./paginators.md#listcertificatesbycapaginator)
- `client.get_paginator("list_certificates")` -> [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
- `client.get_paginator("list_command_executions")` -> [ListCommandExecutionsPaginator](./paginators.md#listcommandexecutionspaginator)
- `client.get_paginator("list_commands")` -> [ListCommandsPaginator](./paginators.md#listcommandspaginator)
- `client.get_paginator("list_custom_metrics")` -> [ListCustomMetricsPaginator](./paginators.md#listcustommetricspaginator)
- `client.get_paginator("list_detect_mitigation_actions_executions")` -> [ListDetectMitigationActionsExecutionsPaginator](./paginators.md#listdetectmitigationactionsexecutionspaginator)
- `client.get_paginator("list_detect_mitigation_actions_tasks")` -> [ListDetectMitigationActionsTasksPaginator](./paginators.md#listdetectmitigationactionstaskspaginator)
- `client.get_paginator("list_dimensions")` -> [ListDimensionsPaginator](./paginators.md#listdimensionspaginator)
- `client.get_paginator("list_domain_configurations")` -> [ListDomainConfigurationsPaginator](./paginators.md#listdomainconfigurationspaginator)
- `client.get_paginator("list_fleet_metrics")` -> [ListFleetMetricsPaginator](./paginators.md#listfleetmetricspaginator)
- `client.get_paginator("list_indices")` -> [ListIndicesPaginator](./paginators.md#listindicespaginator)
- `client.get_paginator("list_job_executions_for_job")` -> [ListJobExecutionsForJobPaginator](./paginators.md#listjobexecutionsforjobpaginator)
- `client.get_paginator("list_job_executions_for_thing")` -> [ListJobExecutionsForThingPaginator](./paginators.md#listjobexecutionsforthingpaginator)
- `client.get_paginator("list_job_templates")` -> [ListJobTemplatesPaginator](./paginators.md#listjobtemplatespaginator)
- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_managed_job_templates")` -> [ListManagedJobTemplatesPaginator](./paginators.md#listmanagedjobtemplatespaginator)
- `client.get_paginator("list_metric_values")` -> [ListMetricValuesPaginator](./paginators.md#listmetricvaluespaginator)
- `client.get_paginator("list_mitigation_actions")` -> [ListMitigationActionsPaginator](./paginators.md#listmitigationactionspaginator)
- `client.get_paginator("list_ota_updates")` -> [ListOTAUpdatesPaginator](./paginators.md#listotaupdatespaginator)
- `client.get_paginator("list_outgoing_certificates")` -> [ListOutgoingCertificatesPaginator](./paginators.md#listoutgoingcertificatespaginator)
- `client.get_paginator("list_package_versions")` -> [ListPackageVersionsPaginator](./paginators.md#listpackageversionspaginator)
- `client.get_paginator("list_packages")` -> [ListPackagesPaginator](./paginators.md#listpackagespaginator)
- `client.get_paginator("list_policies")` -> [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- `client.get_paginator("list_policy_principals")` -> [ListPolicyPrincipalsPaginator](./paginators.md#listpolicyprincipalspaginator)
- `client.get_paginator("list_principal_policies")` -> [ListPrincipalPoliciesPaginator](./paginators.md#listprincipalpoliciespaginator)
- `client.get_paginator("list_principal_things")` -> [ListPrincipalThingsPaginator](./paginators.md#listprincipalthingspaginator)
- `client.get_paginator("list_principal_things_v2")` -> [ListPrincipalThingsV2Paginator](./paginators.md#listprincipalthingsv2paginator)
- `client.get_paginator("list_provisioning_template_versions")` -> [ListProvisioningTemplateVersionsPaginator](./paginators.md#listprovisioningtemplateversionspaginator)
- `client.get_paginator("list_provisioning_templates")` -> [ListProvisioningTemplatesPaginator](./paginators.md#listprovisioningtemplatespaginator)
- `client.get_paginator("list_related_resources_for_audit_finding")` -> [ListRelatedResourcesForAuditFindingPaginator](./paginators.md#listrelatedresourcesforauditfindingpaginator)
- `client.get_paginator("list_role_aliases")` -> [ListRoleAliasesPaginator](./paginators.md#listrolealiasespaginator)
- `client.get_paginator("list_sbom_validation_results")` -> [ListSbomValidationResultsPaginator](./paginators.md#listsbomvalidationresultspaginator)
- `client.get_paginator("list_scheduled_audits")` -> [ListScheduledAuditsPaginator](./paginators.md#listscheduledauditspaginator)
- `client.get_paginator("list_security_profiles_for_target")` -> [ListSecurityProfilesForTargetPaginator](./paginators.md#listsecurityprofilesfortargetpaginator)
- `client.get_paginator("list_security_profiles")` -> [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
- `client.get_paginator("list_streams")` -> [ListStreamsPaginator](./paginators.md#liststreamspaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_targets_for_policy")` -> [ListTargetsForPolicyPaginator](./paginators.md#listtargetsforpolicypaginator)
- `client.get_paginator("list_targets_for_security_profile")` -> [ListTargetsForSecurityProfilePaginator](./paginators.md#listtargetsforsecurityprofilepaginator)
- `client.get_paginator("list_thing_groups_for_thing")` -> [ListThingGroupsForThingPaginator](./paginators.md#listthinggroupsforthingpaginator)
- `client.get_paginator("list_thing_groups")` -> [ListThingGroupsPaginator](./paginators.md#listthinggroupspaginator)
- `client.get_paginator("list_thing_principals")` -> [ListThingPrincipalsPaginator](./paginators.md#listthingprincipalspaginator)
- `client.get_paginator("list_thing_principals_v2")` -> [ListThingPrincipalsV2Paginator](./paginators.md#listthingprincipalsv2paginator)
- `client.get_paginator("list_thing_registration_task_reports")` -> [ListThingRegistrationTaskReportsPaginator](./paginators.md#listthingregistrationtaskreportspaginator)
- `client.get_paginator("list_thing_registration_tasks")` -> [ListThingRegistrationTasksPaginator](./paginators.md#listthingregistrationtaskspaginator)
- `client.get_paginator("list_thing_types")` -> [ListThingTypesPaginator](./paginators.md#listthingtypespaginator)
- `client.get_paginator("list_things_in_billing_group")` -> [ListThingsInBillingGroupPaginator](./paginators.md#listthingsinbillinggrouppaginator)
- `client.get_paginator("list_things_in_thing_group")` -> [ListThingsInThingGroupPaginator](./paginators.md#listthingsinthinggrouppaginator)
- `client.get_paginator("list_things")` -> [ListThingsPaginator](./paginators.md#listthingspaginator)
- `client.get_paginator("list_topic_rule_destinations")` -> [ListTopicRuleDestinationsPaginator](./paginators.md#listtopicruledestinationspaginator)
- `client.get_paginator("list_topic_rules")` -> [ListTopicRulesPaginator](./paginators.md#listtopicrulespaginator)
- `client.get_paginator("list_v2_logging_levels")` -> [ListV2LoggingLevelsPaginator](./paginators.md#listv2logginglevelspaginator)
- `client.get_paginator("list_violation_events")` -> [ListViolationEventsPaginator](./paginators.md#listviolationeventspaginator)



