# MQ module

> [Index](../README.md) > MQ


!!! note ""

    Auto-generated documentation for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
    type annotations stubs module [types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

## How to install



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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_mq.paginator import ListBrokersPaginator

def get_list_brokers_paginator() -> ListBrokersPaginator:
    return client.get_paginator("list_brokers"))
```

- [ListBrokersPaginator](./paginators.md#listbrokerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mq.literals import AuthenticationStrategyType

def get_value() -> AuthenticationStrategyType:
    return "LDAP"
```

- [AuthenticationStrategyType](./literals.md#authenticationstrategytype)
- [BrokerStateType](./literals.md#brokerstatetype)
- [BrokerStorageTypeType](./literals.md#brokerstoragetypetype)
- [ChangeTypeType](./literals.md#changetypetype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [DeploymentModeType](./literals.md#deploymentmodetype)
- [EngineTypeType](./literals.md#enginetypetype)
- [ListBrokersPaginatorName](./literals.md#listbrokerspaginatorname)
- [SanitizationWarningReasonType](./literals.md#sanitizationwarningreasontype)
- [MQServiceName](./literals.md#mqservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mq.type_defs import ActionRequiredTypeDef

def get_value() -> ActionRequiredTypeDef:
    return {
        "ActionRequiredCode": ...,
    }
```

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
- [CreateConfigurationRequestRequestTypeDef](./type_defs.md#createconfigurationrequestrequesttypedef)
- [CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [DeleteBrokerRequestRequestTypeDef](./type_defs.md#deletebrokerrequestrequesttypedef)
- [DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DescribeBrokerEngineTypesRequestRequestTypeDef](./type_defs.md#describebrokerenginetypesrequestrequesttypedef)
- [DescribeBrokerInstanceOptionsRequestRequestTypeDef](./type_defs.md#describebrokerinstanceoptionsrequestrequesttypedef)
- [DescribeBrokerRequestRequestTypeDef](./type_defs.md#describebrokerrequestrequesttypedef)
- [LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef)
- [UserSummaryTypeDef](./type_defs.md#usersummarytypedef)
- [DescribeConfigurationRequestRequestTypeDef](./type_defs.md#describeconfigurationrequestrequesttypedef)
- [DescribeConfigurationRevisionRequestRequestTypeDef](./type_defs.md#describeconfigurationrevisionrequestrequesttypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [UserPendingChangesTypeDef](./type_defs.md#userpendingchangestypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBrokersRequestRequestTypeDef](./type_defs.md#listbrokersrequestrequesttypedef)
- [ListConfigurationRevisionsRequestRequestTypeDef](./type_defs.md#listconfigurationrevisionsrequestrequesttypedef)
- [ListConfigurationsRequestRequestTypeDef](./type_defs.md#listconfigurationsrequestrequesttypedef)
- [ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [PendingLogsTypeDef](./type_defs.md#pendinglogstypedef)
- [RebootBrokerRequestRequestTypeDef](./type_defs.md#rebootbrokerrequestrequesttypedef)
- [SanitizationWarningTypeDef](./type_defs.md#sanitizationwarningtypedef)
- [UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [BrokerInstanceOptionTypeDef](./type_defs.md#brokerinstanceoptiontypedef)
- [BrokerEngineTypeTypeDef](./type_defs.md#brokerenginetypetypedef)
- [ConfigurationsTypeDef](./type_defs.md#configurationstypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [CreateBrokerRequestRequestTypeDef](./type_defs.md#createbrokerrequestrequesttypedef)
- [UpdateBrokerRequestRequestTypeDef](./type_defs.md#updatebrokerrequestrequesttypedef)
- [CreateBrokerResponseTypeDef](./type_defs.md#createbrokerresponsetypedef)
- [CreateConfigurationResponseTypeDef](./type_defs.md#createconfigurationresponsetypedef)
- [DeleteBrokerResponseTypeDef](./type_defs.md#deletebrokerresponsetypedef)
- [DescribeConfigurationResponseTypeDef](./type_defs.md#describeconfigurationresponsetypedef)
- [DescribeConfigurationRevisionResponseTypeDef](./type_defs.md#describeconfigurationrevisionresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef)
- [ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [UpdateBrokerResponseTypeDef](./type_defs.md#updatebrokerresponsetypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [ListBrokersRequestListBrokersPaginateTypeDef](./type_defs.md#listbrokersrequestlistbrokerspaginatetypedef)
- [LogsSummaryTypeDef](./type_defs.md#logssummarytypedef)
- [UpdateConfigurationResponseTypeDef](./type_defs.md#updateconfigurationresponsetypedef)
- [DescribeBrokerInstanceOptionsResponseTypeDef](./type_defs.md#describebrokerinstanceoptionsresponsetypedef)
- [DescribeBrokerEngineTypesResponseTypeDef](./type_defs.md#describebrokerenginetypesresponsetypedef)
- [ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef)
- [DescribeBrokerResponseTypeDef](./type_defs.md#describebrokerresponsetypedef)

