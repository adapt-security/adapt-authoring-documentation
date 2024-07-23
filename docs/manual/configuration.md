# Configuration reference
This page lists all configuration options supported by the [core bundle](coremodules) of Adapt authoring modules.

### Quick navigation

<ul class="toc">
<li><a href="#/configuration?id=adapt-authoring-adaptframework">adapt-authoring-adaptframework</a></li>
<li><a href="#/configuration?id=adapt-authoring-api">adapt-authoring-api</a></li>
<li><a href="#/configuration?id=adapt-authoring-assets">adapt-authoring-assets</a></li>
<li><a href="#/configuration?id=adapt-authoring-auth">adapt-authoring-auth</a></li>
<li><a href="#/configuration?id=adapt-authoring-browserslist">adapt-authoring-browserslist</a></li>
<li><a href="#/configuration?id=adapt-authoring-collab">adapt-authoring-collab</a></li>
<li><a href="#/configuration?id=adapt-authoring-contentplugin">adapt-authoring-contentplugin</a></li>
<li><a href="#/configuration?id=adapt-authoring-core">adapt-authoring-core</a></li>
<li><a href="#/configuration?id=adapt-authoring-docs">adapt-authoring-docs</a></li>
<li><a href="#/configuration?id=adapt-authoring-jsonschema">adapt-authoring-jsonschema</a></li>
<li><a href="#/configuration?id=adapt-authoring-lang">adapt-authoring-lang</a></li>
<li><a href="#/configuration?id=adapt-authoring-localauth">adapt-authoring-localauth</a></li>
<li><a href="#/configuration?id=adapt-authoring-logger">adapt-authoring-logger</a></li>
<li><a href="#/configuration?id=adapt-authoring-mailer">adapt-authoring-mailer</a></li>
<li><a href="#/configuration?id=adapt-authoring-middleware">adapt-authoring-middleware</a></li>
<li><a href="#/configuration?id=adapt-authoring-mongodb">adapt-authoring-mongodb</a></li>
<li><a href="#/configuration?id=adapt-authoring-mongodblogger">adapt-authoring-mongodblogger</a></li>
<li><a href="#/configuration?id=adapt-authoring-ratelimiter">adapt-authoring-ratelimiter</a></li>
<li><a href="#/configuration?id=adapt-authoring-roles">adapt-authoring-roles</a></li>
<li><a href="#/configuration?id=adapt-authoring-server">adapt-authoring-server</a></li>
<li><a href="#/configuration?id=adapt-authoring-sessions">adapt-authoring-sessions</a></li>
<li><a href="#/configuration?id=adapt-authoring-ui">adapt-authoring-ui</a></li>
<li><a href="#/configuration?id=adapt-authoring-users">adapt-authoring-users</a></li>
</ul>


## Quick reference
See below for an overview of all available configuration options.

