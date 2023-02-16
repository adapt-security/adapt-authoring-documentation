# Errors Reference

This page documents all errors which are likely to be thrown in the system, along with the appropriate HTTP status code and any supplemental data which is stored with the error. 

Supplemental data can be used at the point that errors are translated to provide more context to a specific error. All data stored with an error can be assumed to be a primitive type for easy printing.

### Quick navigation

<ul class="toc">
<li><a href="#/errorsref?id=ACCOUNT_DISABLED">ACCOUNT_DISABLED</a></li>
<li><a href="#/errorsref?id=ACCOUNT_LOCKED_PERM">ACCOUNT_LOCKED_PERM</a></li>
<li><a href="#/errorsref?id=ACCOUNT_LOCKED_TEMP">ACCOUNT_LOCKED_TEMP</a></li>
<li><a href="#/errorsref?id=ACCOUNT_NOT_LOCALAUTHD">ACCOUNT_NOT_LOCALAUTHD</a></li>
<li><a href="#/errorsref?id=API_MODULE_INVALID_CLASS">API_MODULE_INVALID_CLASS</a></li>
<li><a href="#/errorsref?id=ASSET_TYPE_EXISTS">ASSET_TYPE_EXISTS</a></li>
<li><a href="#/errorsref?id=ASSET_TYPE_INVALID">ASSET_TYPE_INVALID</a></li>
<li><a href="#/errorsref?id=ASSET_TYPE_UNKNOWN">ASSET_TYPE_UNKNOWN</a></li>
<li><a href="#/errorsref?id=AUTH_HEADER_UNSUPPORTED">AUTH_HEADER_UNSUPPORTED</a></li>
<li><a href="#/errorsref?id=AUTH_PLUGIN_INVALID_CLASS">AUTH_PLUGIN_INVALID_CLASS</a></li>
<li><a href="#/errorsref?id=AUTH_TOKEN_EXPIRED">AUTH_TOKEN_EXPIRED</a></li>
<li><a href="#/errorsref?id=AUTH_TOKEN_INVALID">AUTH_TOKEN_INVALID</a></li>
<li><a href="#/errorsref?id=AUTH_TOKEN_NOT_BEFORE">AUTH_TOKEN_NOT_BEFORE</a></li>
<li><a href="#/errorsref?id=AUTH_TYPE_DEF_MISSING">AUTH_TYPE_DEF_MISSING</a></li>
<li><a href="#/errorsref?id=BODY_PARSE_FAILED">BODY_PARSE_FAILED</a></li>
<li><a href="#/errorsref?id=BROWSERSLIST_UPDATE_FAILED">BROWSERSLIST_UPDATE_FAILED</a></li>
<li><a href="#/errorsref?id=BUILD_DATA_RETRIEVAL_FAILED">BUILD_DATA_RETRIEVAL_FAILED</a></li>
<li><a href="#/errorsref?id=BUILD_NOT_FOUND">BUILD_NOT_FOUND</a></li>
<li><a href="#/errorsref?id=CLI_BUILD_FAILED">CLI_BUILD_FAILED</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_ALREADY_EXISTS">CONTENTPLUGIN_ALREADY_EXISTS</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_ATTR_CLASH">CONTENTPLUGIN_ATTR_CLASH</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_ATTR_MISSING">CONTENTPLUGIN_ATTR_MISSING</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_CLI_INSTALL_FAILED">CONTENTPLUGIN_CLI_INSTALL_FAILED</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_INCOMPAT_FW">CONTENTPLUGIN_INCOMPAT_FW</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_INSTALL_FAILED">CONTENTPLUGIN_INSTALL_FAILED</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_INVALID_ZIP">CONTENTPLUGIN_INVALID_ZIP</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_IN_USE">CONTENTPLUGIN_IN_USE</a></li>
<li><a href="#/errorsref?id=CONTENTPLUGIN_NEWER_INSTALLED">CONTENTPLUGIN_NEWER_INSTALLED</a></li>
<li><a href="#/errorsref?id=COURSE_NOT_FOUND">COURSE_NOT_FOUND</a></li>
<li><a href="#/errorsref?id=DESTROY_SESSION_FAIL">DESTROY_SESSION_FAIL</a></li>
<li><a href="#/errorsref?id=DUPL_AUTHORED_MODULE_NAME">DUPL_AUTHORED_MODULE_NAME</a></li>
<li><a href="#/errorsref?id=DUPL_AUTH_PLUGIN_REG">DUPL_AUTH_PLUGIN_REG</a></li>
<li><a href="#/errorsref?id=DUPL_USER">DUPL_USER</a></li>
<li><a href="#/errorsref?id=EACCES">EACCES</a></li>
<li><a href="#/errorsref?id=EADDRINUSE">EADDRINUSE</a></li>
<li><a href="#/errorsref?id=ECONNREFUSED">ECONNREFUSED</a></li>
<li><a href="#/errorsref?id=EEXIST">EEXIST</a></li>
<li><a href="#/errorsref?id=ENDPOINT_NOT_FOUND">ENDPOINT_NOT_FOUND</a></li>
<li><a href="#/errorsref?id=ENOENT">ENOENT</a></li>
<li><a href="#/errorsref?id=ENOTEMPTY">ENOTEMPTY</a></li>
<li><a href="#/errorsref?id=FILE_EXCEEDS_MAX_SIZE">FILE_EXCEEDS_MAX_SIZE</a></li>
<li><a href="#/errorsref?id=FILE_SYNTAX_ERROR">FILE_SYNTAX_ERROR</a></li>
<li><a href="#/errorsref?id=FUNC_DISABLED">FUNC_DISABLED</a></li>
<li><a href="#/errorsref?id=FUNC_NOT_OVERRIDDEN">FUNC_NOT_OVERRIDDEN</a></li>
<li><a href="#/errorsref?id=FW_BUILD_NOT_FOUND">FW_BUILD_NOT_FOUND</a></li>
<li><a href="#/errorsref?id=FW_INCOMPAT">FW_INCOMPAT</a></li>
<li><a href="#/errorsref?id=FW_INSTALL_FAILED">FW_INSTALL_FAILED</a></li>
<li><a href="#/errorsref?id=GENERATE_THUMB_FAIL">GENERATE_THUMB_FAIL</a></li>
<li><a href="#/errorsref?id=HTTP_METHOD_NOT_SUPPORTED">HTTP_METHOD_NOT_SUPPORTED</a></li>
<li><a href="#/errorsref?id=IMPORT_CONTENT_FAILED">IMPORT_CONTENT_FAILED</a></li>
<li><a href="#/errorsref?id=IMPORT_INVALID">IMPORT_INVALID</a></li>
<li><a href="#/errorsref?id=IMPORT_PLUGINS_FAILED">IMPORT_PLUGINS_FAILED</a></li>
<li><a href="#/errorsref?id=INCORRECT_PASSWORD">INCORRECT_PASSWORD</a></li>
<li><a href="#/errorsref?id=INVALID_ASSET_URL">INVALID_ASSET_URL</a></li>
<li><a href="#/errorsref?id=INVALID_COURSE">INVALID_COURSE</a></li>
<li><a href="#/errorsref?id=INVALID_LOGIN_DETAILS">INVALID_LOGIN_DETAILS</a></li>
<li><a href="#/errorsref?id=INVALID_OBJECTID">INVALID_OBJECTID</a></li>
<li><a href="#/errorsref?id=INVALID_PARAMS">INVALID_PARAMS</a></li>
<li><a href="#/errorsref?id=INVALID_PARENT">INVALID_PARENT</a></li>
<li><a href="#/errorsref?id=INVALID_PASSWORD">INVALID_PASSWORD</a></li>
<li><a href="#/errorsref?id=INVALID_PASSWORD_LENGTH">INVALID_PASSWORD_LENGTH</a></li>
<li><a href="#/errorsref?id=INVALID_PASSWORD_LOWERCASE">INVALID_PASSWORD_LOWERCASE</a></li>
<li><a href="#/errorsref?id=INVALID_PASSWORD_NUMBER">INVALID_PASSWORD_NUMBER</a></li>
<li><a href="#/errorsref?id=INVALID_PASSWORD_SPECIAL">INVALID_PASSWORD_SPECIAL</a></li>
<li><a href="#/errorsref?id=INVALID_PASSWORD_UPPERCASE">INVALID_PASSWORD_UPPERCASE</a></li>
<li><a href="#/errorsref?id=MAIL_NOT_ENABLED">MAIL_NOT_ENABLED</a></li>
<li><a href="#/errorsref?id=MAIL_SEND_FAILED">MAIL_SEND_FAILED</a></li>
<li><a href="#/errorsref?id=MISSING_ASSETS">MISSING_ASSETS</a></li>
<li><a href="#/errorsref?id=MISSING_AUTH_HEADER">MISSING_AUTH_HEADER</a></li>
<li><a href="#/errorsref?id=MISSING_PLUGINS">MISSING_PLUGINS</a></li>
<li><a href="#/errorsref?id=MISSING_SCHEMA_NAME">MISSING_SCHEMA_NAME</a></li>
<li><a href="#/errorsref?id=MODIFY_PROTECTED_ATTR">MODIFY_PROTECTED_ATTR</a></li>
<li><a href="#/errorsref?id=MODULE_NOT_FOUND">MODULE_NOT_FOUND</a></li>
<li><a href="#/errorsref?id=MONGO_CONN_FAILED">MONGO_CONN_FAILED</a></li>
<li><a href="#/errorsref?id=MONGO_DUPL_INDEX">MONGO_DUPL_INDEX</a></li>
<li><a href="#/errorsref?id=MONGO_ERROR">MONGO_ERROR</a></li>
<li><a href="#/errorsref?id=MONGO_IMMUTABLE_FIELD">MONGO_IMMUTABLE_FIELD</a></li>
<li><a href="#/errorsref?id=NOT_FOUND">NOT_FOUND</a></li>
<li><a href="#/errorsref?id=NO_COLL_NAME">NO_COLL_NAME</a></li>
<li><a href="#/errorsref?id=NO_NET_CONN">NO_NET_CONN</a></li>
<li><a href="#/errorsref?id=NO_ROOT_OR_ROUTER_DEF">NO_ROOT_OR_ROUTER_DEF</a></li>
<li><a href="#/errorsref?id=NO_ROUTES_DEF">NO_ROUTES_DEF</a></li>
<li><a href="#/errorsref?id=NO_SCHEMA_DEF">NO_SCHEMA_DEF</a></li>
<li><a href="#/errorsref?id=RATE_LIMIT_EXCEEDED">RATE_LIMIT_EXCEEDED</a></li>
<li><a href="#/errorsref?id=REPO_NOT_FOUND">REPO_NOT_FOUND</a></li>
<li><a href="#/errorsref?id=RESOURCE_IN_USE">RESOURCE_IN_USE</a></li>
<li><a href="#/errorsref?id=SCHEMA_LOAD_FAILED">SCHEMA_LOAD_FAILED</a></li>
<li><a href="#/errorsref?id=SERVER_ERROR">SERVER_ERROR</a></li>
<li><a href="#/errorsref?id=SERVER_START">SERVER_START</a></li>
<li><a href="#/errorsref?id=SUPER_USER_EXISTS">SUPER_USER_EXISTS</a></li>
<li><a href="#/errorsref?id=UNAUTHENTICATED">UNAUTHENTICATED</a></li>
<li><a href="#/errorsref?id=UNAUTHORISED">UNAUTHORISED</a></li>
<li><a href="#/errorsref?id=UNEXPECTED_FILE_TYPES">UNEXPECTED_FILE_TYPES</a></li>
<li><a href="#/errorsref?id=UNKNOWN_AUTH_TYPE">UNKNOWN_AUTH_TYPE</a></li>
<li><a href="#/errorsref?id=UNKNOWN_LANG">UNKNOWN_LANG</a></li>
<li><a href="#/errorsref?id=UNKNOWN_SCHEMA_NAME">UNKNOWN_SCHEMA_NAME</a></li>
<li><a href="#/errorsref?id=USER_REG_FAILED">USER_REG_FAILED</a></li>
<li><a href="#/errorsref?id=VALIDATION_FAILED">VALIDATION_FAILED</a></li>
</ul>


