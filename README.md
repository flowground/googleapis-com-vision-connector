# ![LOGO](logo.png) Cloud Vision **flow**ground Connector

## Description

A generated **flow**ground connector for the Cloud Vision API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/vision/v1/swagger.json<br/>
Generated at: 2019-05-07T17:42:06+03:00

## API Description

Integrates Google Vision features, including image labeling, face, logo, and landmark detection, optical character recognition (OCR), and detection of explicit content, into applications.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Run asynchronous image detection and annotation for a list of generic<br/>
> files, such as PDF files, which may contain multiple pages and multiple<br/>
> images per page. Progress and results can be retrieved through the<br/>
> `google.longrunning.Operations` interface.<br/>
> `Operation.metadata` contains `OperationMetadata` (metadata).<br/>
> `Operation.response` contains `AsyncBatchAnnotateFilesResponse` (results).

*Tags:* `files`

#### Input Parameters
* `$.xgafv` - _optional_ - V1 error format.
    Possible values: 1, 2.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Run image detection and annotation for a batch of images.

*Tags:* `images`

#### Input Parameters
* `$.xgafv` - _optional_ - V1 error format.
    Possible values: 1, 2.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Permanently deletes a ProductSet. Products and ReferenceImages in the<br/>
> ProductSet are not deleted.<br/>
> <br/>
> The actual image files are not deleted from Google Cloud Storage.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns NOT_FOUND if the ProductSet does not exist.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - Resource name of the ProductSet to delete.

Format is:
`projects/PROJECT_ID/locations/LOC_ID/productSets/PRODUCT_SET_ID`
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets information associated with a ProductSet.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns NOT_FOUND if the ProductSet does not exist.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - Resource name of the ProductSet to get.

Format is:
`projects/PROJECT_ID/locations/LOG_ID/productSets/PRODUCT_SET_ID`
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Makes changes to a ProductSet resource.<br/>
> Only display_name can be updated currently.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns NOT_FOUND if the ProductSet does not exist.<br/>
> * Returns INVALID_ARGUMENT if display_name is present in update_mask but<br/>
>   missing from the request or longer than 4096 characters.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The resource name of the ProductSet.

Format is:
`projects/PROJECT_ID/locations/LOC_ID/productSets/PRODUCT_SET_ID`.

This field is ignored when creating a ProductSet.
* `updateMask` - _optional_ - The FieldMask that specifies which fields to
update.
If update_mask isn't specified, all mutable fields are to be updated.
Valid mask path is `display_name`.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists the Products in a ProductSet, in an unspecified order. If the<br/>
> ProductSet does not exist, the products field of the response will be<br/>
> empty.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns INVALID_ARGUMENT if page_size is greater than 100 or less than 1.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The ProductSet resource for which to retrieve Products.

Format is:
`projects/PROJECT_ID/locations/LOC_ID/productSets/PRODUCT_SET_ID`
* `pageSize` - _optional_ - The maximum number of items to return. Default 10, maximum 100.
* `pageToken` - _optional_ - The next_page_token returned from a previous List request, if any.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Adds a Product to the specified ProductSet. If the Product is already<br/>
> present, no change is made.<br/>
> <br/>
> One Product can be added to at most 100 ProductSets.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns NOT_FOUND if the Product or the ProductSet doesn't exist.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The resource name for the ProductSet to modify.

Format is:
`projects/PROJECT_ID/locations/LOC_ID/productSets/PRODUCT_SET_ID`
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Starts asynchronous cancellation on a long-running operation.  The server<br/>
> makes a best effort to cancel the operation, but success is not<br/>
> guaranteed.  If the server doesn't support this method, it returns<br/>
> `google.rpc.Code.UNIMPLEMENTED`.  Clients can use<br/>
> Operations.GetOperation or<br/>
> other methods to check whether the cancellation succeeded or whether the<br/>
> operation completed despite cancellation. On successful cancellation,<br/>
> the operation is not deleted; instead, it becomes an operation with<br/>
> an Operation.error value with a google.rpc.Status.code of 1,<br/>
> corresponding to `Code.CANCELLED`.

*Tags:* `operations`

#### Input Parameters
* `name` - _required_ - The name of the operation resource to be cancelled.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Removes a Product from the specified ProductSet.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns NOT_FOUND If the Product is not found under the ProductSet.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The resource name for the ProductSet to modify.

Format is:
`projects/PROJECT_ID/locations/LOC_ID/productSets/PRODUCT_SET_ID`
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists ProductSets in an unspecified order.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns INVALID_ARGUMENT if page_size is greater than 100, or less<br/>
>   than 1.

*Tags:* `projects`

