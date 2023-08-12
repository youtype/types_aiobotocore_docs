# AmplifyUIBuilderClient

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > AmplifyUIBuilderClient

!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

## AmplifyUIBuilderClient

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client)

```python
AmplifyUIBuilderClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("amplifyuibuilder").exceptions` structure.

```python
AmplifyUIBuilderClient.exceptions usage example

async with session.create_client("amplifyuibuilder") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServerException,
        client.InvalidParameterException,
        client.ResourceConflictException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
AmplifyUIBuilderClient usage type checking example

from types_aiobotocore_amplifyuibuilder.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_component

Creates a new component for an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").create_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_component)

```python
# create_component method definition

await def create_component(
    self,
    *,
    appId: str,
    environmentName: str,
    componentToCreate: CreateComponentDataTypeDef,  # (1)
    clientToken: str = ...,
) -> CreateComponentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateComponentDataTypeDef](./type_defs.md#createcomponentdatatypedef) 
2. See [:material-code-braces: CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef) 


```python
# create_component method usage example with argument unpacking

kwargs: CreateComponentRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "componentToCreate": ...,
}

parent.create_component(**kwargs)
```

1. See [:material-code-braces: CreateComponentRequestRequestTypeDef](./type_defs.md#createcomponentrequestrequesttypedef) 

### create\_form

Creates a new form for an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").create_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)

```python
# create_form method definition

await def create_form(
    self,
    *,
    appId: str,
    environmentName: str,
    formToCreate: CreateFormDataTypeDef,  # (1)
    clientToken: str = ...,
) -> CreateFormResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateFormDataTypeDef](./type_defs.md#createformdatatypedef) 
2. See [:material-code-braces: CreateFormResponseTypeDef](./type_defs.md#createformresponsetypedef) 


```python
# create_form method usage example with argument unpacking

kwargs: CreateFormRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "formToCreate": ...,
}

parent.create_form(**kwargs)
```

1. See [:material-code-braces: CreateFormRequestRequestTypeDef](./type_defs.md#createformrequestrequesttypedef) 

### create\_theme

Creates a theme to apply to the components in an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").create_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_theme)

```python
# create_theme method definition

await def create_theme(
    self,
    *,
    appId: str,
    environmentName: str,
    themeToCreate: CreateThemeDataTypeDef,  # (1)
    clientToken: str = ...,
) -> CreateThemeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateThemeDataTypeDef](./type_defs.md#createthemedatatypedef) 
2. See [:material-code-braces: CreateThemeResponseTypeDef](./type_defs.md#createthemeresponsetypedef) 


```python
# create_theme method usage example with argument unpacking

kwargs: CreateThemeRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "themeToCreate": ...,
}

parent.create_theme(**kwargs)
```

1. See [:material-code-braces: CreateThemeRequestRequestTypeDef](./type_defs.md#createthemerequestrequesttypedef) 

### delete\_component

Deletes a component from an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").delete_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_component)

```python
# delete_component method definition

await def delete_component(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_component method usage example with argument unpacking

kwargs: DeleteComponentRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
}

parent.delete_component(**kwargs)
```

1. See [:material-code-braces: DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef) 

### delete\_form

Deletes a form from an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").delete_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_form)

```python
# delete_form method definition

await def delete_form(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_form method usage example with argument unpacking

kwargs: DeleteFormRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
}

parent.delete_form(**kwargs)
```

1. See [:material-code-braces: DeleteFormRequestRequestTypeDef](./type_defs.md#deleteformrequestrequesttypedef) 

### delete\_theme

Deletes a theme from an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").delete_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_theme)

```python
# delete_theme method definition

await def delete_theme(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_theme method usage example with argument unpacking

kwargs: DeleteThemeRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
}

parent.delete_theme(**kwargs)
```

1. See [:material-code-braces: DeleteThemeRequestRequestTypeDef](./type_defs.md#deletethemerequestrequesttypedef) 

### exchange\_code\_for\_token

Exchanges an access code for a token.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").exchange_code_for_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.exchange_code_for_token)

```python
# exchange_code_for_token method definition

await def exchange_code_for_token(
    self,
    *,
    provider: TokenProvidersType,  # (1)
    request: ExchangeCodeForTokenRequestBodyTypeDef,  # (2)
) -> ExchangeCodeForTokenResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TokenProvidersType](./literals.md#tokenproviderstype) 
2. See [:material-code-braces: ExchangeCodeForTokenRequestBodyTypeDef](./type_defs.md#exchangecodefortokenrequestbodytypedef) 
3. See [:material-code-braces: ExchangeCodeForTokenResponseTypeDef](./type_defs.md#exchangecodefortokenresponsetypedef) 


```python
# exchange_code_for_token method usage example with argument unpacking

kwargs: ExchangeCodeForTokenRequestRequestTypeDef = {  # (1)
    "provider": ...,
    "request": ...,
}

parent.exchange_code_for_token(**kwargs)
```

1. See [:material-code-braces: ExchangeCodeForTokenRequestRequestTypeDef](./type_defs.md#exchangecodefortokenrequestrequesttypedef) 

### export\_components

Exports component configurations to code that is ready to integrate into an
Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").export_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.export_components)

```python
# export_components method definition

await def export_components(
    self,
    *,
    appId: str,
    environmentName: str,
    nextToken: str = ...,
) -> ExportComponentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef) 


```python
# export_components method usage example with argument unpacking

kwargs: ExportComponentsRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.export_components(**kwargs)
```

1. See [:material-code-braces: ExportComponentsRequestRequestTypeDef](./type_defs.md#exportcomponentsrequestrequesttypedef) 

### export\_forms

Exports form configurations to code that is ready to integrate into an Amplify
app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").export_forms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.export_forms)

```python
# export_forms method definition

await def export_forms(
    self,
    *,
    appId: str,
    environmentName: str,
    nextToken: str = ...,
) -> ExportFormsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportFormsResponseTypeDef](./type_defs.md#exportformsresponsetypedef) 


```python
# export_forms method usage example with argument unpacking

kwargs: ExportFormsRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.export_forms(**kwargs)
```

1. See [:material-code-braces: ExportFormsRequestRequestTypeDef](./type_defs.md#exportformsrequestrequesttypedef) 

### export\_themes

Exports theme configurations to code that is ready to integrate into an Amplify
app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").export_themes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.export_themes)

```python
# export_themes method definition

await def export_themes(
    self,
    *,
    appId: str,
    environmentName: str,
    nextToken: str = ...,
) -> ExportThemesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef) 


```python
# export_themes method usage example with argument unpacking

kwargs: ExportThemesRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.export_themes(**kwargs)
```

1. See [:material-code-braces: ExportThemesRequestRequestTypeDef](./type_defs.md#exportthemesrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.generate_presigned_url)

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


### get\_codegen\_job

Returns an existing code generation job.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_codegen_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_codegen_job)

```python
# get_codegen_job method definition

await def get_codegen_job(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
) -> GetCodegenJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCodegenJobResponseTypeDef](./type_defs.md#getcodegenjobresponsetypedef) 


```python
# get_codegen_job method usage example with argument unpacking

kwargs: GetCodegenJobRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
}

parent.get_codegen_job(**kwargs)
```

1. See [:material-code-braces: GetCodegenJobRequestRequestTypeDef](./type_defs.md#getcodegenjobrequestrequesttypedef) 

### get\_component

Returns an existing component for an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_component)

```python
# get_component method definition

await def get_component(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
) -> GetComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComponentResponseTypeDef](./type_defs.md#getcomponentresponsetypedef) 


```python
# get_component method usage example with argument unpacking

kwargs: GetComponentRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
}

parent.get_component(**kwargs)
```

1. See [:material-code-braces: GetComponentRequestRequestTypeDef](./type_defs.md#getcomponentrequestrequesttypedef) 

### get\_form

Returns an existing form for an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_form)

```python
# get_form method definition

await def get_form(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
) -> GetFormResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFormResponseTypeDef](./type_defs.md#getformresponsetypedef) 


```python
# get_form method usage example with argument unpacking

kwargs: GetFormRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
}

parent.get_form(**kwargs)
```

1. See [:material-code-braces: GetFormRequestRequestTypeDef](./type_defs.md#getformrequestrequesttypedef) 

### get\_metadata

Returns existing metadata for an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_metadata)

```python
# get_metadata method definition

await def get_metadata(
    self,
    *,
    appId: str,
    environmentName: str,
) -> GetMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMetadataResponseTypeDef](./type_defs.md#getmetadataresponsetypedef) 


```python
# get_metadata method usage example with argument unpacking

kwargs: GetMetadataRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.get_metadata(**kwargs)
```

1. See [:material-code-braces: GetMetadataRequestRequestTypeDef](./type_defs.md#getmetadatarequestrequesttypedef) 

### get\_theme

Returns an existing theme for an Amplify app.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_theme)

```python
# get_theme method definition

await def get_theme(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
) -> GetThemeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetThemeResponseTypeDef](./type_defs.md#getthemeresponsetypedef) 


```python
# get_theme method usage example with argument unpacking

kwargs: GetThemeRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
}

parent.get_theme(**kwargs)
```

1. See [:material-code-braces: GetThemeRequestRequestTypeDef](./type_defs.md#getthemerequestrequesttypedef) 

### list\_codegen\_jobs

Retrieves a list of code generation jobs for a specified Amplify app and backend
environment.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").list_codegen_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_codegen_jobs)

```python
# list_codegen_jobs method definition

await def list_codegen_jobs(
    self,
    *,
    appId: str,
    environmentName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCodegenJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCodegenJobsResponseTypeDef](./type_defs.md#listcodegenjobsresponsetypedef) 


```python
# list_codegen_jobs method usage example with argument unpacking

kwargs: ListCodegenJobsRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.list_codegen_jobs(**kwargs)
```

1. See [:material-code-braces: ListCodegenJobsRequestRequestTypeDef](./type_defs.md#listcodegenjobsrequestrequesttypedef) 

### list\_components

Retrieves a list of components for a specified Amplify app and backend
environment.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").list_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_components)

```python
# list_components method definition

await def list_components(
    self,
    *,
    appId: str,
    environmentName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListComponentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python
# list_components method usage example with argument unpacking

kwargs: ListComponentsRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.list_components(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef) 

### list\_forms

Retrieves a list of forms for a specified Amplify app and backend environment.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").list_forms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_forms)

```python
# list_forms method definition

await def list_forms(
    self,
    *,
    appId: str,
    environmentName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFormsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFormsResponseTypeDef](./type_defs.md#listformsresponsetypedef) 


```python
# list_forms method usage example with argument unpacking

kwargs: ListFormsRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.list_forms(**kwargs)
```

1. See [:material-code-braces: ListFormsRequestRequestTypeDef](./type_defs.md#listformsrequestrequesttypedef) 

### list\_themes

Retrieves a list of themes for a specified Amplify app and backend environment.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").list_themes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_themes)

```python
# list_themes method definition

await def list_themes(
    self,
    *,
    appId: str,
    environmentName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListThemesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef) 


```python
# list_themes method usage example with argument unpacking

kwargs: ListThemesRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.list_themes(**kwargs)
```

1. See [:material-code-braces: ListThemesRequestRequestTypeDef](./type_defs.md#listthemesrequestrequesttypedef) 

### put\_metadata\_flag

Stores the metadata information about a feature on a form.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").put_metadata_flag` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.put_metadata_flag)

```python
# put_metadata_flag method definition

await def put_metadata_flag(
    self,
    *,
    appId: str,
    environmentName: str,
    featureName: str,
    body: PutMetadataFlagBodyTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PutMetadataFlagBodyTypeDef](./type_defs.md#putmetadataflagbodytypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_metadata_flag method usage example with argument unpacking

kwargs: PutMetadataFlagRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "featureName": ...,
    "body": ...,
}

parent.put_metadata_flag(**kwargs)
```

1. See [:material-code-braces: PutMetadataFlagRequestRequestTypeDef](./type_defs.md#putmetadataflagrequestrequesttypedef) 

### refresh\_token

Refreshes a previously issued access token that might have expired.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").refresh_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)

```python
# refresh_token method definition

await def refresh_token(
    self,
    *,
    provider: TokenProvidersType,  # (1)
    refreshTokenBody: RefreshTokenRequestBodyTypeDef,  # (2)
) -> RefreshTokenResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TokenProvidersType](./literals.md#tokenproviderstype) 
2. See [:material-code-braces: RefreshTokenRequestBodyTypeDef](./type_defs.md#refreshtokenrequestbodytypedef) 
3. See [:material-code-braces: RefreshTokenResponseTypeDef](./type_defs.md#refreshtokenresponsetypedef) 


```python
# refresh_token method usage example with argument unpacking

kwargs: RefreshTokenRequestRequestTypeDef = {  # (1)
    "provider": ...,
    "refreshTokenBody": ...,
}

parent.refresh_token(**kwargs)
```

1. See [:material-code-braces: RefreshTokenRequestRequestTypeDef](./type_defs.md#refreshtokenrequestrequesttypedef) 

### start\_codegen\_job

Starts a code generation job for a specified Amplify app and backend
environment.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").start_codegen_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)

```python
# start_codegen_job method definition

await def start_codegen_job(
    self,
    *,
    appId: str,
    environmentName: str,
    codegenJobToCreate: StartCodegenJobDataTypeDef,  # (1)
    clientToken: str = ...,
) -> StartCodegenJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartCodegenJobDataTypeDef](./type_defs.md#startcodegenjobdatatypedef) 
2. See [:material-code-braces: StartCodegenJobResponseTypeDef](./type_defs.md#startcodegenjobresponsetypedef) 


```python
# start_codegen_job method usage example with argument unpacking

kwargs: StartCodegenJobRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "codegenJobToCreate": ...,
}

parent.start_codegen_job(**kwargs)
```

1. See [:material-code-braces: StartCodegenJobRequestRequestTypeDef](./type_defs.md#startcodegenjobrequestrequesttypedef) 

### update\_component

Updates an existing component.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").update_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_component)

```python
# update_component method definition

await def update_component(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
    updatedComponent: UpdateComponentDataTypeDef,  # (1)
    clientToken: str = ...,
) -> UpdateComponentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateComponentDataTypeDef](./type_defs.md#updatecomponentdatatypedef) 
2. See [:material-code-braces: UpdateComponentResponseTypeDef](./type_defs.md#updatecomponentresponsetypedef) 


```python
# update_component method usage example with argument unpacking

kwargs: UpdateComponentRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
    "updatedComponent": ...,
}

parent.update_component(**kwargs)
```

1. See [:material-code-braces: UpdateComponentRequestRequestTypeDef](./type_defs.md#updatecomponentrequestrequesttypedef) 

### update\_form

Updates an existing form.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").update_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_form)

```python
# update_form method definition

await def update_form(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
    updatedForm: UpdateFormDataTypeDef,  # (1)
    clientToken: str = ...,
) -> UpdateFormResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateFormDataTypeDef](./type_defs.md#updateformdatatypedef) 
2. See [:material-code-braces: UpdateFormResponseTypeDef](./type_defs.md#updateformresponsetypedef) 


```python
# update_form method usage example with argument unpacking

kwargs: UpdateFormRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
    "updatedForm": ...,
}

parent.update_form(**kwargs)
```

1. See [:material-code-braces: UpdateFormRequestRequestTypeDef](./type_defs.md#updateformrequestrequesttypedef) 

### update\_theme

Updates an existing theme.

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").update_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_theme)

```python
# update_theme method definition

await def update_theme(
    self,
    *,
    appId: str,
    environmentName: str,
    id: str,
    updatedTheme: UpdateThemeDataTypeDef,  # (1)
    clientToken: str = ...,
) -> UpdateThemeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateThemeDataTypeDef](./type_defs.md#updatethemedatatypedef) 
2. See [:material-code-braces: UpdateThemeResponseTypeDef](./type_defs.md#updatethemeresponsetypedef) 


```python
# update_theme method usage example with argument unpacking

kwargs: UpdateThemeRequestRequestTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
    "id": ...,
    "updatedTheme": ...,
}

parent.update_theme(**kwargs)
```

1. See [:material-code-braces: UpdateThemeRequestRequestTypeDef](./type_defs.md#updatethemerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> AmplifyUIBuilderClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator` method with overloads.

- `client.get_paginator("export_components")` -> [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
- `client.get_paginator("export_forms")` -> [ExportFormsPaginator](./paginators.md#exportformspaginator)
- `client.get_paginator("export_themes")` -> [ExportThemesPaginator](./paginators.md#exportthemespaginator)
- `client.get_paginator("list_codegen_jobs")` -> [ListCodegenJobsPaginator](./paginators.md#listcodegenjobspaginator)
- `client.get_paginator("list_components")` -> [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- `client.get_paginator("list_forms")` -> [ListFormsPaginator](./paginators.md#listformspaginator)
- `client.get_paginator("list_themes")` -> [ListThemesPaginator](./paginators.md#listthemespaginator)



