# CloudSearchClient

> [Index](../README.md) > [CloudSearch](./README.md) > CloudSearchClient

!!! note ""

    Auto-generated documentation for [CloudSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#cloudsearch)
    type annotations stubs module [types-aiobotocore-cloudsearch](https://pypi.org/project/types-aiobotocore-cloudsearch/).

## CloudSearchClient

Type annotations and code completion for `#!python session.create_client("cloudsearch")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client)

```python
# CloudSearchClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cloudsearch.client import CloudSearchClient

session = get_session()
async with session.create_client("cloudsearch") as client:
    client: CloudSearchClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudsearch").exceptions` structure.

```python
# CloudSearchClient.exceptions usage example

async with session.create_client("cloudsearch") as client:
    try:
        do_something(client)
    except (
            client.BaseException,
        client.ClientError,
        client.DisabledOperationException,
        client.InternalException,
        client.InvalidTypeException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CloudSearchClient usage type checking example

from types_aiobotocore_cloudsearch.client import Exceptions

def handle_error(exc: Exceptions.BaseException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("cloudsearch").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("cloudsearch").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("cloudsearch").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### build\_suggesters

Indexes the search suggestions.

Type annotations and code completion for `#!python session.create_client("cloudsearch").build_suggesters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/build_suggesters.html)

```python
# build_suggesters method definition

await def build_suggesters(
    self,
    *,
    DomainName: str,
) -> BuildSuggestersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BuildSuggestersResponseTypeDef](./type_defs.md#buildsuggestersresponsetypedef) 


```python
# build_suggesters method usage example with argument unpacking

kwargs: BuildSuggestersRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.build_suggesters(**kwargs)
```

1. See [:material-code-braces: BuildSuggestersRequestRequestTypeDef](./type_defs.md#buildsuggestersrequestrequesttypedef) 

### create\_domain

Creates a new search domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").create_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/create_domain.html)

```python
# create_domain method definition

await def create_domain(
    self,
    *,
    DomainName: str,
) -> CreateDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef) 


```python
# create_domain method usage example with argument unpacking

kwargs: CreateDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.create_domain(**kwargs)
```

1. See [:material-code-braces: CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef) 

### define\_analysis\_scheme

Configures an analysis scheme that can be applied to a <code>text</code> or
<code>text-array</code> field to define language-specific text processing
options.

Type annotations and code completion for `#!python session.create_client("cloudsearch").define_analysis_scheme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/define_analysis_scheme.html)

```python
# define_analysis_scheme method definition

await def define_analysis_scheme(
    self,
    *,
    DomainName: str,
    AnalysisScheme: AnalysisSchemeTypeDef,  # (1)
) -> DefineAnalysisSchemeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnalysisSchemeTypeDef](./type_defs.md#analysisschemetypedef) 
2. See [:material-code-braces: DefineAnalysisSchemeResponseTypeDef](./type_defs.md#defineanalysisschemeresponsetypedef) 


```python
# define_analysis_scheme method usage example with argument unpacking

kwargs: DefineAnalysisSchemeRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "AnalysisScheme": ...,
}

parent.define_analysis_scheme(**kwargs)
```

1. See [:material-code-braces: DefineAnalysisSchemeRequestRequestTypeDef](./type_defs.md#defineanalysisschemerequestrequesttypedef) 

### define\_expression

Configures an <code><a>Expression</a></code> for the search domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").define_expression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/define_expression.html)

```python
# define_expression method definition

await def define_expression(
    self,
    *,
    DomainName: str,
    Expression: ExpressionTypeDef,  # (1)
) -> DefineExpressionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: DefineExpressionResponseTypeDef](./type_defs.md#defineexpressionresponsetypedef) 


```python
# define_expression method usage example with argument unpacking

kwargs: DefineExpressionRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Expression": ...,
}

parent.define_expression(**kwargs)
```

1. See [:material-code-braces: DefineExpressionRequestRequestTypeDef](./type_defs.md#defineexpressionrequestrequesttypedef) 

### define\_index\_field

Configures an <code><a>IndexField</a></code> for the search domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").define_index_field` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/define_index_field.html)

```python
# define_index_field method definition

await def define_index_field(
    self,
    *,
    DomainName: str,
    IndexField: IndexFieldTypeDef,  # (1)
) -> DefineIndexFieldResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IndexFieldTypeDef](./type_defs.md#indexfieldtypedef) 
2. See [:material-code-braces: DefineIndexFieldResponseTypeDef](./type_defs.md#defineindexfieldresponsetypedef) 


```python
# define_index_field method usage example with argument unpacking

kwargs: DefineIndexFieldRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "IndexField": ...,
}

