# WellArchitectedClient

> [Index](../README.md) > [WellArchitected](./README.md) > WellArchitectedClient

!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## WellArchitectedClient

Type annotations and code completion for `#!python session.create_client("wellarchitected")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client)

```python
# WellArchitectedClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_wellarchitected.client import WellArchitectedClient

session = get_session()
async with session.create_client("wellarchitected") as client:
    client: WellArchitectedClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("wellarchitected").exceptions` structure.

```python
# WellArchitectedClient.exceptions usage example

async with session.create_client("wellarchitected") as client:
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
# WellArchitectedClient usage type checking example

from types_aiobotocore_wellarchitected.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_lenses

Associate a lens to a workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").associate_lenses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_lenses)

```python
# associate_lenses method definition

await def associate_lenses(
    self,
    *,
    WorkloadId: str,
    LensAliases: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_lenses method usage example with argument unpacking

kwargs: AssociateLensesInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAliases": ...,
}

parent.associate_lenses(**kwargs)
```

1. See [:material-code-braces: AssociateLensesInputRequestTypeDef](./type_defs.md#associatelensesinputrequesttypedef) 

### associate\_profiles

Associate a profile with a workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").associate_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_profiles)

```python
# associate_profiles method definition

await def associate_profiles(
    self,
    *,
    WorkloadId: str,
    ProfileArns: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_profiles method usage example with argument unpacking

kwargs: AssociateProfilesInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "ProfileArns": ...,
}

parent.associate_profiles(**kwargs)
```

1. See [:material-code-braces: AssociateProfilesInputRequestTypeDef](./type_defs.md#associateprofilesinputrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("wellarchitected").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("wellarchitected").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_lens\_share

Create a lens share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_lens_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_lens_share)

```python
# create_lens_share method definition

await def create_lens_share(
    self,
    *,
    LensAlias: str,
    SharedWith: str,
    ClientRequestToken: str,
) -> CreateLensShareOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLensShareOutputTypeDef](./type_defs.md#createlensshareoutputtypedef) 


```python
# create_lens_share method usage example with argument unpacking

kwargs: CreateLensShareInputRequestTypeDef = {  # (1)
    "LensAlias": ...,
    "SharedWith": ...,
    "ClientRequestToken": ...,
}

parent.create_lens_share(**kwargs)
```

1. See [:material-code-braces: CreateLensShareInputRequestTypeDef](./type_defs.md#createlensshareinputrequesttypedef) 

### create\_lens\_version

Create a new lens version.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_lens_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_lens_version)

```python
# create_lens_version method definition

await def create_lens_version(
    self,
    *,
    LensAlias: str,
    LensVersion: str,
    ClientRequestToken: str,
    IsMajorVersion: bool = ...,
) -> CreateLensVersionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLensVersionOutputTypeDef](./type_defs.md#createlensversionoutputtypedef) 


```python
# create_lens_version method usage example with argument unpacking

kwargs: CreateLensVersionInputRequestTypeDef = {  # (1)
    "LensAlias": ...,
    "LensVersion": ...,
    "ClientRequestToken": ...,
}

parent.create_lens_version(**kwargs)
```

1. See [:material-code-braces: CreateLensVersionInputRequestTypeDef](./type_defs.md#createlensversioninputrequesttypedef) 

### create\_milestone

Create a milestone for an existing workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_milestone` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_milestone)

```python
# create_milestone method definition

await def create_milestone(
    self,
    *,
    WorkloadId: str,
    MilestoneName: str,
    ClientRequestToken: str,
) -> CreateMilestoneOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateMilestoneOutputTypeDef](./type_defs.md#createmilestoneoutputtypedef) 


```python
# create_milestone method usage example with argument unpacking

kwargs: CreateMilestoneInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "MilestoneName": ...,
    "ClientRequestToken": ...,
}

parent.create_milestone(**kwargs)
```

1. See [:material-code-braces: CreateMilestoneInputRequestTypeDef](./type_defs.md#createmilestoneinputrequesttypedef) 

### create\_profile

Create a profile.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)

```python
# create_profile method definition

await def create_profile(
    self,
    *,
    ProfileName: str,
    ProfileDescription: str,
    ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],  # (1)
    ClientRequestToken: str,
    Tags: Mapping[str, str] = ...,
) -> CreateProfileOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ProfileQuestionUpdateTypeDef](./type_defs.md#profilequestionupdatetypedef) 
2. See [:material-code-braces: CreateProfileOutputTypeDef](./type_defs.md#createprofileoutputtypedef) 


```python
# create_profile method usage example with argument unpacking

kwargs: CreateProfileInputRequestTypeDef = {  # (1)
    "ProfileName": ...,
    "ProfileDescription": ...,
    "ProfileQuestions": ...,
    "ClientRequestToken": ...,
}

parent.create_profile(**kwargs)
```

1. See [:material-code-braces: CreateProfileInputRequestTypeDef](./type_defs.md#createprofileinputrequesttypedef) 

### create\_profile\_share

Create a profile share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_profile_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile_share)

```python
# create_profile_share method definition

await def create_profile_share(
    self,
    *,
    ProfileArn: str,
    SharedWith: str,
    ClientRequestToken: str,
) -> CreateProfileShareOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateProfileShareOutputTypeDef](./type_defs.md#createprofileshareoutputtypedef) 


```python
# create_profile_share method usage example with argument unpacking

kwargs: CreateProfileShareInputRequestTypeDef = {  # (1)
    "ProfileArn": ...,
    "SharedWith": ...,
    "ClientRequestToken": ...,
}

parent.create_profile_share(**kwargs)
```

1. See [:material-code-braces: CreateProfileShareInputRequestTypeDef](./type_defs.md#createprofileshareinputrequesttypedef) 

### create\_review\_template

Create a review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_review_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_review_template)

```python
# create_review_template method definition

await def create_review_template(
    self,
    *,
    TemplateName: str,
    Description: str,
    Lenses: Sequence[str],
    ClientRequestToken: str,
    Notes: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateReviewTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateReviewTemplateOutputTypeDef](./type_defs.md#createreviewtemplateoutputtypedef) 


```python
# create_review_template method usage example with argument unpacking

kwargs: CreateReviewTemplateInputRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "Description": ...,
    "Lenses": ...,
    "ClientRequestToken": ...,
}

parent.create_review_template(**kwargs)
```

1. See [:material-code-braces: CreateReviewTemplateInputRequestTypeDef](./type_defs.md#createreviewtemplateinputrequesttypedef) 

### create\_template\_share

Create a review template share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_template_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_template_share)

```python
# create_template_share method definition

await def create_template_share(
    self,
    *,
    TemplateArn: str,
    SharedWith: str,
    ClientRequestToken: str,
) -> CreateTemplateShareOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateTemplateShareOutputTypeDef](./type_defs.md#createtemplateshareoutputtypedef) 


```python
# create_template_share method usage example with argument unpacking

kwargs: CreateTemplateShareInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "SharedWith": ...,
    "ClientRequestToken": ...,
}

parent.create_template_share(**kwargs)
```

1. See [:material-code-braces: CreateTemplateShareInputRequestTypeDef](./type_defs.md#createtemplateshareinputrequesttypedef) 

### create\_workload

Create a new workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)

```python
# create_workload method definition

await def create_workload(
    self,
    *,
    WorkloadName: str,
    Description: str,
    Environment: WorkloadEnvironmentType,  # (1)
    Lenses: Sequence[str],
    ClientRequestToken: str,
    AccountIds: Sequence[str] = ...,
    AwsRegions: Sequence[str] = ...,
    NonAwsRegions: Sequence[str] = ...,
    PillarPriorities: Sequence[str] = ...,
    ArchitecturalDesign: str = ...,
    ReviewOwner: str = ...,
    IndustryType: str = ...,
    Industry: str = ...,
    Notes: str = ...,
    Tags: Mapping[str, str] = ...,
    DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,  # (2)
    Applications: Sequence[str] = ...,
    ProfileArns: Sequence[str] = ...,
    ReviewTemplateArns: Sequence[str] = ...,
    JiraConfiguration: WorkloadJiraConfigurationInputTypeDef = ...,  # (3)
) -> CreateWorkloadOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: WorkloadEnvironmentType](./literals.md#workloadenvironmenttype) 
2. See [:material-code-braces: WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef) 
3. See [:material-code-braces: WorkloadJiraConfigurationInputTypeDef](./type_defs.md#workloadjiraconfigurationinputtypedef) 
4. See [:material-code-braces: CreateWorkloadOutputTypeDef](./type_defs.md#createworkloadoutputtypedef) 


```python
# create_workload method usage example with argument unpacking

kwargs: CreateWorkloadInputRequestTypeDef = {  # (1)
    "WorkloadName": ...,
    "Description": ...,
    "Environment": ...,
    "Lenses": ...,
    "ClientRequestToken": ...,
}

parent.create_workload(**kwargs)
```

1. See [:material-code-braces: CreateWorkloadInputRequestTypeDef](./type_defs.md#createworkloadinputrequesttypedef) 

### create\_workload\_share

Create a workload share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").create_workload_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload_share)

```python
# create_workload_share method definition

await def create_workload_share(
    self,
    *,
    WorkloadId: str,
    SharedWith: str,
    PermissionType: PermissionTypeType,  # (1)
    ClientRequestToken: str,
) -> CreateWorkloadShareOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: CreateWorkloadShareOutputTypeDef](./type_defs.md#createworkloadshareoutputtypedef) 


```python
# create_workload_share method usage example with argument unpacking

kwargs: CreateWorkloadShareInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "SharedWith": ...,
    "PermissionType": ...,
    "ClientRequestToken": ...,
}

parent.create_workload_share(**kwargs)
```

1. See [:material-code-braces: CreateWorkloadShareInputRequestTypeDef](./type_defs.md#createworkloadshareinputrequesttypedef) 

### delete\_lens

Delete an existing lens.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_lens` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_lens)

```python
# delete_lens method definition

await def delete_lens(
    self,
    *,
    LensAlias: str,
    ClientRequestToken: str,
    LensStatus: LensStatusTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LensStatusTypeType](./literals.md#lensstatustypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_lens method usage example with argument unpacking

kwargs: DeleteLensInputRequestTypeDef = {  # (1)
    "LensAlias": ...,
    "ClientRequestToken": ...,
    "LensStatus": ...,
}

parent.delete_lens(**kwargs)
```

1. See [:material-code-braces: DeleteLensInputRequestTypeDef](./type_defs.md#deletelensinputrequesttypedef) 

### delete\_lens\_share

Delete a lens share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_lens_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_lens_share)

```python
# delete_lens_share method definition

await def delete_lens_share(
    self,
    *,
    ShareId: str,
    LensAlias: str,
    ClientRequestToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_lens_share method usage example with argument unpacking

kwargs: DeleteLensShareInputRequestTypeDef = {  # (1)
    "ShareId": ...,
    "LensAlias": ...,
    "ClientRequestToken": ...,
}

parent.delete_lens_share(**kwargs)
```

1. See [:material-code-braces: DeleteLensShareInputRequestTypeDef](./type_defs.md#deletelensshareinputrequesttypedef) 

### delete\_profile

Delete a profile.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile)

```python
# delete_profile method definition

await def delete_profile(
    self,
    *,
    ProfileArn: str,
    ClientRequestToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_profile method usage example with argument unpacking

kwargs: DeleteProfileInputRequestTypeDef = {  # (1)
    "ProfileArn": ...,
    "ClientRequestToken": ...,
}

parent.delete_profile(**kwargs)
```

1. See [:material-code-braces: DeleteProfileInputRequestTypeDef](./type_defs.md#deleteprofileinputrequesttypedef) 

### delete\_profile\_share

Delete a profile share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_profile_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile_share)

```python
# delete_profile_share method definition

await def delete_profile_share(
    self,
    *,
    ShareId: str,
    ProfileArn: str,
    ClientRequestToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_profile_share method usage example with argument unpacking

kwargs: DeleteProfileShareInputRequestTypeDef = {  # (1)
    "ShareId": ...,
    "ProfileArn": ...,
    "ClientRequestToken": ...,
}

parent.delete_profile_share(**kwargs)
```

1. See [:material-code-braces: DeleteProfileShareInputRequestTypeDef](./type_defs.md#deleteprofileshareinputrequesttypedef) 

### delete\_review\_template

Delete a review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_review_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_review_template)

```python
# delete_review_template method definition

await def delete_review_template(
    self,
    *,
    TemplateArn: str,
    ClientRequestToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_review_template method usage example with argument unpacking

kwargs: DeleteReviewTemplateInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "ClientRequestToken": ...,
}

parent.delete_review_template(**kwargs)
```

1. See [:material-code-braces: DeleteReviewTemplateInputRequestTypeDef](./type_defs.md#deletereviewtemplateinputrequesttypedef) 

### delete\_template\_share

Delete a review template share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_template_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_template_share)

```python
# delete_template_share method definition

await def delete_template_share(
    self,
    *,
    ShareId: str,
    TemplateArn: str,
    ClientRequestToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_template_share method usage example with argument unpacking

kwargs: DeleteTemplateShareInputRequestTypeDef = {  # (1)
    "ShareId": ...,
    "TemplateArn": ...,
    "ClientRequestToken": ...,
}

parent.delete_template_share(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateShareInputRequestTypeDef](./type_defs.md#deletetemplateshareinputrequesttypedef) 

### delete\_workload

Delete an existing workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_workload)

```python
# delete_workload method definition

await def delete_workload(
    self,
    *,
    WorkloadId: str,
    ClientRequestToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_workload method usage example with argument unpacking

kwargs: DeleteWorkloadInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "ClientRequestToken": ...,
}

parent.delete_workload(**kwargs)
```

1. See [:material-code-braces: DeleteWorkloadInputRequestTypeDef](./type_defs.md#deleteworkloadinputrequesttypedef) 

### delete\_workload\_share

Delete a workload share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").delete_workload_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_workload_share)

```python
# delete_workload_share method definition

await def delete_workload_share(
    self,
    *,
    ShareId: str,
    WorkloadId: str,
    ClientRequestToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_workload_share method usage example with argument unpacking

kwargs: DeleteWorkloadShareInputRequestTypeDef = {  # (1)
    "ShareId": ...,
    "WorkloadId": ...,
    "ClientRequestToken": ...,
}

parent.delete_workload_share(**kwargs)
```

1. See [:material-code-braces: DeleteWorkloadShareInputRequestTypeDef](./type_defs.md#deleteworkloadshareinputrequesttypedef) 

### disassociate\_lenses

Disassociate a lens from a workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").disassociate_lenses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_lenses)

```python
# disassociate_lenses method definition

await def disassociate_lenses(
    self,
    *,
    WorkloadId: str,
    LensAliases: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_lenses method usage example with argument unpacking

kwargs: DisassociateLensesInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAliases": ...,
}

parent.disassociate_lenses(**kwargs)
```

1. See [:material-code-braces: DisassociateLensesInputRequestTypeDef](./type_defs.md#disassociatelensesinputrequesttypedef) 

### disassociate\_profiles

Disassociate a profile from a workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").disassociate_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_profiles)

```python
# disassociate_profiles method definition

await def disassociate_profiles(
    self,
    *,
    WorkloadId: str,
    ProfileArns: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_profiles method usage example with argument unpacking

kwargs: DisassociateProfilesInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "ProfileArns": ...,
}

parent.disassociate_profiles(**kwargs)
```

1. See [:material-code-braces: DisassociateProfilesInputRequestTypeDef](./type_defs.md#disassociateprofilesinputrequesttypedef) 

### export\_lens

Export an existing lens.

Type annotations and code completion for `#!python session.create_client("wellarchitected").export_lens` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.export_lens)

```python
# export_lens method definition

await def export_lens(
    self,
    *,
    LensAlias: str,
    LensVersion: str = ...,
) -> ExportLensOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportLensOutputTypeDef](./type_defs.md#exportlensoutputtypedef) 


```python
# export_lens method usage example with argument unpacking

kwargs: ExportLensInputRequestTypeDef = {  # (1)
    "LensAlias": ...,
}

parent.export_lens(**kwargs)
```

1. See [:material-code-braces: ExportLensInputRequestTypeDef](./type_defs.md#exportlensinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("wellarchitected").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.generate_presigned_url)

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


### get\_answer

Get the answer to a specific question in a workload review.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_answer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_answer)

```python
# get_answer method definition

await def get_answer(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    QuestionId: str,
    MilestoneNumber: int = ...,
) -> GetAnswerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnswerOutputTypeDef](./type_defs.md#getansweroutputtypedef) 


```python
# get_answer method usage example with argument unpacking

kwargs: GetAnswerInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
    "QuestionId": ...,
}

parent.get_answer(**kwargs)
```

1. See [:material-code-braces: GetAnswerInputRequestTypeDef](./type_defs.md#getanswerinputrequesttypedef) 

### get\_consolidated\_report

Get a consolidated report of your workloads.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_consolidated_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)

```python
# get_consolidated_report method definition

await def get_consolidated_report(
    self,
    *,
    Format: ReportFormatType,  # (1)
    IncludeSharedResources: bool = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetConsolidatedReportOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReportFormatType](./literals.md#reportformattype) 
2. See [:material-code-braces: GetConsolidatedReportOutputTypeDef](./type_defs.md#getconsolidatedreportoutputtypedef) 


```python
# get_consolidated_report method usage example with argument unpacking

kwargs: GetConsolidatedReportInputRequestTypeDef = {  # (1)
    "Format": ...,
}

parent.get_consolidated_report(**kwargs)
```

1. See [:material-code-braces: GetConsolidatedReportInputRequestTypeDef](./type_defs.md#getconsolidatedreportinputrequesttypedef) 

### get\_global\_settings

Global settings for all workloads.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_global_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_global_settings)

```python
# get_global_settings method definition

await def get_global_settings(
    self,
) -> GetGlobalSettingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGlobalSettingsOutputTypeDef](./type_defs.md#getglobalsettingsoutputtypedef) 

### get\_lens

Get an existing lens.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_lens` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)

```python
# get_lens method definition

await def get_lens(
    self,
    *,
    LensAlias: str,
    LensVersion: str = ...,
) -> GetLensOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLensOutputTypeDef](./type_defs.md#getlensoutputtypedef) 


```python
# get_lens method usage example with argument unpacking

kwargs: GetLensInputRequestTypeDef = {  # (1)
    "LensAlias": ...,
}

parent.get_lens(**kwargs)
```

1. See [:material-code-braces: GetLensInputRequestTypeDef](./type_defs.md#getlensinputrequesttypedef) 

### get\_lens\_review

Get lens review.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_lens_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens_review)

```python
# get_lens_review method definition

await def get_lens_review(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    MilestoneNumber: int = ...,
) -> GetLensReviewOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLensReviewOutputTypeDef](./type_defs.md#getlensreviewoutputtypedef) 


```python
# get_lens_review method usage example with argument unpacking

kwargs: GetLensReviewInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
}

parent.get_lens_review(**kwargs)
```

1. See [:material-code-braces: GetLensReviewInputRequestTypeDef](./type_defs.md#getlensreviewinputrequesttypedef) 

### get\_lens\_review\_report

Get lens review report.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_lens_review_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens_review_report)

```python
# get_lens_review_report method definition

await def get_lens_review_report(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    MilestoneNumber: int = ...,
) -> GetLensReviewReportOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLensReviewReportOutputTypeDef](./type_defs.md#getlensreviewreportoutputtypedef) 


```python
# get_lens_review_report method usage example with argument unpacking

kwargs: GetLensReviewReportInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
}

parent.get_lens_review_report(**kwargs)
```

1. See [:material-code-braces: GetLensReviewReportInputRequestTypeDef](./type_defs.md#getlensreviewreportinputrequesttypedef) 

### get\_lens\_version\_difference

Get lens version differences.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_lens_version_difference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens_version_difference)

```python
# get_lens_version_difference method definition

await def get_lens_version_difference(
    self,
    *,
    LensAlias: str,
    BaseLensVersion: str = ...,
    TargetLensVersion: str = ...,
) -> GetLensVersionDifferenceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLensVersionDifferenceOutputTypeDef](./type_defs.md#getlensversiondifferenceoutputtypedef) 


```python
# get_lens_version_difference method usage example with argument unpacking

kwargs: GetLensVersionDifferenceInputRequestTypeDef = {  # (1)
    "LensAlias": ...,
}

parent.get_lens_version_difference(**kwargs)
```

1. See [:material-code-braces: GetLensVersionDifferenceInputRequestTypeDef](./type_defs.md#getlensversiondifferenceinputrequesttypedef) 

### get\_milestone

Get a milestone for an existing workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_milestone` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_milestone)

```python
# get_milestone method definition

await def get_milestone(
    self,
    *,
    WorkloadId: str,
    MilestoneNumber: int,
) -> GetMilestoneOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMilestoneOutputTypeDef](./type_defs.md#getmilestoneoutputtypedef) 


```python
# get_milestone method usage example with argument unpacking

kwargs: GetMilestoneInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "MilestoneNumber": ...,
}

parent.get_milestone(**kwargs)
```

1. See [:material-code-braces: GetMilestoneInputRequestTypeDef](./type_defs.md#getmilestoneinputrequesttypedef) 

### get\_profile

Get profile information.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile)

```python
# get_profile method definition

await def get_profile(
    self,
    *,
    ProfileArn: str,
    ProfileVersion: str = ...,
) -> GetProfileOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProfileOutputTypeDef](./type_defs.md#getprofileoutputtypedef) 


```python
# get_profile method usage example with argument unpacking

kwargs: GetProfileInputRequestTypeDef = {  # (1)
    "ProfileArn": ...,
}

parent.get_profile(**kwargs)
```

1. See [:material-code-braces: GetProfileInputRequestTypeDef](./type_defs.md#getprofileinputrequesttypedef) 

### get\_profile\_template

Get profile template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_profile_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile_template)

```python
# get_profile_template method definition

await def get_profile_template(
    self,
) -> GetProfileTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProfileTemplateOutputTypeDef](./type_defs.md#getprofiletemplateoutputtypedef) 

### get\_review\_template

Get review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_review_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_review_template)

```python
# get_review_template method definition

await def get_review_template(
    self,
    *,
    TemplateArn: str,
) -> GetReviewTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReviewTemplateOutputTypeDef](./type_defs.md#getreviewtemplateoutputtypedef) 


```python
# get_review_template method usage example with argument unpacking

kwargs: GetReviewTemplateInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.get_review_template(**kwargs)
```

1. See [:material-code-braces: GetReviewTemplateInputRequestTypeDef](./type_defs.md#getreviewtemplateinputrequesttypedef) 

### get\_review\_template\_answer

Get review template answer.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_review_template_answer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_review_template_answer)

```python
# get_review_template_answer method definition

await def get_review_template_answer(
    self,
    *,
    TemplateArn: str,
    LensAlias: str,
    QuestionId: str,
) -> GetReviewTemplateAnswerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReviewTemplateAnswerOutputTypeDef](./type_defs.md#getreviewtemplateansweroutputtypedef) 


```python
# get_review_template_answer method usage example with argument unpacking

kwargs: GetReviewTemplateAnswerInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "LensAlias": ...,
    "QuestionId": ...,
}

parent.get_review_template_answer(**kwargs)
```

1. See [:material-code-braces: GetReviewTemplateAnswerInputRequestTypeDef](./type_defs.md#getreviewtemplateanswerinputrequesttypedef) 

### get\_review\_template\_lens\_review

Get a lens review associated with a review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_review_template_lens_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_review_template_lens_review)

```python
# get_review_template_lens_review method definition

await def get_review_template_lens_review(
    self,
    *,
    TemplateArn: str,
    LensAlias: str,
) -> GetReviewTemplateLensReviewOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReviewTemplateLensReviewOutputTypeDef](./type_defs.md#getreviewtemplatelensreviewoutputtypedef) 


```python
# get_review_template_lens_review method usage example with argument unpacking

kwargs: GetReviewTemplateLensReviewInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "LensAlias": ...,
}

parent.get_review_template_lens_review(**kwargs)
```

1. See [:material-code-braces: GetReviewTemplateLensReviewInputRequestTypeDef](./type_defs.md#getreviewtemplatelensreviewinputrequesttypedef) 

### get\_workload

Get an existing workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").get_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_workload)

```python
# get_workload method definition

await def get_workload(
    self,
    *,
    WorkloadId: str,
) -> GetWorkloadOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadOutputTypeDef](./type_defs.md#getworkloadoutputtypedef) 


```python
# get_workload method usage example with argument unpacking

kwargs: GetWorkloadInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
}

parent.get_workload(**kwargs)
```

1. See [:material-code-braces: GetWorkloadInputRequestTypeDef](./type_defs.md#getworkloadinputrequesttypedef) 

### import\_lens

Import a new custom lens or update an existing custom lens.

Type annotations and code completion for `#!python session.create_client("wellarchitected").import_lens` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)

```python
# import_lens method definition

await def import_lens(
    self,
    *,
    JSONString: str,
    ClientRequestToken: str,
    LensAlias: str = ...,
    Tags: Mapping[str, str] = ...,
) -> ImportLensOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ImportLensOutputTypeDef](./type_defs.md#importlensoutputtypedef) 


```python
# import_lens method usage example with argument unpacking

kwargs: ImportLensInputRequestTypeDef = {  # (1)
    "JSONString": ...,
    "ClientRequestToken": ...,
}

parent.import_lens(**kwargs)
```

1. See [:material-code-braces: ImportLensInputRequestTypeDef](./type_defs.md#importlensinputrequesttypedef) 

### list\_answers

List of answers for a particular workload and lens.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_answers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)

```python
# list_answers method definition

await def list_answers(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    PillarId: str = ...,
    MilestoneNumber: int = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    QuestionPriority: QuestionPriorityType = ...,  # (1)
) -> ListAnswersOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QuestionPriorityType](./literals.md#questionprioritytype) 
2. See [:material-code-braces: ListAnswersOutputTypeDef](./type_defs.md#listanswersoutputtypedef) 


```python
# list_answers method usage example with argument unpacking

kwargs: ListAnswersInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
}

parent.list_answers(**kwargs)
```

1. See [:material-code-braces: ListAnswersInputRequestTypeDef](./type_defs.md#listanswersinputrequesttypedef) 

### list\_check\_details

List of Trusted Advisor check details by account related to the workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_check_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_details)

```python
# list_check_details method definition

await def list_check_details(
    self,
    *,
    WorkloadId: str,
    LensArn: str,
    PillarId: str,
    QuestionId: str,
    ChoiceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCheckDetailsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCheckDetailsOutputTypeDef](./type_defs.md#listcheckdetailsoutputtypedef) 


```python
# list_check_details method usage example with argument unpacking

kwargs: ListCheckDetailsInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensArn": ...,
    "PillarId": ...,
    "QuestionId": ...,
    "ChoiceId": ...,
}

parent.list_check_details(**kwargs)
```

1. See [:material-code-braces: ListCheckDetailsInputRequestTypeDef](./type_defs.md#listcheckdetailsinputrequesttypedef) 

### list\_check\_summaries

List of Trusted Advisor checks summarized for all accounts related to the
workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_check_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_check_summaries)

```python
# list_check_summaries method definition

await def list_check_summaries(
    self,
    *,
    WorkloadId: str,
    LensArn: str,
    PillarId: str,
    QuestionId: str,
    ChoiceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCheckSummariesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCheckSummariesOutputTypeDef](./type_defs.md#listchecksummariesoutputtypedef) 


```python
# list_check_summaries method usage example with argument unpacking

kwargs: ListCheckSummariesInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensArn": ...,
    "PillarId": ...,
    "QuestionId": ...,
    "ChoiceId": ...,
}

parent.list_check_summaries(**kwargs)
```

1. See [:material-code-braces: ListCheckSummariesInputRequestTypeDef](./type_defs.md#listchecksummariesinputrequesttypedef) 

### list\_lens\_review\_improvements

List the improvements of a particular lens review.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_lens_review_improvements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)

```python
# list_lens_review_improvements method definition

await def list_lens_review_improvements(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    PillarId: str = ...,
    MilestoneNumber: int = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    QuestionPriority: QuestionPriorityType = ...,  # (1)
) -> ListLensReviewImprovementsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QuestionPriorityType](./literals.md#questionprioritytype) 
2. See [:material-code-braces: ListLensReviewImprovementsOutputTypeDef](./type_defs.md#listlensreviewimprovementsoutputtypedef) 


```python
# list_lens_review_improvements method usage example with argument unpacking

kwargs: ListLensReviewImprovementsInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
}

parent.list_lens_review_improvements(**kwargs)
```

1. See [:material-code-braces: ListLensReviewImprovementsInputRequestTypeDef](./type_defs.md#listlensreviewimprovementsinputrequesttypedef) 

### list\_lens\_reviews

List lens reviews for a particular workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_lens_reviews` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)

```python
# list_lens_reviews method definition

await def list_lens_reviews(
    self,
    *,
    WorkloadId: str,
    MilestoneNumber: int = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLensReviewsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLensReviewsOutputTypeDef](./type_defs.md#listlensreviewsoutputtypedef) 


```python
# list_lens_reviews method usage example with argument unpacking

kwargs: ListLensReviewsInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
}

parent.list_lens_reviews(**kwargs)
```

1. See [:material-code-braces: ListLensReviewsInputRequestTypeDef](./type_defs.md#listlensreviewsinputrequesttypedef) 

### list\_lens\_shares

List the lens shares associated with the lens.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_lens_shares` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_shares)

```python
# list_lens_shares method definition

await def list_lens_shares(
    self,
    *,
    LensAlias: str,
    SharedWithPrefix: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: ShareStatusType = ...,  # (1)
) -> ListLensSharesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ListLensSharesOutputTypeDef](./type_defs.md#listlenssharesoutputtypedef) 


```python
# list_lens_shares method usage example with argument unpacking

kwargs: ListLensSharesInputRequestTypeDef = {  # (1)
    "LensAlias": ...,
}

parent.list_lens_shares(**kwargs)
```

1. See [:material-code-braces: ListLensSharesInputRequestTypeDef](./type_defs.md#listlenssharesinputrequesttypedef) 

### list\_lenses

List the available lenses.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_lenses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lenses)

```python
# list_lenses method definition

await def list_lenses(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    LensType: LensTypeType = ...,  # (1)
    LensStatus: LensStatusTypeType = ...,  # (2)
    LensName: str = ...,
) -> ListLensesOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LensTypeType](./literals.md#lenstypetype) 
2. See [:material-code-brackets: LensStatusTypeType](./literals.md#lensstatustypetype) 
3. See [:material-code-braces: ListLensesOutputTypeDef](./type_defs.md#listlensesoutputtypedef) 


```python
# list_lenses method usage example with argument unpacking

kwargs: ListLensesInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_lenses(**kwargs)
```

1. See [:material-code-braces: ListLensesInputRequestTypeDef](./type_defs.md#listlensesinputrequesttypedef) 

### list\_milestones

List all milestones for an existing workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_milestones` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_milestones)

```python
# list_milestones method definition

await def list_milestones(
    self,
    *,
    WorkloadId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMilestonesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMilestonesOutputTypeDef](./type_defs.md#listmilestonesoutputtypedef) 


```python
# list_milestones method usage example with argument unpacking

kwargs: ListMilestonesInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
}

parent.list_milestones(**kwargs)
```

1. See [:material-code-braces: ListMilestonesInputRequestTypeDef](./type_defs.md#listmilestonesinputrequesttypedef) 

### list\_notifications

List lens notifications.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_notifications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)

```python
# list_notifications method definition

await def list_notifications(
    self,
    *,
    WorkloadId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    ResourceArn: str = ...,
) -> ListNotificationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNotificationsOutputTypeDef](./type_defs.md#listnotificationsoutputtypedef) 


```python
# list_notifications method usage example with argument unpacking

kwargs: ListNotificationsInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
}

parent.list_notifications(**kwargs)
```

1. See [:material-code-braces: ListNotificationsInputRequestTypeDef](./type_defs.md#listnotificationsinputrequesttypedef) 

### list\_profile\_notifications

List profile notifications.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_profile_notifications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_notifications)

```python
# list_profile_notifications method definition

await def list_profile_notifications(
    self,
    *,
    WorkloadId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProfileNotificationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProfileNotificationsOutputTypeDef](./type_defs.md#listprofilenotificationsoutputtypedef) 


```python
# list_profile_notifications method usage example with argument unpacking

kwargs: ListProfileNotificationsInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
}

parent.list_profile_notifications(**kwargs)
```

1. See [:material-code-braces: ListProfileNotificationsInputRequestTypeDef](./type_defs.md#listprofilenotificationsinputrequesttypedef) 

### list\_profile\_shares

List profile shares.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_profile_shares` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)

```python
# list_profile_shares method definition

await def list_profile_shares(
    self,
    *,
    ProfileArn: str,
    SharedWithPrefix: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: ShareStatusType = ...,  # (1)
) -> ListProfileSharesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ListProfileSharesOutputTypeDef](./type_defs.md#listprofilesharesoutputtypedef) 


```python
# list_profile_shares method usage example with argument unpacking

kwargs: ListProfileSharesInputRequestTypeDef = {  # (1)
    "ProfileArn": ...,
}

parent.list_profile_shares(**kwargs)
```

1. See [:material-code-braces: ListProfileSharesInputRequestTypeDef](./type_defs.md#listprofilesharesinputrequesttypedef) 

### list\_profiles

List profiles.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)

```python
# list_profiles method definition

await def list_profiles(
    self,
    *,
    ProfileNamePrefix: str = ...,
    ProfileOwnerType: ProfileOwnerTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProfilesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProfileOwnerTypeType](./literals.md#profileownertypetype) 
2. See [:material-code-braces: ListProfilesOutputTypeDef](./type_defs.md#listprofilesoutputtypedef) 


```python
# list_profiles method usage example with argument unpacking

kwargs: ListProfilesInputRequestTypeDef = {  # (1)
    "ProfileNamePrefix": ...,
}

parent.list_profiles(**kwargs)
```

1. See [:material-code-braces: ListProfilesInputRequestTypeDef](./type_defs.md#listprofilesinputrequesttypedef) 

### list\_review\_template\_answers

List the answers of a review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_review_template_answers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_review_template_answers)

```python
# list_review_template_answers method definition

await def list_review_template_answers(
    self,
    *,
    TemplateArn: str,
    LensAlias: str,
    PillarId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListReviewTemplateAnswersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListReviewTemplateAnswersOutputTypeDef](./type_defs.md#listreviewtemplateanswersoutputtypedef) 


```python
# list_review_template_answers method usage example with argument unpacking

kwargs: ListReviewTemplateAnswersInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "LensAlias": ...,
}

parent.list_review_template_answers(**kwargs)
```

1. See [:material-code-braces: ListReviewTemplateAnswersInputRequestTypeDef](./type_defs.md#listreviewtemplateanswersinputrequesttypedef) 

### list\_review\_templates

List review templates.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_review_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_review_templates)

```python
# list_review_templates method definition

await def list_review_templates(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListReviewTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListReviewTemplatesOutputTypeDef](./type_defs.md#listreviewtemplatesoutputtypedef) 


```python
# list_review_templates method usage example with argument unpacking

kwargs: ListReviewTemplatesInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_review_templates(**kwargs)
```

1. See [:material-code-braces: ListReviewTemplatesInputRequestTypeDef](./type_defs.md#listreviewtemplatesinputrequesttypedef) 

### list\_share\_invitations

List the share invitations.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_share_invitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)

```python
# list_share_invitations method definition

await def list_share_invitations(
    self,
    *,
    WorkloadNamePrefix: str = ...,
    LensNamePrefix: str = ...,
    ShareResourceType: ShareResourceTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    ProfileNamePrefix: str = ...,
    TemplateNamePrefix: str = ...,
) -> ListShareInvitationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShareResourceTypeType](./literals.md#shareresourcetypetype) 
2. See [:material-code-braces: ListShareInvitationsOutputTypeDef](./type_defs.md#listshareinvitationsoutputtypedef) 


```python
# list_share_invitations method usage example with argument unpacking

kwargs: ListShareInvitationsInputRequestTypeDef = {  # (1)
    "WorkloadNamePrefix": ...,
}

parent.list_share_invitations(**kwargs)
```

1. See [:material-code-braces: ListShareInvitationsInputRequestTypeDef](./type_defs.md#listshareinvitationsinputrequesttypedef) 

### list\_tags\_for\_resource

List the tags for a resource.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    WorkloadArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "WorkloadArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### list\_template\_shares

List review template shares.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_template_shares` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_template_shares)

```python
# list_template_shares method definition

await def list_template_shares(
    self,
    *,
    TemplateArn: str,
    SharedWithPrefix: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: ShareStatusType = ...,  # (1)
) -> ListTemplateSharesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ListTemplateSharesOutputTypeDef](./type_defs.md#listtemplatesharesoutputtypedef) 


```python
# list_template_shares method usage example with argument unpacking

kwargs: ListTemplateSharesInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.list_template_shares(**kwargs)
```

1. See [:material-code-braces: ListTemplateSharesInputRequestTypeDef](./type_defs.md#listtemplatesharesinputrequesttypedef) 

### list\_workload\_shares

List the workload shares associated with the workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_workload_shares` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)

```python
# list_workload_shares method definition

await def list_workload_shares(
    self,
    *,
    WorkloadId: str,
    SharedWithPrefix: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: ShareStatusType = ...,  # (1)
) -> ListWorkloadSharesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ListWorkloadSharesOutputTypeDef](./type_defs.md#listworkloadsharesoutputtypedef) 


```python
# list_workload_shares method usage example with argument unpacking

kwargs: ListWorkloadSharesInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
}

parent.list_workload_shares(**kwargs)
```

1. See [:material-code-braces: ListWorkloadSharesInputRequestTypeDef](./type_defs.md#listworkloadsharesinputrequesttypedef) 

### list\_workloads

Paginated list of workloads.

Type annotations and code completion for `#!python session.create_client("wellarchitected").list_workloads` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workloads)

```python
# list_workloads method definition

await def list_workloads(
    self,
    *,
    WorkloadNamePrefix: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListWorkloadsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef) 


```python
# list_workloads method usage example with argument unpacking

kwargs: ListWorkloadsInputRequestTypeDef = {  # (1)
    "WorkloadNamePrefix": ...,
}

parent.list_workloads(**kwargs)
```

1. See [:material-code-braces: ListWorkloadsInputRequestTypeDef](./type_defs.md#listworkloadsinputrequesttypedef) 

### tag\_resource

Adds one or more tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("wellarchitected").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    WorkloadArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "WorkloadArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Deletes specified tags from a resource.

Type annotations and code completion for `#!python session.create_client("wellarchitected").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    WorkloadArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "WorkloadArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_answer

Update the answer to a specific question in a workload review.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_answer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)

```python
# update_answer method definition

await def update_answer(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    QuestionId: str,
    SelectedChoices: Sequence[str] = ...,
    ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,  # (1)
    Notes: str = ...,
    IsApplicable: bool = ...,
    Reason: AnswerReasonType = ...,  # (2)
) -> UpdateAnswerOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ChoiceUpdateTypeDef](./type_defs.md#choiceupdatetypedef) 
2. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
3. See [:material-code-braces: UpdateAnswerOutputTypeDef](./type_defs.md#updateansweroutputtypedef) 


```python
# update_answer method usage example with argument unpacking

kwargs: UpdateAnswerInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
    "QuestionId": ...,
}

parent.update_answer(**kwargs)
```

1. See [:material-code-braces: UpdateAnswerInputRequestTypeDef](./type_defs.md#updateanswerinputrequesttypedef) 

### update\_global\_settings

Update whether the Amazon Web Services account is opted into organization
sharing and discovery integration
features.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_global_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)

```python
# update_global_settings method definition

await def update_global_settings(
    self,
    *,
    OrganizationSharingStatus: OrganizationSharingStatusType = ...,  # (1)
    DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...,  # (2)
    JiraConfiguration: AccountJiraConfigurationInputTypeDef = ...,  # (3)
) -> EmptyResponseMetadataTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: OrganizationSharingStatusType](./literals.md#organizationsharingstatustype) 
2. See [:material-code-brackets: DiscoveryIntegrationStatusType](./literals.md#discoveryintegrationstatustype) 
3. See [:material-code-braces: AccountJiraConfigurationInputTypeDef](./type_defs.md#accountjiraconfigurationinputtypedef) 
4. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_global_settings method usage example with argument unpacking

kwargs: UpdateGlobalSettingsInputRequestTypeDef = {  # (1)
    "OrganizationSharingStatus": ...,
}

parent.update_global_settings(**kwargs)
```

1. See [:material-code-braces: UpdateGlobalSettingsInputRequestTypeDef](./type_defs.md#updateglobalsettingsinputrequesttypedef) 

### update\_integration

Update integration features.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_integration)

```python
# update_integration method definition

await def update_integration(
    self,
    *,
    WorkloadId: str,
    ClientRequestToken: str,
    IntegratingService: IntegratingServiceType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IntegratingServiceType](./literals.md#integratingservicetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_integration method usage example with argument unpacking

kwargs: UpdateIntegrationInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "ClientRequestToken": ...,
    "IntegratingService": ...,
}

parent.update_integration(**kwargs)
```

1. See [:material-code-braces: UpdateIntegrationInputRequestTypeDef](./type_defs.md#updateintegrationinputrequesttypedef) 

### update\_lens\_review

Update lens review for a particular workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_lens_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)

```python
# update_lens_review method definition

await def update_lens_review(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    LensNotes: str = ...,
    PillarNotes: Mapping[str, str] = ...,
    JiraConfiguration: JiraSelectedQuestionConfigurationTypeDef = ...,  # (1)
) -> UpdateLensReviewOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: JiraSelectedQuestionConfigurationTypeDef](./type_defs.md#jiraselectedquestionconfigurationtypedef) 
2. See [:material-code-braces: UpdateLensReviewOutputTypeDef](./type_defs.md#updatelensreviewoutputtypedef) 


```python
# update_lens_review method usage example with argument unpacking

kwargs: UpdateLensReviewInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
}

parent.update_lens_review(**kwargs)
```

1. See [:material-code-braces: UpdateLensReviewInputRequestTypeDef](./type_defs.md#updatelensreviewinputrequesttypedef) 

### update\_profile

Update a profile.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)

```python
# update_profile method definition

await def update_profile(
    self,
    *,
    ProfileArn: str,
    ProfileDescription: str = ...,
    ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...,  # (1)
) -> UpdateProfileOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ProfileQuestionUpdateTypeDef](./type_defs.md#profilequestionupdatetypedef) 
2. See [:material-code-braces: UpdateProfileOutputTypeDef](./type_defs.md#updateprofileoutputtypedef) 


```python
# update_profile method usage example with argument unpacking

kwargs: UpdateProfileInputRequestTypeDef = {  # (1)
    "ProfileArn": ...,
}

parent.update_profile(**kwargs)
```

1. See [:material-code-braces: UpdateProfileInputRequestTypeDef](./type_defs.md#updateprofileinputrequesttypedef) 

### update\_review\_template

Update a review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_review_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template)

```python
# update_review_template method definition

await def update_review_template(
    self,
    *,
    TemplateArn: str,
    TemplateName: str = ...,
    Description: str = ...,
    Notes: str = ...,
    LensesToAssociate: Sequence[str] = ...,
    LensesToDisassociate: Sequence[str] = ...,
) -> UpdateReviewTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateReviewTemplateOutputTypeDef](./type_defs.md#updatereviewtemplateoutputtypedef) 


```python
# update_review_template method usage example with argument unpacking

kwargs: UpdateReviewTemplateInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.update_review_template(**kwargs)
```

1. See [:material-code-braces: UpdateReviewTemplateInputRequestTypeDef](./type_defs.md#updatereviewtemplateinputrequesttypedef) 

### update\_review\_template\_answer

Update a review template answer.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_review_template_answer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_answer)

```python
# update_review_template_answer method definition

await def update_review_template_answer(
    self,
    *,
    TemplateArn: str,
    LensAlias: str,
    QuestionId: str,
    SelectedChoices: Sequence[str] = ...,
    ChoiceUpdates: Mapping[str, ChoiceUpdateTypeDef] = ...,  # (1)
    Notes: str = ...,
    IsApplicable: bool = ...,
    Reason: AnswerReasonType = ...,  # (2)
) -> UpdateReviewTemplateAnswerOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ChoiceUpdateTypeDef](./type_defs.md#choiceupdatetypedef) 
2. See [:material-code-brackets: AnswerReasonType](./literals.md#answerreasontype) 
3. See [:material-code-braces: UpdateReviewTemplateAnswerOutputTypeDef](./type_defs.md#updatereviewtemplateansweroutputtypedef) 


```python
# update_review_template_answer method usage example with argument unpacking

kwargs: UpdateReviewTemplateAnswerInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "LensAlias": ...,
    "QuestionId": ...,
}

parent.update_review_template_answer(**kwargs)
```

1. See [:material-code-braces: UpdateReviewTemplateAnswerInputRequestTypeDef](./type_defs.md#updatereviewtemplateanswerinputrequesttypedef) 

### update\_review\_template\_lens\_review

Update a lens review associated with a review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_review_template_lens_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_review_template_lens_review)

```python
# update_review_template_lens_review method definition

await def update_review_template_lens_review(
    self,
    *,
    TemplateArn: str,
    LensAlias: str,
    LensNotes: str = ...,
    PillarNotes: Mapping[str, str] = ...,
) -> UpdateReviewTemplateLensReviewOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateReviewTemplateLensReviewOutputTypeDef](./type_defs.md#updatereviewtemplatelensreviewoutputtypedef) 


```python
# update_review_template_lens_review method usage example with argument unpacking

kwargs: UpdateReviewTemplateLensReviewInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "LensAlias": ...,
}

parent.update_review_template_lens_review(**kwargs)
```

1. See [:material-code-braces: UpdateReviewTemplateLensReviewInputRequestTypeDef](./type_defs.md#updatereviewtemplatelensreviewinputrequesttypedef) 

### update\_share\_invitation

Update a workload or custom lens share invitation.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_share_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_share_invitation)

```python
# update_share_invitation method definition

await def update_share_invitation(
    self,
    *,
    ShareInvitationId: str,
    ShareInvitationAction: ShareInvitationActionType,  # (1)
) -> UpdateShareInvitationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShareInvitationActionType](./literals.md#shareinvitationactiontype) 
2. See [:material-code-braces: UpdateShareInvitationOutputTypeDef](./type_defs.md#updateshareinvitationoutputtypedef) 


```python
# update_share_invitation method usage example with argument unpacking

kwargs: UpdateShareInvitationInputRequestTypeDef = {  # (1)
    "ShareInvitationId": ...,
    "ShareInvitationAction": ...,
}

parent.update_share_invitation(**kwargs)
```

1. See [:material-code-braces: UpdateShareInvitationInputRequestTypeDef](./type_defs.md#updateshareinvitationinputrequesttypedef) 

### update\_workload

Update an existing workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)

```python
# update_workload method definition

await def update_workload(
    self,
    *,
    WorkloadId: str,
    WorkloadName: str = ...,
    Description: str = ...,
    Environment: WorkloadEnvironmentType = ...,  # (1)
    AccountIds: Sequence[str] = ...,
    AwsRegions: Sequence[str] = ...,
    NonAwsRegions: Sequence[str] = ...,
    PillarPriorities: Sequence[str] = ...,
    ArchitecturalDesign: str = ...,
    ReviewOwner: str = ...,
    IsReviewOwnerUpdateAcknowledged: bool = ...,
    IndustryType: str = ...,
    Industry: str = ...,
    Notes: str = ...,
    ImprovementStatus: WorkloadImprovementStatusType = ...,  # (2)
    DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,  # (3)
    Applications: Sequence[str] = ...,
    JiraConfiguration: WorkloadJiraConfigurationInputTypeDef = ...,  # (4)
) -> UpdateWorkloadOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: WorkloadEnvironmentType](./literals.md#workloadenvironmenttype) 
2. See [:material-code-brackets: WorkloadImprovementStatusType](./literals.md#workloadimprovementstatustype) 
3. See [:material-code-braces: WorkloadDiscoveryConfigTypeDef](./type_defs.md#workloaddiscoveryconfigtypedef) 
4. See [:material-code-braces: WorkloadJiraConfigurationInputTypeDef](./type_defs.md#workloadjiraconfigurationinputtypedef) 
5. See [:material-code-braces: UpdateWorkloadOutputTypeDef](./type_defs.md#updateworkloadoutputtypedef) 


```python
# update_workload method usage example with argument unpacking

kwargs: UpdateWorkloadInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
}

parent.update_workload(**kwargs)
```

1. See [:material-code-braces: UpdateWorkloadInputRequestTypeDef](./type_defs.md#updateworkloadinputrequesttypedef) 

### update\_workload\_share

Update a workload share.

Type annotations and code completion for `#!python session.create_client("wellarchitected").update_workload_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload_share)

```python
# update_workload_share method definition

await def update_workload_share(
    self,
    *,
    ShareId: str,
    WorkloadId: str,
    PermissionType: PermissionTypeType,  # (1)
) -> UpdateWorkloadShareOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: UpdateWorkloadShareOutputTypeDef](./type_defs.md#updateworkloadshareoutputtypedef) 


```python
# update_workload_share method usage example with argument unpacking

kwargs: UpdateWorkloadShareInputRequestTypeDef = {  # (1)
    "ShareId": ...,
    "WorkloadId": ...,
    "PermissionType": ...,
}

parent.update_workload_share(**kwargs)
```

1. See [:material-code-braces: UpdateWorkloadShareInputRequestTypeDef](./type_defs.md#updateworkloadshareinputrequesttypedef) 

### upgrade\_lens\_review

Upgrade lens review for a particular workload.

Type annotations and code completion for `#!python session.create_client("wellarchitected").upgrade_lens_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_lens_review)

```python
# upgrade_lens_review method definition

await def upgrade_lens_review(
    self,
    *,
    WorkloadId: str,
    LensAlias: str,
    MilestoneName: str,
    ClientRequestToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# upgrade_lens_review method usage example with argument unpacking

kwargs: UpgradeLensReviewInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "LensAlias": ...,
    "MilestoneName": ...,
}

parent.upgrade_lens_review(**kwargs)
```

1. See [:material-code-braces: UpgradeLensReviewInputRequestTypeDef](./type_defs.md#upgradelensreviewinputrequesttypedef) 

### upgrade\_profile\_version

Upgrade a profile.

Type annotations and code completion for `#!python session.create_client("wellarchitected").upgrade_profile_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)

```python
# upgrade_profile_version method definition

await def upgrade_profile_version(
    self,
    *,
    WorkloadId: str,
    ProfileArn: str,
    MilestoneName: str = ...,
    ClientRequestToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# upgrade_profile_version method usage example with argument unpacking

kwargs: UpgradeProfileVersionInputRequestTypeDef = {  # (1)
    "WorkloadId": ...,
    "ProfileArn": ...,
}

parent.upgrade_profile_version(**kwargs)
```

1. See [:material-code-braces: UpgradeProfileVersionInputRequestTypeDef](./type_defs.md#upgradeprofileversioninputrequesttypedef) 

### upgrade\_review\_template\_lens\_review

Upgrade the lens review of a review template.

Type annotations and code completion for `#!python session.create_client("wellarchitected").upgrade_review_template_lens_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_review_template_lens_review)

```python
# upgrade_review_template_lens_review method definition

await def upgrade_review_template_lens_review(
    self,
    *,
    TemplateArn: str,
    LensAlias: str,
    ClientRequestToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# upgrade_review_template_lens_review method usage example with argument unpacking

kwargs: UpgradeReviewTemplateLensReviewInputRequestTypeDef = {  # (1)
    "TemplateArn": ...,
    "LensAlias": ...,
}

parent.upgrade_review_template_lens_review(**kwargs)
```

1. See [:material-code-braces: UpgradeReviewTemplateLensReviewInputRequestTypeDef](./type_defs.md#upgradereviewtemplatelensreviewinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("wellarchitected").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "WellArchitectedClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("wellarchitected").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.__aexit__)

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





