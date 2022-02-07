<a id="acmclient-for-aiobotocore-acm-module"></a>

# ACMClient for aiobotocore ACM module

> [Index](..) > [ACM](.) > ACMClient

Auto-generated documentation for
[ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
type annotations stubs module
[types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

- [ACMClient for aiobotocore ACM module](#acmclient-for-aiobotocore-acm-module)
  - [ACMClient](#acmclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_tags_to_certificate](#add_tags_to_certificate)
    - [can_paginate](#can_paginate)
    - [delete_certificate](#delete_certificate)
    - [describe_certificate](#describe_certificate)
    - [export_certificate](#export_certificate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_account_configuration](#get_account_configuration)
    - [get_certificate](#get_certificate)
    - [import_certificate](#import_certificate)
    - [list_certificates](#list_certificates)
    - [list_tags_for_certificate](#list_tags_for_certificate)
    - [put_account_configuration](#put_account_configuration)
    - [remove_tags_from_certificate](#remove_tags_from_certificate)
    - [renew_certificate](#renew_certificate)
    - [request_certificate](#request_certificate)
    - [resend_validation_email](#resend_validation_email)
    - [update_certificate_options](#update_certificate_options)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="acmclient"></a>

## ACMClient

Type annotations for `session.create_client("acm")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_acm.client import ACMClient

session = get_session()
async with session.create_client("acm") as client:
    client: ACMClient
```

Boto3 documentation:
[ACM.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_acm.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InvalidArgsException`
- `Exceptions.InvalidArnException`
- `Exceptions.InvalidDomainValidationOptionsException`
- `Exceptions.InvalidParameterException`
- `Exceptions.InvalidStateException`
- `Exceptions.InvalidTagException`
- `Exceptions.LimitExceededException`
- `Exceptions.RequestInProgressException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.TagPolicyException`
- `Exceptions.ThrottlingException`
- `Exceptions.TooManyTagsException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ACMClient exceptions.

Type annotations for `session.create_client("acm").exceptions` method.

Boto3 documentation:
[ACM.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add_tags_to_certificate"></a>

### add_tags_to_certificate

Adds one or more tags to an ACM certificate.

Type annotations for `session.create_client("acm").add_tags_to_certificate`
method.

Boto3 documentation:
[ACM.Client.add_tags_to_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.add_tags_to_certificate)

Asynchronous method. Use `await add_tags_to_certificate(...)` for a synchronous
call.

Arguments mapping described in
[AddTagsToCertificateRequestRequestTypeDef](./type_defs.md#addtagstocertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("acm").can_paginate` method.

Boto3 documentation:
[ACM.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="delete_certificate"></a>

### delete_certificate

Deletes a certificate and its associated private key.

Type annotations for `session.create_client("acm").delete_certificate` method.

Boto3 documentation:
[ACM.Client.delete_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.delete_certificate)

Asynchronous method. Use `await delete_certificate(...)` for a synchronous
call.

Arguments mapping described in
[DeleteCertificateRequestRequestTypeDef](./type_defs.md#deletecertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*

<a id="describe_certificate"></a>

### describe_certificate

Returns detailed metadata about the specified ACM certificate.

Type annotations for `session.create_client("acm").describe_certificate`
method.

Boto3 documentation:
[ACM.Client.describe_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.describe_certificate)

Asynchronous method. Use `await describe_certificate(...)` for a synchronous
call.

Arguments mapping described in
[DescribeCertificateRequestRequestTypeDef](./type_defs.md#describecertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef).

<a id="export_certificate"></a>

### export_certificate

Exports a private certificate issued by a private certificate authority (CA)
for use anywhere.

Type annotations for `session.create_client("acm").export_certificate` method.

Boto3 documentation:
[ACM.Client.export_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.export_certificate)

Asynchronous method. Use `await export_certificate(...)` for a synchronous
call.

Arguments mapping described in
[ExportCertificateRequestRequestTypeDef](./type_defs.md#exportcertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*
- `Passphrase`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*

Returns a `Coroutine` for
[ExportCertificateResponseTypeDef](./type_defs.md#exportcertificateresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("acm").generate_presigned_url`
method.

Boto3 documentation:
[ACM.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_account_configuration"></a>

### get_account_configuration

Returns the account configuration options associated with an Amazon Web
Services account.

Type annotations for `session.create_client("acm").get_account_configuration`
method.

Boto3 documentation:
[ACM.Client.get_account_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_account_configuration)

Asynchronous method. Use `await get_account_configuration(...)` for a
synchronous call.

Returns a `Coroutine` for
[GetAccountConfigurationResponseTypeDef](./type_defs.md#getaccountconfigurationresponsetypedef).

<a id="get_certificate"></a>

### get_certificate

Retrieves an Amazon-issued certificate and its certificate chain.

Type annotations for `session.create_client("acm").get_certificate` method.

Boto3 documentation:
[ACM.Client.get_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_certificate)

Asynchronous method. Use `await get_certificate(...)` for a synchronous call.

Arguments mapping described in
[GetCertificateRequestRequestTypeDef](./type_defs.md#getcertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*

Returns a `Coroutine` for
[GetCertificateResponseTypeDef](./type_defs.md#getcertificateresponsetypedef).

<a id="import_certificate"></a>

### import_certificate

Imports a certificate into Amazon Web Services Certificate Manager (ACM) to use
with services that are integrated with ACM.

Type annotations for `session.create_client("acm").import_certificate` method.

Boto3 documentation:
[ACM.Client.import_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)

Asynchronous method. Use `await import_certificate(...)` for a synchronous
call.

Arguments mapping described in
[ImportCertificateRequestRequestTypeDef](./type_defs.md#importcertificaterequestrequesttypedef).

Keyword-only arguments:

- `Certificate`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*
- `PrivateKey`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*
- `CertificateArn`: `str`
- `CertificateChain`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[ImportCertificateResponseTypeDef](./type_defs.md#importcertificateresponsetypedef).

<a id="list_certificates"></a>

### list_certificates

Retrieves a list of certificate ARNs and domain names.

Type annotations for `session.create_client("acm").list_certificates` method.

Boto3 documentation:
[ACM.Client.list_certificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_certificates)

Asynchronous method. Use `await list_certificates(...)` for a synchronous call.

Arguments mapping described in
[ListCertificatesRequestRequestTypeDef](./type_defs.md#listcertificatesrequestrequesttypedef).

Keyword-only arguments:

- `CertificateStatuses`:
  `Sequence`\[[CertificateStatusType](./literals.md#certificatestatustype)\]
- `Includes`: [FiltersTypeDef](./type_defs.md#filterstypedef)
- `NextToken`: `str`
- `MaxItems`: `int`

Returns a `Coroutine` for
[ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef).

<a id="list_tags_for_certificate"></a>

### list_tags_for_certificate

Lists the tags that have been applied to the ACM certificate.

Type annotations for `session.create_client("acm").list_tags_for_certificate`
method.

Boto3 documentation:
[ACM.Client.list_tags_for_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_tags_for_certificate)

Asynchronous method. Use `await list_tags_for_certificate(...)` for a
synchronous call.

Arguments mapping described in
[ListTagsForCertificateRequestRequestTypeDef](./type_defs.md#listtagsforcertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForCertificateResponseTypeDef](./type_defs.md#listtagsforcertificateresponsetypedef).

<a id="put_account_configuration"></a>

### put_account_configuration

Adds or modifies account-level configurations in ACM.

Type annotations for `session.create_client("acm").put_account_configuration`
method.

Boto3 documentation:
[ACM.Client.put_account_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.put_account_configuration)

Asynchronous method. Use `await put_account_configuration(...)` for a
synchronous call.

Arguments mapping described in
[PutAccountConfigurationRequestRequestTypeDef](./type_defs.md#putaccountconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `IdempotencyToken`: `str` *(required)*
- `ExpiryEvents`:
  [ExpiryEventsConfigurationTypeDef](./type_defs.md#expiryeventsconfigurationtypedef)

<a id="remove_tags_from_certificate"></a>

### remove_tags_from_certificate

Remove one or more tags from an ACM certificate.

Type annotations for
`session.create_client("acm").remove_tags_from_certificate` method.

Boto3 documentation:
[ACM.Client.remove_tags_from_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.remove_tags_from_certificate)

Asynchronous method. Use `await remove_tags_from_certificate(...)` for a
synchronous call.

Arguments mapping described in
[RemoveTagsFromCertificateRequestRequestTypeDef](./type_defs.md#removetagsfromcertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

<a id="renew_certificate"></a>

### renew_certificate

Renews an eligible ACM certificate.

Type annotations for `session.create_client("acm").renew_certificate` method.

Boto3 documentation:
[ACM.Client.renew_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.renew_certificate)

Asynchronous method. Use `await renew_certificate(...)` for a synchronous call.

Arguments mapping described in
[RenewCertificateRequestRequestTypeDef](./type_defs.md#renewcertificaterequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*

<a id="request_certificate"></a>

### request_certificate

Requests an ACM certificate for use with other Amazon Web Services services.

Type annotations for `session.create_client("acm").request_certificate` method.

Boto3 documentation:
[ACM.Client.request_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.request_certificate)

Asynchronous method. Use `await request_certificate(...)` for a synchronous
call.

Arguments mapping described in
[RequestCertificateRequestRequestTypeDef](./type_defs.md#requestcertificaterequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*
- `ValidationMethod`:
  [ValidationMethodType](./literals.md#validationmethodtype)
- `SubjectAlternativeNames`: `Sequence`\[`str`\]
- `IdempotencyToken`: `str`
- `DomainValidationOptions`:
  `Sequence`\[[DomainValidationOptionTypeDef](./type_defs.md#domainvalidationoptiontypedef)\]
- `Options`:
  [CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef)
- `CertificateAuthorityArn`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[RequestCertificateResponseTypeDef](./type_defs.md#requestcertificateresponsetypedef).

<a id="resend_validation_email"></a>

### resend_validation_email

Resends the email that requests domain ownership validation.

Type annotations for `session.create_client("acm").resend_validation_email`
method.

Boto3 documentation:
[ACM.Client.resend_validation_email](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.resend_validation_email)

Asynchronous method. Use `await resend_validation_email(...)` for a synchronous
call.

Arguments mapping described in
[ResendValidationEmailRequestRequestTypeDef](./type_defs.md#resendvalidationemailrequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*
- `Domain`: `str` *(required)*
- `ValidationDomain`: `str` *(required)*

<a id="update_certificate_options"></a>

### update_certificate_options

Updates a certificate.

Type annotations for `session.create_client("acm").update_certificate_options`
method.

Boto3 documentation:
[ACM.Client.update_certificate_options](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.update_certificate_options)

Asynchronous method. Use `await update_certificate_options(...)` for a
synchronous call.

Arguments mapping described in
[UpdateCertificateOptionsRequestRequestTypeDef](./type_defs.md#updatecertificateoptionsrequestrequesttypedef).

Keyword-only arguments:

- `CertificateArn`: `str` *(required)*
- `Options`:
  [CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef)
  *(required)*

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("acm").__aenter__` method.

Boto3 documentation:
[ACM.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ACMClient](#acmclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("acm").__aexit__` method.

Boto3 documentation:
[ACM.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("acm").get_paginator` method with
overloads.

- `client.get_paginator("list_certificates")` ->
  [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("acm").get_waiter` method with
overloads.

- `client.get_waiter("certificate_validated")` ->
  [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)