parent.define_index_field(**kwargs)
```

1. See [:material-code-braces: DefineIndexFieldRequestRequestTypeDef](./type_defs.md#defineindexfieldrequestrequesttypedef) 

### define\_suggester

Configures a suggester for a domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").define_suggester` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/define_suggester.html)

```python
# define_suggester method definition

await def define_suggester(
    self,
    *,
    DomainName: str,
    Suggester: SuggesterTypeDef,  # (1)
) -> DefineSuggesterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SuggesterTypeDef](./type_defs.md#suggestertypedef) 
2. See [:material-code-braces: DefineSuggesterResponseTypeDef](./type_defs.md#definesuggesterresponsetypedef) 


```python
# define_suggester method usage example with argument unpacking

kwargs: DefineSuggesterRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Suggester": ...,
}

parent.define_suggester(**kwargs)
```

1. See [:material-code-braces: DefineSuggesterRequestRequestTypeDef](./type_defs.md#definesuggesterrequestrequesttypedef) 

### delete\_analysis\_scheme

Deletes an analysis scheme.

Type annotations and code completion for `#!python session.create_client("cloudsearch").delete_analysis_scheme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/delete_analysis_scheme.html)

```python
# delete_analysis_scheme method definition

await def delete_analysis_scheme(
    self,
    *,
    DomainName: str,
    AnalysisSchemeName: str,
) -> DeleteAnalysisSchemeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAnalysisSchemeResponseTypeDef](./type_defs.md#deleteanalysisschemeresponsetypedef) 


```python
# delete_analysis_scheme method usage example with argument unpacking

kwargs: DeleteAnalysisSchemeRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "AnalysisSchemeName": ...,
}

parent.delete_analysis_scheme(**kwargs)
```

1. See [:material-code-braces: DeleteAnalysisSchemeRequestRequestTypeDef](./type_defs.md#deleteanalysisschemerequestrequesttypedef) 

### delete\_domain

Permanently deletes a search domain and all of its data.

Type annotations and code completion for `#!python session.create_client("cloudsearch").delete_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/delete_domain.html)

```python
# delete_domain method definition

await def delete_domain(
    self,
    *,
    DomainName: str,
) -> DeleteDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDomainResponseTypeDef](./type_defs.md#deletedomainresponsetypedef) 


```python
# delete_domain method usage example with argument unpacking

kwargs: DeleteDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.delete_domain(**kwargs)
```

1. See [:material-code-braces: DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef) 

### delete\_expression

Removes an <code><a>Expression</a></code> from the search domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").delete_expression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/delete_expression.html)

```python
# delete_expression method definition

await def delete_expression(
    self,
    *,
    DomainName: str,
    ExpressionName: str,
) -> DeleteExpressionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteExpressionResponseTypeDef](./type_defs.md#deleteexpressionresponsetypedef) 


```python
# delete_expression method usage example with argument unpacking

kwargs: DeleteExpressionRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ExpressionName": ...,
}

parent.delete_expression(**kwargs)
```

1. See [:material-code-braces: DeleteExpressionRequestRequestTypeDef](./type_defs.md#deleteexpressionrequestrequesttypedef) 

### delete\_index\_field

Removes an <code><a>IndexField</a></code> from the search domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").delete_index_field` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/delete_index_field.html)

```python
# delete_index_field method definition

await def delete_index_field(
    self,
    *,
    DomainName: str,
    IndexFieldName: str,
) -> DeleteIndexFieldResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIndexFieldResponseTypeDef](./type_defs.md#deleteindexfieldresponsetypedef) 


```python
# delete_index_field method usage example with argument unpacking

kwargs: DeleteIndexFieldRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "IndexFieldName": ...,
}

parent.delete_index_field(**kwargs)
```

1. See [:material-code-braces: DeleteIndexFieldRequestRequestTypeDef](./type_defs.md#deleteindexfieldrequestrequesttypedef) 

### delete\_suggester

Deletes a suggester.

Type annotations and code completion for `#!python session.create_client("cloudsearch").delete_suggester` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/delete_suggester.html)

```python
# delete_suggester method definition

await def delete_suggester(
    self,
    *,
    DomainName: str,
    SuggesterName: str,
) -> DeleteSuggesterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSuggesterResponseTypeDef](./type_defs.md#deletesuggesterresponsetypedef) 


```python
# delete_suggester method usage example with argument unpacking

kwargs: DeleteSuggesterRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "SuggesterName": ...,
}