#### Input Parameters
* `pageSize` - _optional_ - The maximum number of items to return. Default 10, maximum 100.
* `pageToken` - _optional_ - The next_page_token returned from a previous List request, if any.
* `parent` - _required_ - The project from which ProductSets should be listed.

Format is `projects/PROJECT_ID/locations/LOC_ID`.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates and returns a new ProductSet resource.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns INVALID_ARGUMENT if display_name is missing, or is longer than<br/>
>   4096 characters.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - The project in which the ProductSet should be created.

Format is `projects/PROJECT_ID/locations/LOC_ID`.
* `productSetId` - _optional_ - A user-supplied resource id for this ProductSet. If set, the server will
attempt to use this value as the resource id. If it is already in use, an
error is returned with code ALREADY_EXISTS. Must be at most 128 characters
long. It cannot contain the character `/`.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Asynchronous API that imports a list of reference images to specified<br/>
> product sets based on a list of image information.<br/>
> <br/>
> The google.longrunning.Operation API can be used to keep track of the<br/>
> progress and results of the request.<br/>
> `Operation.metadata` contains `BatchOperationMetadata`. (progress)<br/>
> `Operation.response` contains `ImportProductSetsResponse`. (results)<br/>
> <br/>
> The input source of this method is a csv file on Google Cloud Storage.<br/>
> For the format of the csv file please see<br/>
> ImportProductSetsGcsSource.csv_file_uri.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - The project in which the ProductSets should be imported.

Format is `projects/PROJECT_ID/locations/LOC_ID`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists products in an unspecified order.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns INVALID_ARGUMENT if page_size is greater than 100 or less than 1.

*Tags:* `projects`

#### Input Parameters
* `pageSize` - _optional_ - The maximum number of items to return. Default 10, maximum 100.
* `pageToken` - _optional_ - The next_page_token returned from a previous List request, if any.
* `parent` - _required_ - The project OR ProductSet from which Products should be listed.

Format:
`projects/PROJECT_ID/locations/LOC_ID`
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates and returns a new product resource.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns INVALID_ARGUMENT if display_name is missing or longer than 4096<br/>
>   characters.<br/>
> * Returns INVALID_ARGUMENT if description is longer than 4096 characters.<br/>
> * Returns INVALID_ARGUMENT if product_category is missing or invalid.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - The project in which the Product should be created.

Format is
`projects/PROJECT_ID/locations/LOC_ID`.
* `productId` - _optional_ - A user-supplied resource id for this Product. If set, the server will
attempt to use this value as the resource id. If it is already in use, an
error is returned with code ALREADY_EXISTS. Must be at most 128 characters
long. It cannot contain the character `/`.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists reference images.<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns NOT_FOUND if the parent product does not exist.<br/>
> * Returns INVALID_ARGUMENT if the page_size is greater than 100, or less<br/>
>   than 1.

*Tags:* `projects`

#### Input Parameters
* `pageSize` - _optional_ - The maximum number of items to return. Default 10, maximum 100.
* `pageToken` - _optional_ - A token identifying a page of results to be returned. This is the value
of `nextPageToken` returned in a previous reference image list request.

Defaults to the first page if not specified.
* `parent` - _required_ - Resource name of the product containing the reference images.

Format is
`projects/PROJECT_ID/locations/LOC_ID/products/PRODUCT_ID`.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates and returns a new ReferenceImage resource.<br/>
> <br/>
> The `bounding_poly` field is optional. If `bounding_poly` is not specified,<br/>
> the system will try to detect regions of interest in the image that are<br/>
> compatible with the product_category on the parent product. If it is<br/>
> specified, detection is ALWAYS skipped. The system converts polygons into<br/>
> non-rotated rectangles.<br/>
> <br/>
> Note that the pipeline will resize the image if the image resolution is too<br/>
> large to process (above 50MP).<br/>
> <br/>
> Possible errors:<br/>
> <br/>
> * Returns INVALID_ARGUMENT if the image_uri is missing or longer than 4096<br/>
>   characters.<br/>
> * Returns INVALID_ARGUMENT if the product does not exist.<br/>
> * Returns INVALID_ARGUMENT if bounding_poly is not provided, and nothing<br/>
>   compatible with the parent product's product_category is detected.<br/>
> * Returns INVALID_ARGUMENT if bounding_poly contains more than 10 polygons.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - Resource name of the product in which to create the reference image.

Format is
`projects/PROJECT_ID/locations/LOC_ID/products/PRODUCT_ID`.
* `referenceImageId` - _optional_ - A user-supplied resource id for the ReferenceImage to be added. If set,
the server will attempt to use this value as the resource id. If it is
already in use, an error is returned with code ALREADY_EXISTS. Must be at
most 128 characters long. It cannot contain the character `/`.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-vision-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
