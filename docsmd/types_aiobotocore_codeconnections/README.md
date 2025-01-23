# CodeConnections module

> [Index](../README.md) > CodeConnections


!!! note ""

    Auto-generated documentation for [CodeConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#codeconnections)
    type annotations stubs module [types-aiobotocore-codeconnections](https://pypi.org/project/types-aiobotocore-codeconnections/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CodeConnections` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CodeConnections` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[codeconnections]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[codeconnections]'

# standalone installation
python -m pip install types-aiobotocore-codeconnections
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codeconnections
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeConnectionsClient

Type annotations and code completion for  `#!python session.create_client("codeconnections")` as [CodeConnectionsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#CodeConnections.Client)

```python
# CodeConnectionsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_codeconnections.client import CodeConnectionsClient


session = get_session()
async with session.create_client("codeconnections") as client:
    client: CodeConnectionsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BlockerStatusType usage example

from types_aiobotocore_codeconnections.literals import BlockerStatusType

def get_value() -> BlockerStatusType:
    return "ACTIVE"
```

- [BlockerStatusType](./literals.md#blockerstatustype)
- [BlockerTypeType](./literals.md#blockertypetype)
- [ConnectionStatusType](./literals.md#connectionstatustype)
- [ProviderTypeType](./literals.md#providertypetype)
- [PublishDeploymentStatusType](./literals.md#publishdeploymentstatustype)
- [PullRequestCommentType](./literals.md#pullrequestcommenttype)
- [RepositorySyncStatusType](./literals.md#repositorysyncstatustype)
- [ResourceSyncStatusType](./literals.md#resourcesyncstatustype)
- [SyncConfigurationTypeType](./literals.md#syncconfigurationtypetype)
- [TriggerResourceUpdateOnType](./literals.md#triggerresourceupdateontype)
- [CodeConnectionsServiceName](./literals.md#codeconnectionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ConnectionTypeDef](./type_defs.md#connectiontypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [RepositoryLinkInfoTypeDef](./type_defs.md#repositorylinkinfotypedef)
- [CreateSyncConfigurationInputRequestTypeDef](./type_defs.md#createsyncconfigurationinputrequesttypedef)
- [SyncConfigurationTypeDef](./type_defs.md#syncconfigurationtypedef)
- [DeleteConnectionInputRequestTypeDef](./type_defs.md#deleteconnectioninputrequesttypedef)
- [DeleteHostInputRequestTypeDef](./type_defs.md#deletehostinputrequesttypedef)
- [DeleteRepositoryLinkInputRequestTypeDef](./type_defs.md#deleterepositorylinkinputrequesttypedef)
- [DeleteSyncConfigurationInputRequestTypeDef](./type_defs.md#deletesyncconfigurationinputrequesttypedef)
- [GetConnectionInputRequestTypeDef](./type_defs.md#getconnectioninputrequesttypedef)
- [GetHostInputRequestTypeDef](./type_defs.md#gethostinputrequesttypedef)
- [VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef)
- [GetRepositoryLinkInputRequestTypeDef](./type_defs.md#getrepositorylinkinputrequesttypedef)
- [GetRepositorySyncStatusInputRequestTypeDef](./type_defs.md#getrepositorysyncstatusinputrequesttypedef)
- [GetResourceSyncStatusInputRequestTypeDef](./type_defs.md#getresourcesyncstatusinputrequesttypedef)
- [RevisionTypeDef](./type_defs.md#revisiontypedef)
- [GetSyncBlockerSummaryInputRequestTypeDef](./type_defs.md#getsyncblockersummaryinputrequesttypedef)
- [GetSyncConfigurationInputRequestTypeDef](./type_defs.md#getsyncconfigurationinputrequesttypedef)
- [ListConnectionsInputRequestTypeDef](./type_defs.md#listconnectionsinputrequesttypedef)
- [ListHostsInputRequestTypeDef](./type_defs.md#listhostsinputrequesttypedef)
- [ListRepositoryLinksInputRequestTypeDef](./type_defs.md#listrepositorylinksinputrequesttypedef)
- [ListRepositorySyncDefinitionsInputRequestTypeDef](./type_defs.md#listrepositorysyncdefinitionsinputrequesttypedef)
- [RepositorySyncDefinitionTypeDef](./type_defs.md#repositorysyncdefinitiontypedef)
- [ListSyncConfigurationsInputRequestTypeDef](./type_defs.md#listsyncconfigurationsinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [RepositorySyncEventTypeDef](./type_defs.md#repositorysynceventtypedef)
- [ResourceSyncEventTypeDef](./type_defs.md#resourcesynceventtypedef)
- [SyncBlockerContextTypeDef](./type_defs.md#syncblockercontexttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateRepositoryLinkInputRequestTypeDef](./type_defs.md#updaterepositorylinkinputrequesttypedef)
- [UpdateSyncBlockerInputRequestTypeDef](./type_defs.md#updatesyncblockerinputrequesttypedef)
- [UpdateSyncConfigurationInputRequestTypeDef](./type_defs.md#updatesyncconfigurationinputrequesttypedef)
- [CreateConnectionInputRequestTypeDef](./type_defs.md#createconnectioninputrequesttypedef)
- [CreateRepositoryLinkInputRequestTypeDef](./type_defs.md#createrepositorylinkinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef)
- [CreateHostOutputTypeDef](./type_defs.md#createhostoutputtypedef)
- [GetConnectionOutputTypeDef](./type_defs.md#getconnectionoutputtypedef)
- [ListConnectionsOutputTypeDef](./type_defs.md#listconnectionsoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [CreateHostInputRequestTypeDef](./type_defs.md#createhostinputrequesttypedef)
- [UpdateHostInputRequestTypeDef](./type_defs.md#updatehostinputrequesttypedef)
- [CreateRepositoryLinkOutputTypeDef](./type_defs.md#createrepositorylinkoutputtypedef)
- [GetRepositoryLinkOutputTypeDef](./type_defs.md#getrepositorylinkoutputtypedef)
- [ListRepositoryLinksOutputTypeDef](./type_defs.md#listrepositorylinksoutputtypedef)
- [UpdateRepositoryLinkOutputTypeDef](./type_defs.md#updaterepositorylinkoutputtypedef)
- [CreateSyncConfigurationOutputTypeDef](./type_defs.md#createsyncconfigurationoutputtypedef)
- [GetSyncConfigurationOutputTypeDef](./type_defs.md#getsyncconfigurationoutputtypedef)
- [ListSyncConfigurationsOutputTypeDef](./type_defs.md#listsyncconfigurationsoutputtypedef)
- [UpdateSyncConfigurationOutputTypeDef](./type_defs.md#updatesyncconfigurationoutputtypedef)
- [GetHostOutputTypeDef](./type_defs.md#gethostoutputtypedef)
- [HostTypeDef](./type_defs.md#hosttypedef)
- [ListRepositorySyncDefinitionsOutputTypeDef](./type_defs.md#listrepositorysyncdefinitionsoutputtypedef)
- [RepositorySyncAttemptTypeDef](./type_defs.md#repositorysyncattempttypedef)
- [ResourceSyncAttemptTypeDef](./type_defs.md#resourcesyncattempttypedef)
- [SyncBlockerTypeDef](./type_defs.md#syncblockertypedef)
- [ListHostsOutputTypeDef](./type_defs.md#listhostsoutputtypedef)
- [GetRepositorySyncStatusOutputTypeDef](./type_defs.md#getrepositorysyncstatusoutputtypedef)
- [GetResourceSyncStatusOutputTypeDef](./type_defs.md#getresourcesyncstatusoutputtypedef)
- [SyncBlockerSummaryTypeDef](./type_defs.md#syncblockersummarytypedef)
- [UpdateSyncBlockerOutputTypeDef](./type_defs.md#updatesyncblockeroutputtypedef)
- [GetSyncBlockerSummaryOutputTypeDef](./type_defs.md#getsyncblockersummaryoutputtypedef)