| Error code | Description | HTTP status code | Supplemental data |
| - | - | :-: | - |
| `ACCOUNT_DISABLED` | Account has been disabled | 403 | <ul></ul> |
| `ACCOUNT_LOCKED_PERM` | User account has been permanently locked | 401 | <ul></ul> |
| `ACCOUNT_LOCKED_TEMP` | User account has been temporarily locked | 401 | <ul><li>`remaining`: The amount of time remaining before account is unlocked</li></ul> |
| `ACCOUNT_NOT_LOCALAUTHD` | Specified account is not authenticated with local auth | 400 | <ul></ul> |
| `API_MODULE_INVALID_CLASS` | Module does not extend AbstractApiModule | 500 | <ul><li>`name`: Name of the module</li></ul> |
| `ASSET_TYPE_EXISTS` | An asset type with this name already exists | 500 | <ul><li>`name`: Repo name</li></ul> |
| `ASSET_TYPE_INVALID` | Asset type does not extend AbstractAsset | 500 | <ul><li>`name`: Asset type</li></ul> |
| `ASSET_TYPE_UNKNOWN` | Asset type is not registered | 500 | <ul><li>`name`: Asset type</li></ul> |
| `AUTH_HEADER_UNSUPPORTED` | Authorization header type is unsupported by the API | 401 | <ul><li>`type`: Authorisation type provided</li></ul> |
| `AUTH_PLUGIN_INVALID_CLASS` | Auth plugin must extend AbstractAuthPlugin | 500 | <ul></ul> |
| `AUTH_TOKEN_EXPIRED` | Auth token has expired, a new one must be created | 401 | <ul></ul> |
| `AUTH_TOKEN_INVALID` | Auth token is not valid | 401 | <ul><li>`error`: The error message</li></ul> |
| `AUTH_TOKEN_NOT_BEFORE` | The auth token nbf is after the current time, and the token is therefore not valid | 401 | <ul><li>`error`: The error message</li></ul> |
| `AUTH_TYPE_DEF_MISSING` | Auth type is not defined | 500 | <ul></ul> |
| `BODY_PARSE_FAILED` | Failed to parse request body data | 400 | <ul><li>`error`: The error message</li></ul> |
| `BROWSERSLIST_UPDATE_FAILED` | Failed to update browserslist DB | 500 | <ul><li>`error`: The error message</li></ul> |
| `BUILD_DATA_RETRIEVAL_FAILED` | Failed to retrieve build data from the database | 500 | <ul><li>`error`: The error message</li></ul> |
| `BUILD_NOT_FOUND` | Framework build data cannot be found | 404 | <ul></ul> |
| `CLI_BUILD_FAILED` | Framework build using the adapt-cli failed | 500 | <ul><li>`cmd`: The command that caused the error</li><li>`message`: A detailed error message passed from adapt-cli</li></ul> |
| `CONTENTPLUGIN_ALREADY_EXISTS` | Plugin ${name}@${version} already exists | 400 | <ul><li>`name`: Name of content plugin</li><li>`version`: Version of content plugin</li></ul> |
| `CONTENTPLUGIN_ATTR_CLASH` | Target attribute '${targetAttribute}' already exists in ${name} | 400 | <ul><li>`name`: Name of content plugin</li><li>`targetAttribute`: Offending target attribute</li></ul> |
| `CONTENTPLUGIN_ATTR_MISSING` | Plugin ${name} is missing a targetAttribute value | 400 | <ul><li>`name`: Name of content plugin</li></ul> |
| `CONTENTPLUGIN_CLI_INSTALL_FAILED` | Installation via adapt-cli failed | 500 | <ul><li>`name`: Name of content plugin</li></ul> |
| `CONTENTPLUGIN_INCOMPAT_FW` | Plugin ${name}@${version} incompatible with installed framework (requires ${requiredFramework}, found ${installedFramework}) | 400 | <ul><li>`installedFramework`: Version of the framework which is installed</li><li>`name`: Name of content plugin</li><li>`requiredFramework`: Version of the framework which is required</li><li>`version`: Version of content plugin</li></ul> |
| `CONTENTPLUGIN_INSTALL_FAILED` | Installation of plugins failed | 500 | <ul><li>`errors`: List of errors</li></ul> |
| `CONTENTPLUGIN_INVALID_ZIP` | Invalid plugin data provided | 400 | <ul></ul> |
| `CONTENTPLUGIN_IN_USE` | Content plugin is in use in existing courses | 400 | <ul><li>`courses`: List of courses using the content plugin</li></ul> |
| `CONTENTPLUGIN_NEWER_INSTALLED` | Plugin ${name}@${newVersion} already exists at a higher version (${existingVersion}) | 400 | <ul><li>`existingVersion`: Installed version</li><li>`name`: Name of content plugin</li><li>`newVersion`: Version to install</li></ul> |
| `COURSE_NOT_FOUND` | Requested course could not be found | 404 | <ul></ul> |
| `DESTROY_SESSION_FAIL` | Failed to terminate user session | 500 | <ul><li>`error`: The error message</li></ul> |
| `DUPL_AUTHORED_MODULE_NAME` | Function must be overridden in child class | 500 | <ul></ul> |
| `DUPL_AUTH_PLUGIN_REG` | An auth plugin is already registered with the same name | 500 | <ul></ul> |
| `DUPL_USER` | A user already exists with the passed email address | 400 | <ul><li>`email`: Email address of the user</li></ul> |
| `EACCES` | An attempt was made to access a file in a way forbidden by its file access permissions | 500 | <ul></ul> |
| `EADDRINUSE` | An attempt to bind a server to a local address failed due to another server on the local system already occupying that address | 500 | <ul></ul> |
| `ECONNREFUSED` | No connection could be made because the target machine actively refused it | 500 | <ul></ul> |
| `EEXIST` | An existing file was the target of an operation that required that the target not exist | 500 | <ul></ul> |
| `ENDPOINT_NOT_FOUND` | API endpoint does not exist | 404 | <ul><li>`endpoint`: The missing endpoint</li><li>`method`: The HTTP method</li></ul> |
| `ENOENT` | No entity (file or directory) could be found by the given path | 500 | <ul></ul> |
| `ENOTEMPTY` | A directory with entries was the target of an operation that requires an empty directory | 500 | <ul></ul> |
| `FILE_EXCEEDS_MAX_SIZE` | Uploaded file exceeds the size limit | 413 | <ul><li>`maxSize`: The maximum file size</li><li>`size`: Size of file</li></ul> |
| `FILE_SYNTAX_ERROR` | File contains a syntax error | 500 | <ul><li>`path`: Path to the invalid file</li><li>`message`: The error message</li></ul> |
| `FUNC_DISABLED` | Function has been disabled | 500 | <ul><li>`name`: The name of the function</li></ul> |
| `FUNC_NOT_OVERRIDDEN` | Function must be overridden in child class | 500 | <ul><li>`name`: The name of the function</li></ul> |
| `FW_BUILD_NOT_FOUND` | Framework build could not be found in the database | 404 | <ul><li>`_id`: Database document _id value for the missing course build</li></ul> |
| `FW_INCOMPAT` | Course for import uses a framework version incompatible with that installed | 400 | <ul><li>`import`: Framework version used in import course</li><li>`installed`: Framework version currently installed on the server</li></ul> |
| `FW_INSTALL_FAILED` | Installation of the framework failed | 500 | <ul></ul> |
| `GENERATE_THUMB_FAIL` | Failed to generate asset thumbnail | 500 | <ul><li>`error`: Error message</li></ul> |
| `HTTP_METHOD_NOT_SUPPORTED` | HTTP method for a given request is not supported | 404 | <ul><li>`method`: The invalid HTTP method</li></ul> |
| `IMPORT_CONTENT_FAILED` | Import of framework content failed | 400 | <ul><li>`errors`: Accompanying errors</li></ul> |
| `IMPORT_INVALID` | An invalid import zip has been provided | 400 | <ul></ul> |
| `IMPORT_PLUGINS_FAILED` | Import of framework plugins failed | 500 | <ul></ul> |
| `INCORRECT_PASSWORD` | Provided password does not match that stored | 401 | <ul></ul> |
| `INVALID_ASSET_URL` | Invalid URL has been specified for external asset | 400 | <ul><li>`url`: The asset URL</li></ul> |
| `INVALID_COURSE` | An invalid course has been provided | 400 | <ul></ul> |
| `INVALID_LOGIN_DETAILS` | Invalid login details were provided | 401 | <ul></ul> |
| `INVALID_OBJECTID` | Not a valid ObjectId | 400 | <ul><li>`value`: The value</li></ul> |
| `INVALID_PARAMS` | Invalid parameters have been provided | 400 | <ul><li>`params`: The invalid params</li></ul> |
| `INVALID_PARENT` | Specified item is not a valid content item Invalid parent itemparent | 500 | <ul><li>`parentId`: _id of the parent item</li></ul> |
| `INVALID_PASSWORD` | Password failed validation | 401 | <ul><li>`errors`: The validation errors</li></ul> |
| `INVALID_PASSWORD_LENGTH` | Password must be at least the required number of characters | 401 | <ul><li>`length`: the minimum required number of characters</li></ul> |
| `INVALID_PASSWORD_LOWERCASE` | Password must contain at least one lowercase character | 401 | <ul></ul> |
| `INVALID_PASSWORD_NUMBER` | Password must contain at least one number | 401 | <ul></ul> |
| `INVALID_PASSWORD_SPECIAL` | Password must contain at least one special character (#?!@$%^&*-) | 401 | <ul></ul> |
| `INVALID_PASSWORD_UPPERCASE` | Password must contain at least one uppercase character | 401 | <ul></ul> |
| `MAIL_NOT_ENABLED` | Email functionality is not enabled | 500 | <ul></ul> |
| `MAIL_SEND_FAILED` | Failed to send error email | 500 | <ul></ul> |
| `MISSING_ASSETS` | Assets are missing | 500 | <ul><li>`errors`: The errors</li></ul> |
| `MISSING_AUTH_HEADER` | Authorization headers are missing from request | 401 | <ul></ul> |
| `MISSING_PLUGINS` | Course for import uses plugins which are missing from the server | 400 | <ul></ul> |
| `MISSING_SCHEMA_NAME` | Schema name is not defined | 400 | <ul></ul> |
| `MODIFY_PROTECTED_ATTR` | Attempted to modify a protected data attribute | 400 | <ul><li>`attribute`: The protected attribute</li></ul> |
| `MODULE_NOT_FOUND` | A module file could not be resolved while attempting a require() or import operation | 500 | <ul></ul> |
| `MONGO_CONN_FAILED` | An error occurred connecting to the MongoDB instance | 500 | <ul><li>`error`: The error message</li><li>`uri`: The connection URI</li></ul> |
| `MONGO_DUPL_INDEX` | A document already exists with the same indexed value | 400 | <ul><li>`action`: The action being performed on the database collection</li><li>`collectionName`: Name of the collection being processed</li><li>`error`: The error message</li></ul> |
| `MONGO_ERROR` | An error occurred while performing a MongoDB action | 500 | <ul><li>`action`: The action being performed on the database collection</li><li>`collectionName`: Name of the collection being processed</li><li>`error`: The error message</li></ul> |
| `MONGO_IMMUTABLE_FIELD` | Attempting to modify an immutable field | 400 | <ul><li>`action`: The action being performed on the database collection</li><li>`collectionName`: Name of the collection being processed</li><li>`error`: The error message</li></ul> |
| `NOT_FOUND` | Requested item could not be found | 404 | <ul><li>`id`: An identifier for the missing item</li><li>`type`: Type of the missing item</li></ul> |
| `NO_COLL_NAME` | module is missing a collection name | 500 | <ul></ul> |
| `NO_NET_CONN` | No network connection | 400 | <ul><li>`hostname`: The hostname we were trying to reach</li></ul> |
| `NO_ROOT_OR_ROUTER_DEF` | module is missing both a root and router definition | 500 | <ul></ul> |
| `NO_ROUTES_DEF` | module is missing API routes definition | 500 | <ul></ul> |
| `NO_SCHEMA_DEF` | No json schema has been defined | 404 | <ul></ul> |
| `RATE_LIMIT_EXCEEDED` | API rate limit has been exceeded | 429 | <ul></ul> |
| `REPO_NOT_FOUND` | The requested asset repository doesn't exist | 500 | <ul><li>`name`: Repo name</li></ul> |
| `RESOURCE_IN_USE` | Resource is currently being using in courses | 400 | <ul><li>`type`: Type of resource</li><li>`courses`: Courses using the resource</li></ul> |
| `SCHEMA_LOAD_FAILED` | Failed to load a JSON schema | 500 | <ul><li>`schemaName`: Schema name</li></ul> |
| `SERVER_ERROR` | Generic server error | 500 | <ul><li>`error`: The original error</li></ul> |
| `SERVER_START` | Failed to start server | 500 | <ul><li>`error`: The error</li></ul> |
| `SUPER_USER_EXISTS` | A Super Admin account already exists | 400 | <ul></ul> |
| `UNAUTHENTICATED` | Request is not authenticated for access to the API | 401 | <ul></ul> |
| `UNAUTHORISED` | Request is not authorised to perform the required operation | 403 | <ul><li>`method`: The request HTTP method</li><li>`url`: The request URL</li></ul> |
| `UNEXPECTED_FILE_TYPES` | Recieved unexpected file types | 400 | <ul><li>`expectedFileTypes`: The list of expected file types</li><li>`invalidFiles`: The list of invalid files</li></ul> |
| `UNKNOWN_AUTH_TYPE` | Request is attempting to use an unknown authentication type | 401 | <ul><li>`authType`: Authentication type</li></ul> |
| `UNKNOWN_LANG` | unknown language | 400 | <ul><li>`lang`: language</li></ul> |
| `UNKNOWN_SCHEMA_NAME` | Failed to determine schema name | 500 | <ul><li>`_id`: The database _id</li><li>`_type`: The _type value</li><li>`_component`: The _component value</li></ul> |
| `USER_REG_FAILED` | User registration failed | 400 | <ul><li>`error`: The error</li></ul> |
| `VALIDATION_FAILED` | Data validation failed | 400 | <ul><li>`data`: the data failing validation</li><li>`errors`: all validation errors</li><li>`schemaName`: Schema name</li></ul> |