parent.delete_suggester(**kwargs)
```

1. See [:material-code-braces: DeleteSuggesterRequestRequestTypeDef](./type_defs.md#deletesuggesterrequestrequesttypedef) 

### describe\_analysis\_schemes

Gets the analysis schemes configured for a domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_analysis_schemes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_analysis_schemes.html)

```python
# describe_analysis_schemes method definition

await def describe_analysis_schemes(
    self,
    *,
    DomainName: str,
    AnalysisSchemeNames: Sequence[str] = ...,
    Deployed: bool = ...,
) -> DescribeAnalysisSchemesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAnalysisSchemesResponseTypeDef](./type_defs.md#describeanalysisschemesresponsetypedef) 


```python
# describe_analysis_schemes method usage example with argument unpacking

kwargs: DescribeAnalysisSchemesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_analysis_schemes(**kwargs)
```

1. See [:material-code-braces: DescribeAnalysisSchemesRequestRequestTypeDef](./type_defs.md#describeanalysisschemesrequestrequesttypedef) 

### describe\_availability\_options

Gets the availability options configured for a domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_availability_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_availability_options.html)

```python
# describe_availability_options method definition

await def describe_availability_options(
    self,
    *,
    DomainName: str,
    Deployed: bool = ...,
) -> DescribeAvailabilityOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAvailabilityOptionsResponseTypeDef](./type_defs.md#describeavailabilityoptionsresponsetypedef) 


```python
# describe_availability_options method usage example with argument unpacking

kwargs: DescribeAvailabilityOptionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_availability_options(**kwargs)
```

1. See [:material-code-braces: DescribeAvailabilityOptionsRequestRequestTypeDef](./type_defs.md#describeavailabilityoptionsrequestrequesttypedef) 

### describe\_domain\_endpoint\_options

Returns the domain's endpoint options, specifically whether all requests to the
domain must arrive over HTTPS.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_domain_endpoint_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_domain_endpoint_options.html)

```python
# describe_domain_endpoint_options method definition

await def describe_domain_endpoint_options(
    self,
    *,
    DomainName: str,
    Deployed: bool = ...,
) -> DescribeDomainEndpointOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainEndpointOptionsResponseTypeDef](./type_defs.md#describedomainendpointoptionsresponsetypedef) 


```python
# describe_domain_endpoint_options method usage example with argument unpacking

kwargs: DescribeDomainEndpointOptionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_domain_endpoint_options(**kwargs)
```

1. See [:material-code-braces: DescribeDomainEndpointOptionsRequestRequestTypeDef](./type_defs.md#describedomainendpointoptionsrequestrequesttypedef) 

### describe\_domains

Gets information about the search domains owned by this account.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_domains.html)

```python
# describe_domains method definition

await def describe_domains(
    self,
    *,
    DomainNames: Sequence[str] = ...,
) -> DescribeDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainsResponseTypeDef](./type_defs.md#describedomainsresponsetypedef) 


```python
# describe_domains method usage example with argument unpacking

kwargs: DescribeDomainsRequestRequestTypeDef = {  # (1)
    "DomainNames": ...,
}

parent.describe_domains(**kwargs)
```

1. See [:material-code-braces: DescribeDomainsRequestRequestTypeDef](./type_defs.md#describedomainsrequestrequesttypedef) 

### describe\_expressions

Gets the expressions configured for the search domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_expressions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_expressions.html)

```python
# describe_expressions method definition

await def describe_expressions(
    self,
    *,
    DomainName: str,
    ExpressionNames: Sequence[str] = ...,
    Deployed: bool = ...,
) -> DescribeExpressionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeExpressionsResponseTypeDef](./type_defs.md#describeexpressionsresponsetypedef) 


```python
# describe_expressions method usage example with argument unpacking

kwargs: DescribeExpressionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_expressions(**kwargs)
```

1. See [:material-code-braces: DescribeExpressionsRequestRequestTypeDef](./type_defs.md#describeexpressionsrequestrequesttypedef) 

### describe\_index\_fields

Gets information about the index fields configured for the search domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_index_fields` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_index_fields.html)

```python
# describe_index_fields method definition

await def describe_index_fields(
    self,
    *,
    DomainName: str,
    FieldNames: Sequence[str] = ...,
    Deployed: bool = ...,
) -> DescribeIndexFieldsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIndexFieldsResponseTypeDef](./type_defs.md#describeindexfieldsresponsetypedef) 


```python
# describe_index_fields method usage example with argument unpacking

kwargs: DescribeIndexFieldsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_index_fields(**kwargs)
```

1. See [:material-code-braces: DescribeIndexFieldsRequestRequestTypeDef](./type_defs.md#describeindexfieldsrequestrequesttypedef) 

### describe\_scaling\_parameters

Gets the scaling parameters configured for a domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_scaling_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_scaling_parameters.html)

```python
# describe_scaling_parameters method definition

await def describe_scaling_parameters(
    self,
    *,
    DomainName: str,
) -> DescribeScalingParametersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeScalingParametersResponseTypeDef](./type_defs.md#describescalingparametersresponsetypedef) 


```python
# describe_scaling_parameters method usage example with argument unpacking

kwargs: DescribeScalingParametersRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_scaling_parameters(**kwargs)
```

1. See [:material-code-braces: DescribeScalingParametersRequestRequestTypeDef](./type_defs.md#describescalingparametersrequestrequesttypedef) 

### describe\_service\_access\_policies

Gets information about the access policies that control access to the domain's
document and search endpoints.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_service_access_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_service_access_policies.html)

```python
# describe_service_access_policies method definition

await def describe_service_access_policies(
    self,
    *,
    DomainName: str,
    Deployed: bool = ...,
) -> DescribeServiceAccessPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServiceAccessPoliciesResponseTypeDef](./type_defs.md#describeserviceaccesspoliciesresponsetypedef) 


```python
# describe_service_access_policies method usage example with argument unpacking

kwargs: DescribeServiceAccessPoliciesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_service_access_policies(**kwargs)
```

1. See [:material-code-braces: DescribeServiceAccessPoliciesRequestRequestTypeDef](./type_defs.md#describeserviceaccesspoliciesrequestrequesttypedef) 

### describe\_suggesters

Gets the suggesters configured for a domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").describe_suggesters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/describe_suggesters.html)

```python
# describe_suggesters method definition

await def describe_suggesters(
    self,
    *,
    DomainName: str,
    SuggesterNames: Sequence[str] = ...,
    Deployed: bool = ...,
) -> DescribeSuggestersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSuggestersResponseTypeDef](./type_defs.md#describesuggestersresponsetypedef) 


```python
# describe_suggesters method usage example with argument unpacking

kwargs: DescribeSuggestersRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_suggesters(**kwargs)
```

1. See [:material-code-braces: DescribeSuggestersRequestRequestTypeDef](./type_defs.md#describesuggestersrequestrequesttypedef) 

### index\_documents

Tells the search domain to start indexing its documents using the latest
indexing options.

Type annotations and code completion for `#!python session.create_client("cloudsearch").index_documents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/index_documents.html)

```python
# index_documents method definition

await def index_documents(
    self,
    *,
    DomainName: str,
) -> IndexDocumentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: IndexDocumentsResponseTypeDef](./type_defs.md#indexdocumentsresponsetypedef) 


```python
# index_documents method usage example with argument unpacking

kwargs: IndexDocumentsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.index_documents(**kwargs)
```

1. See [:material-code-braces: IndexDocumentsRequestRequestTypeDef](./type_defs.md#indexdocumentsrequestrequesttypedef) 

### list\_domain\_names

Lists all search domains owned by an account.

Type annotations and code completion for `#!python session.create_client("cloudsearch").list_domain_names` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/list_domain_names.html)

```python
# list_domain_names method definition

await def list_domain_names(
    self,
) -> ListDomainNamesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainNamesResponseTypeDef](./type_defs.md#listdomainnamesresponsetypedef) 

### update\_availability\_options

Configures the availability options for a domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").update_availability_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/update_availability_options.html)

```python
# update_availability_options method definition

await def update_availability_options(
    self,
    *,
    DomainName: str,
    MultiAZ: bool,
) -> UpdateAvailabilityOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAvailabilityOptionsResponseTypeDef](./type_defs.md#updateavailabilityoptionsresponsetypedef) 


```python
# update_availability_options method usage example with argument unpacking

kwargs: UpdateAvailabilityOptionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "MultiAZ": ...,
}

parent.update_availability_options(**kwargs)
```

1. See [:material-code-braces: UpdateAvailabilityOptionsRequestRequestTypeDef](./type_defs.md#updateavailabilityoptionsrequestrequesttypedef) 

### update\_domain\_endpoint\_options

Updates the domain's endpoint options, specifically whether all requests to the
domain must arrive over HTTPS.

Type annotations and code completion for `#!python session.create_client("cloudsearch").update_domain_endpoint_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/update_domain_endpoint_options.html)

```python
# update_domain_endpoint_options method definition

await def update_domain_endpoint_options(
    self,
    *,
    DomainName: str,
    DomainEndpointOptions: DomainEndpointOptionsTypeDef,  # (1)
) -> UpdateDomainEndpointOptionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
2. See [:material-code-braces: UpdateDomainEndpointOptionsResponseTypeDef](./type_defs.md#updatedomainendpointoptionsresponsetypedef) 


```python
# update_domain_endpoint_options method usage example with argument unpacking

kwargs: UpdateDomainEndpointOptionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "DomainEndpointOptions": ...,
}

parent.update_domain_endpoint_options(**kwargs)
```

1. See [:material-code-braces: UpdateDomainEndpointOptionsRequestRequestTypeDef](./type_defs.md#updatedomainendpointoptionsrequestrequesttypedef) 

### update\_scaling\_parameters

Configures scaling parameters for a domain.

Type annotations and code completion for `#!python session.create_client("cloudsearch").update_scaling_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/update_scaling_parameters.html)

```python
# update_scaling_parameters method definition

await def update_scaling_parameters(
    self,
    *,
    DomainName: str,
    ScalingParameters: ScalingParametersTypeDef,  # (1)
) -> UpdateScalingParametersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ScalingParametersTypeDef](./type_defs.md#scalingparameterstypedef) 
2. See [:material-code-braces: UpdateScalingParametersResponseTypeDef](./type_defs.md#updatescalingparametersresponsetypedef) 


```python
# update_scaling_parameters method usage example with argument unpacking

kwargs: UpdateScalingParametersRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ScalingParameters": ...,
}

parent.update_scaling_parameters(**kwargs)
```

1. See [:material-code-braces: UpdateScalingParametersRequestRequestTypeDef](./type_defs.md#updatescalingparametersrequestrequesttypedef) 

### update\_service\_access\_policies

Configures the access rules that control access to the domain's document and
search endpoints.

Type annotations and code completion for `#!python session.create_client("cloudsearch").update_service_access_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch/client/update_service_access_policies.html)

```python
# update_service_access_policies method definition

await def update_service_access_policies(
    self,
    *,
    DomainName: str,
    AccessPolicies: str,
) -> UpdateServiceAccessPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServiceAccessPoliciesResponseTypeDef](./type_defs.md#updateserviceaccesspoliciesresponsetypedef) 


```python
# update_service_access_policies method usage example with argument unpacking

kwargs: UpdateServiceAccessPoliciesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "AccessPolicies": ...,
}

parent.update_service_access_policies(**kwargs)
```

1. See [:material-code-braces: UpdateServiceAccessPoliciesRequestRequestTypeDef](./type_defs.md#updateserviceaccesspoliciesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudsearch").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CloudSearchClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudsearch").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch.Client)

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