```javascript
export default {
  'adapt-authoring-adaptframework': {
    // Path to the folder where framework builds will be generated
    buildDir: "$TEMP/framework-builds", // string, optional
    // How long a build should remain valid for. Expects an amount followed by a space and then the unit (e.g. 5 hours)
    buildLifespan: "7d", // string, optional
    // Whether the Adapt framework can be updated via the REST API
    enableUpdateApi: true, // boolean, optional
    // Path to the adapt_framework source folder
    frameworkDir: "$TEMP/adapt_framework", // string, optional
    // URL of the Adapt framework git repository to install
    frameworkRepository: undefined, // string, optional
  },
  'adapt-authoring-api': {
    // Default lifespan of data cache
    defaultCacheLifespan: "5s", // string, optional
    // Default size of page
    defaultPageSize: 100, // number, optional
    // Maximum page size
    maxPageSize: 250, // number, optional
  },
  'adapt-authoring-assets': {
    // Assets repository location
    assetDir: "$DATA/assets", // string, optional
    // Default repository to use for asset storage
    defaultAssetRepository: "local", // string, optional
    // File types allowed for upload
    expectedFileTypes: ["application/pdf","application/zip","audio/mpeg","audio/wav","font/woff","font/woff2","image/gif","image/jpeg","image/png","image/svg+xml","text/vtt","video/mp4"], // array, optional
    // Maximum file upload size
    maxFileSize: "50mb", // string, optional
    // Location of local thumbs dir
    thumbnailDir: "$TEMP/asset-thumbs", // string, optional
    // File extension for thumbnails
    thumbnailExt: ".png", // string, optional
    // Maximum width for thumbnails
    thumbnailWidth: 320, // number, optional
  },
  'adapt-authoring-auth': {
    // Enables auth (note: this has no effect in production environments)
    isEnabled: true, // boolean, optional
    // How long a token should remain valid for
    defaultTokenLifespan: "7d", // string, optional
    // In enabled, a warning is logged on app start for any routes with missing permissions (note: any routes without defined permissions are inaccessible)
    logMissingPermissions: true, // boolean, optional
    // Whether a user must be authenticated to generate an API auth token
    secureTokenGeneration: true, // boolean, optional
    // A secret used to encode/decode Json Web Tokens
    tokenSecret: undefined, // string, required
    // The identity of the issuer of the token
    tokenIssuer: "adapt", // string, optional
  },
  'adapt-authoring-browserslist': {
    // Whether the browserslist DB should be updated prior to each framework build
    runOnBuild: true, // boolean, optional
    // The amount of time to wait in between browserslist DB rebuilds. Setting to 0 will disable this feature.
    updateInterval: "0", // string, optional
  },
  'adapt-authoring-collab': {
    // Whether this module is a template
    websocketURL: "ws://localhost:3000", // string, optional
    // Time in minutes until a user is classed as inactive
    idleTime: 1, // number, optional
  },
  'adapt-authoring-contentplugin': {
    // Location of locally installed plugins
    pluginDir: "$DATA/contentplugins", // string, optional
  },
  'adapt-authoring-core': {
    // Whether this app configuration is a production environment
    isProduction: true, // boolean, optional
    // Directory for persistant application data
    dataDir: "$ROOT/APP_DATA/data", // string, optional
    // Temporary directory for application data
    tempDir: "$ROOT/APP_DATA/temp", // string, optional
  },
  'adapt-authoring-docs': {
    // Path to store documentation build files
    outputDir: "$TEMP/docs-build", // string, optional
    // Sections for categorising documentation manual pages
    manualSections: {"getting-started":{"title":"Getting started"},"basics":{"title":"The basics"},"advanced":{"title":"Advanced topics"},"ui":{"title":"Front-end app"},"other-guides":{"title":"Other guides","default":true},"contributing":{"title":"Contributing"},"reference":{"title":"Reference"}}, // object, optional
  },
  'adapt-authoring-jsonschema': {
    // Whether schema data should be cached
    enableCache: true, // boolean, optional
    // Custom RegExp overrides for Ajv string formats
    formatOverrides: {}, // object, optional
    // Attributes which should be whitelisted when run through the XSS sanitiser.
    xssWhitelist: {}, // object, optional
    // If set to false, the xssWhitelist value will EXTEND the default XSS whitelist. If set to true, it will REPLACE it.
    xssWhitelistOverride: false, // boolean, optional
  },
  'adapt-authoring-lang': {
    // The default language used by the server
    defaultLang: "en", // string, optional
  },
  'adapt-authoring-localauth': {
    // The number of rounds performed when generating a password hash
    saltRounds: 10, // number, optional
    // The number of failed login attempts allowed before the account is locked for a short period of time
    failsUntilTemporaryLock: 5, // number, optional
    // The number of failed login attempts allowed before the account is permanently locked
    failsUntilPermanentLock: 20, // number, optional
    // The amount of time a locked user must wait before attempting to log in again
    temporaryLockDuration: "1m", // string, optional
    // The amount of time a password reset token remains valid for
    resetTokenLifespan: "3h", // string, optional
    // The amount of time an invite password reset token remains valid for
    inviteTokenLifespan: "7d", // string, optional
    // Minimum password length
    minPasswordLength: 8, // number, optional
    // Whether the password must contain at least one number
    passwordMustHaveNumber: false, // boolean, optional
    // Whether the password must contain at least one uppercase character
    passwordMustHaveUppercase: false, // boolean, optional
    // Whether the password must contain at least one lowercase character
    passwordMustHaveLowercase: false, // boolean, optional
    // Whether the password must contain at least one special character
    passwordMustHaveSpecial: false, // boolean, optional
  },
  'adapt-authoring-logger': {
    // Configures which log levels of log should be shown. Accepts generic levels, module-specific levels and not logic (e.g. 'debug', 'debug.core' and '!debug' respectively).
    levels: ["error","warn","success","info","debug"], // array, optional
    // Whether to mute log messages
    mute: false, // boolean,string, optional
    // The date format to use
    dateFormat: "iso", // string, optional
    // Whether to prepend a timestamp to each log message
    showTimestamp: true, // boolean, optional
  },
  'adapt-authoring-mailer': {
    // Whether the mailer module is enabled
    isEnabled: false, // boolean, optional
    // Connection URL for the SMTP service
    connectionUrl: undefined, // string, optional
    // Default email address to use as the sender
    defaultSenderAddress: undefined, // string, optional
  },
  'adapt-authoring-middleware': {
    // Content types the API accepts (may use MIME types or extension names)
    acceptedTypes: ["application/json"], // array, optional
    // Limit the size of any uploaded file
    fileUploadMaxFileSize: "50mb", // string, optional
    // Temporary directory for file uploads
    uploadTempDir: "$TEMP/file-uploads", // string, optional
  },
  'adapt-authoring-mongodb': {
    // The MongoDB connection URI used to connect to your MongoDB deployment.
    connectionUri: undefined, // string, required
  },
  'adapt-authoring-mongodblogger': {
    // Whether errors in the MongoDBLoggerModule module should be logged using the default logger. Can cause mass logs in some cases.
    logInternalErrors: false, // boolean, optional
    // The maximum number of logs stored at any one time (the oldest logs will be replaced first).
    maxLogCount: 5000, // number, optional
  },
  'adapt-authoring-ratelimiter': {
    // The number of API requests allowed by a single IP within the specified time limit
    apiRequestLimit: 50, // number, optional
    // Amount of time before the request count is reset
    apiRequestLimitDuration: "1s", // string, optional
  },
  'adapt-authoring-roles': {
    // List of defined roles to be loaded on app start
    roleDefinitions: [{"shortName":"authuser","displayName":"Authenticated user","scopes":["clear:session","read:config","read:lang","read:me","write:me","disavow:auth"]},{"shortName":"contentcreator","displayName":"Content creator","extends":"authuser","scopes":["export:adapt","import:adapt","preview:adapt","publish:adapt","read:assets","write:assets","read:content","write:content","read:contentplugin","read:roles","read:schema","read:tags","write:tags","read:users"]},{"shortName":"superuser","displayName":"Super user","scopes":["*:*"]}], // array, optional
    // The roles which are applied by default to new users (expects role shortname)
    defaultRoles: ["authuser"], // array, optional
    // Same as defaultRoles, but allows different roles to be specified for different auth types
    defaultRolesForAuthTypes: {}, // object, optional
  },
  'adapt-authoring-server': {
    // Name of the host machine the server is running from
    host: undefined, // string, required
    // Port to be used for listening to incoming connections
    port: undefined, // number,string, required
    // URL the server can be accessed from
    url: undefined, // string, required
    // Whether to trust the client's x-Forwarded-For header for the request IP address. Only enable if using your own trusted reverse proxy
    trustProxy: false, // boolean, optional
    // Will log the execution time of each request
    debugRequestTime: false, // boolean, optional
    // Whether to log errors in their entirety
    verboseErrorLogging: false, // boolean, optional
  },
  'adapt-authoring-sessions': {
    // Name of the database collection used to store user session data
    collectionName: "usersessions", // string, optional
    // The amount of time a session should remain valid
    lifespan: "1h", // string, optional
    // Determines whether sessions should only expire after a period of inactivity (max age determined by the lifespan option)
    rolling: true, // boolean, optional
    // Asserts that a cookie must not be sent with cross-origin requests
    sameSite: "strict", // string, optional
    // A secret used to encode/decode user sessions
    secret: undefined, // string, required
    // If true, cookie is only sent to the server when a request is made with the https scheme
    secure: false, // boolean,string, optional
  },
  'adapt-authoring-ui': {
    // Location of UI build files
    buildDir: "$TEMP/ui-build", // string, optional
    // Location of UI source files
    srcDir: "$TEMP/ui-src", // string, optional
  },
  'adapt-authoring-users': {
    // If true, all user emails will be converted to lower-case
    forceLowerCaseEmail: true, // boolean, optional
  },
};
```

