# DeadlineCloudClient

> [Index](../README.md) > [DeadlineCloud](./README.md) > DeadlineCloudClient

!!! note ""

    Auto-generated documentation for [DeadlineCloud](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#deadlinecloud)
    type annotations stubs module [types-aiobotocore-deadline](https://pypi.org/project/types-aiobotocore-deadline/).

## DeadlineCloudClient

Type annotations and code completion for `#!python session.create_client("deadline")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#DeadlineCloud.Client)

```python
# DeadlineCloudClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_deadline.client import DeadlineCloudClient

session = get_session()
async with session.create_client("deadline") as client:
    client: DeadlineCloudClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("deadline").exceptions` structure.

```python
# DeadlineCloudClient.exceptions usage example

async with session.create_client("deadline") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerErrorException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# DeadlineCloudClient usage type checking example

from types_aiobotocore_deadline.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("deadline").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("deadline").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("deadline").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### associate\_member\_to\_farm

Assigns a farm membership level to a member.

Type annotations and code completion for `#!python session.create_client("deadline").associate_member_to_farm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/associate_member_to_farm.html)

```python
# associate_member_to_farm method definition

await def associate_member_to_farm(
    self,
    *,
    farmId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 


```python
# associate_member_to_farm method usage example with argument unpacking

kwargs: AssociateMemberToFarmRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "principalId": ...,
    "principalType": ...,
    "identityStoreId": ...,
    "membershipLevel": ...,
}

parent.associate_member_to_farm(**kwargs)
```

1. See [:material-code-braces: AssociateMemberToFarmRequestRequestTypeDef](./type_defs.md#associatemembertofarmrequestrequesttypedef) 

### associate\_member\_to\_fleet

Assigns a fleet membership level to a member.

Type annotations and code completion for `#!python session.create_client("deadline").associate_member_to_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/associate_member_to_fleet.html)

```python
# associate_member_to_fleet method definition

await def associate_member_to_fleet(
    self,
    *,
    farmId: str,
    fleetId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 


```python
# associate_member_to_fleet method usage example with argument unpacking

kwargs: AssociateMemberToFleetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "principalId": ...,
    "principalType": ...,
    "identityStoreId": ...,
    "membershipLevel": ...,
}

parent.associate_member_to_fleet(**kwargs)
```

1. See [:material-code-braces: AssociateMemberToFleetRequestRequestTypeDef](./type_defs.md#associatemembertofleetrequestrequesttypedef) 

### associate\_member\_to\_job

Assigns a job membership level to a member.

Type annotations and code completion for `#!python session.create_client("deadline").associate_member_to_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/associate_member_to_job.html)

```python
# associate_member_to_job method definition

await def associate_member_to_job(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 


```python
# associate_member_to_job method usage example with argument unpacking

kwargs: AssociateMemberToJobRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "principalId": ...,
    "principalType": ...,
    "identityStoreId": ...,
    "membershipLevel": ...,
}

parent.associate_member_to_job(**kwargs)
```

1. See [:material-code-braces: AssociateMemberToJobRequestRequestTypeDef](./type_defs.md#associatemembertojobrequestrequesttypedef) 

### associate\_member\_to\_queue

Assigns a queue membership level to a member.

Type annotations and code completion for `#!python session.create_client("deadline").associate_member_to_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/associate_member_to_queue.html)

```python
# associate_member_to_queue method definition

await def associate_member_to_queue(
    self,
    *,
    farmId: str,
    queueId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 


```python
# associate_member_to_queue method usage example with argument unpacking

kwargs: AssociateMemberToQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "principalId": ...,
    "principalType": ...,
    "identityStoreId": ...,
    "membershipLevel": ...,
}

parent.associate_member_to_queue(**kwargs)
```

1. See [:material-code-braces: AssociateMemberToQueueRequestRequestTypeDef](./type_defs.md#associatemembertoqueuerequestrequesttypedef) 

### assume\_fleet\_role\_for\_read

Get Amazon Web Services credentials from the fleet role.

Type annotations and code completion for `#!python session.create_client("deadline").assume_fleet_role_for_read` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/assume_fleet_role_for_read.html)

```python
# assume_fleet_role_for_read method definition

await def assume_fleet_role_for_read(
    self,
    *,
    farmId: str,
    fleetId: str,
) -> AssumeFleetRoleForReadResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeFleetRoleForReadResponseTypeDef](./type_defs.md#assumefleetroleforreadresponsetypedef) 


```python
# assume_fleet_role_for_read method usage example with argument unpacking

kwargs: AssumeFleetRoleForReadRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.assume_fleet_role_for_read(**kwargs)
```

1. See [:material-code-braces: AssumeFleetRoleForReadRequestRequestTypeDef](./type_defs.md#assumefleetroleforreadrequestrequesttypedef) 

### assume\_fleet\_role\_for\_worker

Get credentials from the fleet role for a worker.

Type annotations and code completion for `#!python session.create_client("deadline").assume_fleet_role_for_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/assume_fleet_role_for_worker.html)

```python
# assume_fleet_role_for_worker method definition

await def assume_fleet_role_for_worker(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
) -> AssumeFleetRoleForWorkerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeFleetRoleForWorkerResponseTypeDef](./type_defs.md#assumefleetroleforworkerresponsetypedef) 


```python
# assume_fleet_role_for_worker method usage example with argument unpacking

kwargs: AssumeFleetRoleForWorkerRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
}

parent.assume_fleet_role_for_worker(**kwargs)
```

1. See [:material-code-braces: AssumeFleetRoleForWorkerRequestRequestTypeDef](./type_defs.md#assumefleetroleforworkerrequestrequesttypedef) 

### assume\_queue\_role\_for\_read

Gets Amazon Web Services credentials from the queue role.

Type annotations and code completion for `#!python session.create_client("deadline").assume_queue_role_for_read` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/assume_queue_role_for_read.html)

```python
# assume_queue_role_for_read method definition

await def assume_queue_role_for_read(
    self,
    *,
    farmId: str,
    queueId: str,
) -> AssumeQueueRoleForReadResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeQueueRoleForReadResponseTypeDef](./type_defs.md#assumequeueroleforreadresponsetypedef) 


```python
# assume_queue_role_for_read method usage example with argument unpacking

kwargs: AssumeQueueRoleForReadRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.assume_queue_role_for_read(**kwargs)
```

1. See [:material-code-braces: AssumeQueueRoleForReadRequestRequestTypeDef](./type_defs.md#assumequeueroleforreadrequestrequesttypedef) 

### assume\_queue\_role\_for\_user

Allows a user to assume a role for a queue.

Type annotations and code completion for `#!python session.create_client("deadline").assume_queue_role_for_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/assume_queue_role_for_user.html)

```python
# assume_queue_role_for_user method definition

await def assume_queue_role_for_user(
    self,
    *,
    farmId: str,
    queueId: str,
) -> AssumeQueueRoleForUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeQueueRoleForUserResponseTypeDef](./type_defs.md#assumequeueroleforuserresponsetypedef) 


```python
# assume_queue_role_for_user method usage example with argument unpacking

kwargs: AssumeQueueRoleForUserRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.assume_queue_role_for_user(**kwargs)
```

1. See [:material-code-braces: AssumeQueueRoleForUserRequestRequestTypeDef](./type_defs.md#assumequeueroleforuserrequestrequesttypedef) 

### assume\_queue\_role\_for\_worker

Allows a worker to assume a queue role.

Type annotations and code completion for `#!python session.create_client("deadline").assume_queue_role_for_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/assume_queue_role_for_worker.html)

```python
# assume_queue_role_for_worker method definition

await def assume_queue_role_for_worker(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
    queueId: str,
) -> AssumeQueueRoleForWorkerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeQueueRoleForWorkerResponseTypeDef](./type_defs.md#assumequeueroleforworkerresponsetypedef) 


```python
# assume_queue_role_for_worker method usage example with argument unpacking

kwargs: AssumeQueueRoleForWorkerRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
    "queueId": ...,
}

parent.assume_queue_role_for_worker(**kwargs)
```

1. See [:material-code-braces: AssumeQueueRoleForWorkerRequestRequestTypeDef](./type_defs.md#assumequeueroleforworkerrequestrequesttypedef) 

### batch\_get\_job\_entity

Get batched job details for a worker.

Type annotations and code completion for `#!python session.create_client("deadline").batch_get_job_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/batch_get_job_entity.html)

```python
# batch_get_job_entity method definition

await def batch_get_job_entity(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
    identifiers: Sequence[JobEntityIdentifiersUnionTypeDef],  # (1)
) -> BatchGetJobEntityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: JobEntityIdentifiersUnionTypeDef](./type_defs.md#jobentityidentifiersuniontypedef) 
2. See [:material-code-braces: BatchGetJobEntityResponseTypeDef](./type_defs.md#batchgetjobentityresponsetypedef) 


```python
# batch_get_job_entity method usage example with argument unpacking

kwargs: BatchGetJobEntityRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
    "identifiers": ...,
}

parent.batch_get_job_entity(**kwargs)
```

1. See [:material-code-braces: BatchGetJobEntityRequestRequestTypeDef](./type_defs.md#batchgetjobentityrequestrequesttypedef) 

### copy\_job\_template

Copies a job template to an Amazon S3 bucket.

Type annotations and code completion for `#!python session.create_client("deadline").copy_job_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/copy_job_template.html)

```python
# copy_job_template method definition

await def copy_job_template(
    self,
    *,
    farmId: str,
    jobId: str,
    queueId: str,
    targetS3Location: S3LocationTypeDef,  # (1)
) -> CopyJobTemplateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: CopyJobTemplateResponseTypeDef](./type_defs.md#copyjobtemplateresponsetypedef) 


```python
# copy_job_template method usage example with argument unpacking

kwargs: CopyJobTemplateRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "jobId": ...,
    "queueId": ...,
    "targetS3Location": ...,
}

parent.copy_job_template(**kwargs)
```

1. See [:material-code-braces: CopyJobTemplateRequestRequestTypeDef](./type_defs.md#copyjobtemplaterequestrequesttypedef) 

### create\_budget

Creates a budget to set spending thresholds for your rendering activity.

Type annotations and code completion for `#!python session.create_client("deadline").create_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_budget.html)

```python
# create_budget method definition

await def create_budget(
    self,
    *,
    farmId: str,
    usageTrackingResource: UsageTrackingResourceTypeDef,  # (1)
    displayName: str,
    approximateDollarLimit: float,
    actions: Sequence[BudgetActionToAddTypeDef],  # (2)
    schedule: BudgetScheduleTypeDef,  # (3)
    clientToken: str = ...,
    description: str = ...,
) -> CreateBudgetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: UsageTrackingResourceTypeDef](./type_defs.md#usagetrackingresourcetypedef) 
2. See [:material-code-braces: BudgetActionToAddTypeDef](./type_defs.md#budgetactiontoaddtypedef) 
3. See [:material-code-braces: BudgetScheduleTypeDef](./type_defs.md#budgetscheduletypedef) 
4. See [:material-code-braces: CreateBudgetResponseTypeDef](./type_defs.md#createbudgetresponsetypedef) 


```python
# create_budget method usage example with argument unpacking

kwargs: CreateBudgetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "usageTrackingResource": ...,
    "displayName": ...,
    "approximateDollarLimit": ...,
    "actions": ...,
    "schedule": ...,
}

parent.create_budget(**kwargs)
```

1. See [:material-code-braces: CreateBudgetRequestRequestTypeDef](./type_defs.md#createbudgetrequestrequesttypedef) 

### create\_farm

Creates a farm to allow space for queues and fleets.

Type annotations and code completion for `#!python session.create_client("deadline").create_farm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_farm.html)

```python
# create_farm method definition

await def create_farm(
    self,
    *,
    displayName: str,
    clientToken: str = ...,
    description: str = ...,
    kmsKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateFarmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateFarmResponseTypeDef](./type_defs.md#createfarmresponsetypedef) 


```python
# create_farm method usage example with argument unpacking

kwargs: CreateFarmRequestRequestTypeDef = {  # (1)
    "displayName": ...,
}

parent.create_farm(**kwargs)
```

1. See [:material-code-braces: CreateFarmRequestRequestTypeDef](./type_defs.md#createfarmrequestrequesttypedef) 

### create\_fleet

Creates a fleet.

Type annotations and code completion for `#!python session.create_client("deadline").create_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_fleet.html)

```python
# create_fleet method definition

await def create_fleet(
    self,
    *,
    farmId: str,
    displayName: str,
    roleArn: str,
    maxWorkerCount: int,
    configuration: FleetConfigurationTypeDef,  # (1)
    clientToken: str = ...,
    description: str = ...,
    minWorkerCount: int = ...,
    tags: Mapping[str, str] = ...,
) -> CreateFleetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FleetConfigurationTypeDef](./type_defs.md#fleetconfigurationtypedef) 
2. See [:material-code-braces: CreateFleetResponseTypeDef](./type_defs.md#createfleetresponsetypedef) 


```python
# create_fleet method usage example with argument unpacking

kwargs: CreateFleetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "displayName": ...,
    "roleArn": ...,
    "maxWorkerCount": ...,
    "configuration": ...,
}

parent.create_fleet(**kwargs)
```

1. See [:material-code-braces: CreateFleetRequestRequestTypeDef](./type_defs.md#createfleetrequestrequesttypedef) 

### create\_job

Creates a job.

Type annotations and code completion for `#!python session.create_client("deadline").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_job.html)

```python
# create_job method definition

await def create_job(
    self,
    *,
    farmId: str,
    queueId: str,
    priority: int,
    clientToken: str = ...,
    template: str = ...,
    templateType: JobTemplateTypeType = ...,  # (1)
    parameters: Mapping[str, JobParameterTypeDef] = ...,  # (2)
    attachments: AttachmentsTypeDef = ...,  # (3)
    storageProfileId: str = ...,
    targetTaskRunStatus: CreateJobTargetTaskRunStatusType = ...,  # (4)
    maxFailedTasksCount: int = ...,
    maxRetriesPerTask: int = ...,
    sourceJobId: str = ...,
) -> CreateJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: JobTemplateTypeType](./literals.md#jobtemplatetypetype) 
2. See [:material-code-braces: JobParameterTypeDef](./type_defs.md#jobparametertypedef) 
3. See [:material-code-braces: AttachmentsTypeDef](./type_defs.md#attachmentstypedef) 
4. See [:material-code-brackets: CreateJobTargetTaskRunStatusType](./literals.md#createjobtargettaskrunstatustype) 
5. See [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef) 


```python
# create_job method usage example with argument unpacking

kwargs: CreateJobRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "priority": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef) 

### create\_license\_endpoint

Creates a license endpoint to integrate your various licensed software used for
rendering on Deadline Cloud.

Type annotations and code completion for `#!python session.create_client("deadline").create_license_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_license_endpoint.html)

```python
# create_license_endpoint method definition

await def create_license_endpoint(
    self,
    *,
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateLicenseEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLicenseEndpointResponseTypeDef](./type_defs.md#createlicenseendpointresponsetypedef) 


```python
# create_license_endpoint method usage example with argument unpacking

kwargs: CreateLicenseEndpointRequestRequestTypeDef = {  # (1)
    "vpcId": ...,
    "subnetIds": ...,
    "securityGroupIds": ...,
}

parent.create_license_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateLicenseEndpointRequestRequestTypeDef](./type_defs.md#createlicenseendpointrequestrequesttypedef) 

### create\_monitor

Creates an Amazon Web Services Deadline Cloud monitor that you can use to view
your farms, queues, and fleets.

Type annotations and code completion for `#!python session.create_client("deadline").create_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_monitor.html)

```python
# create_monitor method definition

await def create_monitor(
    self,
    *,
    displayName: str,
    identityCenterInstanceArn: str,
    subdomain: str,
    roleArn: str,
    clientToken: str = ...,
) -> CreateMonitorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateMonitorResponseTypeDef](./type_defs.md#createmonitorresponsetypedef) 


```python
# create_monitor method usage example with argument unpacking

kwargs: CreateMonitorRequestRequestTypeDef = {  # (1)
    "displayName": ...,
    "identityCenterInstanceArn": ...,
    "subdomain": ...,
    "roleArn": ...,
}

parent.create_monitor(**kwargs)
```

1. See [:material-code-braces: CreateMonitorRequestRequestTypeDef](./type_defs.md#createmonitorrequestrequesttypedef) 

### create\_queue

Creates a queue to coordinate the order in which jobs run on a farm.

Type annotations and code completion for `#!python session.create_client("deadline").create_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_queue.html)

```python
# create_queue method definition

await def create_queue(
    self,
    *,
    farmId: str,
    displayName: str,
    clientToken: str = ...,
    description: str = ...,
    defaultBudgetAction: DefaultQueueBudgetActionType = ...,  # (1)
    jobAttachmentSettings: JobAttachmentSettingsTypeDef = ...,  # (2)
    roleArn: str = ...,
    jobRunAsUser: JobRunAsUserTypeDef = ...,  # (3)
    requiredFileSystemLocationNames: Sequence[str] = ...,
    allowedStorageProfileIds: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
) -> CreateQueueResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: DefaultQueueBudgetActionType](./literals.md#defaultqueuebudgetactiontype) 
2. See [:material-code-braces: JobAttachmentSettingsTypeDef](./type_defs.md#jobattachmentsettingstypedef) 
3. See [:material-code-braces: JobRunAsUserTypeDef](./type_defs.md#jobrunasusertypedef) 
4. See [:material-code-braces: CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef) 


```python
# create_queue method usage example with argument unpacking

kwargs: CreateQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "displayName": ...,
}

parent.create_queue(**kwargs)
```

1. See [:material-code-braces: CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef) 

### create\_queue\_environment

Creates an environment for a queue that defines how jobs in the queue run.

Type annotations and code completion for `#!python session.create_client("deadline").create_queue_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_queue_environment.html)

```python
# create_queue_environment method definition

await def create_queue_environment(
    self,
    *,
    farmId: str,
    queueId: str,
    priority: int,
    templateType: EnvironmentTemplateTypeType,  # (1)
    template: str,
    clientToken: str = ...,
) -> CreateQueueEnvironmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EnvironmentTemplateTypeType](./literals.md#environmenttemplatetypetype) 
2. See [:material-code-braces: CreateQueueEnvironmentResponseTypeDef](./type_defs.md#createqueueenvironmentresponsetypedef) 


```python
# create_queue_environment method usage example with argument unpacking

kwargs: CreateQueueEnvironmentRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "priority": ...,
    "templateType": ...,
    "template": ...,
}

parent.create_queue_environment(**kwargs)
```

1. See [:material-code-braces: CreateQueueEnvironmentRequestRequestTypeDef](./type_defs.md#createqueueenvironmentrequestrequesttypedef) 

### create\_queue\_fleet\_association

Creates an association between a queue and a fleet.

Type annotations and code completion for `#!python session.create_client("deadline").create_queue_fleet_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_queue_fleet_association.html)

```python
# create_queue_fleet_association method definition

await def create_queue_fleet_association(
    self,
    *,
    farmId: str,
    queueId: str,
    fleetId: str,
) -> Dict[str, Any]:
    ...
```



```python
# create_queue_fleet_association method usage example with argument unpacking

kwargs: CreateQueueFleetAssociationRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "fleetId": ...,
}

parent.create_queue_fleet_association(**kwargs)
```

1. See [:material-code-braces: CreateQueueFleetAssociationRequestRequestTypeDef](./type_defs.md#createqueuefleetassociationrequestrequesttypedef) 

### create\_storage\_profile

Creates a storage profile that specifies the operating system, file type, and
file location of resources used on a farm.

Type annotations and code completion for `#!python session.create_client("deadline").create_storage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_storage_profile.html)

```python
# create_storage_profile method definition

await def create_storage_profile(
    self,
    *,
    farmId: str,
    displayName: str,
    osFamily: StorageProfileOperatingSystemFamilyType,  # (1)
    clientToken: str = ...,
    fileSystemLocations: Sequence[FileSystemLocationTypeDef] = ...,  # (2)
) -> CreateStorageProfileResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
2. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 
3. See [:material-code-braces: CreateStorageProfileResponseTypeDef](./type_defs.md#createstorageprofileresponsetypedef) 


```python
# create_storage_profile method usage example with argument unpacking

kwargs: CreateStorageProfileRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "displayName": ...,
    "osFamily": ...,
}

parent.create_storage_profile(**kwargs)
```

1. See [:material-code-braces: CreateStorageProfileRequestRequestTypeDef](./type_defs.md#createstorageprofilerequestrequesttypedef) 

### create\_worker

Creates a worker.

Type annotations and code completion for `#!python session.create_client("deadline").create_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/create_worker.html)

```python
# create_worker method definition

await def create_worker(
    self,
    *,
    farmId: str,
    fleetId: str,
    hostProperties: HostPropertiesRequestTypeDef = ...,  # (1)
    clientToken: str = ...,
) -> CreateWorkerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HostPropertiesRequestTypeDef](./type_defs.md#hostpropertiesrequesttypedef) 
2. See [:material-code-braces: CreateWorkerResponseTypeDef](./type_defs.md#createworkerresponsetypedef) 


```python
# create_worker method usage example with argument unpacking

kwargs: CreateWorkerRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.create_worker(**kwargs)
```

1. See [:material-code-braces: CreateWorkerRequestRequestTypeDef](./type_defs.md#createworkerrequestrequesttypedef) 

### delete\_budget

Deletes a budget.

Type annotations and code completion for `#!python session.create_client("deadline").delete_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_budget.html)

```python
# delete_budget method definition

await def delete_budget(
    self,
    *,
    farmId: str,
    budgetId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_budget method usage example with argument unpacking

kwargs: DeleteBudgetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "budgetId": ...,
}

parent.delete_budget(**kwargs)
```

1. See [:material-code-braces: DeleteBudgetRequestRequestTypeDef](./type_defs.md#deletebudgetrequestrequesttypedef) 

### delete\_farm

Deletes a farm.

Type annotations and code completion for `#!python session.create_client("deadline").delete_farm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_farm.html)

```python
# delete_farm method definition

await def delete_farm(
    self,
    *,
    farmId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_farm method usage example with argument unpacking

kwargs: DeleteFarmRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.delete_farm(**kwargs)
```

1. See [:material-code-braces: DeleteFarmRequestRequestTypeDef](./type_defs.md#deletefarmrequestrequesttypedef) 

### delete\_fleet

Deletes a fleet.

Type annotations and code completion for `#!python session.create_client("deadline").delete_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_fleet.html)

```python
# delete_fleet method definition

await def delete_fleet(
    self,
    *,
    farmId: str,
    fleetId: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_fleet method usage example with argument unpacking

kwargs: DeleteFleetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.delete_fleet(**kwargs)
```

1. See [:material-code-braces: DeleteFleetRequestRequestTypeDef](./type_defs.md#deletefleetrequestrequesttypedef) 

### delete\_license\_endpoint

Deletes a license endpoint.

Type annotations and code completion for `#!python session.create_client("deadline").delete_license_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_license_endpoint.html)

```python
# delete_license_endpoint method definition

await def delete_license_endpoint(
    self,
    *,
    licenseEndpointId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_license_endpoint method usage example with argument unpacking

kwargs: DeleteLicenseEndpointRequestRequestTypeDef = {  # (1)
    "licenseEndpointId": ...,
}

parent.delete_license_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteLicenseEndpointRequestRequestTypeDef](./type_defs.md#deletelicenseendpointrequestrequesttypedef) 

### delete\_metered\_product

Deletes a metered product.

Type annotations and code completion for `#!python session.create_client("deadline").delete_metered_product` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_metered_product.html)

```python
# delete_metered_product method definition

await def delete_metered_product(
    self,
    *,
    licenseEndpointId: str,
    productId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_metered_product method usage example with argument unpacking

kwargs: DeleteMeteredProductRequestRequestTypeDef = {  # (1)
    "licenseEndpointId": ...,
    "productId": ...,
}

parent.delete_metered_product(**kwargs)
```

1. See [:material-code-braces: DeleteMeteredProductRequestRequestTypeDef](./type_defs.md#deletemeteredproductrequestrequesttypedef) 

### delete\_monitor

Removes a Deadline Cloud monitor.

Type annotations and code completion for `#!python session.create_client("deadline").delete_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_monitor.html)

```python
# delete_monitor method definition

await def delete_monitor(
    self,
    *,
    monitorId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_monitor method usage example with argument unpacking

kwargs: DeleteMonitorRequestRequestTypeDef = {  # (1)
    "monitorId": ...,
}

parent.delete_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteMonitorRequestRequestTypeDef](./type_defs.md#deletemonitorrequestrequesttypedef) 

### delete\_queue

Deletes a queue.

Type annotations and code completion for `#!python session.create_client("deadline").delete_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_queue.html)

```python
# delete_queue method definition

await def delete_queue(
    self,
    *,
    farmId: str,
    queueId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_queue method usage example with argument unpacking

kwargs: DeleteQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.delete_queue(**kwargs)
```

1. See [:material-code-braces: DeleteQueueRequestRequestTypeDef](./type_defs.md#deletequeuerequestrequesttypedef) 

### delete\_queue\_environment

Deletes a queue environment.

Type annotations and code completion for `#!python session.create_client("deadline").delete_queue_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_queue_environment.html)

```python
# delete_queue_environment method definition

await def delete_queue_environment(
    self,
    *,
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_queue_environment method usage example with argument unpacking

kwargs: DeleteQueueEnvironmentRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "queueEnvironmentId": ...,
}

parent.delete_queue_environment(**kwargs)
```

1. See [:material-code-braces: DeleteQueueEnvironmentRequestRequestTypeDef](./type_defs.md#deletequeueenvironmentrequestrequesttypedef) 

### delete\_queue\_fleet\_association

Deletes a queue-fleet association.

Type annotations and code completion for `#!python session.create_client("deadline").delete_queue_fleet_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_queue_fleet_association.html)

```python
# delete_queue_fleet_association method definition

await def delete_queue_fleet_association(
    self,
    *,
    farmId: str,
    queueId: str,
    fleetId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_queue_fleet_association method usage example with argument unpacking

kwargs: DeleteQueueFleetAssociationRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "fleetId": ...,
}

parent.delete_queue_fleet_association(**kwargs)
```

1. See [:material-code-braces: DeleteQueueFleetAssociationRequestRequestTypeDef](./type_defs.md#deletequeuefleetassociationrequestrequesttypedef) 

### delete\_storage\_profile

Deletes a storage profile.

Type annotations and code completion for `#!python session.create_client("deadline").delete_storage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_storage_profile.html)

```python
# delete_storage_profile method definition

await def delete_storage_profile(
    self,
    *,
    farmId: str,
    storageProfileId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_storage_profile method usage example with argument unpacking

kwargs: DeleteStorageProfileRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "storageProfileId": ...,
}

parent.delete_storage_profile(**kwargs)
```

1. See [:material-code-braces: DeleteStorageProfileRequestRequestTypeDef](./type_defs.md#deletestorageprofilerequestrequesttypedef) 

### delete\_worker

Deletes a worker.

Type annotations and code completion for `#!python session.create_client("deadline").delete_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/delete_worker.html)

```python
# delete_worker method definition

await def delete_worker(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_worker method usage example with argument unpacking

kwargs: DeleteWorkerRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
}

parent.delete_worker(**kwargs)
```

1. See [:material-code-braces: DeleteWorkerRequestRequestTypeDef](./type_defs.md#deleteworkerrequestrequesttypedef) 

### disassociate\_member\_from\_farm

Disassociates a member from a farm.

Type annotations and code completion for `#!python session.create_client("deadline").disassociate_member_from_farm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/disassociate_member_from_farm.html)

```python
# disassociate_member_from_farm method definition

await def disassociate_member_from_farm(
    self,
    *,
    farmId: str,
    principalId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_member_from_farm method usage example with argument unpacking

kwargs: DisassociateMemberFromFarmRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "principalId": ...,
}

parent.disassociate_member_from_farm(**kwargs)
```

1. See [:material-code-braces: DisassociateMemberFromFarmRequestRequestTypeDef](./type_defs.md#disassociatememberfromfarmrequestrequesttypedef) 

### disassociate\_member\_from\_fleet

Disassociates a member from a fleet.

Type annotations and code completion for `#!python session.create_client("deadline").disassociate_member_from_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/disassociate_member_from_fleet.html)

```python
# disassociate_member_from_fleet method definition

await def disassociate_member_from_fleet(
    self,
    *,
    farmId: str,
    fleetId: str,
    principalId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_member_from_fleet method usage example with argument unpacking

kwargs: DisassociateMemberFromFleetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "principalId": ...,
}

parent.disassociate_member_from_fleet(**kwargs)
```

1. See [:material-code-braces: DisassociateMemberFromFleetRequestRequestTypeDef](./type_defs.md#disassociatememberfromfleetrequestrequesttypedef) 

### disassociate\_member\_from\_job

Disassociates a member from a job.

Type annotations and code completion for `#!python session.create_client("deadline").disassociate_member_from_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/disassociate_member_from_job.html)

```python
# disassociate_member_from_job method definition

await def disassociate_member_from_job(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    principalId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_member_from_job method usage example with argument unpacking

kwargs: DisassociateMemberFromJobRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "principalId": ...,
}

parent.disassociate_member_from_job(**kwargs)
```

1. See [:material-code-braces: DisassociateMemberFromJobRequestRequestTypeDef](./type_defs.md#disassociatememberfromjobrequestrequesttypedef) 

### disassociate\_member\_from\_queue

Disassociates a member from a queue.

Type annotations and code completion for `#!python session.create_client("deadline").disassociate_member_from_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/disassociate_member_from_queue.html)

```python
# disassociate_member_from_queue method definition

await def disassociate_member_from_queue(
    self,
    *,
    farmId: str,
    queueId: str,
    principalId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_member_from_queue method usage example with argument unpacking

kwargs: DisassociateMemberFromQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "principalId": ...,
}

parent.disassociate_member_from_queue(**kwargs)
```

1. See [:material-code-braces: DisassociateMemberFromQueueRequestRequestTypeDef](./type_defs.md#disassociatememberfromqueuerequestrequesttypedef) 

### get\_budget

Get a budget.

Type annotations and code completion for `#!python session.create_client("deadline").get_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_budget.html)

```python
# get_budget method definition

await def get_budget(
    self,
    *,
    farmId: str,
    budgetId: str,
) -> GetBudgetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBudgetResponseTypeDef](./type_defs.md#getbudgetresponsetypedef) 


```python
# get_budget method usage example with argument unpacking

kwargs: GetBudgetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "budgetId": ...,
}

parent.get_budget(**kwargs)
```

1. See [:material-code-braces: GetBudgetRequestRequestTypeDef](./type_defs.md#getbudgetrequestrequesttypedef) 

### get\_farm

Get a farm.

Type annotations and code completion for `#!python session.create_client("deadline").get_farm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_farm.html)

```python
# get_farm method definition

await def get_farm(
    self,
    *,
    farmId: str,
) -> GetFarmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFarmResponseTypeDef](./type_defs.md#getfarmresponsetypedef) 


```python
# get_farm method usage example with argument unpacking

kwargs: GetFarmRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.get_farm(**kwargs)
```

1. See [:material-code-braces: GetFarmRequestRequestTypeDef](./type_defs.md#getfarmrequestrequesttypedef) 

### get\_fleet

Get a fleet.

Type annotations and code completion for `#!python session.create_client("deadline").get_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_fleet.html)

```python
# get_fleet method definition

await def get_fleet(
    self,
    *,
    farmId: str,
    fleetId: str,
) -> GetFleetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFleetResponseTypeDef](./type_defs.md#getfleetresponsetypedef) 


```python
# get_fleet method usage example with argument unpacking

kwargs: GetFleetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.get_fleet(**kwargs)
```

1. See [:material-code-braces: GetFleetRequestRequestTypeDef](./type_defs.md#getfleetrequestrequesttypedef) 

### get\_job

Gets a Deadline Cloud job.

Type annotations and code completion for `#!python session.create_client("deadline").get_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_job.html)

```python
# get_job method definition

await def get_job(
    self,
    *,
    farmId: str,
    jobId: str,
    queueId: str,
) -> GetJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef) 


```python
# get_job method usage example with argument unpacking

kwargs: GetJobRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "jobId": ...,
    "queueId": ...,
}

parent.get_job(**kwargs)
```

1. See [:material-code-braces: GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef) 

### get\_license\_endpoint

Gets a licence endpoint.

Type annotations and code completion for `#!python session.create_client("deadline").get_license_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_license_endpoint.html)

```python
# get_license_endpoint method definition

await def get_license_endpoint(
    self,
    *,
    licenseEndpointId: str,
) -> GetLicenseEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLicenseEndpointResponseTypeDef](./type_defs.md#getlicenseendpointresponsetypedef) 


```python
# get_license_endpoint method usage example with argument unpacking

kwargs: GetLicenseEndpointRequestRequestTypeDef = {  # (1)
    "licenseEndpointId": ...,
}

parent.get_license_endpoint(**kwargs)
```

1. See [:material-code-braces: GetLicenseEndpointRequestRequestTypeDef](./type_defs.md#getlicenseendpointrequestrequesttypedef) 

### get\_monitor

Gets information about the specified monitor.

Type annotations and code completion for `#!python session.create_client("deadline").get_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_monitor.html)

```python
# get_monitor method definition

await def get_monitor(
    self,
    *,
    monitorId: str,
) -> GetMonitorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMonitorResponseTypeDef](./type_defs.md#getmonitorresponsetypedef) 


```python
# get_monitor method usage example with argument unpacking

kwargs: GetMonitorRequestRequestTypeDef = {  # (1)
    "monitorId": ...,
}

parent.get_monitor(**kwargs)
```

1. See [:material-code-braces: GetMonitorRequestRequestTypeDef](./type_defs.md#getmonitorrequestrequesttypedef) 

### get\_queue

Gets a queue.

Type annotations and code completion for `#!python session.create_client("deadline").get_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_queue.html)

```python
# get_queue method definition

await def get_queue(
    self,
    *,
    farmId: str,
    queueId: str,
) -> GetQueueResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueueResponseTypeDef](./type_defs.md#getqueueresponsetypedef) 


```python
# get_queue method usage example with argument unpacking

kwargs: GetQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.get_queue(**kwargs)
```

1. See [:material-code-braces: GetQueueRequestRequestTypeDef](./type_defs.md#getqueuerequestrequesttypedef) 

### get\_queue\_environment

Gets a queue environment.

Type annotations and code completion for `#!python session.create_client("deadline").get_queue_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_queue_environment.html)

```python
# get_queue_environment method definition

await def get_queue_environment(
    self,
    *,
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
) -> GetQueueEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueueEnvironmentResponseTypeDef](./type_defs.md#getqueueenvironmentresponsetypedef) 


```python
# get_queue_environment method usage example with argument unpacking

kwargs: GetQueueEnvironmentRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "queueEnvironmentId": ...,
}

parent.get_queue_environment(**kwargs)
```

1. See [:material-code-braces: GetQueueEnvironmentRequestRequestTypeDef](./type_defs.md#getqueueenvironmentrequestrequesttypedef) 

### get\_queue\_fleet\_association

Gets a queue-fleet association.

Type annotations and code completion for `#!python session.create_client("deadline").get_queue_fleet_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_queue_fleet_association.html)

```python
# get_queue_fleet_association method definition

await def get_queue_fleet_association(
    self,
    *,
    farmId: str,
    queueId: str,
    fleetId: str,
) -> GetQueueFleetAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueueFleetAssociationResponseTypeDef](./type_defs.md#getqueuefleetassociationresponsetypedef) 


```python
# get_queue_fleet_association method usage example with argument unpacking

kwargs: GetQueueFleetAssociationRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "fleetId": ...,
}

parent.get_queue_fleet_association(**kwargs)
```

1. See [:material-code-braces: GetQueueFleetAssociationRequestRequestTypeDef](./type_defs.md#getqueuefleetassociationrequestrequesttypedef) 

### get\_session

Gets a session.

Type annotations and code completion for `#!python session.create_client("deadline").get_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_session.html)

```python
# get_session method definition

await def get_session(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: str,
) -> GetSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef) 


```python
# get_session method usage example with argument unpacking

kwargs: GetSessionRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "sessionId": ...,
}

parent.get_session(**kwargs)
```

1. See [:material-code-braces: GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef) 

### get\_session\_action

Gets a session action for the job.

Type annotations and code completion for `#!python session.create_client("deadline").get_session_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_session_action.html)

```python
# get_session_action method definition

await def get_session_action(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    sessionActionId: str,
) -> GetSessionActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionActionResponseTypeDef](./type_defs.md#getsessionactionresponsetypedef) 


```python
# get_session_action method usage example with argument unpacking

kwargs: GetSessionActionRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "sessionActionId": ...,
}

parent.get_session_action(**kwargs)
```

1. See [:material-code-braces: GetSessionActionRequestRequestTypeDef](./type_defs.md#getsessionactionrequestrequesttypedef) 

### get\_sessions\_statistics\_aggregation

Gets a set of statistics for queues or farms.

Type annotations and code completion for `#!python session.create_client("deadline").get_sessions_statistics_aggregation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_sessions_statistics_aggregation.html)

```python
# get_sessions_statistics_aggregation method definition

await def get_sessions_statistics_aggregation(
    self,
    *,
    farmId: str,
    aggregationId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetSessionsStatisticsAggregationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionsStatisticsAggregationResponseTypeDef](./type_defs.md#getsessionsstatisticsaggregationresponsetypedef) 


```python
# get_sessions_statistics_aggregation method usage example with argument unpacking

kwargs: GetSessionsStatisticsAggregationRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "aggregationId": ...,
}

parent.get_sessions_statistics_aggregation(**kwargs)
```

1. See [:material-code-braces: GetSessionsStatisticsAggregationRequestRequestTypeDef](./type_defs.md#getsessionsstatisticsaggregationrequestrequesttypedef) 

### get\_step

Gets a step.

Type annotations and code completion for `#!python session.create_client("deadline").get_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_step.html)

```python
# get_step method definition

await def get_step(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
) -> GetStepResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStepResponseTypeDef](./type_defs.md#getstepresponsetypedef) 


```python
# get_step method usage example with argument unpacking

kwargs: GetStepRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "stepId": ...,
}

parent.get_step(**kwargs)
```

1. See [:material-code-braces: GetStepRequestRequestTypeDef](./type_defs.md#getsteprequestrequesttypedef) 

### get\_storage\_profile

Gets a storage profile.

Type annotations and code completion for `#!python session.create_client("deadline").get_storage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_storage_profile.html)

```python
# get_storage_profile method definition

await def get_storage_profile(
    self,
    *,
    farmId: str,
    storageProfileId: str,
) -> GetStorageProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStorageProfileResponseTypeDef](./type_defs.md#getstorageprofileresponsetypedef) 


```python
# get_storage_profile method usage example with argument unpacking

kwargs: GetStorageProfileRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "storageProfileId": ...,
}

parent.get_storage_profile(**kwargs)
```

1. See [:material-code-braces: GetStorageProfileRequestRequestTypeDef](./type_defs.md#getstorageprofilerequestrequesttypedef) 

### get\_storage\_profile\_for\_queue

Gets a storage profile for a queue.

Type annotations and code completion for `#!python session.create_client("deadline").get_storage_profile_for_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_storage_profile_for_queue.html)

```python
# get_storage_profile_for_queue method definition

await def get_storage_profile_for_queue(
    self,
    *,
    farmId: str,
    queueId: str,
    storageProfileId: str,
) -> GetStorageProfileForQueueResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStorageProfileForQueueResponseTypeDef](./type_defs.md#getstorageprofileforqueueresponsetypedef) 


```python
# get_storage_profile_for_queue method usage example with argument unpacking

kwargs: GetStorageProfileForQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "storageProfileId": ...,
}

parent.get_storage_profile_for_queue(**kwargs)
```

1. See [:material-code-braces: GetStorageProfileForQueueRequestRequestTypeDef](./type_defs.md#getstorageprofileforqueuerequestrequesttypedef) 

### get\_task

Gets a task.

Type annotations and code completion for `#!python session.create_client("deadline").get_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_task.html)

```python
# get_task method definition

await def get_task(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    taskId: str,
) -> GetTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTaskResponseTypeDef](./type_defs.md#gettaskresponsetypedef) 


```python
# get_task method usage example with argument unpacking

kwargs: GetTaskRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "stepId": ...,
    "taskId": ...,
}

parent.get_task(**kwargs)
```

1. See [:material-code-braces: GetTaskRequestRequestTypeDef](./type_defs.md#gettaskrequestrequesttypedef) 

### get\_worker

Gets a worker.

Type annotations and code completion for `#!python session.create_client("deadline").get_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/get_worker.html)

```python
# get_worker method definition

await def get_worker(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
) -> GetWorkerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkerResponseTypeDef](./type_defs.md#getworkerresponsetypedef) 


```python
# get_worker method usage example with argument unpacking

kwargs: GetWorkerRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
}

parent.get_worker(**kwargs)
```

1. See [:material-code-braces: GetWorkerRequestRequestTypeDef](./type_defs.md#getworkerrequestrequesttypedef) 

### list\_available\_metered\_products

A list of the available metered products.

Type annotations and code completion for `#!python session.create_client("deadline").list_available_metered_products` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_available_metered_products.html)

```python
# list_available_metered_products method definition

await def list_available_metered_products(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAvailableMeteredProductsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAvailableMeteredProductsResponseTypeDef](./type_defs.md#listavailablemeteredproductsresponsetypedef) 


```python
# list_available_metered_products method usage example with argument unpacking

kwargs: ListAvailableMeteredProductsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_available_metered_products(**kwargs)
```

1. See [:material-code-braces: ListAvailableMeteredProductsRequestRequestTypeDef](./type_defs.md#listavailablemeteredproductsrequestrequesttypedef) 

### list\_budgets

A list of budgets in a farm.

Type annotations and code completion for `#!python session.create_client("deadline").list_budgets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_budgets.html)

```python
# list_budgets method definition

await def list_budgets(
    self,
    *,
    farmId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    status: BudgetStatusType = ...,  # (1)
) -> ListBudgetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
2. See [:material-code-braces: ListBudgetsResponseTypeDef](./type_defs.md#listbudgetsresponsetypedef) 


```python
# list_budgets method usage example with argument unpacking

kwargs: ListBudgetsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.list_budgets(**kwargs)
```

1. See [:material-code-braces: ListBudgetsRequestRequestTypeDef](./type_defs.md#listbudgetsrequestrequesttypedef) 

### list\_farm\_members

Lists the members of a farm.

Type annotations and code completion for `#!python session.create_client("deadline").list_farm_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_farm_members.html)

```python
# list_farm_members method definition

await def list_farm_members(
    self,
    *,
    farmId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFarmMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFarmMembersResponseTypeDef](./type_defs.md#listfarmmembersresponsetypedef) 


```python
# list_farm_members method usage example with argument unpacking

kwargs: ListFarmMembersRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.list_farm_members(**kwargs)
```

1. See [:material-code-braces: ListFarmMembersRequestRequestTypeDef](./type_defs.md#listfarmmembersrequestrequesttypedef) 

### list\_farms

Lists farms.

Type annotations and code completion for `#!python session.create_client("deadline").list_farms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_farms.html)

```python
# list_farms method definition

await def list_farms(
    self,
    *,
    nextToken: str = ...,
    principalId: str = ...,
    maxResults: int = ...,
) -> ListFarmsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFarmsResponseTypeDef](./type_defs.md#listfarmsresponsetypedef) 


```python
# list_farms method usage example with argument unpacking

kwargs: ListFarmsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_farms(**kwargs)
```

1. See [:material-code-braces: ListFarmsRequestRequestTypeDef](./type_defs.md#listfarmsrequestrequesttypedef) 

### list\_fleet\_members

Lists fleet members.

Type annotations and code completion for `#!python session.create_client("deadline").list_fleet_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_fleet_members.html)

```python
# list_fleet_members method definition

await def list_fleet_members(
    self,
    *,
    farmId: str,
    fleetId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFleetMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFleetMembersResponseTypeDef](./type_defs.md#listfleetmembersresponsetypedef) 


```python
# list_fleet_members method usage example with argument unpacking

kwargs: ListFleetMembersRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.list_fleet_members(**kwargs)
```

1. See [:material-code-braces: ListFleetMembersRequestRequestTypeDef](./type_defs.md#listfleetmembersrequestrequesttypedef) 

### list\_fleets

Lists fleets.

Type annotations and code completion for `#!python session.create_client("deadline").list_fleets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_fleets.html)

```python
# list_fleets method definition

await def list_fleets(
    self,
    *,
    farmId: str,
    principalId: str = ...,
    displayName: str = ...,
    status: FleetStatusType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFleetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
2. See [:material-code-braces: ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef) 


```python
# list_fleets method usage example with argument unpacking

kwargs: ListFleetsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.list_fleets(**kwargs)
```

1. See [:material-code-braces: ListFleetsRequestRequestTypeDef](./type_defs.md#listfleetsrequestrequesttypedef) 

### list\_job\_members

Lists members on a job.

Type annotations and code completion for `#!python session.create_client("deadline").list_job_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_job_members.html)

```python
# list_job_members method definition

await def list_job_members(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListJobMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobMembersResponseTypeDef](./type_defs.md#listjobmembersresponsetypedef) 


```python
# list_job_members method usage example with argument unpacking

kwargs: ListJobMembersRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
}

parent.list_job_members(**kwargs)
```

1. See [:material-code-braces: ListJobMembersRequestRequestTypeDef](./type_defs.md#listjobmembersrequestrequesttypedef) 

### list\_job\_parameter\_definitions

Lists parameter definitions of a job.

Type annotations and code completion for `#!python session.create_client("deadline").list_job_parameter_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_job_parameter_definitions.html)

```python
# list_job_parameter_definitions method definition

await def list_job_parameter_definitions(
    self,
    *,
    farmId: str,
    jobId: str,
    queueId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListJobParameterDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobParameterDefinitionsResponseTypeDef](./type_defs.md#listjobparameterdefinitionsresponsetypedef) 


```python
# list_job_parameter_definitions method usage example with argument unpacking

kwargs: ListJobParameterDefinitionsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "jobId": ...,
    "queueId": ...,
}

parent.list_job_parameter_definitions(**kwargs)
```

1. See [:material-code-braces: ListJobParameterDefinitionsRequestRequestTypeDef](./type_defs.md#listjobparameterdefinitionsrequestrequesttypedef) 

### list\_jobs

Lists jobs.

Type annotations and code completion for `#!python session.create_client("deadline").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_jobs.html)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    farmId: str,
    queueId: str,
    principalId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef) 

