# CodeConnections module

> [Index](../README.md) > CodeConnections


!!! note ""

    Auto-generated documentation for [CodeConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#codeconnections)
    type annotations stubs module [types-aiobotocore-codeconnections](https://pypi.org/project/types-aiobotocore-codeconnections/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
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
- [RepositoryLinkInfoTypeDef](./type_defs.md#repositorylinkinfotypedef)
- [CreateSyncConfigurationInputTypeDef](./type_defs.md#createsyncconfigurationinputtypedef)
- [SyncConfigurationTypeDef](./type_defs.md#syncconfigurationtypedef)
- [DeleteConnectionInputTypeDef](./type_defs.md#deleteconnectioninputtypedef)
- [DeleteHostInputTypeDef](./type_defs.md#deletehostinputtypedef)
- [DeleteRepositoryLinkInputTypeDef](./type_defs.md#deleterepositorylinkinputtypedef)
- [DeleteSyncConfigurationInputTypeDef](./type_defs.md#deletesyncconfigurationinputtypedef)
- [GetConnectionInputTypeDef](./type_defs.md#getconnectioninputtypedef)
- [GetHostInputTypeDef](./type_defs.md#gethostinputtypedef)
- [VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef)
- [GetRepositoryLinkInputTypeDef](./type_defs.md#getrepositorylinkinputtypedef)
- [GetRepositorySyncStatusInputTypeDef](./type_defs.md#getrepositorysyncstatusinputtypedef)
- [GetResourceSyncStatusInputTypeDef](./type_defs.md#getresourcesyncstatusinputtypedef)
- [RevisionTypeDef](./type_defs.md#revisiontypedef)
- [GetSyncBlockerSummaryInputTypeDef](./type_defs.md#getsyncblockersummaryinputtypedef)
- [GetSyncConfigurationInputTypeDef](./type_defs.md#getsyncconfigurationinputtypedef)
- [ListConnectionsInputTypeDef](./type_defs.md#listconnectionsinputtypedef)
- [ListHostsInputTypeDef](./type_defs.md#listhostsinputtypedef)
- [ListRepositoryLinksInputTypeDef](./type_defs.md#listrepositorylinksinputtypedef)
- [ListRepositorySyncDefinitionsInputTypeDef](./type_defs.md#listrepositorysyncdefinitionsinputtypedef)
- [RepositorySyncDefinitionTypeDef](./type_defs.md#repositorysyncdefinitiontypedef)
- [ListSyncConfigurationsInputTypeDef](./type_defs.md#listsyncconfigurationsinputtypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [RepositorySyncEventTypeDef](./type_defs.md#repositorysynceventtypedef)
- [ResourceSyncEventTypeDef](./type_defs.md#resourcesynceventtypedef)
- [SyncBlockerContextTypeDef](./type_defs.md#syncblockercontexttypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateRepositoryLinkInputTypeDef](./type_defs.md#updaterepositorylinkinputtypedef)
- [UpdateSyncBlockerInputTypeDef](./type_defs.md#updatesyncblockerinputtypedef)
- [UpdateSyncConfigurationInputTypeDef](./type_defs.md#updatesyncconfigurationinputtypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [CreateConnectionInputTypeDef](./type_defs.md#createconnectioninputtypedef)
- [CreateRepositoryLinkInputTypeDef](./type_defs.md#createrepositorylinkinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef)
- [CreateHostOutputTypeDef](./type_defs.md#createhostoutputtypedef)
- [GetConnectionOutputTypeDef](./type_defs.md#getconnectionoutputtypedef)
- [ListConnectionsOutputTypeDef](./type_defs.md#listconnectionsoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
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
- [VpcConfigurationUnionTypeDef](./type_defs.md#vpcconfigurationuniontypedef)
- [ListHostsOutputTypeDef](./type_defs.md#listhostsoutputtypedef)
- [GetRepositorySyncStatusOutputTypeDef](./type_defs.md#getrepositorysyncstatusoutputtypedef)
- [GetResourceSyncStatusOutputTypeDef](./type_defs.md#getresourcesyncstatusoutputtypedef)
- [SyncBlockerSummaryTypeDef](./type_defs.md#syncblockersummarytypedef)
- [UpdateSyncBlockerOutputTypeDef](./type_defs.md#updatesyncblockeroutputtypedef)
- [CreateHostInputTypeDef](./type_defs.md#createhostinputtypedef)
- [UpdateHostInputTypeDef](./type_defs.md#updatehostinputtypedef)
- [GetSyncBlockerSummaryOutputTypeDef](./type_defs.md#getsyncblockersummaryoutputtypedef)

