<a id="amplifyuibuilderclient-for-aiobotocore-amplifyuibuilder-module"></a>

# AmplifyUIBuilderClient for aiobotocore AmplifyUIBuilder module

> [Index](..) > [AmplifyUIBuilder](.) > AmplifyUIBuilderClient

Auto-generated documentation for
[AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
type annotations stubs module
[types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

- [AmplifyUIBuilderClient for aiobotocore AmplifyUIBuilder module](#amplifyuibuilderclient-for-aiobotocore-amplifyuibuilder-module)
  - [AmplifyUIBuilderClient](#amplifyuibuilderclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_component](#create_component)
    - [create_theme](#create_theme)
    - [delete_component](#delete_component)
    - [delete_theme](#delete_theme)
    - [exchange_code_for_token](#exchange_code_for_token)
    - [export_components](#export_components)
    - [export_themes](#export_themes)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_component](#get_component)
    - [get_theme](#get_theme)
    - [list_components](#list_components)
    - [list_themes](#list_themes)
    - [refresh_token](#refresh_token)
    - [update_component](#update_component)
    - [update_theme](#update_theme)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="amplifyuibuilderclient"></a>

## AmplifyUIBuilderClient

Type annotations for `session.create_client("amplifyuibuilder")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
```

Boto3 documentation:
[AmplifyUIBuilder.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_amplifyuibuilder.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidParameterException`
- `Exceptions.ResourceConflictException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AmplifyUIBuilderClient exceptions.

Type annotations for `session.create_client("amplifyuibuilder").exceptions`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("amplifyuibuilder").can_paginate`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_component"></a>

### create_component

Creates a new component for an Amplify app.

Type annotations for
`session.create_client("amplifyuibuilder").create_component` method.

Boto3 documentation:
[AmplifyUIBuilder.Client.create_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_component)

Asynchronous method. Use `await create_component(...)` for a synchronous call.

Arguments mapping described in
[CreateComponentRequestRequestTypeDef](./type_defs.md#createcomponentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `componentToCreate`:
  [CreateComponentDataTypeDef](./type_defs.md#createcomponentdatatypedef)
  *(required)*
- `environmentName`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef).

<a id="create_theme"></a>

### create_theme

Creates a theme to apply to the components in an Amplify app.

Type annotations for `session.create_client("amplifyuibuilder").create_theme`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.create_theme](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_theme)

Asynchronous method. Use `await create_theme(...)` for a synchronous call.

Arguments mapping described in
[CreateThemeRequestRequestTypeDef](./type_defs.md#createthemerequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `themeToCreate`:
  [CreateThemeDataTypeDef](./type_defs.md#createthemedatatypedef) *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[CreateThemeResponseTypeDef](./type_defs.md#createthemeresponsetypedef).

<a id="delete_component"></a>

### delete_component

Deletes a component from an Amplify app.

Type annotations for
`session.create_client("amplifyuibuilder").delete_component` method.

Boto3 documentation:
[AmplifyUIBuilder.Client.delete_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_component)

Asynchronous method. Use `await delete_component(...)` for a synchronous call.

Arguments mapping described in
[DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `id`: `str` *(required)*

<a id="delete_theme"></a>

### delete_theme

Deletes a theme from an Amplify app.

Type annotations for `session.create_client("amplifyuibuilder").delete_theme`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.delete_theme](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_theme)

Asynchronous method. Use `await delete_theme(...)` for a synchronous call.

Arguments mapping described in
[DeleteThemeRequestRequestTypeDef](./type_defs.md#deletethemerequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `id`: `str` *(required)*

<a id="exchange_code_for_token"></a>

### exchange_code_for_token

Exchanges an access code for a token.

Type annotations for
`session.create_client("amplifyuibuilder").exchange_code_for_token` method.

Boto3 documentation:
[AmplifyUIBuilder.Client.exchange_code_for_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.exchange_code_for_token)

Asynchronous method. Use `await exchange_code_for_token(...)` for a synchronous
call.

Arguments mapping described in
[ExchangeCodeForTokenRequestRequestTypeDef](./type_defs.md#exchangecodefortokenrequestrequesttypedef).

Keyword-only arguments:

- `provider`: `Literal['figma']` (see
  [TokenProvidersType](./literals.md#tokenproviderstype)) *(required)*
- `request`:
  [ExchangeCodeForTokenRequestBodyTypeDef](./type_defs.md#exchangecodefortokenrequestbodytypedef)
  *(required)*

Returns a `Coroutine` for
[ExchangeCodeForTokenResponseTypeDef](./type_defs.md#exchangecodefortokenresponsetypedef).

<a id="export_components"></a>

### export_components

Exports component configurations to code that is ready to integrate into an
Amplify app.

Type annotations for
`session.create_client("amplifyuibuilder").export_components` method.

Boto3 documentation:
[AmplifyUIBuilder.Client.export_components](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.export_components)

Asynchronous method. Use `await export_components(...)` for a synchronous call.

Arguments mapping described in
[ExportComponentsRequestRequestTypeDef](./type_defs.md#exportcomponentsrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*

Returns a `Coroutine` for
[ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef).

<a id="export_themes"></a>

### export_themes

Exports theme configurations to code that is ready to integrate into an Amplify
app.

Type annotations for `session.create_client("amplifyuibuilder").export_themes`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.export_themes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.export_themes)

Asynchronous method. Use `await export_themes(...)` for a synchronous call.

Arguments mapping described in
[ExportThemesRequestRequestTypeDef](./type_defs.md#exportthemesrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*

Returns a `Coroutine` for
[ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("amplifyuibuilder").generate_presigned_url` method.

Boto3 documentation:
[AmplifyUIBuilder.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_component"></a>

### get_component

Returns an existing component for an Amplify app.

Type annotations for `session.create_client("amplifyuibuilder").get_component`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.get_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_component)

Asynchronous method. Use `await get_component(...)` for a synchronous call.

Arguments mapping described in
[GetComponentRequestRequestTypeDef](./type_defs.md#getcomponentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `id`: `str` *(required)*

Returns a `Coroutine` for
[GetComponentResponseTypeDef](./type_defs.md#getcomponentresponsetypedef).

<a id="get_theme"></a>

### get_theme

Returns an existing theme for an Amplify app.

Type annotations for `session.create_client("amplifyuibuilder").get_theme`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.get_theme](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_theme)

Asynchronous method. Use `await get_theme(...)` for a synchronous call.

Arguments mapping described in
[GetThemeRequestRequestTypeDef](./type_defs.md#getthemerequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `id`: `str` *(required)*

Returns a `Coroutine` for
[GetThemeResponseTypeDef](./type_defs.md#getthemeresponsetypedef).

<a id="list_components"></a>

### list_components

Retrieves a list of components for a specified Amplify app and backend
environment.

Type annotations for
`session.create_client("amplifyuibuilder").list_components` method.

Boto3 documentation:
[AmplifyUIBuilder.Client.list_components](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_components)

Asynchronous method. Use `await list_components(...)` for a synchronous call.

Arguments mapping described in
[ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef).

<a id="list_themes"></a>

### list_themes

Retrieves a list of themes for a specified Amplify app and backend environment.

Type annotations for `session.create_client("amplifyuibuilder").list_themes`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.list_themes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_themes)

Asynchronous method. Use `await list_themes(...)` for a synchronous call.

Arguments mapping described in
[ListThemesRequestRequestTypeDef](./type_defs.md#listthemesrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef).

<a id="refresh_token"></a>

### refresh_token

Refreshes a previously issued access token that might have expired.

Type annotations for `session.create_client("amplifyuibuilder").refresh_token`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.refresh_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)

Asynchronous method. Use `await refresh_token(...)` for a synchronous call.

Arguments mapping described in
[RefreshTokenRequestRequestTypeDef](./type_defs.md#refreshtokenrequestrequesttypedef).

Keyword-only arguments:

- `provider`: `Literal['figma']` (see
  [TokenProvidersType](./literals.md#tokenproviderstype)) *(required)*
- `refreshTokenBody`:
  [RefreshTokenRequestBodyTypeDef](./type_defs.md#refreshtokenrequestbodytypedef)
  *(required)*

Returns a `Coroutine` for
[RefreshTokenResponseTypeDef](./type_defs.md#refreshtokenresponsetypedef).

<a id="update_component"></a>

### update_component

Updates an existing component.

Type annotations for
`session.create_client("amplifyuibuilder").update_component` method.

Boto3 documentation:
[AmplifyUIBuilder.Client.update_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_component)

Asynchronous method. Use `await update_component(...)` for a synchronous call.

Arguments mapping described in
[UpdateComponentRequestRequestTypeDef](./type_defs.md#updatecomponentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `id`: `str` *(required)*
- `updatedComponent`:
  [UpdateComponentDataTypeDef](./type_defs.md#updatecomponentdatatypedef)
  *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateComponentResponseTypeDef](./type_defs.md#updatecomponentresponsetypedef).

<a id="update_theme"></a>

### update_theme

Updates an existing theme.

Type annotations for `session.create_client("amplifyuibuilder").update_theme`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.update_theme](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_theme)

Asynchronous method. Use `await update_theme(...)` for a synchronous call.

Arguments mapping described in
[UpdateThemeRequestRequestTypeDef](./type_defs.md#updatethemerequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `id`: `str` *(required)*
- `updatedTheme`:
  [UpdateThemeDataTypeDef](./type_defs.md#updatethemedatatypedef) *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateThemeResponseTypeDef](./type_defs.md#updatethemeresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("amplifyuibuilder").__aenter__`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [AmplifyUIBuilderClient](#amplifyuibuilderclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("amplifyuibuilder").__aexit__`
method.

Boto3 documentation:
[AmplifyUIBuilder.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("amplifyuibuilder").get_paginator`
method with overloads.

- `client.get_paginator("list_components")` ->
  [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- `client.get_paginator("list_themes")` ->
  [ListThemesPaginator](./paginators.md#listthemespaginator)
