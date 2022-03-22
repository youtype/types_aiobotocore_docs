<a id="mqclient-for-aiobotocore-mq-module"></a>

# MQClient for aiobotocore MQ module

> [Index](../README.md) > [MQ](./README.md) > MQClient

Auto-generated documentation for
[MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
type annotations stubs module
[types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

- [MQClient for aiobotocore MQ module](#mqclient-for-aiobotocore-mq-module)
  - [MQClient](#mqclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_broker](#create_broker)
    - [create_configuration](#create_configuration)
    - [create_tags](#create_tags)
    - [create_user](#create_user)
    - [delete_broker](#delete_broker)
    - [delete_tags](#delete_tags)
    - [delete_user](#delete_user)
    - [describe_broker](#describe_broker)
    - [describe_broker_engine_types](#describe_broker_engine_types)
    - [describe_broker_instance_options](#describe_broker_instance_options)
    - [describe_configuration](#describe_configuration)
    - [describe_configuration_revision](#describe_configuration_revision)
    - [describe_user](#describe_user)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_brokers](#list_brokers)
    - [list_configuration_revisions](#list_configuration_revisions)
    - [list_configurations](#list_configurations)
    - [list_tags](#list_tags)
    - [list_users](#list_users)
    - [reboot_broker](#reboot_broker)
    - [update_broker](#update_broker)
    - [update_configuration](#update_configuration)
    - [update_user](#update_user)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="mqclient"></a>

## MQClient

Type annotations for `session.create_client("mq")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_mq.client import MQClient

session = get_session()
async with session.create_client("mq") as client:
    client: MQClient
```

Boto3 documentation:
[MQ.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_mq.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.NotFoundException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MQClient exceptions.

Type annotations for `session.create_client("mq").exceptions` method.

Boto3 documentation:
[MQ.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("mq").can_paginate` method.

Boto3 documentation:
[MQ.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_broker"></a>

### create_broker

Creates a broker.

Type annotations for `session.create_client("mq").create_broker` method.

Boto3 documentation:
[MQ.Client.create_broker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_broker)

Asynchronous method. Use `await create_broker(...)` for a synchronous call.

Arguments mapping described in
[CreateBrokerRequestRequestTypeDef](./type_defs.md#createbrokerrequestrequesttypedef).

Keyword-only arguments:

- `AutoMinorVersionUpgrade`: `bool` *(required)*
- `BrokerName`: `str` *(required)*
- `DeploymentMode`: [DeploymentModeType](./literals.md#deploymentmodetype)
  *(required)*
- `EngineType`: [EngineTypeType](./literals.md#enginetypetype) *(required)*
- `EngineVersion`: `str` *(required)*
- `HostInstanceType`: `str` *(required)*
- `PubliclyAccessible`: `bool` *(required)*
- `Users`: `Sequence`\[[UserTypeDef](./type_defs.md#usertypedef)\] *(required)*
- `AuthenticationStrategy`:
  [AuthenticationStrategyType](./literals.md#authenticationstrategytype)
- `Configuration`:
  [ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef)
- `CreatorRequestId`: `str`
- `EncryptionOptions`:
  [EncryptionOptionsTypeDef](./type_defs.md#encryptionoptionstypedef)
- `LdapServerMetadata`:
  [LdapServerMetadataInputTypeDef](./type_defs.md#ldapservermetadatainputtypedef)
- `Logs`: [LogsTypeDef](./type_defs.md#logstypedef)
- `MaintenanceWindowStartTime`:
  [WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef)
- `SecurityGroups`: `Sequence`\[`str`\]
- `StorageType`: [BrokerStorageTypeType](./literals.md#brokerstoragetypetype)
- `SubnetIds`: `Sequence`\[`str`\]
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateBrokerResponseTypeDef](./type_defs.md#createbrokerresponsetypedef).

<a id="create\_configuration"></a>

### create_configuration

Creates a new configuration for the specified configuration name.

Type annotations for `session.create_client("mq").create_configuration` method.

Boto3 documentation:
[MQ.Client.create_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_configuration)

Asynchronous method. Use `await create_configuration(...)` for a synchronous
call.

Arguments mapping described in
[CreateConfigurationRequestRequestTypeDef](./type_defs.md#createconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `EngineType`: [EngineTypeType](./literals.md#enginetypetype) *(required)*
- `EngineVersion`: `str` *(required)*
- `Name`: `str` *(required)*
- `AuthenticationStrategy`:
  [AuthenticationStrategyType](./literals.md#authenticationstrategytype)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateConfigurationResponseTypeDef](./type_defs.md#createconfigurationresponsetypedef).

<a id="create\_tags"></a>

### create_tags

Add a tag to a resource.

Type annotations for `session.create_client("mq").create_tags` method.

Boto3 documentation:
[MQ.Client.create_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_tags)

Asynchronous method. Use `await create_tags(...)` for a synchronous call.

Arguments mapping described in
[CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\]

<a id="create\_user"></a>

### create_user

Creates an ActiveMQ user.

Type annotations for `session.create_client("mq").create_user` method.

Boto3 documentation:
[MQ.Client.create_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_user)

Asynchronous method. Use `await create_user(...)` for a synchronous call.

Arguments mapping described in
[CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*
- `Password`: `str` *(required)*
- `Username`: `str` *(required)*
- `ConsoleAccess`: `bool`
- `Groups`: `Sequence`\[`str`\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_broker"></a>

### delete_broker

Deletes a broker.

Type annotations for `session.create_client("mq").delete_broker` method.

Boto3 documentation:
[MQ.Client.delete_broker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.delete_broker)

Asynchronous method. Use `await delete_broker(...)` for a synchronous call.

Arguments mapping described in
[DeleteBrokerRequestRequestTypeDef](./type_defs.md#deletebrokerrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteBrokerResponseTypeDef](./type_defs.md#deletebrokerresponsetypedef).

<a id="delete\_tags"></a>

### delete_tags

Removes a tag from a resource.

Type annotations for `session.create_client("mq").delete_tags` method.

Boto3 documentation:
[MQ.Client.delete_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.delete_tags)

Asynchronous method. Use `await delete_tags(...)` for a synchronous call.

Arguments mapping described in
[DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="delete\_user"></a>

### delete_user

Deletes an ActiveMQ user.

Type annotations for `session.create_client("mq").delete_user` method.

Boto3 documentation:
[MQ.Client.delete_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.delete_user)

Asynchronous method. Use `await delete_user(...)` for a synchronous call.

Arguments mapping described in
[DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*
- `Username`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_broker"></a>

### describe_broker

Returns information about the specified broker.

Type annotations for `session.create_client("mq").describe_broker` method.

Boto3 documentation:
[MQ.Client.describe_broker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_broker)

Asynchronous method. Use `await describe_broker(...)` for a synchronous call.

Arguments mapping described in
[DescribeBrokerRequestRequestTypeDef](./type_defs.md#describebrokerrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBrokerResponseTypeDef](./type_defs.md#describebrokerresponsetypedef).

<a id="describe\_broker\_engine\_types"></a>

### describe_broker_engine_types

Describe available engine types and versions.

Type annotations for `session.create_client("mq").describe_broker_engine_types`
method.

Boto3 documentation:
[MQ.Client.describe_broker_engine_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_broker_engine_types)

Asynchronous method. Use `await describe_broker_engine_types(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBrokerEngineTypesRequestRequestTypeDef](./type_defs.md#describebrokerenginetypesrequestrequesttypedef).

Keyword-only arguments:

- `EngineType`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeBrokerEngineTypesResponseTypeDef](./type_defs.md#describebrokerenginetypesresponsetypedef).

<a id="describe\_broker\_instance\_options"></a>

### describe_broker_instance_options

Describe available broker instance options.

Type annotations for
`session.create_client("mq").describe_broker_instance_options` method.

Boto3 documentation:
[MQ.Client.describe_broker_instance_options](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_broker_instance_options)

Asynchronous method. Use `await describe_broker_instance_options(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBrokerInstanceOptionsRequestRequestTypeDef](./type_defs.md#describebrokerinstanceoptionsrequestrequesttypedef).

Keyword-only arguments:

- `EngineType`: `str`
- `HostInstanceType`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `StorageType`: `str`

Returns a `Coroutine` for
[DescribeBrokerInstanceOptionsResponseTypeDef](./type_defs.md#describebrokerinstanceoptionsresponsetypedef).

<a id="describe\_configuration"></a>

### describe_configuration

Returns information about the specified configuration.

Type annotations for `session.create_client("mq").describe_configuration`
method.

Boto3 documentation:
[MQ.Client.describe_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_configuration)

Asynchronous method. Use `await describe_configuration(...)` for a synchronous
call.

Arguments mapping described in
[DescribeConfigurationRequestRequestTypeDef](./type_defs.md#describeconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeConfigurationResponseTypeDef](./type_defs.md#describeconfigurationresponsetypedef).

<a id="describe\_configuration\_revision"></a>

### describe_configuration_revision

Returns the specified configuration revision for the specified configuration.

Type annotations for
`session.create_client("mq").describe_configuration_revision` method.

Boto3 documentation:
[MQ.Client.describe_configuration_revision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_configuration_revision)

Asynchronous method. Use `await describe_configuration_revision(...)` for a
synchronous call.

Arguments mapping described in
[DescribeConfigurationRevisionRequestRequestTypeDef](./type_defs.md#describeconfigurationrevisionrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationId`: `str` *(required)*
- `ConfigurationRevision`: `str` *(required)*

Returns a `Coroutine` for
[DescribeConfigurationRevisionResponseTypeDef](./type_defs.md#describeconfigurationrevisionresponsetypedef).

<a id="describe\_user"></a>

### describe_user

Returns information about an ActiveMQ user.

Type annotations for `session.create_client("mq").describe_user` method.

Boto3 documentation:
[MQ.Client.describe_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.describe_user)

Asynchronous method. Use `await describe_user(...)` for a synchronous call.

Arguments mapping described in
[DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*
- `Username`: `str` *(required)*

Returns a `Coroutine` for
[DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("mq").generate_presigned_url`
method.

Boto3 documentation:
[MQ.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_brokers"></a>

### list_brokers

Returns a list of all brokers.

Type annotations for `session.create_client("mq").list_brokers` method.

Boto3 documentation:
[MQ.Client.list_brokers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.list_brokers)

Asynchronous method. Use `await list_brokers(...)` for a synchronous call.

Arguments mapping described in
[ListBrokersRequestRequestTypeDef](./type_defs.md#listbrokersrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef).

<a id="list\_configuration\_revisions"></a>

### list_configuration_revisions

Returns a list of all revisions for the specified configuration.

Type annotations for `session.create_client("mq").list_configuration_revisions`
method.

Boto3 documentation:
[MQ.Client.list_configuration_revisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.list_configuration_revisions)

Asynchronous method. Use `await list_configuration_revisions(...)` for a
synchronous call.

Arguments mapping described in
[ListConfigurationRevisionsRequestRequestTypeDef](./type_defs.md#listconfigurationrevisionsrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef).

<a id="list\_configurations"></a>

### list_configurations

Returns a list of all configurations.

Type annotations for `session.create_client("mq").list_configurations` method.

Boto3 documentation:
[MQ.Client.list_configurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.list_configurations)

Asynchronous method. Use `await list_configurations(...)` for a synchronous
call.

Arguments mapping described in
[ListConfigurationsRequestRequestTypeDef](./type_defs.md#listconfigurationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef).

<a id="list\_tags"></a>

### list_tags

Lists tags for a resource.

Type annotations for `session.create_client("mq").list_tags` method.

Boto3 documentation:
[MQ.Client.list_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.list_tags)

Asynchronous method. Use `await list_tags(...)` for a synchronous call.

Arguments mapping described in
[ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef).

<a id="list\_users"></a>

### list_users

Returns a list of all ActiveMQ users.

Type annotations for `session.create_client("mq").list_users` method.

Boto3 documentation:
[MQ.Client.list_users](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.list_users)

Asynchronous method. Use `await list_users(...)` for a synchronous call.

Arguments mapping described in
[ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef).

<a id="reboot\_broker"></a>

### reboot_broker

Reboots a broker.

Type annotations for `session.create_client("mq").reboot_broker` method.

Boto3 documentation:
[MQ.Client.reboot_broker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.reboot_broker)

Asynchronous method. Use `await reboot_broker(...)` for a synchronous call.

Arguments mapping described in
[RebootBrokerRequestRequestTypeDef](./type_defs.md#rebootbrokerrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_broker"></a>

### update_broker

Adds a pending configuration change to a broker.

Type annotations for `session.create_client("mq").update_broker` method.

Boto3 documentation:
[MQ.Client.update_broker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_broker)

Asynchronous method. Use `await update_broker(...)` for a synchronous call.

Arguments mapping described in
[UpdateBrokerRequestRequestTypeDef](./type_defs.md#updatebrokerrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*
- `AuthenticationStrategy`:
  [AuthenticationStrategyType](./literals.md#authenticationstrategytype)
- `AutoMinorVersionUpgrade`: `bool`
- `Configuration`:
  [ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef)
- `EngineVersion`: `str`
- `HostInstanceType`: `str`
- `LdapServerMetadata`:
  [LdapServerMetadataInputTypeDef](./type_defs.md#ldapservermetadatainputtypedef)
- `Logs`: [LogsTypeDef](./type_defs.md#logstypedef)
- `MaintenanceWindowStartTime`:
  [WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef)
- `SecurityGroups`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[UpdateBrokerResponseTypeDef](./type_defs.md#updatebrokerresponsetypedef).

<a id="update\_configuration"></a>

### update_configuration

Updates the specified configuration.

Type annotations for `session.create_client("mq").update_configuration` method.

Boto3 documentation:
[MQ.Client.update_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_configuration)

Asynchronous method. Use `await update_configuration(...)` for a synchronous
call.

Arguments mapping described in
[UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationId`: `str` *(required)*
- `Data`: `str` *(required)*
- `Description`: `str`

Returns a `Coroutine` for
[UpdateConfigurationResponseTypeDef](./type_defs.md#updateconfigurationresponsetypedef).

<a id="update\_user"></a>

### update_user

Updates the information for an ActiveMQ user.

Type annotations for `session.create_client("mq").update_user` method.

Boto3 documentation:
[MQ.Client.update_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_user)

Asynchronous method. Use `await update_user(...)` for a synchronous call.

Arguments mapping described in
[UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef).

Keyword-only arguments:

- `BrokerId`: `str` *(required)*
- `Username`: `str` *(required)*
- `ConsoleAccess`: `bool`
- `Groups`: `Sequence`\[`str`\]
- `Password`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("mq").__aenter__` method.

Boto3 documentation:
[MQ.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [MQClient](#mqclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("mq").__aexit__` method.

Boto3 documentation:
[MQ.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("mq").get_paginator` method with
overloads.

- `client.get_paginator("list_brokers")` ->
  [ListBrokersPaginator](./paginators.md#listbrokerspaginator)
