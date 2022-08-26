# CodeStar module

> [Index](../README.md) > CodeStar


!!! note ""

    Auto-generated documentation for [CodeStar](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
    type annotations stubs module [types-aiobotocore-codestar](https://pypi.org/project/types-aiobotocore-codestar/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `CodeStar` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[codestar]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[codestar]'


# standalone installation
python -m pip install types-aiobotocore-codestar
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codestar
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeStarClient

Type annotations and code completion for  `#!python session.create_client("codestar")` as [CodeStarClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codestar.client import CodeStarClient


session = get_session()
async with session.create_client("codestar") as client:
    client: CodeStarClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("codestar").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_codestar.paginator import ListProjectsPaginator

def get_list_projects_paginator() -> ListProjectsPaginator:
    return client.get_paginator("list_projects"))
```

- [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- [ListResourcesPaginator](./paginators.md#listresourcespaginator)
- [ListTeamMembersPaginator](./paginators.md#listteammemberspaginator)
- [ListUserProfilesPaginator](./paginators.md#listuserprofilespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_codestar.literals import ListProjectsPaginatorName

def get_value() -> ListProjectsPaginatorName:
    return "list_projects"
```

- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [ListResourcesPaginatorName](./literals.md#listresourcespaginatorname)
- [ListTeamMembersPaginatorName](./literals.md#listteammemberspaginatorname)
- [ListUserProfilesPaginatorName](./literals.md#listuserprofilespaginatorname)
- [CodeStarServiceName](./literals.md#codestarservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_codestar.type_defs import AssociateTeamMemberRequestRequestTypeDef

def get_value() -> AssociateTeamMemberRequestRequestTypeDef:
    return {
        "projectId": ...,
        "userArn": ...,
        "projectRole": ...,
    }
```

- [AssociateTeamMemberRequestRequestTypeDef](./type_defs.md#associateteammemberrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CodeCommitCodeDestinationTypeDef](./type_defs.md#codecommitcodedestinationtypedef)
- [GitHubCodeDestinationTypeDef](./type_defs.md#githubcodedestinationtypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [CreateUserProfileRequestRequestTypeDef](./type_defs.md#createuserprofilerequestrequesttypedef)
- [DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef)
- [DeleteUserProfileRequestRequestTypeDef](./type_defs.md#deleteuserprofilerequestrequesttypedef)
- [DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef)
- [ProjectStatusTypeDef](./type_defs.md#projectstatustypedef)
- [DescribeUserProfileRequestRequestTypeDef](./type_defs.md#describeuserprofilerequestrequesttypedef)
- [DisassociateTeamMemberRequestRequestTypeDef](./type_defs.md#disassociateteammemberrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef)
- [ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)
- [ListResourcesRequestRequestTypeDef](./type_defs.md#listresourcesrequestrequesttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [ListTagsForProjectRequestRequestTypeDef](./type_defs.md#listtagsforprojectrequestrequesttypedef)
- [ListTeamMembersRequestRequestTypeDef](./type_defs.md#listteammembersrequestrequesttypedef)
- [TeamMemberTypeDef](./type_defs.md#teammembertypedef)
- [ListUserProfilesRequestRequestTypeDef](./type_defs.md#listuserprofilesrequestrequesttypedef)
- [UserProfileSummaryTypeDef](./type_defs.md#userprofilesummarytypedef)
- [TagProjectRequestRequestTypeDef](./type_defs.md#tagprojectrequestrequesttypedef)
- [UntagProjectRequestRequestTypeDef](./type_defs.md#untagprojectrequestrequesttypedef)
- [UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef)
- [UpdateTeamMemberRequestRequestTypeDef](./type_defs.md#updateteammemberrequestrequesttypedef)
- [UpdateUserProfileRequestRequestTypeDef](./type_defs.md#updateuserprofilerequestrequesttypedef)
- [AssociateTeamMemberResultTypeDef](./type_defs.md#associateteammemberresulttypedef)
- [CreateProjectResultTypeDef](./type_defs.md#createprojectresulttypedef)
- [CreateUserProfileResultTypeDef](./type_defs.md#createuserprofileresulttypedef)
- [DeleteProjectResultTypeDef](./type_defs.md#deleteprojectresulttypedef)
- [DeleteUserProfileResultTypeDef](./type_defs.md#deleteuserprofileresulttypedef)
- [DescribeUserProfileResultTypeDef](./type_defs.md#describeuserprofileresulttypedef)
- [ListTagsForProjectResultTypeDef](./type_defs.md#listtagsforprojectresulttypedef)
- [TagProjectResultTypeDef](./type_defs.md#tagprojectresulttypedef)
- [UpdateTeamMemberResultTypeDef](./type_defs.md#updateteammemberresulttypedef)
- [UpdateUserProfileResultTypeDef](./type_defs.md#updateuserprofileresulttypedef)
- [CodeDestinationTypeDef](./type_defs.md#codedestinationtypedef)
- [CodeSourceTypeDef](./type_defs.md#codesourcetypedef)
- [ToolchainSourceTypeDef](./type_defs.md#toolchainsourcetypedef)
- [DescribeProjectResultTypeDef](./type_defs.md#describeprojectresulttypedef)
- [ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef)
- [ListResourcesRequestListResourcesPaginateTypeDef](./type_defs.md#listresourcesrequestlistresourcespaginatetypedef)
- [ListTeamMembersRequestListTeamMembersPaginateTypeDef](./type_defs.md#listteammembersrequestlistteammemberspaginatetypedef)
- [ListUserProfilesRequestListUserProfilesPaginateTypeDef](./type_defs.md#listuserprofilesrequestlistuserprofilespaginatetypedef)
- [ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef)
- [ListResourcesResultTypeDef](./type_defs.md#listresourcesresulttypedef)
- [ListTeamMembersResultTypeDef](./type_defs.md#listteammembersresulttypedef)
- [ListUserProfilesResultTypeDef](./type_defs.md#listuserprofilesresulttypedef)
- [CodeTypeDef](./type_defs.md#codetypedef)
- [ToolchainTypeDef](./type_defs.md#toolchaintypedef)
- [CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef)

