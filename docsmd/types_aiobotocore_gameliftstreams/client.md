# GameLiftStreamsClient

> [Index](../README.md) > [GameLiftStreams](./README.md) > GameLiftStreamsClient

!!! note ""

    Auto-generated documentation for [GameLiftStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams.html#gameliftstreams)
    type annotations stubs module [types-aiobotocore-gameliftstreams](https://pypi.org/project/types-aiobotocore-gameliftstreams/).

## GameLiftStreamsClient

Type annotations and code completion for `#!python session.create_client("gameliftstreams")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams.html#GameLiftStreams.Client)

```python
# GameLiftStreamsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_gameliftstreams.client import GameLiftStreamsClient

session = get_session()
async with session.create_client("gameliftstreams") as client:
    client: GameLiftStreamsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("gameliftstreams").exceptions` structure.

```python
# GameLiftStreamsClient.exceptions usage example

async with session.create_client("gameliftstreams") as client:
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
# GameLiftStreamsClient usage type checking example

from types_aiobotocore_gameliftstreams.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("gameliftstreams").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("gameliftstreams").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/generate_presigned_url.html)

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


### add\_stream\_group\_locations

Add locations that can host stream sessions.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").add_stream_group_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/add_stream_group_locations.html)

```python
# add_stream_group_locations method definition

await def add_stream_group_locations(
    self,
    *,
    Identifier: str,
    LocationConfigurations: Sequence[LocationConfigurationTypeDef],  # (1)
) -> AddStreamGroupLocationsOutputTypeDef:  # (2)
    ...
```

1. See `Sequence[LocationConfigurationTypeDef]`
2. See [:material-code-braces: AddStreamGroupLocationsOutputTypeDef](./type_defs.md#addstreamgrouplocationsoutputtypedef)


```python
# add_stream_group_locations method usage example with argument unpacking

kwargs: AddStreamGroupLocationsInputTypeDef = {  # (1)
    "Identifier": ...,
    "LocationConfigurations": ...,
}

parent.add_stream_group_locations(**kwargs)
```

1. See [:material-code-braces: AddStreamGroupLocationsInputTypeDef](./type_defs.md#addstreamgrouplocationsinputtypedef)

### associate\_applications

When you associate, or link, an application with a stream group, then Amazon
GameLift Streams can launch the application using the stream group's allocated
compute resources.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").associate_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/associate_applications.html)

```python
# associate_applications method definition

await def associate_applications(
    self,
    *,
    Identifier: str,
    ApplicationIdentifiers: Sequence[str],
) -> AssociateApplicationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateApplicationsOutputTypeDef](./type_defs.md#associateapplicationsoutputtypedef)


```python
# associate_applications method usage example with argument unpacking

kwargs: AssociateApplicationsInputTypeDef = {  # (1)
    "Identifier": ...,
    "ApplicationIdentifiers": ...,
}

parent.associate_applications(**kwargs)
```

1. See [:material-code-braces: AssociateApplicationsInputTypeDef](./type_defs.md#associateapplicationsinputtypedef)

### create\_application

Creates an application resource in Amazon GameLift Streams, which specifies the
application content you want to stream, such as a game build or other software,
and configures the settings to run it.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    Description: str,
    RuntimeEnvironment: RuntimeEnvironmentTypeDef,  # (1)
    ExecutablePath: str,
    ApplicationSourceUri: str,
    ApplicationLogPaths: Sequence[str] = ...,
    ApplicationLogOutputUri: str = ...,
    Tags: Mapping[str, str] = ...,
    ClientToken: str = ...,
) -> CreateApplicationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuntimeEnvironmentTypeDef](./type_defs.md#runtimeenvironmenttypedef)
2. See [:material-code-braces: CreateApplicationOutputTypeDef](./type_defs.md#createapplicationoutputtypedef)


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationInputTypeDef = {  # (1)
    "Description": ...,
    "RuntimeEnvironment": ...,
    "ExecutablePath": ...,
    "ApplicationSourceUri": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationInputTypeDef](./type_defs.md#createapplicationinputtypedef)

### create\_stream\_group

Stream groups manage how Amazon GameLift Streams allocates resources and
handles concurrent streams, allowing you to effectively manage capacity and
costs.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").create_stream_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/create_stream_group.html)

```python
# create_stream_group method definition

await def create_stream_group(
    self,
    *,
    Description: str,
    StreamClass: StreamClassType,  # (1)
    DefaultApplicationIdentifier: str = ...,
    LocationConfigurations: Sequence[LocationConfigurationTypeDef] = ...,  # (2)
    Tags: Mapping[str, str] = ...,
    ClientToken: str = ...,
) -> CreateStreamGroupOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: StreamClassType](./literals.md#streamclasstype)
2. See `Sequence[LocationConfigurationTypeDef]`
3. See [:material-code-braces: CreateStreamGroupOutputTypeDef](./type_defs.md#createstreamgroupoutputtypedef)


```python
# create_stream_group method usage example with argument unpacking

kwargs: CreateStreamGroupInputTypeDef = {  # (1)
    "Description": ...,
    "StreamClass": ...,
}

parent.create_stream_group(**kwargs)
```

1. See [:material-code-braces: CreateStreamGroupInputTypeDef](./type_defs.md#createstreamgroupinputtypedef)

### create\_stream\_session\_connection

Enables clients to reconnect to a stream session while preserving all session
state and data in the disconnected session.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").create_stream_session_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/create_stream_session_connection.html)

```python
# create_stream_session_connection method definition

await def create_stream_session_connection(
    self,
    *,
    Identifier: str,
    StreamSessionIdentifier: str,
    SignalRequest: str,
    ClientToken: str = ...,
) -> CreateStreamSessionConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateStreamSessionConnectionOutputTypeDef](./type_defs.md#createstreamsessionconnectionoutputtypedef)


```python
# create_stream_session_connection method usage example with argument unpacking

kwargs: CreateStreamSessionConnectionInputTypeDef = {  # (1)
    "Identifier": ...,
    "StreamSessionIdentifier": ...,
    "SignalRequest": ...,
}

parent.create_stream_session_connection(**kwargs)
```

1. See [:material-code-braces: CreateStreamSessionConnectionInputTypeDef](./type_defs.md#createstreamsessionconnectioninputtypedef)

### delete\_application

Permanently deletes an Amazon GameLift Streams application resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/delete_application.html)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationInputTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationInputTypeDef](./type_defs.md#deleteapplicationinputtypedef)

### delete\_stream\_group

Permanently deletes all compute resources and information related to a stream
group.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").delete_stream_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/delete_stream_group.html)

```python
# delete_stream_group method definition

await def delete_stream_group(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_stream_group method usage example with argument unpacking

kwargs: DeleteStreamGroupInputTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_stream_group(**kwargs)
```

1. See [:material-code-braces: DeleteStreamGroupInputTypeDef](./type_defs.md#deletestreamgroupinputtypedef)

### disassociate\_applications

When you disassociate, or unlink, an application from a stream group, you can
no longer stream this application by using that stream group's allocated
compute resources.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").disassociate_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/disassociate_applications.html)

```python
# disassociate_applications method definition

await def disassociate_applications(
    self,
    *,
    Identifier: str,
    ApplicationIdentifiers: Sequence[str],
) -> DisassociateApplicationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateApplicationsOutputTypeDef](./type_defs.md#disassociateapplicationsoutputtypedef)


```python
# disassociate_applications method usage example with argument unpacking

kwargs: DisassociateApplicationsInputTypeDef = {  # (1)
    "Identifier": ...,
    "ApplicationIdentifiers": ...,
}

parent.disassociate_applications(**kwargs)
```

1. See [:material-code-braces: DisassociateApplicationsInputTypeDef](./type_defs.md#disassociateapplicationsinputtypedef)

### export\_stream\_session\_files

Export the files that your application modifies or generates in a stream
session, which can help you debug or verify your application.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").export_stream_session_files` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/export_stream_session_files.html)

```python
# export_stream_session_files method definition

await def export_stream_session_files(
    self,
    *,
    Identifier: str,
    StreamSessionIdentifier: str,
    OutputUri: str,
) -> dict[str, Any]:
    ...
```

```python
# export_stream_session_files method usage example with argument unpacking

kwargs: ExportStreamSessionFilesInputTypeDef = {  # (1)
    "Identifier": ...,
    "StreamSessionIdentifier": ...,
    "OutputUri": ...,
}

parent.export_stream_session_files(**kwargs)
```

1. See [:material-code-braces: ExportStreamSessionFilesInputTypeDef](./type_defs.md#exportstreamsessionfilesinputtypedef)

### get\_application

Retrieves properties for an Amazon GameLift Streams application resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/get_application.html)

```python
# get_application method definition

await def get_application(
    self,
    *,
    Identifier: str,
) -> GetApplicationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationOutputTypeDef](./type_defs.md#getapplicationoutputtypedef)


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationInputTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationInputTypeDef](./type_defs.md#getapplicationinputtypedef)

### get\_stream\_group

Retrieves properties for a Amazon GameLift Streams stream group resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_stream_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/get_stream_group.html)

```python
# get_stream_group method definition

await def get_stream_group(
    self,
    *,
    Identifier: str,
) -> GetStreamGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStreamGroupOutputTypeDef](./type_defs.md#getstreamgroupoutputtypedef)


```python
# get_stream_group method usage example with argument unpacking

kwargs: GetStreamGroupInputTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_stream_group(**kwargs)
```

1. See [:material-code-braces: GetStreamGroupInputTypeDef](./type_defs.md#getstreamgroupinputtypedef)

### get\_stream\_session

Retrieves properties for a Amazon GameLift Streams stream session resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_stream_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/get_stream_session.html)

```python
# get_stream_session method definition

await def get_stream_session(
    self,
    *,
    Identifier: str,
    StreamSessionIdentifier: str,
) -> GetStreamSessionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStreamSessionOutputTypeDef](./type_defs.md#getstreamsessionoutputtypedef)


```python
# get_stream_session method usage example with argument unpacking

kwargs: GetStreamSessionInputTypeDef = {  # (1)
    "Identifier": ...,
    "StreamSessionIdentifier": ...,
}

parent.get_stream_session(**kwargs)
```

1. See [:material-code-braces: GetStreamSessionInputTypeDef](./type_defs.md#getstreamsessioninputtypedef)

### list\_applications

Retrieves a list of all Amazon GameLift Streams applications that are
associated with the Amazon Web Services account in use.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/list_applications.html)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListApplicationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef)


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsInputTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsInputTypeDef](./type_defs.md#listapplicationsinputtypedef)

### list\_stream\_groups

Retrieves a list of all Amazon GameLift Streams stream groups that are
associated with the Amazon Web Services account in use.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").list_stream_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/list_stream_groups.html)

```python
# list_stream_groups method definition

await def list_stream_groups(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListStreamGroupsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamGroupsOutputTypeDef](./type_defs.md#liststreamgroupsoutputtypedef)


```python
# list_stream_groups method usage example with argument unpacking

kwargs: ListStreamGroupsInputTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_stream_groups(**kwargs)
```

1. See [:material-code-braces: ListStreamGroupsInputTypeDef](./type_defs.md#liststreamgroupsinputtypedef)

### list\_stream\_sessions

Retrieves a list of Amazon GameLift Streams stream sessions that a stream group
is hosting.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").list_stream_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/list_stream_sessions.html)

```python
# list_stream_sessions method definition

await def list_stream_sessions(
    self,
    *,
    Identifier: str,
    Status: StreamSessionStatusType = ...,  # (1)
    ExportFilesStatus: ExportFilesStatusType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListStreamSessionsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: StreamSessionStatusType](./literals.md#streamsessionstatustype)
2. See [:material-code-brackets: ExportFilesStatusType](./literals.md#exportfilesstatustype)
3. See [:material-code-braces: ListStreamSessionsOutputTypeDef](./type_defs.md#liststreamsessionsoutputtypedef)


```python
# list_stream_sessions method usage example with argument unpacking

kwargs: ListStreamSessionsInputTypeDef = {  # (1)
    "Identifier": ...,
}

parent.list_stream_sessions(**kwargs)
```

1. See [:material-code-braces: ListStreamSessionsInputTypeDef](./type_defs.md#liststreamsessionsinputtypedef)

### list\_stream\_sessions\_by\_account

Retrieves a list of Amazon GameLift Streams stream sessions that this user
account has access to.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").list_stream_sessions_by_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/list_stream_sessions_by_account.html)

```python
# list_stream_sessions_by_account method definition

await def list_stream_sessions_by_account(
    self,
    *,
    Status: StreamSessionStatusType = ...,  # (1)
    ExportFilesStatus: ExportFilesStatusType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListStreamSessionsByAccountOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: StreamSessionStatusType](./literals.md#streamsessionstatustype)
2. See [:material-code-brackets: ExportFilesStatusType](./literals.md#exportfilesstatustype)
3. See [:material-code-braces: ListStreamSessionsByAccountOutputTypeDef](./type_defs.md#liststreamsessionsbyaccountoutputtypedef)


```python
# list_stream_sessions_by_account method usage example with argument unpacking

kwargs: ListStreamSessionsByAccountInputTypeDef = {  # (1)
    "Status": ...,
}

parent.list_stream_sessions_by_account(**kwargs)
```

1. See [:material-code-braces: ListStreamSessionsByAccountInputTypeDef](./type_defs.md#liststreamsessionsbyaccountinputtypedef)

### list\_tags\_for\_resource

Retrieves all tags assigned to a Amazon GameLift Streams resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### remove\_stream\_group\_locations

Removes a set of remote locations from this stream group.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").remove_stream_group_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/remove_stream_group_locations.html)

```python
# remove_stream_group_locations method definition

await def remove_stream_group_locations(
    self,
    *,
    Identifier: str,
    Locations: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# remove_stream_group_locations method usage example with argument unpacking

kwargs: RemoveStreamGroupLocationsInputTypeDef = {  # (1)
    "Identifier": ...,
    "Locations": ...,
}

parent.remove_stream_group_locations(**kwargs)
```

1. See [:material-code-braces: RemoveStreamGroupLocationsInputTypeDef](./type_defs.md#removestreamgrouplocationsinputtypedef)

### start\_stream\_session

This action initiates a new stream session and outputs connection information
that clients can use to access the stream.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").start_stream_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/start_stream_session.html)

```python
# start_stream_session method definition

await def start_stream_session(
    self,
    *,
    Identifier: str,
    Protocol: ProtocolType,  # (1)
    SignalRequest: str,
    ApplicationIdentifier: str,
    ClientToken: str = ...,
    Description: str = ...,
    UserId: str = ...,
    Locations: Sequence[str] = ...,
    ConnectionTimeoutSeconds: int = ...,
    SessionLengthSeconds: int = ...,
    AdditionalLaunchArgs: Sequence[str] = ...,
    AdditionalEnvironmentVariables: Mapping[str, str] = ...,
    PerformanceStatsConfiguration: PerformanceStatsConfigurationTypeDef = ...,  # (2)
) -> StartStreamSessionOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype)
2. See [:material-code-braces: PerformanceStatsConfigurationTypeDef](./type_defs.md#performancestatsconfigurationtypedef)
3. See [:material-code-braces: StartStreamSessionOutputTypeDef](./type_defs.md#startstreamsessionoutputtypedef)


```python
# start_stream_session method usage example with argument unpacking

kwargs: StartStreamSessionInputTypeDef = {  # (1)
    "Identifier": ...,
    "Protocol": ...,
    "SignalRequest": ...,
    "ApplicationIdentifier": ...,
}

parent.start_stream_session(**kwargs)
```

1. See [:material-code-braces: StartStreamSessionInputTypeDef](./type_defs.md#startstreamsessioninputtypedef)

### tag\_resource

Assigns one or more tags to a Amazon GameLift Streams resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```

```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### terminate\_stream\_session

Permanently terminates an active stream session.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").terminate_stream_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/terminate_stream_session.html)

```python
# terminate_stream_session method definition

await def terminate_stream_session(
    self,
    *,
    Identifier: str,
    StreamSessionIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# terminate_stream_session method usage example with argument unpacking

kwargs: TerminateStreamSessionInputTypeDef = {  # (1)
    "Identifier": ...,
    "StreamSessionIdentifier": ...,
}

parent.terminate_stream_session(**kwargs)
```

1. See [:material-code-braces: TerminateStreamSessionInputTypeDef](./type_defs.md#terminatestreamsessioninputtypedef)

### untag\_resource

Removes one or more tags from a Amazon GameLift Streams resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_application

Updates the mutable configuration settings for a Amazon GameLift Streams
application resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    Identifier: str,
    Description: str = ...,
    ApplicationLogPaths: Sequence[str] = ...,
    ApplicationLogOutputUri: str = ...,
) -> UpdateApplicationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateApplicationOutputTypeDef](./type_defs.md#updateapplicationoutputtypedef)


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationInputTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationInputTypeDef](./type_defs.md#updateapplicationinputtypedef)

### update\_stream\_group

Updates the configuration settings for an Amazon GameLift Streams stream group
resource.

Type annotations and code completion for `#!python session.create_client("gameliftstreams").update_stream_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams/client/update_stream_group.html)

```python
# update_stream_group method definition

await def update_stream_group(
    self,
    *,
    Identifier: str,
    LocationConfigurations: Sequence[LocationConfigurationTypeDef] = ...,  # (1)
    Description: str = ...,
    DefaultApplicationIdentifier: str = ...,
) -> UpdateStreamGroupOutputTypeDef:  # (2)
    ...
```

1. See `Sequence[LocationConfigurationTypeDef]`
2. See [:material-code-braces: UpdateStreamGroupOutputTypeDef](./type_defs.md#updatestreamgroupoutputtypedef)


```python
# update_stream_group method usage example with argument unpacking

kwargs: UpdateStreamGroupInputTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_stream_group(**kwargs)
```

1. See [:material-code-braces: UpdateStreamGroupInputTypeDef](./type_defs.md#updatestreamgroupinputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("gameliftstreams").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams.html#GameLiftStreams.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("gameliftstreams").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams.html#GameLiftStreams.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_paginator` method with overloads.

- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_stream_groups")` -> [ListStreamGroupsPaginator](./paginators.md#liststreamgroupspaginator)
- `client.get_paginator("list_stream_sessions_by_account")` -> [ListStreamSessionsByAccountPaginator](./paginators.md#liststreamsessionsbyaccountpaginator)
- `client.get_paginator("list_stream_sessions")` -> [ListStreamSessionsPaginator](./paginators.md#liststreamsessionspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("gameliftstreams").get_waiter` method with overloads.

- `client.get_waiter("application_deleted")` -> [ApplicationDeletedWaiter](./waiters.md#applicationdeletedwaiter)
- `client.get_waiter("application_ready")` -> [ApplicationReadyWaiter](./waiters.md#applicationreadywaiter)
- `client.get_waiter("stream_group_active")` -> [StreamGroupActiveWaiter](./waiters.md#streamgroupactivewaiter)
- `client.get_waiter("stream_group_deleted")` -> [StreamGroupDeletedWaiter](./waiters.md#streamgroupdeletedwaiter)
- `client.get_waiter("stream_session_active")` -> [StreamSessionActiveWaiter](./waiters.md#streamsessionactivewaiter)

