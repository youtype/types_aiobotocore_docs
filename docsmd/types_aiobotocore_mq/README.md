# MQ module

> [Index](../README.md) > MQ


!!! note ""

    Auto-generated documentation for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#mq)
    type annotations stubs module [types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MQ` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MQ` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mq]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mq]'

# standalone installation
python -m pip install types-aiobotocore-mq
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mq
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MQClient

Type annotations and code completion for  `#!python session.create_client("mq")` as [MQClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client)

```python
# MQClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_mq.client import MQClient


session = get_session()
async with session.create_client("mq") as client:
    client: MQClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mq").get_paginator("...")`.

```python
# ListBrokersPaginator usage example

from types_aiobotocore_mq.paginator import ListBrokersPaginator

def get_list_brokers_paginator() -> ListBrokersPaginator:
    return client.get_paginator("list_brokers"))
```

- [ListBrokersPaginator](./paginators.md#listbrokerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuthenticationStrategyType usage example

from types_aiobotocore_mq.literals import AuthenticationStrategyType

def get_value() -> AuthenticationStrategyType:
    return "CONFIG_MANAGED"
```

- [AuthenticationStrategyType](./literals.md#authenticationstrategytype)
- [BrokerStateType](./literals.md#brokerstatetype)
- [BrokerStorageTypeType](./literals.md#brokerstoragetypetype)
- [ChangeTypeType](./literals.md#changetypetype)
- [DataReplicationModeType](./literals.md#datareplicationmodetype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [DeploymentModeType](./literals.md#deploymentmodetype)
- [EngineTypeType](./literals.md#enginetypetype)
- [ListBrokersPaginatorName](./literals.md#listbrokerspaginatorname)
- [PromoteModeType](./literals.md#promotemodetype)
- [SanitizationWarningReasonType](./literals.md#sanitizationwarningreasontype)
- [MQServiceName](./literals.md#mqservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionRequiredTypeDef](./type_defs.md#actionrequiredtypedef)
- [AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef)
- [EngineVersionTypeDef](./type_defs.md#engineversiontypedef)
- [BrokerInstanceTypeDef](./type_defs.md#brokerinstancetypedef)
- [BrokerSummaryTypeDef](./type_defs.md#brokersummarytypedef)
- [ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef)
- [ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef)
- [EncryptionOptionsTypeDef](./type_defs.md#encryptionoptionstypedef)
- [LdapServerMetadataInputTypeDef](./type_defs.md#ldapservermetadatainputtypedef)
- [LogsTypeDef](./type_defs.md#logstypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateConfigurationRequestTypeDef](./type_defs.md#createconfigurationrequesttypedef)
- [CreateTagsRequestTypeDef](./type_defs.md#createtagsrequesttypedef)
- [CreateUserRequestTypeDef](./type_defs.md#createuserrequesttypedef)
- [DataReplicationCounterpartTypeDef](./type_defs.md#datareplicationcounterparttypedef)
- [DeleteBrokerRequestTypeDef](./type_defs.md#deletebrokerrequesttypedef)
- [DeleteConfigurationRequestTypeDef](./type_defs.md#deleteconfigurationrequesttypedef)
- [DeleteTagsRequestTypeDef](./type_defs.md#deletetagsrequesttypedef)
- [DeleteUserRequestTypeDef](./type_defs.md#deleteuserrequesttypedef)
- [DescribeBrokerEngineTypesRequestTypeDef](./type_defs.md#describebrokerenginetypesrequesttypedef)
- [DescribeBrokerInstanceOptionsRequestTypeDef](./type_defs.md#describebrokerinstanceoptionsrequesttypedef)
- [DescribeBrokerRequestTypeDef](./type_defs.md#describebrokerrequesttypedef)
- [LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef)
- [UserSummaryTypeDef](./type_defs.md#usersummarytypedef)
- [DescribeConfigurationRequestTypeDef](./type_defs.md#describeconfigurationrequesttypedef)
- [DescribeConfigurationRevisionRequestTypeDef](./type_defs.md#describeconfigurationrevisionrequesttypedef)
- [DescribeUserRequestTypeDef](./type_defs.md#describeuserrequesttypedef)
- [UserPendingChangesTypeDef](./type_defs.md#userpendingchangestypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBrokersRequestTypeDef](./type_defs.md#listbrokersrequesttypedef)
- [ListConfigurationRevisionsRequestTypeDef](./type_defs.md#listconfigurationrevisionsrequesttypedef)
- [ListConfigurationsRequestTypeDef](./type_defs.md#listconfigurationsrequesttypedef)
- [ListTagsRequestTypeDef](./type_defs.md#listtagsrequesttypedef)
- [ListUsersRequestTypeDef](./type_defs.md#listusersrequesttypedef)
- [PendingLogsTypeDef](./type_defs.md#pendinglogstypedef)
- [PromoteRequestTypeDef](./type_defs.md#promoterequesttypedef)
- [RebootBrokerRequestTypeDef](./type_defs.md#rebootbrokerrequesttypedef)
- [SanitizationWarningTypeDef](./type_defs.md#sanitizationwarningtypedef)
- [UpdateConfigurationRequestTypeDef](./type_defs.md#updateconfigurationrequesttypedef)
- [UpdateUserRequestTypeDef](./type_defs.md#updateuserrequesttypedef)
- [BrokerInstanceOptionTypeDef](./type_defs.md#brokerinstanceoptiontypedef)
- [BrokerEngineTypeTypeDef](./type_defs.md#brokerenginetypetypedef)
- [ConfigurationsTypeDef](./type_defs.md#configurationstypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [CreateBrokerRequestTypeDef](./type_defs.md#createbrokerrequesttypedef)
- [UpdateBrokerRequestTypeDef](./type_defs.md#updatebrokerrequesttypedef)
- [CreateBrokerResponseTypeDef](./type_defs.md#createbrokerresponsetypedef)
- [CreateConfigurationResponseTypeDef](./type_defs.md#createconfigurationresponsetypedef)
- [DeleteBrokerResponseTypeDef](./type_defs.md#deletebrokerresponsetypedef)
- [DeleteConfigurationResponseTypeDef](./type_defs.md#deleteconfigurationresponsetypedef)
- [DescribeConfigurationResponseTypeDef](./type_defs.md#describeconfigurationresponsetypedef)
- [DescribeConfigurationRevisionResponseTypeDef](./type_defs.md#describeconfigurationrevisionresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef)
- [ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [PromoteResponseTypeDef](./type_defs.md#promoteresponsetypedef)
- [DataReplicationMetadataOutputTypeDef](./type_defs.md#datareplicationmetadataoutputtypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [ListBrokersRequestPaginateTypeDef](./type_defs.md#listbrokersrequestpaginatetypedef)
- [LogsSummaryTypeDef](./type_defs.md#logssummarytypedef)
- [UpdateConfigurationResponseTypeDef](./type_defs.md#updateconfigurationresponsetypedef)
- [DescribeBrokerInstanceOptionsResponseTypeDef](./type_defs.md#describebrokerinstanceoptionsresponsetypedef)
- [DescribeBrokerEngineTypesResponseTypeDef](./type_defs.md#describebrokerenginetypesresponsetypedef)
- [ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef)
- [UpdateBrokerResponseTypeDef](./type_defs.md#updatebrokerresponsetypedef)
- [DescribeBrokerResponseTypeDef](./type_defs.md#describebrokerresponsetypedef)