## Complete reference
See below for a full list of available configuration options.

<h3 id="adapt-authoring-adaptframework" class="dep">adapt-authoring-adaptframework</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">buildDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Path to the folder where framework builds will be generated</div>
<div class="default"><span class="label">Default</span>: <pre>"$TEMP/framework-builds"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">buildLifespan</span> (string, optional)</div>
<div class="inner">
<div class="description">How long a build should remain valid for. Expects an amount followed by a space and then the unit (e.g. 5 hours)</div>
<div class="default"><span class="label">Default</span>: <pre>"7d"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">enableUpdateApi</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether the Adapt framework can be updated via the REST API</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">frameworkDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Path to the adapt_framework source folder</div>
<div class="default"><span class="label">Default</span>: <pre>"$TEMP/adapt_framework"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">frameworkRepository</span> (string, optional)</div>
<div class="inner">
<div class="description">URL of the Adapt framework git repository to install</div>
<div class="default"><span class="label">Default</span>: <pre>undefined</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-api" class="dep">adapt-authoring-api</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">defaultCacheLifespan</span> (string, optional)</div>
<div class="inner">
<div class="description">Default lifespan of data cache</div>
<div class="default"><span class="label">Default</span>: <pre>"5s"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">defaultPageSize</span> (number, optional)</div>
<div class="inner">
<div class="description">Default size of page</div>
<div class="default"><span class="label">Default</span>: <pre>100</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">maxPageSize</span> (number, optional)</div>
<div class="inner">
<div class="description">Maximum page size</div>
<div class="default"><span class="label">Default</span>: <pre>250</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-assets" class="dep">adapt-authoring-assets</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">assetDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Assets repository location</div>
<div class="default"><span class="label">Default</span>: <pre>"$DATA/assets"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">defaultAssetRepository</span> (string, optional)</div>
<div class="inner">
<div class="description">Default repository to use for asset storage</div>
<div class="default"><span class="label">Default</span>: <pre>"local"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">expectedFileTypes</span> (array, optional)</div>
<div class="inner">
<div class="description">File types allowed for upload</div>
<div class="default"><span class="label">Default</span>: <pre>["application/pdf","application/zip","audio/mpeg","audio/wav","font/woff","font/woff2","image/gif","image/jpeg","image/png","image/svg+xml","text/vtt","video/mp4"]</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">maxFileSize</span> (string, optional)</div>
<div class="inner">
<div class="description">Maximum file upload size</div>
<div class="default"><span class="label">Default</span>: <pre>"50mb"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">thumbnailDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Location of local thumbs dir</div>
<div class="default"><span class="label">Default</span>: <pre>"$TEMP/asset-thumbs"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">thumbnailExt</span> (string, optional)</div>
<div class="inner">
<div class="description">File extension for thumbnails</div>
<div class="default"><span class="label">Default</span>: <pre>".png"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">thumbnailWidth</span> (number, optional)</div>
<div class="inner">
<div class="description">Maximum width for thumbnails</div>
<div class="default"><span class="label">Default</span>: <pre>320</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-auth" class="dep">adapt-authoring-auth</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">isEnabled</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Enables auth (note: this has no effect in production environments)</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">defaultTokenLifespan</span> (string, optional)</div>
<div class="inner">
<div class="description">How long a token should remain valid for</div>
<div class="default"><span class="label">Default</span>: <pre>"7d"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">logMissingPermissions</span> (boolean, optional)</div>
<div class="inner">
<div class="description">In enabled, a warning is logged on app start for any routes with missing permissions (note: any routes without defined permissions are inaccessible)</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">secureTokenGeneration</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether a user must be authenticated to generate an API auth token</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">tokenSecret</span> (string, required)</div>
<div class="inner">
<div class="description">A secret used to encode/decode Json Web Tokens</div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">tokenIssuer</span> (string, optional)</div>
<div class="inner">
<div class="description">The identity of the issuer of the token</div>
<div class="default"><span class="label">Default</span>: <pre>"adapt"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-browserslist" class="dep">adapt-authoring-browserslist</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">runOnBuild</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether the browserslist DB should be updated prior to each framework build</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">updateInterval</span> (string, optional)</div>
<div class="inner">
<div class="description">The amount of time to wait in between browserslist DB rebuilds. Setting to 0 will disable this feature.</div>
<div class="default"><span class="label">Default</span>: <pre>"0"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-collab" class="dep">adapt-authoring-collab</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">websocketURL</span> (string, optional)</div>
<div class="inner">
<div class="description">Whether this module is a template</div>
<div class="default"><span class="label">Default</span>: <pre>"ws://localhost:3000"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">idleTime</span> (number, optional)</div>
<div class="inner">
<div class="description">Time in minutes until a user is classed as inactive</div>
<div class="default"><span class="label">Default</span>: <pre>1</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-contentplugin" class="dep">adapt-authoring-contentplugin</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">pluginDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Location of locally installed plugins</div>
<div class="default"><span class="label">Default</span>: <pre>"$DATA/contentplugins"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-core" class="dep">adapt-authoring-core</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">isProduction</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether this app configuration is a production environment</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">dataDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Directory for persistant application data</div>
<div class="default"><span class="label">Default</span>: <pre>"$ROOT/APP_DATA/data"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">tempDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Temporary directory for application data</div>
<div class="default"><span class="label">Default</span>: <pre>"$ROOT/APP_DATA/temp"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-docs" class="dep">adapt-authoring-docs</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">outputDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Path to store documentation build files</div>
<div class="default"><span class="label">Default</span>: <pre>"$TEMP/docs-build"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">manualSections</span> (object, optional)</div>
<div class="inner">
<div class="description">Sections for categorising documentation manual pages</div>
<div class="default"><span class="label">Default</span>: <pre>{"getting-started":{"title":"Getting started"},"basics":{"title":"The basics"},"advanced":{"title":"Advanced topics"},"ui":{"title":"Front-end app"},"other-guides":{"title":"Other guides","default":true},"contributing":{"title":"Contributing"},"reference":{"title":"Reference"}}</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-jsonschema" class="dep">adapt-authoring-jsonschema</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">enableCache</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether schema data should be cached</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">formatOverrides</span> (object, optional)</div>
<div class="inner">
<div class="description">Custom RegExp overrides for Ajv string formats</div>
<div class="default"><span class="label">Default</span>: <pre>{}</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">xssWhitelist</span> (object, optional)</div>
<div class="inner">
<div class="description">Attributes which should be whitelisted when run through the XSS sanitiser.</div>
<div class="default"><span class="label">Default</span>: <pre>{}</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">xssWhitelistOverride</span> (boolean, optional)</div>
<div class="inner">
<div class="description">If set to false, the xssWhitelist value will EXTEND the default XSS whitelist. If set to true, it will REPLACE it.</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-lang" class="dep">adapt-authoring-lang</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">defaultLang</span> (string, optional)</div>
<div class="inner">
<div class="description">The default language used by the server</div>
<div class="default"><span class="label">Default</span>: <pre>"en"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-localauth" class="dep">adapt-authoring-localauth</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">saltRounds</span> (number, optional)</div>
<div class="inner">
<div class="description">The number of rounds performed when generating a password hash</div>
<div class="default"><span class="label">Default</span>: <pre>10</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">failsUntilTemporaryLock</span> (number, optional)</div>
<div class="inner">
<div class="description">The number of failed login attempts allowed before the account is locked for a short period of time</div>
<div class="default"><span class="label">Default</span>: <pre>5</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">failsUntilPermanentLock</span> (number, optional)</div>
<div class="inner">
<div class="description">The number of failed login attempts allowed before the account is permanently locked</div>
<div class="default"><span class="label">Default</span>: <pre>20</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">temporaryLockDuration</span> (string, optional)</div>
<div class="inner">
<div class="description">The amount of time a locked user must wait before attempting to log in again</div>
<div class="default"><span class="label">Default</span>: <pre>"1m"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">resetTokenLifespan</span> (string, optional)</div>
<div class="inner">
<div class="description">The amount of time a password reset token remains valid for</div>
<div class="default"><span class="label">Default</span>: <pre>"3h"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">inviteTokenLifespan</span> (string, optional)</div>
<div class="inner">
<div class="description">The amount of time an invite password reset token remains valid for</div>
<div class="default"><span class="label">Default</span>: <pre>"7d"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">minPasswordLength</span> (number, optional)</div>
<div class="inner">
<div class="description">Minimum password length</div>
<div class="default"><span class="label">Default</span>: <pre>8</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">passwordMustHaveNumber</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether the password must contain at least one number</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">passwordMustHaveUppercase</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether the password must contain at least one uppercase character</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">passwordMustHaveLowercase</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether the password must contain at least one lowercase character</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">passwordMustHaveSpecial</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether the password must contain at least one special character</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-logger" class="dep">adapt-authoring-logger</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">levels</span> (array, optional)</div>
<div class="inner">
<div class="description">Configures which log levels of log should be shown. Accepts generic levels, module-specific levels and not logic (e.g. 'debug', 'debug.core' and '!debug' respectively).</div>
<div class="default"><span class="label">Default</span>: <pre>["error","warn","success","info","debug"]</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">mute</span> (boolean,string, optional)</div>
<div class="inner">
<div class="description">Whether to mute log messages</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">dateFormat</span> (string, optional)</div>
<div class="inner">
<div class="description">The date format to use</div>
<div class="default"><span class="label">Default</span>: <pre>"iso"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">showTimestamp</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether to prepend a timestamp to each log message</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-mailer" class="dep">adapt-authoring-mailer</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">isEnabled</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether the mailer module is enabled</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">connectionUrl</span> (string, optional)</div>
<div class="inner">
<div class="description">Connection URL for the SMTP service</div>
<div class="default"><span class="label">Default</span>: <pre>undefined</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">defaultSenderAddress</span> (string, optional)</div>
<div class="inner">
<div class="description">Default email address to use as the sender</div>
<div class="default"><span class="label">Default</span>: <pre>undefined</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-middleware" class="dep">adapt-authoring-middleware</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">acceptedTypes</span> (array, optional)</div>
<div class="inner">
<div class="description">Content types the API accepts (may use MIME types or extension names)</div>
<div class="default"><span class="label">Default</span>: <pre>["application/json"]</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">fileUploadMaxFileSize</span> (string, optional)</div>
<div class="inner">
<div class="description">Limit the size of any uploaded file</div>
<div class="default"><span class="label">Default</span>: <pre>"50mb"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">uploadTempDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Temporary directory for file uploads</div>
<div class="default"><span class="label">Default</span>: <pre>"$TEMP/file-uploads"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-mongodb" class="dep">adapt-authoring-mongodb</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">connectionUri</span> (string, required)</div>
<div class="inner">
<div class="description">The MongoDB connection URI used to connect to your MongoDB deployment.</div>
</div>
</div>
</div>