### list\_license\_endpoints

Lists license endpoints.

Type annotations and code completion for `#!python session.create_client("deadline").list_license_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_license_endpoints.html)

```python
# list_license_endpoints method definition

await def list_license_endpoints(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListLicenseEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLicenseEndpointsResponseTypeDef](./type_defs.md#listlicenseendpointsresponsetypedef) 


```python
# list_license_endpoints method usage example with argument unpacking

kwargs: ListLicenseEndpointsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_license_endpoints(**kwargs)
```

1. See [:material-code-braces: ListLicenseEndpointsRequestRequestTypeDef](./type_defs.md#listlicenseendpointsrequestrequesttypedef) 

### list\_metered\_products

Lists metered products.

Type annotations and code completion for `#!python session.create_client("deadline").list_metered_products` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_metered_products.html)

```python
# list_metered_products method definition

await def list_metered_products(
    self,
    *,
    licenseEndpointId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMeteredProductsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMeteredProductsResponseTypeDef](./type_defs.md#listmeteredproductsresponsetypedef) 


```python
# list_metered_products method usage example with argument unpacking

kwargs: ListMeteredProductsRequestRequestTypeDef = {  # (1)
    "licenseEndpointId": ...,
}

parent.list_metered_products(**kwargs)
```

1. See [:material-code-braces: ListMeteredProductsRequestRequestTypeDef](./type_defs.md#listmeteredproductsrequestrequesttypedef) 

### list\_monitors

Gets a list of your monitors in Deadline Cloud.

Type annotations and code completion for `#!python session.create_client("deadline").list_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_monitors.html)

```python
# list_monitors method definition

await def list_monitors(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMonitorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMonitorsResponseTypeDef](./type_defs.md#listmonitorsresponsetypedef) 


```python
# list_monitors method usage example with argument unpacking

kwargs: ListMonitorsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_monitors(**kwargs)
```

1. See [:material-code-braces: ListMonitorsRequestRequestTypeDef](./type_defs.md#listmonitorsrequestrequesttypedef) 

### list\_queue\_environments

Lists queue environments.

Type annotations and code completion for `#!python session.create_client("deadline").list_queue_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_queue_environments.html)

```python
# list_queue_environments method definition

await def list_queue_environments(
    self,
    *,
    farmId: str,
    queueId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListQueueEnvironmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQueueEnvironmentsResponseTypeDef](./type_defs.md#listqueueenvironmentsresponsetypedef) 


```python
# list_queue_environments method usage example with argument unpacking

kwargs: ListQueueEnvironmentsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.list_queue_environments(**kwargs)
```

1. See [:material-code-braces: ListQueueEnvironmentsRequestRequestTypeDef](./type_defs.md#listqueueenvironmentsrequestrequesttypedef) 

### list\_queue\_fleet\_associations

Lists queue-fleet associations.

Type annotations and code completion for `#!python session.create_client("deadline").list_queue_fleet_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_queue_fleet_associations.html)

```python
# list_queue_fleet_associations method definition

await def list_queue_fleet_associations(
    self,
    *,
    farmId: str,
    queueId: str = ...,
    fleetId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListQueueFleetAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQueueFleetAssociationsResponseTypeDef](./type_defs.md#listqueuefleetassociationsresponsetypedef) 


```python
# list_queue_fleet_associations method usage example with argument unpacking

kwargs: ListQueueFleetAssociationsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.list_queue_fleet_associations(**kwargs)
```

1. See [:material-code-braces: ListQueueFleetAssociationsRequestRequestTypeDef](./type_defs.md#listqueuefleetassociationsrequestrequesttypedef) 

### list\_queue\_members

Lists the members in a queue.

Type annotations and code completion for `#!python session.create_client("deadline").list_queue_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_queue_members.html)

```python
# list_queue_members method definition

await def list_queue_members(
    self,
    *,
    farmId: str,
    queueId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListQueueMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQueueMembersResponseTypeDef](./type_defs.md#listqueuemembersresponsetypedef) 


```python
# list_queue_members method usage example with argument unpacking

kwargs: ListQueueMembersRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.list_queue_members(**kwargs)
```

1. See [:material-code-braces: ListQueueMembersRequestRequestTypeDef](./type_defs.md#listqueuemembersrequestrequesttypedef) 

### list\_queues

Lists queues.

Type annotations and code completion for `#!python session.create_client("deadline").list_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_queues.html)

```python
# list_queues method definition

await def list_queues(
    self,
    *,
    farmId: str,
    principalId: str = ...,
    status: QueueStatusType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListQueuesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
2. See [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


```python
# list_queues method usage example with argument unpacking

kwargs: ListQueuesRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.list_queues(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef) 

### list\_session\_actions

Lists session actions.

Type annotations and code completion for `#!python session.create_client("deadline").list_session_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_session_actions.html)

```python
# list_session_actions method definition

await def list_session_actions(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: str = ...,
    taskId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSessionActionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSessionActionsResponseTypeDef](./type_defs.md#listsessionactionsresponsetypedef) 


```python
# list_session_actions method usage example with argument unpacking

kwargs: ListSessionActionsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
}

parent.list_session_actions(**kwargs)
```

1. See [:material-code-braces: ListSessionActionsRequestRequestTypeDef](./type_defs.md#listsessionactionsrequestrequesttypedef) 

### list\_sessions

Lists sessions.

Type annotations and code completion for `#!python session.create_client("deadline").list_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_sessions.html)

```python
# list_sessions method definition

await def list_sessions(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSessionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 


```python
# list_sessions method usage example with argument unpacking

kwargs: ListSessionsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
}

parent.list_sessions(**kwargs)
```

1. See [:material-code-braces: ListSessionsRequestRequestTypeDef](./type_defs.md#listsessionsrequestrequesttypedef) 

### list\_sessions\_for\_worker

Lists sessions for a worker.

Type annotations and code completion for `#!python session.create_client("deadline").list_sessions_for_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_sessions_for_worker.html)

```python
# list_sessions_for_worker method definition

await def list_sessions_for_worker(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSessionsForWorkerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSessionsForWorkerResponseTypeDef](./type_defs.md#listsessionsforworkerresponsetypedef) 


```python
# list_sessions_for_worker method usage example with argument unpacking

kwargs: ListSessionsForWorkerRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
}

parent.list_sessions_for_worker(**kwargs)
```

1. See [:material-code-braces: ListSessionsForWorkerRequestRequestTypeDef](./type_defs.md#listsessionsforworkerrequestrequesttypedef) 

### list\_step\_consumers

Lists step consumers.

Type annotations and code completion for `#!python session.create_client("deadline").list_step_consumers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_step_consumers.html)

```python
# list_step_consumers method definition

await def list_step_consumers(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStepConsumersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStepConsumersResponseTypeDef](./type_defs.md#liststepconsumersresponsetypedef) 


```python
# list_step_consumers method usage example with argument unpacking

kwargs: ListStepConsumersRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "stepId": ...,
}

parent.list_step_consumers(**kwargs)
```

1. See [:material-code-braces: ListStepConsumersRequestRequestTypeDef](./type_defs.md#liststepconsumersrequestrequesttypedef) 

### list\_step\_dependencies

Lists the dependencies for a step.

Type annotations and code completion for `#!python session.create_client("deadline").list_step_dependencies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_step_dependencies.html)

```python
# list_step_dependencies method definition

await def list_step_dependencies(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStepDependenciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStepDependenciesResponseTypeDef](./type_defs.md#liststepdependenciesresponsetypedef) 


```python
# list_step_dependencies method usage example with argument unpacking

kwargs: ListStepDependenciesRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "stepId": ...,
}

parent.list_step_dependencies(**kwargs)
```

1. See [:material-code-braces: ListStepDependenciesRequestRequestTypeDef](./type_defs.md#liststepdependenciesrequestrequesttypedef) 

### list\_steps

Lists steps for a job.

Type annotations and code completion for `#!python session.create_client("deadline").list_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_steps.html)

```python
# list_steps method definition

await def list_steps(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStepsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStepsResponseTypeDef](./type_defs.md#liststepsresponsetypedef) 


```python
# list_steps method usage example with argument unpacking

kwargs: ListStepsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
}

parent.list_steps(**kwargs)
```

1. See [:material-code-braces: ListStepsRequestRequestTypeDef](./type_defs.md#liststepsrequestrequesttypedef) 

### list\_storage\_profiles

Lists storage profiles.

Type annotations and code completion for `#!python session.create_client("deadline").list_storage_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_storage_profiles.html)

```python
# list_storage_profiles method definition

await def list_storage_profiles(
    self,
    *,
    farmId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStorageProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStorageProfilesResponseTypeDef](./type_defs.md#liststorageprofilesresponsetypedef) 


```python
# list_storage_profiles method usage example with argument unpacking

kwargs: ListStorageProfilesRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.list_storage_profiles(**kwargs)
```

1. See [:material-code-braces: ListStorageProfilesRequestRequestTypeDef](./type_defs.md#liststorageprofilesrequestrequesttypedef) 

### list\_storage\_profiles\_for\_queue

Lists storage profiles for a queue.

Type annotations and code completion for `#!python session.create_client("deadline").list_storage_profiles_for_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_storage_profiles_for_queue.html)

```python
# list_storage_profiles_for_queue method definition

await def list_storage_profiles_for_queue(
    self,
    *,
    farmId: str,
    queueId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStorageProfilesForQueueResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStorageProfilesForQueueResponseTypeDef](./type_defs.md#liststorageprofilesforqueueresponsetypedef) 


```python
# list_storage_profiles_for_queue method usage example with argument unpacking

kwargs: ListStorageProfilesForQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.list_storage_profiles_for_queue(**kwargs)
```

1. See [:material-code-braces: ListStorageProfilesForQueueRequestRequestTypeDef](./type_defs.md#liststorageprofilesforqueuerequestrequesttypedef) 

### list\_tags\_for\_resource

Lists tags for a resource.

Type annotations and code completion for `#!python session.create_client("deadline").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_tags_for_resource.html)

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

### list\_tasks

Lists tasks for a job.

Type annotations and code completion for `#!python session.create_client("deadline").list_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_tasks.html)

```python
# list_tasks method definition

await def list_tasks(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTasksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef) 


```python
# list_tasks method usage example with argument unpacking

kwargs: ListTasksRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "stepId": ...,
}

parent.list_tasks(**kwargs)
```

1. See [:material-code-braces: ListTasksRequestRequestTypeDef](./type_defs.md#listtasksrequestrequesttypedef) 

### list\_workers

Lists workers.

Type annotations and code completion for `#!python session.create_client("deadline").list_workers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/list_workers.html)

```python
# list_workers method definition

await def list_workers(
    self,
    *,
    farmId: str,
    fleetId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListWorkersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkersResponseTypeDef](./type_defs.md#listworkersresponsetypedef) 


```python
# list_workers method usage example with argument unpacking

kwargs: ListWorkersRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.list_workers(**kwargs)
```

1. See [:material-code-braces: ListWorkersRequestRequestTypeDef](./type_defs.md#listworkersrequestrequesttypedef) 

### put\_metered\_product

Adds a metered product.

Type annotations and code completion for `#!python session.create_client("deadline").put_metered_product` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/put_metered_product.html)

```python
# put_metered_product method definition

await def put_metered_product(
    self,
    *,
    licenseEndpointId: str,
    productId: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_metered_product method usage example with argument unpacking

kwargs: PutMeteredProductRequestRequestTypeDef = {  # (1)
    "licenseEndpointId": ...,
    "productId": ...,
}

parent.put_metered_product(**kwargs)
```

1. See [:material-code-braces: PutMeteredProductRequestRequestTypeDef](./type_defs.md#putmeteredproductrequestrequesttypedef) 

### search\_jobs

Searches for jobs.

Type annotations and code completion for `#!python session.create_client("deadline").search_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/search_jobs.html)

```python
# search_jobs method definition

await def search_jobs(
    self,
    *,
    farmId: str,
    queueIds: Sequence[str],
    itemOffset: int,
    filterExpressions: SearchGroupedFilterExpressionsTypeDef = ...,  # (1)
    sortExpressions: Sequence[SearchSortExpressionTypeDef] = ...,  # (2)
    pageSize: int = ...,
) -> SearchJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
3. See [:material-code-braces: SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef) 


```python
# search_jobs method usage example with argument unpacking

kwargs: SearchJobsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueIds": ...,
    "itemOffset": ...,
}

parent.search_jobs(**kwargs)
```

1. See [:material-code-braces: SearchJobsRequestRequestTypeDef](./type_defs.md#searchjobsrequestrequesttypedef) 

### search\_steps

Searches for steps.

Type annotations and code completion for `#!python session.create_client("deadline").search_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/search_steps.html)

```python
# search_steps method definition

await def search_steps(
    self,
    *,
    farmId: str,
    queueIds: Sequence[str],
    itemOffset: int,
    jobId: str = ...,
    filterExpressions: SearchGroupedFilterExpressionsTypeDef = ...,  # (1)
    sortExpressions: Sequence[SearchSortExpressionTypeDef] = ...,  # (2)
    pageSize: int = ...,
) -> SearchStepsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
3. See [:material-code-braces: SearchStepsResponseTypeDef](./type_defs.md#searchstepsresponsetypedef) 


```python
# search_steps method usage example with argument unpacking

kwargs: SearchStepsRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueIds": ...,
    "itemOffset": ...,
}

parent.search_steps(**kwargs)
```

1. See [:material-code-braces: SearchStepsRequestRequestTypeDef](./type_defs.md#searchstepsrequestrequesttypedef) 

### search\_tasks

Searches for tasks.

Type annotations and code completion for `#!python session.create_client("deadline").search_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/search_tasks.html)

```python
# search_tasks method definition

await def search_tasks(
    self,
    *,
    farmId: str,
    queueIds: Sequence[str],
    itemOffset: int,
    jobId: str = ...,
    filterExpressions: SearchGroupedFilterExpressionsTypeDef = ...,  # (1)
    sortExpressions: Sequence[SearchSortExpressionTypeDef] = ...,  # (2)
    pageSize: int = ...,
) -> SearchTasksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
3. See [:material-code-braces: SearchTasksResponseTypeDef](./type_defs.md#searchtasksresponsetypedef) 


```python
# search_tasks method usage example with argument unpacking

kwargs: SearchTasksRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueIds": ...,
    "itemOffset": ...,
}

parent.search_tasks(**kwargs)
```

1. See [:material-code-braces: SearchTasksRequestRequestTypeDef](./type_defs.md#searchtasksrequestrequesttypedef) 

### search\_workers

Searches for workers.

Type annotations and code completion for `#!python session.create_client("deadline").search_workers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/search_workers.html)

```python
# search_workers method definition

await def search_workers(
    self,
    *,
    farmId: str,
    fleetIds: Sequence[str],
    itemOffset: int,
    filterExpressions: SearchGroupedFilterExpressionsTypeDef = ...,  # (1)
    sortExpressions: Sequence[SearchSortExpressionTypeDef] = ...,  # (2)
    pageSize: int = ...,
) -> SearchWorkersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
3. See [:material-code-braces: SearchWorkersResponseTypeDef](./type_defs.md#searchworkersresponsetypedef) 


```python
# search_workers method usage example with argument unpacking

kwargs: SearchWorkersRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetIds": ...,
    "itemOffset": ...,
}

parent.search_workers(**kwargs)
```

1. See [:material-code-braces: SearchWorkersRequestRequestTypeDef](./type_defs.md#searchworkersrequestrequesttypedef) 

### start\_sessions\_statistics\_aggregation

Starts an asynchronous request for getting aggregated statistics about queues
and farms.

Type annotations and code completion for `#!python session.create_client("deadline").start_sessions_statistics_aggregation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/start_sessions_statistics_aggregation.html)

```python
# start_sessions_statistics_aggregation method definition

await def start_sessions_statistics_aggregation(
    self,
    *,
    farmId: str,
    resourceIds: SessionsStatisticsResourcesTypeDef,  # (1)
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    groupBy: Sequence[UsageGroupByFieldType],  # (2)
    statistics: Sequence[UsageStatisticType],  # (3)
    timezone: str = ...,
    period: PeriodType = ...,  # (4)
) -> StartSessionsStatisticsAggregationResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SessionsStatisticsResourcesTypeDef](./type_defs.md#sessionsstatisticsresourcestypedef) 
2. See [:material-code-brackets: UsageGroupByFieldType](./literals.md#usagegroupbyfieldtype) 
3. See [:material-code-brackets: UsageStatisticType](./literals.md#usagestatistictype) 
4. See [:material-code-brackets: PeriodType](./literals.md#periodtype) 
5. See [:material-code-braces: StartSessionsStatisticsAggregationResponseTypeDef](./type_defs.md#startsessionsstatisticsaggregationresponsetypedef) 


```python
# start_sessions_statistics_aggregation method usage example with argument unpacking

kwargs: StartSessionsStatisticsAggregationRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "resourceIds": ...,
    "startTime": ...,
    "endTime": ...,
    "groupBy": ...,
    "statistics": ...,
}

parent.start_sessions_statistics_aggregation(**kwargs)
```

1. See [:material-code-braces: StartSessionsStatisticsAggregationRequestRequestTypeDef](./type_defs.md#startsessionsstatisticsaggregationrequestrequesttypedef) 

### tag\_resource

Tags a resource using the resource's ARN and desired tags.

Type annotations and code completion for `#!python session.create_client("deadline").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag from a resource using the resource's ARN and tag to remove.

Type annotations and code completion for `#!python session.create_client("deadline").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/untag_resource.html)

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

### update\_budget

Updates a budget that sets spending thresholds for rendering activity.

Type annotations and code completion for `#!python session.create_client("deadline").update_budget` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_budget.html)

```python
# update_budget method definition

await def update_budget(
    self,
    *,
    farmId: str,
    budgetId: str,
    clientToken: str = ...,
    displayName: str = ...,
    description: str = ...,
    status: BudgetStatusType = ...,  # (1)
    approximateDollarLimit: float = ...,
    actionsToAdd: Sequence[BudgetActionToAddTypeDef] = ...,  # (2)
    actionsToRemove: Sequence[BudgetActionToRemoveTypeDef] = ...,  # (3)
    schedule: BudgetScheduleTypeDef = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
2. See [:material-code-braces: BudgetActionToAddTypeDef](./type_defs.md#budgetactiontoaddtypedef) 
3. See [:material-code-braces: BudgetActionToRemoveTypeDef](./type_defs.md#budgetactiontoremovetypedef) 
4. See [:material-code-braces: BudgetScheduleTypeDef](./type_defs.md#budgetscheduletypedef) 


```python
# update_budget method usage example with argument unpacking

kwargs: UpdateBudgetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "budgetId": ...,
}

parent.update_budget(**kwargs)
```

1. See [:material-code-braces: UpdateBudgetRequestRequestTypeDef](./type_defs.md#updatebudgetrequestrequesttypedef) 

### update\_farm

Updates a farm.

Type annotations and code completion for `#!python session.create_client("deadline").update_farm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_farm.html)

```python
# update_farm method definition

await def update_farm(
    self,
    *,
    farmId: str,
    displayName: str = ...,
    description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_farm method usage example with argument unpacking

kwargs: UpdateFarmRequestRequestTypeDef = {  # (1)
    "farmId": ...,
}

parent.update_farm(**kwargs)
```

1. See [:material-code-braces: UpdateFarmRequestRequestTypeDef](./type_defs.md#updatefarmrequestrequesttypedef) 

### update\_fleet

Updates a fleet.

Type annotations and code completion for `#!python session.create_client("deadline").update_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_fleet.html)

```python
# update_fleet method definition

await def update_fleet(
    self,
    *,
    farmId: str,
    fleetId: str,
    clientToken: str = ...,
    displayName: str = ...,
    description: str = ...,
    roleArn: str = ...,
    minWorkerCount: int = ...,
    maxWorkerCount: int = ...,
    configuration: FleetConfigurationTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: FleetConfigurationTypeDef](./type_defs.md#fleetconfigurationtypedef) 


```python
# update_fleet method usage example with argument unpacking

kwargs: UpdateFleetRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.update_fleet(**kwargs)
```

1. See [:material-code-braces: UpdateFleetRequestRequestTypeDef](./type_defs.md#updatefleetrequestrequesttypedef) 

### update\_job

Updates a job.

Type annotations and code completion for `#!python session.create_client("deadline").update_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_job.html)

```python
# update_job method definition

await def update_job(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    clientToken: str = ...,
    targetTaskRunStatus: JobTargetTaskRunStatusType = ...,  # (1)
    priority: int = ...,
    maxFailedTasksCount: int = ...,
    maxRetriesPerTask: int = ...,
    lifecycleStatus: UpdateJobLifecycleStatusType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
2. See [:material-code-brackets: UpdateJobLifecycleStatusType](./literals.md#updatejoblifecyclestatustype) 


```python
# update_job method usage example with argument unpacking

kwargs: UpdateJobRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
}

parent.update_job(**kwargs)
```

1. See [:material-code-braces: UpdateJobRequestRequestTypeDef](./type_defs.md#updatejobrequestrequesttypedef) 

### update\_monitor

Modifies the settings for a Deadline Cloud monitor.

Type annotations and code completion for `#!python session.create_client("deadline").update_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_monitor.html)

```python
# update_monitor method definition

await def update_monitor(
    self,
    *,
    monitorId: str,
    subdomain: str = ...,
    displayName: str = ...,
    roleArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_monitor method usage example with argument unpacking

kwargs: UpdateMonitorRequestRequestTypeDef = {  # (1)
    "monitorId": ...,
}

parent.update_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateMonitorRequestRequestTypeDef](./type_defs.md#updatemonitorrequestrequesttypedef) 

### update\_queue

Updates a queue.

Type annotations and code completion for `#!python session.create_client("deadline").update_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_queue.html)

```python
# update_queue method definition

await def update_queue(
    self,
    *,
    farmId: str,
    queueId: str,
    clientToken: str = ...,
    displayName: str = ...,
    description: str = ...,
    defaultBudgetAction: DefaultQueueBudgetActionType = ...,  # (1)
    jobAttachmentSettings: JobAttachmentSettingsTypeDef = ...,  # (2)
    roleArn: str = ...,
    jobRunAsUser: JobRunAsUserTypeDef = ...,  # (3)
    requiredFileSystemLocationNamesToAdd: Sequence[str] = ...,
    requiredFileSystemLocationNamesToRemove: Sequence[str] = ...,
    allowedStorageProfileIdsToAdd: Sequence[str] = ...,
    allowedStorageProfileIdsToRemove: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DefaultQueueBudgetActionType](./literals.md#defaultqueuebudgetactiontype) 
2. See [:material-code-braces: JobAttachmentSettingsTypeDef](./type_defs.md#jobattachmentsettingstypedef) 
3. See [:material-code-braces: JobRunAsUserTypeDef](./type_defs.md#jobrunasusertypedef) 


```python
# update_queue method usage example with argument unpacking

kwargs: UpdateQueueRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.update_queue(**kwargs)
```

1. See [:material-code-braces: UpdateQueueRequestRequestTypeDef](./type_defs.md#updatequeuerequestrequesttypedef) 

### update\_queue\_environment

Updates the queue environment.

Type annotations and code completion for `#!python session.create_client("deadline").update_queue_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_queue_environment.html)

```python
# update_queue_environment method definition

await def update_queue_environment(
    self,
    *,
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
    clientToken: str = ...,
    priority: int = ...,
    templateType: EnvironmentTemplateTypeType = ...,  # (1)
    template: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: EnvironmentTemplateTypeType](./literals.md#environmenttemplatetypetype) 


```python
# update_queue_environment method usage example with argument unpacking

kwargs: UpdateQueueEnvironmentRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "queueEnvironmentId": ...,
}

parent.update_queue_environment(**kwargs)
```

1. See [:material-code-braces: UpdateQueueEnvironmentRequestRequestTypeDef](./type_defs.md#updatequeueenvironmentrequestrequesttypedef) 

### update\_queue\_fleet\_association

Updates a queue-fleet association.

Type annotations and code completion for `#!python session.create_client("deadline").update_queue_fleet_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_queue_fleet_association.html)

```python
# update_queue_fleet_association method definition

await def update_queue_fleet_association(
    self,
    *,
    farmId: str,
    queueId: str,
    fleetId: str,
    status: UpdateQueueFleetAssociationStatusType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: UpdateQueueFleetAssociationStatusType](./literals.md#updatequeuefleetassociationstatustype) 


```python
# update_queue_fleet_association method usage example with argument unpacking

kwargs: UpdateQueueFleetAssociationRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "fleetId": ...,
    "status": ...,
}

parent.update_queue_fleet_association(**kwargs)
```

1. See [:material-code-braces: UpdateQueueFleetAssociationRequestRequestTypeDef](./type_defs.md#updatequeuefleetassociationrequestrequesttypedef) 

### update\_session

Updates a session.

Type annotations and code completion for `#!python session.create_client("deadline").update_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_session.html)

```python
# update_session method definition

await def update_session(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: str,
    targetLifecycleStatus: SessionLifecycleTargetStatusType,  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SessionLifecycleTargetStatusType](./literals.md#sessionlifecycletargetstatustype) 


```python
# update_session method usage example with argument unpacking

kwargs: UpdateSessionRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "sessionId": ...,
    "targetLifecycleStatus": ...,
}

parent.update_session(**kwargs)
```

1. See [:material-code-braces: UpdateSessionRequestRequestTypeDef](./type_defs.md#updatesessionrequestrequesttypedef) 

### update\_step

Updates a step.

Type annotations and code completion for `#!python session.create_client("deadline").update_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_step.html)

```python
# update_step method definition

await def update_step(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    targetTaskRunStatus: StepTargetTaskRunStatusType,  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: StepTargetTaskRunStatusType](./literals.md#steptargettaskrunstatustype) 


```python
# update_step method usage example with argument unpacking

kwargs: UpdateStepRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "stepId": ...,
    "targetTaskRunStatus": ...,
}

parent.update_step(**kwargs)
```

1. See [:material-code-braces: UpdateStepRequestRequestTypeDef](./type_defs.md#updatesteprequestrequesttypedef) 

### update\_storage\_profile

Updates a storage profile.

Type annotations and code completion for `#!python session.create_client("deadline").update_storage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_storage_profile.html)

```python
# update_storage_profile method definition

await def update_storage_profile(
    self,
    *,
    farmId: str,
    storageProfileId: str,
    clientToken: str = ...,
    displayName: str = ...,
    osFamily: StorageProfileOperatingSystemFamilyType = ...,  # (1)
    fileSystemLocationsToAdd: Sequence[FileSystemLocationTypeDef] = ...,  # (2)
    fileSystemLocationsToRemove: Sequence[FileSystemLocationTypeDef] = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
2. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 
3. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 


```python
# update_storage_profile method usage example with argument unpacking

kwargs: UpdateStorageProfileRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "storageProfileId": ...,
}

parent.update_storage_profile(**kwargs)
```

1. See [:material-code-braces: UpdateStorageProfileRequestRequestTypeDef](./type_defs.md#updatestorageprofilerequestrequesttypedef) 

### update\_task

Updates a task.

Type annotations and code completion for `#!python session.create_client("deadline").update_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_task.html)

```python
# update_task method definition

await def update_task(
    self,
    *,
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    taskId: str,
    targetRunStatus: TaskTargetRunStatusType,  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TaskTargetRunStatusType](./literals.md#tasktargetrunstatustype) 


```python
# update_task method usage example with argument unpacking

kwargs: UpdateTaskRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "jobId": ...,
    "stepId": ...,
    "taskId": ...,
    "targetRunStatus": ...,
}

parent.update_task(**kwargs)
```

1. See [:material-code-braces: UpdateTaskRequestRequestTypeDef](./type_defs.md#updatetaskrequestrequesttypedef) 

### update\_worker

Updates a worker.

Type annotations and code completion for `#!python session.create_client("deadline").update_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_worker.html)

```python
# update_worker method definition

await def update_worker(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
    status: UpdatedWorkerStatusType = ...,  # (1)
    capabilities: WorkerCapabilitiesTypeDef = ...,  # (2)
    hostProperties: HostPropertiesRequestTypeDef = ...,  # (3)
) -> UpdateWorkerResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: UpdatedWorkerStatusType](./literals.md#updatedworkerstatustype) 
2. See [:material-code-braces: WorkerCapabilitiesTypeDef](./type_defs.md#workercapabilitiestypedef) 
3. See [:material-code-braces: HostPropertiesRequestTypeDef](./type_defs.md#hostpropertiesrequesttypedef) 
4. See [:material-code-braces: UpdateWorkerResponseTypeDef](./type_defs.md#updateworkerresponsetypedef) 


```python
# update_worker method usage example with argument unpacking

kwargs: UpdateWorkerRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
}

parent.update_worker(**kwargs)
```

1. See [:material-code-braces: UpdateWorkerRequestRequestTypeDef](./type_defs.md#updateworkerrequestrequesttypedef) 

### update\_worker\_schedule

Updates the schedule for a worker.

Type annotations and code completion for `#!python session.create_client("deadline").update_worker_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/client/update_worker_schedule.html)

```python
# update_worker_schedule method definition

await def update_worker_schedule(
    self,
    *,
    farmId: str,
    fleetId: str,
    workerId: str,
    updatedSessionActions: Mapping[str, UpdatedSessionActionInfoTypeDef] = ...,  # (1)
) -> UpdateWorkerScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdatedSessionActionInfoTypeDef](./type_defs.md#updatedsessionactioninfotypedef) 
2. See [:material-code-braces: UpdateWorkerScheduleResponseTypeDef](./type_defs.md#updateworkerscheduleresponsetypedef) 


```python
# update_worker_schedule method usage example with argument unpacking

kwargs: UpdateWorkerScheduleRequestRequestTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
    "workerId": ...,
}

parent.update_worker_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateWorkerScheduleRequestRequestTypeDef](./type_defs.md#updateworkerschedulerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("deadline").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#DeadlineCloud.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "DeadlineCloudClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("deadline").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#DeadlineCloud.Client)

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

Type annotations and code completion for `#!python session.create_client("deadline").get_paginator` method with overloads.

- `client.get_paginator("get_sessions_statistics_aggregation")` -> [GetSessionsStatisticsAggregationPaginator](./paginators.md#getsessionsstatisticsaggregationpaginator)
- `client.get_paginator("list_available_metered_products")` -> [ListAvailableMeteredProductsPaginator](./paginators.md#listavailablemeteredproductspaginator)
- `client.get_paginator("list_budgets")` -> [ListBudgetsPaginator](./paginators.md#listbudgetspaginator)
- `client.get_paginator("list_farm_members")` -> [ListFarmMembersPaginator](./paginators.md#listfarmmemberspaginator)
- `client.get_paginator("list_farms")` -> [ListFarmsPaginator](./paginators.md#listfarmspaginator)
- `client.get_paginator("list_fleet_members")` -> [ListFleetMembersPaginator](./paginators.md#listfleetmemberspaginator)
- `client.get_paginator("list_fleets")` -> [ListFleetsPaginator](./paginators.md#listfleetspaginator)
- `client.get_paginator("list_job_members")` -> [ListJobMembersPaginator](./paginators.md#listjobmemberspaginator)
- `client.get_paginator("list_job_parameter_definitions")` -> [ListJobParameterDefinitionsPaginator](./paginators.md#listjobparameterdefinitionspaginator)
- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_license_endpoints")` -> [ListLicenseEndpointsPaginator](./paginators.md#listlicenseendpointspaginator)
- `client.get_paginator("list_metered_products")` -> [ListMeteredProductsPaginator](./paginators.md#listmeteredproductspaginator)
- `client.get_paginator("list_monitors")` -> [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
- `client.get_paginator("list_queue_environments")` -> [ListQueueEnvironmentsPaginator](./paginators.md#listqueueenvironmentspaginator)
- `client.get_paginator("list_queue_fleet_associations")` -> [ListQueueFleetAssociationsPaginator](./paginators.md#listqueuefleetassociationspaginator)
- `client.get_paginator("list_queue_members")` -> [ListQueueMembersPaginator](./paginators.md#listqueuememberspaginator)
- `client.get_paginator("list_queues")` -> [ListQueuesPaginator](./paginators.md#listqueuespaginator)
- `client.get_paginator("list_session_actions")` -> [ListSessionActionsPaginator](./paginators.md#listsessionactionspaginator)
- `client.get_paginator("list_sessions_for_worker")` -> [ListSessionsForWorkerPaginator](./paginators.md#listsessionsforworkerpaginator)
- `client.get_paginator("list_sessions")` -> [ListSessionsPaginator](./paginators.md#listsessionspaginator)
- `client.get_paginator("list_step_consumers")` -> [ListStepConsumersPaginator](./paginators.md#liststepconsumerspaginator)
- `client.get_paginator("list_step_dependencies")` -> [ListStepDependenciesPaginator](./paginators.md#liststepdependenciespaginator)
- `client.get_paginator("list_steps")` -> [ListStepsPaginator](./paginators.md#liststepspaginator)
- `client.get_paginator("list_storage_profiles_for_queue")` -> [ListStorageProfilesForQueuePaginator](./paginators.md#liststorageprofilesforqueuepaginator)
- `client.get_paginator("list_storage_profiles")` -> [ListStorageProfilesPaginator](./paginators.md#liststorageprofilespaginator)
- `client.get_paginator("list_tasks")` -> [ListTasksPaginator](./paginators.md#listtaskspaginator)
- `client.get_paginator("list_workers")` -> [ListWorkersPaginator](./paginators.md#listworkerspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter` method with overloads.

- `client.get_waiter("fleet_active")` -> [FleetActiveWaiter](./waiters.md#fleetactivewaiter)
- `client.get_waiter("job_create_complete")` -> [JobCreateCompleteWaiter](./waiters.md#jobcreatecompletewaiter)
- `client.get_waiter("license_endpoint_deleted")` -> [LicenseEndpointDeletedWaiter](./waiters.md#licenseendpointdeletedwaiter)
- `client.get_waiter("license_endpoint_valid")` -> [LicenseEndpointValidWaiter](./waiters.md#licenseendpointvalidwaiter)
- `client.get_waiter("queue_fleet_association_stopped")` -> [QueueFleetAssociationStoppedWaiter](./waiters.md#queuefleetassociationstoppedwaiter)
- `client.get_waiter("queue_scheduling_blocked")` -> [QueueSchedulingBlockedWaiter](./waiters.md#queueschedulingblockedwaiter)
- `client.get_waiter("queue_scheduling")` -> [QueueSchedulingWaiter](./waiters.md#queueschedulingwaiter)

