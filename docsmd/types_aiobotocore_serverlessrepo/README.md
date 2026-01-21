# ServerlessApplicationRepository module

> [Index](../README.md) > ServerlessApplicationRepository


!!! note ""

    Auto-generated documentation for [ServerlessApplicationRepository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#serverlessapplicationrepository)
    type annotations stubs module [types-aiobotocore-serverlessrepo](https://pypi.org/project/types-aiobotocore-serverlessrepo/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ServerlessApplicationRepository` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ServerlessApplicationRepository` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[serverlessrepo]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[serverlessrepo]'

# standalone installation
python -m pip install types-aiobotocore-serverlessrepo
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-serverlessrepo
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ServerlessApplicationRepositoryClient

Type annotations and code completion for  `#!python session.create_client("serverlessrepo")` as [ServerlessApplicationRepositoryClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client)

```python
# ServerlessApplicationRepositoryClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_serverlessrepo.client import ServerlessApplicationRepositoryClient


session = get_session()
async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("serverlessrepo").get_paginator("...")`.

```python
# ListApplicationDependenciesPaginator usage example

from types_aiobotocore_serverlessrepo.paginator import ListApplicationDependenciesPaginator

def get_list_application_dependencies_paginator() -> ListApplicationDependenciesPaginator:
    return client.get_paginator("list_application_dependencies"))
```

- [ListApplicationDependenciesPaginator](./paginators.md#listapplicationdependenciespaginator)
- [ListApplicationVersionsPaginator](./paginators.md#listapplicationversionspaginator)
- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CapabilityType usage example

from types_aiobotocore_serverlessrepo.literals import CapabilityType

def get_value() -> CapabilityType:
    return "CAPABILITY_AUTO_EXPAND"
```

- [CapabilityType](./literals.md#capabilitytype)
- [ListApplicationDependenciesPaginatorName](./literals.md#listapplicationdependenciespaginatorname)
- [ListApplicationVersionsPaginatorName](./literals.md#listapplicationversionspaginatorname)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [StatusType](./literals.md#statustype)
- [ServerlessApplicationRepositoryServiceName](./literals.md#serverlessapplicationrepositoryservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ApplicationDependencySummaryTypeDef](./type_defs.md#applicationdependencysummarytypedef)
- [ApplicationPolicyStatementOutputTypeDef](./type_defs.md#applicationpolicystatementoutputtypedef)
- [ApplicationPolicyStatementTypeDef](./type_defs.md#applicationpolicystatementtypedef)
- [ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef)
- [CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateApplicationVersionRequestTypeDef](./type_defs.md#createapplicationversionrequesttypedef)
- [ParameterDefinitionTypeDef](./type_defs.md#parameterdefinitiontypedef)
- [ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateCloudFormationTemplateRequestTypeDef](./type_defs.md#createcloudformationtemplaterequesttypedef)
- [DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)
- [GetApplicationPolicyRequestTypeDef](./type_defs.md#getapplicationpolicyrequesttypedef)
- [GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef)
- [GetCloudFormationTemplateRequestTypeDef](./type_defs.md#getcloudformationtemplaterequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApplicationDependenciesRequestTypeDef](./type_defs.md#listapplicationdependenciesrequesttypedef)
- [ListApplicationVersionsRequestTypeDef](./type_defs.md#listapplicationversionsrequesttypedef)
- [VersionSummaryTypeDef](./type_defs.md#versionsummarytypedef)
- [ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)
- [RollbackTriggerTypeDef](./type_defs.md#rollbacktriggertypedef)
- [UnshareApplicationRequestTypeDef](./type_defs.md#unshareapplicationrequesttypedef)
- [UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)
- [ApplicationPolicyStatementUnionTypeDef](./type_defs.md#applicationpolicystatementuniontypedef)
- [CreateCloudFormationChangeSetResponseTypeDef](./type_defs.md#createcloudformationchangesetresponsetypedef)
- [CreateCloudFormationTemplateResponseTypeDef](./type_defs.md#createcloudformationtemplateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetApplicationPolicyResponseTypeDef](./type_defs.md#getapplicationpolicyresponsetypedef)
- [GetCloudFormationTemplateResponseTypeDef](./type_defs.md#getcloudformationtemplateresponsetypedef)
- [ListApplicationDependenciesResponseTypeDef](./type_defs.md#listapplicationdependenciesresponsetypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [PutApplicationPolicyResponseTypeDef](./type_defs.md#putapplicationpolicyresponsetypedef)
- [CreateApplicationVersionResponseTypeDef](./type_defs.md#createapplicationversionresponsetypedef)
- [VersionTypeDef](./type_defs.md#versiontypedef)
- [ListApplicationDependenciesRequestPaginateTypeDef](./type_defs.md#listapplicationdependenciesrequestpaginatetypedef)
- [ListApplicationVersionsRequestPaginateTypeDef](./type_defs.md#listapplicationversionsrequestpaginatetypedef)
- [ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef)
- [ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef)
- [RollbackConfigurationTypeDef](./type_defs.md#rollbackconfigurationtypedef)
- [PutApplicationPolicyRequestTypeDef](./type_defs.md#putapplicationpolicyrequesttypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)
- [UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef)
- [CreateCloudFormationChangeSetRequestTypeDef](./type_defs.md#createcloudformationchangesetrequesttypedef)