<h3 id="adapt-authoring-mongodblogger" class="dep">adapt-authoring-mongodblogger</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">logInternalErrors</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether errors in the MongoDBLoggerModule module should be logged using the default logger. Can cause mass logs in some cases.</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">maxLogCount</span> (number, optional)</div>
<div class="inner">
<div class="description">The maximum number of logs stored at any one time (the oldest logs will be replaced first).</div>
<div class="default"><span class="label">Default</span>: <pre>5000</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-ratelimiter" class="dep">adapt-authoring-ratelimiter</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">apiRequestLimit</span> (number, optional)</div>
<div class="inner">
<div class="description">The number of API requests allowed by a single IP within the specified time limit</div>
<div class="default"><span class="label">Default</span>: <pre>50</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">apiRequestLimitDuration</span> (string, optional)</div>
<div class="inner">
<div class="description">Amount of time before the request count is reset</div>
<div class="default"><span class="label">Default</span>: <pre>"1s"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-roles" class="dep">adapt-authoring-roles</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">roleDefinitions</span> (array, optional)</div>
<div class="inner">
<div class="description">List of defined roles to be loaded on app start</div>
<div class="default"><span class="label">Default</span>: <pre>[{"shortName":"authuser","displayName":"Authenticated user","scopes":["clear:session","read:config","read:lang","read:me","write:me","disavow:auth"]},{"shortName":"contentcreator","displayName":"Content creator","extends":"authuser","scopes":["export:adapt","import:adapt","preview:adapt","publish:adapt","read:assets","write:assets","read:content","write:content","read:contentplugin","read:roles","read:schema","read:tags","write:tags","read:users"]},{"shortName":"superuser","displayName":"Super user","scopes":["*:*"]}]</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">defaultRoles</span> (array, optional)</div>
<div class="inner">
<div class="description">The roles which are applied by default to new users (expects role shortname)</div>
<div class="default"><span class="label">Default</span>: <pre>["authuser"]</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">defaultRolesForAuthTypes</span> (object, optional)</div>
<div class="inner">
<div class="description">Same as defaultRoles, but allows different roles to be specified for different auth types</div>
<div class="default"><span class="label">Default</span>: <pre>{}</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-server" class="dep">adapt-authoring-server</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">host</span> (string, required)</div>
<div class="inner">
<div class="description">Name of the host machine the server is running from</div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">port</span> (number,string, required)</div>
<div class="inner">
<div class="description">Port to be used for listening to incoming connections</div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">url</span> (string, required)</div>
<div class="inner">
<div class="description">URL the server can be accessed from</div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">trustProxy</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether to trust the client's x-Forwarded-For header for the request IP address. Only enable if using your own trusted reverse proxy</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">debugRequestTime</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Will log the execution time of each request</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">verboseErrorLogging</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Whether to log errors in their entirety</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-sessions" class="dep">adapt-authoring-sessions</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">collectionName</span> (string, optional)</div>
<div class="inner">
<div class="description">Name of the database collection used to store user session data</div>
<div class="default"><span class="label">Default</span>: <pre>"usersessions"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">lifespan</span> (string, optional)</div>
<div class="inner">
<div class="description">The amount of time a session should remain valid</div>
<div class="default"><span class="label">Default</span>: <pre>"1h"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">rolling</span> (boolean, optional)</div>
<div class="inner">
<div class="description">Determines whether sessions should only expire after a period of inactivity (max age determined by the lifespan option)</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">sameSite</span> (string, optional)</div>
<div class="inner">
<div class="description">Asserts that a cookie must not be sent with cross-origin requests</div>
<div class="default"><span class="label">Default</span>: <pre>"strict"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">secret</span> (string, required)</div>
<div class="inner">
<div class="description">A secret used to encode/decode user sessions</div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">secure</span> (boolean,string, optional)</div>
<div class="inner">
<div class="description">If true, cookie is only sent to the server when a request is made with the https scheme</div>
<div class="default"><span class="label">Default</span>: <pre>false</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-ui" class="dep">adapt-authoring-ui</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">buildDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Location of UI build files</div>
<div class="default"><span class="label">Default</span>: <pre>"$TEMP/ui-build"</pre></div>
</div>
</div>
<div class="attribute">
<div class="title"><span class="main">srcDir</span> (string, optional)</div>
<div class="inner">
<div class="description">Location of UI source files</div>
<div class="default"><span class="label">Default</span>: <pre>"$TEMP/ui-src"</pre></div>
</div>
</div>
</div>

<h3 id="adapt-authoring-users" class="dep">adapt-authoring-users</h3>

<div class="options">
<div class="attribute">
<div class="title"><span class="main">forceLowerCaseEmail</span> (boolean, optional)</div>
<div class="inner">
<div class="description">If true, all user emails will be converted to lower-case</div>
<div class="default"><span class="label">Default</span>: <pre>true</pre></div>
</div>
</div>
</div>


