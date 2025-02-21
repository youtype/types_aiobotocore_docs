# LicenseManagerClient

> [Index](../README.md) > [LicenseManager](./README.md) > LicenseManagerClient

!!! note ""

    Auto-generated documentation for [LicenseManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#licensemanager)
    type annotations stubs module [types-aiobotocore-license-manager](https://pypi.org/project/types-aiobotocore-license-manager/).

## LicenseManagerClient

Type annotations and code completion for `#!python session.create_client("license-manager")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)

```python
# LicenseManagerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_license_manager.client import LicenseManagerClient

session = get_session()
async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("license-manager").exceptions` structure.

```python
# LicenseManagerClient.exceptions usage example

async with session.create_client("license-manager") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.AuthorizationException,
        client.ClientError,
        client.ConflictException,
        client.EntitlementNotAllowedException,
        client.FailedDependencyException,
        client.FilterLimitExceededException,
        client.InvalidParameterValueException,
        client.InvalidResourceStateException,
        client.LicenseUsageException,
        client.NoEntitlementsAllowedException,
        client.RateLimitExceededException,
        client.RedirectException,
        client.ResourceLimitExceededException,
        client.ResourceNotFoundException,
        client.ServerInternalException,
        client.UnsupportedDigitalSignatureMethodException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# LicenseManagerClient usage type checking example

from types_aiobotocore_license_manager.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("license-manager").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("license-manager").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/generate_presigned_url.html)

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


### accept\_grant

Accepts the specified grant.

Type annotations and code completion for `#!python session.create_client("license-manager").accept_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/accept_grant.html)

```python
# accept_grant method definition

await def accept_grant(
    self,
    *,
    GrantArn: str,
) -> AcceptGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptGrantResponseTypeDef](./type_defs.md#acceptgrantresponsetypedef) 


```python
# accept_grant method usage example with argument unpacking

kwargs: AcceptGrantRequestTypeDef = {  # (1)
    "GrantArn": ...,
}

parent.accept_grant(**kwargs)
```

1. See [:material-code-braces: AcceptGrantRequestTypeDef](./type_defs.md#acceptgrantrequesttypedef) 

### check\_in\_license

Checks in the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").check_in_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/check_in_license.html)

```python
# check_in_license method definition

await def check_in_license(
    self,
    *,
    LicenseConsumptionToken: str,
    Beneficiary: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# check_in_license method usage example with argument unpacking

kwargs: CheckInLicenseRequestTypeDef = {  # (1)
    "LicenseConsumptionToken": ...,
}

parent.check_in_license(**kwargs)
```

1. See [:material-code-braces: CheckInLicenseRequestTypeDef](./type_defs.md#checkinlicenserequesttypedef) 

### checkout\_borrow\_license

Checks out the specified license for offline use.

Type annotations and code completion for `#!python session.create_client("license-manager").checkout_borrow_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/checkout_borrow_license.html)

```python
# checkout_borrow_license method definition

await def checkout_borrow_license(
    self,
    *,
    LicenseArn: str,
    Entitlements: Sequence[EntitlementDataTypeDef],  # (1)
    DigitalSignatureMethod: DigitalSignatureMethodType,  # (2)
    ClientToken: str,
    NodeId: str = ...,
    CheckoutMetadata: Sequence[MetadataTypeDef] = ...,  # (3)
) -> CheckoutBorrowLicenseResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: EntitlementDataTypeDef](./type_defs.md#entitlementdatatypedef) 
2. See [:material-code-brackets: DigitalSignatureMethodType](./literals.md#digitalsignaturemethodtype) 
3. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
4. See [:material-code-braces: CheckoutBorrowLicenseResponseTypeDef](./type_defs.md#checkoutborrowlicenseresponsetypedef) 


```python
# checkout_borrow_license method usage example with argument unpacking

kwargs: CheckoutBorrowLicenseRequestTypeDef = {  # (1)
    "LicenseArn": ...,
    "Entitlements": ...,
    "DigitalSignatureMethod": ...,
    "ClientToken": ...,
}

parent.checkout_borrow_license(**kwargs)
```

1. See [:material-code-braces: CheckoutBorrowLicenseRequestTypeDef](./type_defs.md#checkoutborrowlicenserequesttypedef) 

### checkout\_license

Checks out the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").checkout_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/checkout_license.html)

```python
# checkout_license method definition

await def checkout_license(
    self,
    *,
    ProductSKU: str,
    CheckoutType: CheckoutTypeType,  # (1)
    KeyFingerprint: str,
    Entitlements: Sequence[EntitlementDataTypeDef],  # (2)
    ClientToken: str,
    Beneficiary: str = ...,
    NodeId: str = ...,
) -> CheckoutLicenseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CheckoutTypeType](./literals.md#checkouttypetype) 
2. See [:material-code-braces: EntitlementDataTypeDef](./type_defs.md#entitlementdatatypedef) 
3. See [:material-code-braces: CheckoutLicenseResponseTypeDef](./type_defs.md#checkoutlicenseresponsetypedef) 


```python
# checkout_license method usage example with argument unpacking

kwargs: CheckoutLicenseRequestTypeDef = {  # (1)
    "ProductSKU": ...,
    "CheckoutType": ...,
    "KeyFingerprint": ...,
    "Entitlements": ...,
    "ClientToken": ...,
}

parent.checkout_license(**kwargs)
```

1. See [:material-code-braces: CheckoutLicenseRequestTypeDef](./type_defs.md#checkoutlicenserequesttypedef) 

### create\_grant

Creates a grant for the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").create_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_grant.html)

```python
# create_grant method definition

await def create_grant(
    self,
    *,
    ClientToken: str,
    GrantName: str,
    LicenseArn: str,
    Principals: Sequence[str],
    HomeRegion: str,
    AllowedOperations: Sequence[AllowedOperationType],  # (1)
) -> CreateGrantResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AllowedOperationType](./literals.md#allowedoperationtype) 
2. See [:material-code-braces: CreateGrantResponseTypeDef](./type_defs.md#creategrantresponsetypedef) 


```python
# create_grant method usage example with argument unpacking

kwargs: CreateGrantRequestTypeDef = {  # (1)
    "ClientToken": ...,
    "GrantName": ...,
    "LicenseArn": ...,
    "Principals": ...,
    "HomeRegion": ...,
    "AllowedOperations": ...,
}

parent.create_grant(**kwargs)
```

1. See [:material-code-braces: CreateGrantRequestTypeDef](./type_defs.md#creategrantrequesttypedef) 

### create\_grant\_version

Creates a new version of the specified grant.

Type annotations and code completion for `#!python session.create_client("license-manager").create_grant_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_grant_version.html)

```python
# create_grant_version method definition

await def create_grant_version(
    self,
    *,
    ClientToken: str,
    GrantArn: str,
    GrantName: str = ...,
    AllowedOperations: Sequence[AllowedOperationType] = ...,  # (1)
    Status: GrantStatusType = ...,  # (2)
    StatusReason: str = ...,
    SourceVersion: str = ...,
    Options: OptionsTypeDef = ...,  # (3)
) -> CreateGrantVersionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AllowedOperationType](./literals.md#allowedoperationtype) 
2. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
3. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
4. See [:material-code-braces: CreateGrantVersionResponseTypeDef](./type_defs.md#creategrantversionresponsetypedef) 


```python
# create_grant_version method usage example with argument unpacking

kwargs: CreateGrantVersionRequestTypeDef = {  # (1)
    "ClientToken": ...,
    "GrantArn": ...,
}

parent.create_grant_version(**kwargs)
```

1. See [:material-code-braces: CreateGrantVersionRequestTypeDef](./type_defs.md#creategrantversionrequesttypedef) 

### create\_license

Creates a license.

Type annotations and code completion for `#!python session.create_client("license-manager").create_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_license.html)

```python
# create_license method definition

await def create_license(
    self,
    *,
    LicenseName: str,
    ProductName: str,
    ProductSKU: str,
    Issuer: IssuerTypeDef,  # (1)
    HomeRegion: str,
    Validity: DatetimeRangeTypeDef,  # (2)
    Entitlements: Sequence[EntitlementTypeDef],  # (3)
    Beneficiary: str,
    ConsumptionConfiguration: ConsumptionConfigurationTypeDef,  # (4)
    ClientToken: str,
    LicenseMetadata: Sequence[MetadataTypeDef] = ...,  # (5)
) -> CreateLicenseResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: IssuerTypeDef](./type_defs.md#issuertypedef) 
2. See [:material-code-braces: DatetimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
3. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
4. See [:material-code-braces: ConsumptionConfigurationTypeDef](./type_defs.md#consumptionconfigurationtypedef) 
5. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
6. See [:material-code-braces: CreateLicenseResponseTypeDef](./type_defs.md#createlicenseresponsetypedef) 


```python
# create_license method usage example with argument unpacking

kwargs: CreateLicenseRequestTypeDef = {  # (1)
    "LicenseName": ...,
    "ProductName": ...,
    "ProductSKU": ...,
    "Issuer": ...,
    "HomeRegion": ...,
    "Validity": ...,
    "Entitlements": ...,
    "Beneficiary": ...,
    "ConsumptionConfiguration": ...,
    "ClientToken": ...,
}

parent.create_license(**kwargs)
```

1. See [:material-code-braces: CreateLicenseRequestTypeDef](./type_defs.md#createlicenserequesttypedef) 

### create\_license\_configuration

Creates a license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").create_license_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_license_configuration.html)

```python
# create_license_configuration method definition

await def create_license_configuration(
    self,
    *,
    Name: str,
    LicenseCountingType: LicenseCountingTypeType,  # (1)
    Description: str = ...,
    LicenseCount: int = ...,
    LicenseCountHardLimit: bool = ...,
    LicenseRules: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    DisassociateWhenNotFound: bool = ...,
    ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,  # (3)
) -> CreateLicenseConfigurationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: LicenseCountingTypeType](./literals.md#licensecountingtypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ProductInformationTypeDef](./type_defs.md#productinformationtypedef) [:material-code-braces: ProductInformationOutputTypeDef](./type_defs.md#productinformationoutputtypedef) 
4. See [:material-code-braces: CreateLicenseConfigurationResponseTypeDef](./type_defs.md#createlicenseconfigurationresponsetypedef) 


```python
# create_license_configuration method usage example with argument unpacking

kwargs: CreateLicenseConfigurationRequestTypeDef = {  # (1)
    "Name": ...,
    "LicenseCountingType": ...,
}

parent.create_license_configuration(**kwargs)
```

1. See [:material-code-braces: CreateLicenseConfigurationRequestTypeDef](./type_defs.md#createlicenseconfigurationrequesttypedef) 

### create\_license\_conversion\_task\_for\_resource

Creates a new license conversion task.

Type annotations and code completion for `#!python session.create_client("license-manager").create_license_conversion_task_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_license_conversion_task_for_resource.html)

```python
# create_license_conversion_task_for_resource method definition

await def create_license_conversion_task_for_resource(
    self,
    *,
    ResourceArn: str,
    SourceLicenseContext: LicenseConversionContextTypeDef,  # (1)
    DestinationLicenseContext: LicenseConversionContextTypeDef,  # (1)
) -> CreateLicenseConversionTaskForResourceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
2. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
3. See [:material-code-braces: CreateLicenseConversionTaskForResourceResponseTypeDef](./type_defs.md#createlicenseconversiontaskforresourceresponsetypedef) 


```python
# create_license_conversion_task_for_resource method usage example with argument unpacking

kwargs: CreateLicenseConversionTaskForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "SourceLicenseContext": ...,
    "DestinationLicenseContext": ...,
}

parent.create_license_conversion_task_for_resource(**kwargs)
```

1. See [:material-code-braces: CreateLicenseConversionTaskForResourceRequestTypeDef](./type_defs.md#createlicenseconversiontaskforresourcerequesttypedef) 

### create\_license\_manager\_report\_generator

Creates a report generator.

Type annotations and code completion for `#!python session.create_client("license-manager").create_license_manager_report_generator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_license_manager_report_generator.html)

```python
# create_license_manager_report_generator method definition

await def create_license_manager_report_generator(
    self,
    *,
    ReportGeneratorName: str,
    Type: Sequence[ReportTypeType],  # (1)
    ReportContext: ReportContextUnionTypeDef,  # (2)
    ReportFrequency: ReportFrequencyTypeDef,  # (3)
    ClientToken: str,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateLicenseManagerReportGeneratorResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ReportContextTypeDef](./type_defs.md#reportcontexttypedef) [:material-code-braces: ReportContextOutputTypeDef](./type_defs.md#reportcontextoutputtypedef) 
3. See [:material-code-braces: ReportFrequencyTypeDef](./type_defs.md#reportfrequencytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateLicenseManagerReportGeneratorResponseTypeDef](./type_defs.md#createlicensemanagerreportgeneratorresponsetypedef) 


```python
# create_license_manager_report_generator method usage example with argument unpacking

kwargs: CreateLicenseManagerReportGeneratorRequestTypeDef = {  # (1)
    "ReportGeneratorName": ...,
    "Type": ...,
    "ReportContext": ...,
    "ReportFrequency": ...,
    "ClientToken": ...,
}

parent.create_license_manager_report_generator(**kwargs)
```

1. See [:material-code-braces: CreateLicenseManagerReportGeneratorRequestTypeDef](./type_defs.md#createlicensemanagerreportgeneratorrequesttypedef) 

### create\_license\_version

Creates a new version of the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").create_license_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_license_version.html)

```python
# create_license_version method definition

await def create_license_version(
    self,
    *,
    LicenseArn: str,
    LicenseName: str,
    ProductName: str,
    Issuer: IssuerTypeDef,  # (1)
    HomeRegion: str,
    Validity: DatetimeRangeTypeDef,  # (2)
    Entitlements: Sequence[EntitlementTypeDef],  # (3)
    ConsumptionConfiguration: ConsumptionConfigurationTypeDef,  # (4)
    Status: LicenseStatusType,  # (5)
    ClientToken: str,
    LicenseMetadata: Sequence[MetadataTypeDef] = ...,  # (6)
    SourceVersion: str = ...,
) -> CreateLicenseVersionResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: IssuerTypeDef](./type_defs.md#issuertypedef) 
2. See [:material-code-braces: DatetimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
3. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
4. See [:material-code-braces: ConsumptionConfigurationTypeDef](./type_defs.md#consumptionconfigurationtypedef) 
5. See [:material-code-brackets: LicenseStatusType](./literals.md#licensestatustype) 
6. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
7. See [:material-code-braces: CreateLicenseVersionResponseTypeDef](./type_defs.md#createlicenseversionresponsetypedef) 


```python
# create_license_version method usage example with argument unpacking

kwargs: CreateLicenseVersionRequestTypeDef = {  # (1)
    "LicenseArn": ...,
    "LicenseName": ...,
    "ProductName": ...,
    "Issuer": ...,
    "HomeRegion": ...,
    "Validity": ...,
    "Entitlements": ...,
    "ConsumptionConfiguration": ...,
    "Status": ...,
    "ClientToken": ...,
}

parent.create_license_version(**kwargs)
```

1. See [:material-code-braces: CreateLicenseVersionRequestTypeDef](./type_defs.md#createlicenseversionrequesttypedef) 

### create\_token

Creates a long-lived token.

Type annotations and code completion for `#!python session.create_client("license-manager").create_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/create_token.html)

```python
# create_token method definition

await def create_token(
    self,
    *,
    LicenseArn: str,
    ClientToken: str,
    RoleArns: Sequence[str] = ...,
    ExpirationInDays: int = ...,
    TokenProperties: Sequence[str] = ...,
) -> CreateTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateTokenResponseTypeDef](./type_defs.md#createtokenresponsetypedef) 


```python
# create_token method usage example with argument unpacking

kwargs: CreateTokenRequestTypeDef = {  # (1)
    "LicenseArn": ...,
    "ClientToken": ...,
}

parent.create_token(**kwargs)
```

1. See [:material-code-braces: CreateTokenRequestTypeDef](./type_defs.md#createtokenrequesttypedef) 

### delete\_grant

Deletes the specified grant.

Type annotations and code completion for `#!python session.create_client("license-manager").delete_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/delete_grant.html)

```python
# delete_grant method definition

await def delete_grant(
    self,
    *,
    GrantArn: str,
    Version: str,
    StatusReason: str = ...,
) -> DeleteGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGrantResponseTypeDef](./type_defs.md#deletegrantresponsetypedef) 


```python
# delete_grant method usage example with argument unpacking

kwargs: DeleteGrantRequestTypeDef = {  # (1)
    "GrantArn": ...,
    "Version": ...,
}

parent.delete_grant(**kwargs)
```

1. See [:material-code-braces: DeleteGrantRequestTypeDef](./type_defs.md#deletegrantrequesttypedef) 

### delete\_license

Deletes the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").delete_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/delete_license.html)

```python
# delete_license method definition

await def delete_license(
    self,
    *,
    LicenseArn: str,
    SourceVersion: str,
) -> DeleteLicenseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteLicenseResponseTypeDef](./type_defs.md#deletelicenseresponsetypedef) 


```python
# delete_license method usage example with argument unpacking

kwargs: DeleteLicenseRequestTypeDef = {  # (1)
    "LicenseArn": ...,
    "SourceVersion": ...,
}

parent.delete_license(**kwargs)
```

1. See [:material-code-braces: DeleteLicenseRequestTypeDef](./type_defs.md#deletelicenserequesttypedef) 

### delete\_license\_configuration

Deletes the specified license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").delete_license_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/delete_license_configuration.html)

```python
# delete_license_configuration method definition

await def delete_license_configuration(
    self,
    *,
    LicenseConfigurationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_license_configuration method usage example with argument unpacking

kwargs: DeleteLicenseConfigurationRequestTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.delete_license_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteLicenseConfigurationRequestTypeDef](./type_defs.md#deletelicenseconfigurationrequesttypedef) 

### delete\_license\_manager\_report\_generator

Deletes the specified report generator.

Type annotations and code completion for `#!python session.create_client("license-manager").delete_license_manager_report_generator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/delete_license_manager_report_generator.html)

```python
# delete_license_manager_report_generator method definition

await def delete_license_manager_report_generator(
    self,
    *,
    LicenseManagerReportGeneratorArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_license_manager_report_generator method usage example with argument unpacking

kwargs: DeleteLicenseManagerReportGeneratorRequestTypeDef = {  # (1)
    "LicenseManagerReportGeneratorArn": ...,
}

parent.delete_license_manager_report_generator(**kwargs)
```

1. See [:material-code-braces: DeleteLicenseManagerReportGeneratorRequestTypeDef](./type_defs.md#deletelicensemanagerreportgeneratorrequesttypedef) 

### delete\_token

Deletes the specified token.

Type annotations and code completion for `#!python session.create_client("license-manager").delete_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/delete_token.html)

```python
# delete_token method definition

await def delete_token(
    self,
    *,
    TokenId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_token method usage example with argument unpacking

kwargs: DeleteTokenRequestTypeDef = {  # (1)
    "TokenId": ...,
}

parent.delete_token(**kwargs)
```

1. See [:material-code-braces: DeleteTokenRequestTypeDef](./type_defs.md#deletetokenrequesttypedef) 

### extend\_license\_consumption

Extends the expiration date for license consumption.

Type annotations and code completion for `#!python session.create_client("license-manager").extend_license_consumption` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/extend_license_consumption.html)

```python
# extend_license_consumption method definition

await def extend_license_consumption(
    self,
    *,
    LicenseConsumptionToken: str,
    DryRun: bool = ...,
) -> ExtendLicenseConsumptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExtendLicenseConsumptionResponseTypeDef](./type_defs.md#extendlicenseconsumptionresponsetypedef) 


```python
# extend_license_consumption method usage example with argument unpacking

kwargs: ExtendLicenseConsumptionRequestTypeDef = {  # (1)
    "LicenseConsumptionToken": ...,
}

parent.extend_license_consumption(**kwargs)
```

1. See [:material-code-braces: ExtendLicenseConsumptionRequestTypeDef](./type_defs.md#extendlicenseconsumptionrequesttypedef) 

### get\_access\_token

Gets a temporary access token to use with AssumeRoleWithWebIdentity.

Type annotations and code completion for `#!python session.create_client("license-manager").get_access_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_access_token.html)

```python
# get_access_token method definition

await def get_access_token(
    self,
    *,
    Token: str,
    TokenProperties: Sequence[str] = ...,
) -> GetAccessTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessTokenResponseTypeDef](./type_defs.md#getaccesstokenresponsetypedef) 


```python
# get_access_token method usage example with argument unpacking

kwargs: GetAccessTokenRequestTypeDef = {  # (1)
    "Token": ...,
}

parent.get_access_token(**kwargs)
```

1. See [:material-code-braces: GetAccessTokenRequestTypeDef](./type_defs.md#getaccesstokenrequesttypedef) 

### get\_grant

Gets detailed information about the specified grant.

Type annotations and code completion for `#!python session.create_client("license-manager").get_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_grant.html)

```python
# get_grant method definition

await def get_grant(
    self,
    *,
    GrantArn: str,
    Version: str = ...,
) -> GetGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGrantResponseTypeDef](./type_defs.md#getgrantresponsetypedef) 


```python
# get_grant method usage example with argument unpacking

kwargs: GetGrantRequestTypeDef = {  # (1)
    "GrantArn": ...,
}

parent.get_grant(**kwargs)
```

1. See [:material-code-braces: GetGrantRequestTypeDef](./type_defs.md#getgrantrequesttypedef) 

### get\_license

Gets detailed information about the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").get_license` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_license.html)

```python
# get_license method definition

await def get_license(
    self,
    *,
    LicenseArn: str,
    Version: str = ...,
) -> GetLicenseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLicenseResponseTypeDef](./type_defs.md#getlicenseresponsetypedef) 


```python
# get_license method usage example with argument unpacking

kwargs: GetLicenseRequestTypeDef = {  # (1)
    "LicenseArn": ...,
}

parent.get_license(**kwargs)
```

1. See [:material-code-braces: GetLicenseRequestTypeDef](./type_defs.md#getlicenserequesttypedef) 

### get\_license\_configuration

Gets detailed information about the specified license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").get_license_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_license_configuration.html)

```python
# get_license_configuration method definition

await def get_license_configuration(
    self,
    *,
    LicenseConfigurationArn: str,
) -> GetLicenseConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLicenseConfigurationResponseTypeDef](./type_defs.md#getlicenseconfigurationresponsetypedef) 


```python
# get_license_configuration method usage example with argument unpacking

kwargs: GetLicenseConfigurationRequestTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.get_license_configuration(**kwargs)
```

1. See [:material-code-braces: GetLicenseConfigurationRequestTypeDef](./type_defs.md#getlicenseconfigurationrequesttypedef) 

### get\_license\_conversion\_task

Gets information about the specified license type conversion task.

Type annotations and code completion for `#!python session.create_client("license-manager").get_license_conversion_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_license_conversion_task.html)

```python
# get_license_conversion_task method definition

await def get_license_conversion_task(
    self,
    *,
    LicenseConversionTaskId: str,
) -> GetLicenseConversionTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLicenseConversionTaskResponseTypeDef](./type_defs.md#getlicenseconversiontaskresponsetypedef) 


```python
# get_license_conversion_task method usage example with argument unpacking

kwargs: GetLicenseConversionTaskRequestTypeDef = {  # (1)
    "LicenseConversionTaskId": ...,
}

parent.get_license_conversion_task(**kwargs)
```

1. See [:material-code-braces: GetLicenseConversionTaskRequestTypeDef](./type_defs.md#getlicenseconversiontaskrequesttypedef) 

### get\_license\_manager\_report\_generator

Gets information about the specified report generator.

Type annotations and code completion for `#!python session.create_client("license-manager").get_license_manager_report_generator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_license_manager_report_generator.html)

```python
# get_license_manager_report_generator method definition

await def get_license_manager_report_generator(
    self,
    *,
    LicenseManagerReportGeneratorArn: str,
) -> GetLicenseManagerReportGeneratorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLicenseManagerReportGeneratorResponseTypeDef](./type_defs.md#getlicensemanagerreportgeneratorresponsetypedef) 


```python
# get_license_manager_report_generator method usage example with argument unpacking

kwargs: GetLicenseManagerReportGeneratorRequestTypeDef = {  # (1)
    "LicenseManagerReportGeneratorArn": ...,
}

parent.get_license_manager_report_generator(**kwargs)
```

1. See [:material-code-braces: GetLicenseManagerReportGeneratorRequestTypeDef](./type_defs.md#getlicensemanagerreportgeneratorrequesttypedef) 

### get\_license\_usage

Gets detailed information about the usage of the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").get_license_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_license_usage.html)

```python
# get_license_usage method definition

await def get_license_usage(
    self,
    *,
    LicenseArn: str,
) -> GetLicenseUsageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLicenseUsageResponseTypeDef](./type_defs.md#getlicenseusageresponsetypedef) 


```python
# get_license_usage method usage example with argument unpacking

kwargs: GetLicenseUsageRequestTypeDef = {  # (1)
    "LicenseArn": ...,
}

parent.get_license_usage(**kwargs)
```

1. See [:material-code-braces: GetLicenseUsageRequestTypeDef](./type_defs.md#getlicenseusagerequesttypedef) 

### get\_service\_settings

Gets the License Manager settings for the current Region.

Type annotations and code completion for `#!python session.create_client("license-manager").get_service_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/get_service_settings.html)

```python
# get_service_settings method definition

await def get_service_settings(
    self,
) -> GetServiceSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceSettingsResponseTypeDef](./type_defs.md#getservicesettingsresponsetypedef) 

### list\_associations\_for\_license\_configuration

Lists the resource associations for the specified license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").list_associations_for_license_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_associations_for_license_configuration.html)

```python
# list_associations_for_license_configuration method definition

await def list_associations_for_license_configuration(
    self,
    *,
    LicenseConfigurationArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAssociationsForLicenseConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssociationsForLicenseConfigurationResponseTypeDef](./type_defs.md#listassociationsforlicenseconfigurationresponsetypedef) 


```python
# list_associations_for_license_configuration method usage example with argument unpacking

kwargs: ListAssociationsForLicenseConfigurationRequestTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.list_associations_for_license_configuration(**kwargs)
```

1. See [:material-code-braces: ListAssociationsForLicenseConfigurationRequestTypeDef](./type_defs.md#listassociationsforlicenseconfigurationrequesttypedef) 

### list\_distributed\_grants

Lists the grants distributed for the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").list_distributed_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_distributed_grants.html)

```python
# list_distributed_grants method definition

await def list_distributed_grants(
    self,
    *,
    GrantArns: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDistributedGrantsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListDistributedGrantsResponseTypeDef](./type_defs.md#listdistributedgrantsresponsetypedef) 


```python
# list_distributed_grants method usage example with argument unpacking

kwargs: ListDistributedGrantsRequestTypeDef = {  # (1)
    "GrantArns": ...,
}

parent.list_distributed_grants(**kwargs)
```

1. See [:material-code-braces: ListDistributedGrantsRequestTypeDef](./type_defs.md#listdistributedgrantsrequesttypedef) 

### list\_failures\_for\_license\_configuration\_operations

Lists the license configuration operations that failed.

Type annotations and code completion for `#!python session.create_client("license-manager").list_failures_for_license_configuration_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_failures_for_license_configuration_operations.html)

```python
# list_failures_for_license_configuration_operations method definition

await def list_failures_for_license_configuration_operations(
    self,
    *,
    LicenseConfigurationArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFailuresForLicenseConfigurationOperationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFailuresForLicenseConfigurationOperationsResponseTypeDef](./type_defs.md#listfailuresforlicenseconfigurationoperationsresponsetypedef) 


```python
# list_failures_for_license_configuration_operations method usage example with argument unpacking

kwargs: ListFailuresForLicenseConfigurationOperationsRequestTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.list_failures_for_license_configuration_operations(**kwargs)
```

1. See [:material-code-braces: ListFailuresForLicenseConfigurationOperationsRequestTypeDef](./type_defs.md#listfailuresforlicenseconfigurationoperationsrequesttypedef) 

### list\_license\_configurations

Lists the license configurations for your account.

Type annotations and code completion for `#!python session.create_client("license-manager").list_license_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_license_configurations.html)

```python
# list_license_configurations method definition

await def list_license_configurations(
    self,
    *,
    LicenseConfigurationArns: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListLicenseConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLicenseConfigurationsResponseTypeDef](./type_defs.md#listlicenseconfigurationsresponsetypedef) 


```python
# list_license_configurations method usage example with argument unpacking

kwargs: ListLicenseConfigurationsRequestTypeDef = {  # (1)
    "LicenseConfigurationArns": ...,
}

parent.list_license_configurations(**kwargs)
```

1. See [:material-code-braces: ListLicenseConfigurationsRequestTypeDef](./type_defs.md#listlicenseconfigurationsrequesttypedef) 

### list\_license\_conversion\_tasks

Lists the license type conversion tasks for your account.

Type annotations and code completion for `#!python session.create_client("license-manager").list_license_conversion_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_license_conversion_tasks.html)

```python
# list_license_conversion_tasks method definition

await def list_license_conversion_tasks(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListLicenseConversionTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLicenseConversionTasksResponseTypeDef](./type_defs.md#listlicenseconversiontasksresponsetypedef) 


```python
# list_license_conversion_tasks method usage example with argument unpacking

kwargs: ListLicenseConversionTasksRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_license_conversion_tasks(**kwargs)
```

1. See [:material-code-braces: ListLicenseConversionTasksRequestTypeDef](./type_defs.md#listlicenseconversiontasksrequesttypedef) 

### list\_license\_manager\_report\_generators

Lists the report generators for your account.

Type annotations and code completion for `#!python session.create_client("license-manager").list_license_manager_report_generators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_license_manager_report_generators.html)

```python
# list_license_manager_report_generators method definition

await def list_license_manager_report_generators(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLicenseManagerReportGeneratorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLicenseManagerReportGeneratorsResponseTypeDef](./type_defs.md#listlicensemanagerreportgeneratorsresponsetypedef) 


```python
# list_license_manager_report_generators method usage example with argument unpacking

kwargs: ListLicenseManagerReportGeneratorsRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_license_manager_report_generators(**kwargs)
```

1. See [:material-code-braces: ListLicenseManagerReportGeneratorsRequestTypeDef](./type_defs.md#listlicensemanagerreportgeneratorsrequesttypedef) 

### list\_license\_specifications\_for\_resource

Describes the license configurations for the specified resource.

Type annotations and code completion for `#!python session.create_client("license-manager").list_license_specifications_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_license_specifications_for_resource.html)

```python
# list_license_specifications_for_resource method definition

await def list_license_specifications_for_resource(
    self,
    *,
    ResourceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLicenseSpecificationsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLicenseSpecificationsForResourceResponseTypeDef](./type_defs.md#listlicensespecificationsforresourceresponsetypedef) 


```python
# list_license_specifications_for_resource method usage example with argument unpacking

kwargs: ListLicenseSpecificationsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_license_specifications_for_resource(**kwargs)
```

1. See [:material-code-braces: ListLicenseSpecificationsForResourceRequestTypeDef](./type_defs.md#listlicensespecificationsforresourcerequesttypedef) 

### list\_license\_versions

Lists all versions of the specified license.

Type annotations and code completion for `#!python session.create_client("license-manager").list_license_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_license_versions.html)

```python
# list_license_versions method definition

await def list_license_versions(
    self,
    *,
    LicenseArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLicenseVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLicenseVersionsResponseTypeDef](./type_defs.md#listlicenseversionsresponsetypedef) 


```python
# list_license_versions method usage example with argument unpacking

kwargs: ListLicenseVersionsRequestTypeDef = {  # (1)
    "LicenseArn": ...,
}

parent.list_license_versions(**kwargs)
```

1. See [:material-code-braces: ListLicenseVersionsRequestTypeDef](./type_defs.md#listlicenseversionsrequesttypedef) 

### list\_licenses

Lists the licenses for your account.

Type annotations and code completion for `#!python session.create_client("license-manager").list_licenses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_licenses.html)

```python
# list_licenses method definition

await def list_licenses(
    self,
    *,
    LicenseArns: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLicensesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLicensesResponseTypeDef](./type_defs.md#listlicensesresponsetypedef) 


```python
# list_licenses method usage example with argument unpacking

kwargs: ListLicensesRequestTypeDef = {  # (1)
    "LicenseArns": ...,
}

parent.list_licenses(**kwargs)
```

1. See [:material-code-braces: ListLicensesRequestTypeDef](./type_defs.md#listlicensesrequesttypedef) 

### list\_received\_grants

Lists grants that are received.

Type annotations and code completion for `#!python session.create_client("license-manager").list_received_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_received_grants.html)

```python
# list_received_grants method definition

await def list_received_grants(
    self,
    *,
    GrantArns: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListReceivedGrantsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListReceivedGrantsResponseTypeDef](./type_defs.md#listreceivedgrantsresponsetypedef) 


```python
# list_received_grants method usage example with argument unpacking

kwargs: ListReceivedGrantsRequestTypeDef = {  # (1)
    "GrantArns": ...,
}

parent.list_received_grants(**kwargs)
```

1. See [:material-code-braces: ListReceivedGrantsRequestTypeDef](./type_defs.md#listreceivedgrantsrequesttypedef) 

### list\_received\_grants\_for\_organization

Lists the grants received for all accounts in the organization.

Type annotations and code completion for `#!python session.create_client("license-manager").list_received_grants_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_received_grants_for_organization.html)

```python
# list_received_grants_for_organization method definition

await def list_received_grants_for_organization(
    self,
    *,
    LicenseArn: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListReceivedGrantsForOrganizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListReceivedGrantsForOrganizationResponseTypeDef](./type_defs.md#listreceivedgrantsfororganizationresponsetypedef) 


```python
# list_received_grants_for_organization method usage example with argument unpacking

kwargs: ListReceivedGrantsForOrganizationRequestTypeDef = {  # (1)
    "LicenseArn": ...,
}

parent.list_received_grants_for_organization(**kwargs)
```

1. See [:material-code-braces: ListReceivedGrantsForOrganizationRequestTypeDef](./type_defs.md#listreceivedgrantsfororganizationrequesttypedef) 

### list\_received\_licenses

Lists received licenses.

Type annotations and code completion for `#!python session.create_client("license-manager").list_received_licenses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_received_licenses.html)

```python
# list_received_licenses method definition

await def list_received_licenses(
    self,
    *,
    LicenseArns: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListReceivedLicensesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListReceivedLicensesResponseTypeDef](./type_defs.md#listreceivedlicensesresponsetypedef) 


```python
# list_received_licenses method usage example with argument unpacking

kwargs: ListReceivedLicensesRequestTypeDef = {  # (1)
    "LicenseArns": ...,
}

parent.list_received_licenses(**kwargs)
```

1. See [:material-code-braces: ListReceivedLicensesRequestTypeDef](./type_defs.md#listreceivedlicensesrequesttypedef) 

### list\_received\_licenses\_for\_organization

Lists the licenses received for all accounts in the organization.

Type annotations and code completion for `#!python session.create_client("license-manager").list_received_licenses_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_received_licenses_for_organization.html)

```python
# list_received_licenses_for_organization method definition

await def list_received_licenses_for_organization(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListReceivedLicensesForOrganizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListReceivedLicensesForOrganizationResponseTypeDef](./type_defs.md#listreceivedlicensesfororganizationresponsetypedef) 


```python
# list_received_licenses_for_organization method usage example with argument unpacking

kwargs: ListReceivedLicensesForOrganizationRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_received_licenses_for_organization(**kwargs)
```

1. See [:material-code-braces: ListReceivedLicensesForOrganizationRequestTypeDef](./type_defs.md#listreceivedlicensesfororganizationrequesttypedef) 

### list\_resource\_inventory

Lists resources managed using Systems Manager inventory.

Type annotations and code completion for `#!python session.create_client("license-manager").list_resource_inventory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_resource_inventory.html)

```python
# list_resource_inventory method definition

await def list_resource_inventory(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[InventoryFilterTypeDef] = ...,  # (1)
) -> ListResourceInventoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: ListResourceInventoryResponseTypeDef](./type_defs.md#listresourceinventoryresponsetypedef) 


```python
# list_resource_inventory method usage example with argument unpacking

kwargs: ListResourceInventoryRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resource_inventory(**kwargs)
```

1. See [:material-code-braces: ListResourceInventoryRequestTypeDef](./type_defs.md#listresourceinventoryrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_tags_for_resource.html)

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

### list\_tokens

Lists your tokens.

Type annotations and code completion for `#!python session.create_client("license-manager").list_tokens` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_tokens.html)

```python
# list_tokens method definition

await def list_tokens(
    self,
    *,
    TokenIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTokensResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListTokensResponseTypeDef](./type_defs.md#listtokensresponsetypedef) 


```python
# list_tokens method usage example with argument unpacking

kwargs: ListTokensRequestTypeDef = {  # (1)
    "TokenIds": ...,
}

parent.list_tokens(**kwargs)
```

1. See [:material-code-braces: ListTokensRequestTypeDef](./type_defs.md#listtokensrequesttypedef) 

### list\_usage\_for\_license\_configuration

Lists all license usage records for a license configuration, displaying license
consumption details by resource at a selected point in time.

Type annotations and code completion for `#!python session.create_client("license-manager").list_usage_for_license_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/list_usage_for_license_configuration.html)

```python
# list_usage_for_license_configuration method definition

await def list_usage_for_license_configuration(
    self,
    *,
    LicenseConfigurationArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListUsageForLicenseConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListUsageForLicenseConfigurationResponseTypeDef](./type_defs.md#listusageforlicenseconfigurationresponsetypedef) 


```python
# list_usage_for_license_configuration method usage example with argument unpacking

kwargs: ListUsageForLicenseConfigurationRequestTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.list_usage_for_license_configuration(**kwargs)
```

1. See [:material-code-braces: ListUsageForLicenseConfigurationRequestTypeDef](./type_defs.md#listusageforlicenseconfigurationrequesttypedef) 

### reject\_grant

Rejects the specified grant.

Type annotations and code completion for `#!python session.create_client("license-manager").reject_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/reject_grant.html)

```python
# reject_grant method definition

await def reject_grant(
    self,
    *,
    GrantArn: str,
) -> RejectGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RejectGrantResponseTypeDef](./type_defs.md#rejectgrantresponsetypedef) 


```python
# reject_grant method usage example with argument unpacking

kwargs: RejectGrantRequestTypeDef = {  # (1)
    "GrantArn": ...,
}

parent.reject_grant(**kwargs)
```

1. See [:material-code-braces: RejectGrantRequestTypeDef](./type_defs.md#rejectgrantrequesttypedef) 

### tag\_resource

Adds the specified tags to the specified license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes the specified tags from the specified license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
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

### update\_license\_configuration

Modifies the attributes of an existing license configuration.

Type annotations and code completion for `#!python session.create_client("license-manager").update_license_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/update_license_configuration.html)

```python
# update_license_configuration method definition

await def update_license_configuration(
    self,
    *,
    LicenseConfigurationArn: str,
    LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,  # (1)
    LicenseRules: Sequence[str] = ...,
    LicenseCount: int = ...,
    LicenseCountHardLimit: bool = ...,
    Name: str = ...,
    Description: str = ...,
    ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,  # (2)
    DisassociateWhenNotFound: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: LicenseConfigurationStatusType](./literals.md#licenseconfigurationstatustype) 
2. See [:material-code-braces: ProductInformationTypeDef](./type_defs.md#productinformationtypedef) [:material-code-braces: ProductInformationOutputTypeDef](./type_defs.md#productinformationoutputtypedef) 


```python
# update_license_configuration method usage example with argument unpacking

kwargs: UpdateLicenseConfigurationRequestTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.update_license_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateLicenseConfigurationRequestTypeDef](./type_defs.md#updatelicenseconfigurationrequesttypedef) 

### update\_license\_manager\_report\_generator

Updates a report generator.

Type annotations and code completion for `#!python session.create_client("license-manager").update_license_manager_report_generator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/update_license_manager_report_generator.html)

```python
# update_license_manager_report_generator method definition

await def update_license_manager_report_generator(
    self,
    *,
    LicenseManagerReportGeneratorArn: str,
    ReportGeneratorName: str,
    Type: Sequence[ReportTypeType],  # (1)
    ReportContext: ReportContextUnionTypeDef,  # (2)
    ReportFrequency: ReportFrequencyTypeDef,  # (3)
    ClientToken: str,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ReportContextTypeDef](./type_defs.md#reportcontexttypedef) [:material-code-braces: ReportContextOutputTypeDef](./type_defs.md#reportcontextoutputtypedef) 
3. See [:material-code-braces: ReportFrequencyTypeDef](./type_defs.md#reportfrequencytypedef) 


```python
# update_license_manager_report_generator method usage example with argument unpacking

kwargs: UpdateLicenseManagerReportGeneratorRequestTypeDef = {  # (1)
    "LicenseManagerReportGeneratorArn": ...,
    "ReportGeneratorName": ...,
    "Type": ...,
    "ReportContext": ...,
    "ReportFrequency": ...,
    "ClientToken": ...,
}

parent.update_license_manager_report_generator(**kwargs)
```

1. See [:material-code-braces: UpdateLicenseManagerReportGeneratorRequestTypeDef](./type_defs.md#updatelicensemanagerreportgeneratorrequesttypedef) 

### update\_license\_specifications\_for\_resource

Adds or removes the specified license configurations for the specified Amazon
Web Services resource.

Type annotations and code completion for `#!python session.create_client("license-manager").update_license_specifications_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/update_license_specifications_for_resource.html)

```python
# update_license_specifications_for_resource method definition

await def update_license_specifications_for_resource(
    self,
    *,
    ResourceArn: str,
    AddLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,  # (1)
    RemoveLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LicenseSpecificationTypeDef](./type_defs.md#licensespecificationtypedef) 
2. See [:material-code-braces: LicenseSpecificationTypeDef](./type_defs.md#licensespecificationtypedef) 


```python
# update_license_specifications_for_resource method usage example with argument unpacking

kwargs: UpdateLicenseSpecificationsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.update_license_specifications_for_resource(**kwargs)
```

1. See [:material-code-braces: UpdateLicenseSpecificationsForResourceRequestTypeDef](./type_defs.md#updatelicensespecificationsforresourcerequesttypedef) 

### update\_service\_settings

Updates License Manager settings for the current Region.

Type annotations and code completion for `#!python session.create_client("license-manager").update_service_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/client/update_service_settings.html)

```python
# update_service_settings method definition

await def update_service_settings(
    self,
    *,
    S3BucketArn: str = ...,
    SnsTopicArn: str = ...,
    OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,  # (1)
    EnableCrossAccountsDiscovery: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: OrganizationConfigurationTypeDef](./type_defs.md#organizationconfigurationtypedef) 


```python
# update_service_settings method usage example with argument unpacking

kwargs: UpdateServiceSettingsRequestTypeDef = {  # (1)
    "S3BucketArn": ...,
}

parent.update_service_settings(**kwargs)
```

1. See [:material-code-braces: UpdateServiceSettingsRequestTypeDef](./type_defs.md#updateservicesettingsrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("license-manager").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("license-manager").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("license-manager").get_paginator` method with overloads.

- `client.get_paginator("list_associations_for_license_configuration")` -> [ListAssociationsForLicenseConfigurationPaginator](./paginators.md#listassociationsforlicenseconfigurationpaginator)
- `client.get_paginator("list_license_configurations")` -> [ListLicenseConfigurationsPaginator](./paginators.md#listlicenseconfigurationspaginator)
- `client.get_paginator("list_license_specifications_for_resource")` -> [ListLicenseSpecificationsForResourcePaginator](./paginators.md#listlicensespecificationsforresourcepaginator)
- `client.get_paginator("list_resource_inventory")` -> [ListResourceInventoryPaginator](./paginators.md#listresourceinventorypaginator)
- `client.get_paginator("list_usage_for_license_configuration")` -> [ListUsageForLicenseConfigurationPaginator](./paginators.md#listusageforlicenseconfigurationpaginator)



