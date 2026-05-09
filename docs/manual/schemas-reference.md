# Schemas reference

This page documents all schemas defined in the authoring tool core bundle. Where relevant, any schema inheritance is noted, along with which fields are required.

### Quick navigation

<ul class="toc">
<li><a href="#/schemas-reference?id=adaptbuild">adaptbuild</a></li>
<li><a href="#/schemas-reference?id=apiroutes">apiroutes</a></li>
<li><a href="#/schemas-reference?id=asset">asset</a></li>
<li><a href="#/schemas-reference?id=authored">authored</a></li>
<li><a href="#/schemas-reference?id=authroutes">authroutes</a></li>
<li><a href="#/schemas-reference?id=authtoken">authtoken</a></li>
<li><a href="#/schemas-reference?id=authuser">authuser</a></li>
<li><a href="#/schemas-reference?id=contentassets">contentassets</a></li>
<li><a href="#/schemas-reference?id=contentplugin">contentplugin</a></li>
<li><a href="#/schemas-reference?id=coursethemepreset">coursethemepreset</a></li>
<li><a href="#/schemas-reference?id=localauthuser">localauthuser</a></li>
<li><a href="#/schemas-reference?id=localpassword">localpassword</a></li>
<li><a href="#/schemas-reference?id=log">log</a></li>
<li><a href="#/schemas-reference?id=maildata">maildata</a></li>
<li><a href="#/schemas-reference?id=role">role</a></li>
<li><a href="#/schemas-reference?id=routeitem">routeitem</a></li>
<li><a href="#/schemas-reference?id=routes">routes</a></li>
<li><a href="#/schemas-reference?id=tag">tag</a></li>
<li><a href="#/schemas-reference?id=tags">tags</a></li>
<li><a href="#/schemas-reference?id=user">user</a></li>
<li><a href="#/schemas-reference?id=userroles">userroles</a></li>
</ul>


<h3 id="adaptbuild" class="dep">adaptbuild</h3>
      
      <div class="desc">An Adapt course build instance</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>action</td>
<td>string</td>
<td></td>
<td>The course _id</td>
</tr>
<tr class="required">
<td>courseId</td>
<td>string</td>
<td></td>
<td>The course _id</td>
</tr>
<tr class="required">
<td>location</td>
<td>string</td>
<td></td>
<td>Location of the course preview</td>
</tr>
<tr class="required">
<td>expiresAt</td>
<td>string</td>
<td></td>
<td>When the preview should be purged from the server</td>
</tr>
<tr class="required">
<td>createdBy</td>
<td>string</td>
<td></td>
<td>User which initiated the build</td>
</tr>
<tr class="">
<td>versions</td>
<td>object</td>
<td></td>
<td>Versions of framework and plugins used in the build</td>
</tr>
</table>
      
      <h3 id="apiroutes" class="dep">apiroutes</h3>
      
      <div class="extension">Merges with <a href="#/schemas-reference?id=routes">routes</a></div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>schemaName</td>
<td>string</td>
<td></td>
<td>Schema name for the module's data model</td>
</tr>
<tr class="">
<td>collectionName</td>
<td>string</td>
<td></td>
<td>MongoDB collection name</td>
</tr>
<tr class="">
<td>useDefaultRoutes</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Whether to generate default CRUD routes</td>
</tr>
</table>
      
      <h3 id="asset" class="dep">asset</h3>
      
      <div class="desc">Asset metadata</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>description</td>
<td>string</td>
<td></td>
<td>The asset description</td>
</tr>
<tr class="">
<td>hash</td>
<td>string</td>
<td></td>
<td>SHA-256 hash of the asset file contents for duplicate detection</td>
</tr>
<tr class="">
<td>duration</td>
<td>number</td>
<td></td>
<td>The asset file's duration</td>
</tr>
<tr class="">
<td>hasThumb</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Whether the asset has a thumbnail</td>
</tr>
<tr class="">
<td>path</td>
<td>string</td>
<td></td>
<td>The relative path to the stored asset</td>
</tr>
<tr class="">
<td>repo</td>
<td>string</td>
<td><pre>"local"</pre></td>
<td>Specifies the type of asset repository used to store this asset</td>
</tr>
<tr class="">
<td>resolution</td>
<td>string</td>
<td></td>
<td>The asset file's resolution</td>
</tr>
<tr class="">
<td>size</td>
<td>number</td>
<td></td>
<td>The size of the asset</td>
</tr>
<tr class="">
<td>subtype</td>
<td>string</td>
<td></td>
<td>The asset subtype (identifies the exact kind of data of the specified type)</td>
</tr>
<tr class="required">
<td>title</td>
<td>string</td>
<td></td>
<td>The asset title</td>
</tr>
<tr class="">
<td>type</td>
<td>string</td>
<td></td>
<td>The asset type (audio, video, image etc)</td>
</tr>
<tr class="">
<td>url</td>
<td>string</td>
<td></td>
<td>If using an external asset, this should be the URL to the asset</td>
</tr>
</table>
      
      <h3 id="authored" class="dep">authored</h3>
      
      <div class="desc">Adds properties relating to authoring</div>

<div class="extension">This is a merge schema</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>createdAt</td>
<td>string</td>
<td></td>
<td>Date that the data was created</td>
</tr>
<tr class="required">
<td>createdBy</td>
<td>string</td>
<td></td>
<td>Author of the data</td>
</tr>
<tr class="required">
<td>updatedAt</td>
<td>string</td>
<td></td>
<td>Date that the data was last modified</td>
</tr>
</table>
      
      <h3 id="authroutes" class="dep">authroutes</h3>
      
      <div class="extension">Merges with <a href="#/schemas-reference?id=routes">routes</a></div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>type</td>
<td>string</td>
<td></td>
<td>Auth type identifier (e.g. 'local')</td>
</tr>
<tr class="">
<td>routes</td>
<td>array</td>
<td></td>
<td> </td>
</tr>
</table>
      
      <h3 id="authtoken" class="dep">authtoken</h3>
      
      <div class="desc">An authorisation token</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>signature</td>
<td>string</td>
<td></td>
<td>The JWT token signature for verification purposes</td>
</tr>
<tr class="required">
<td>userId</td>
<td>string</td>
<td></td>
<td>ID of the user this token belongs to</td>
</tr>
<tr class="required">
<td>createdAt</td>
<td>string</td>
<td></td>
<td>Token creation timestamp</td>
</tr>
<tr class="">
<td>usedAt</td>
<td>string</td>
<td></td>
<td>Token last use timestamp</td>
</tr>
<tr class="required">
<td>authType</td>
<td>string</td>
<td></td>
<td>Type of authentication used with this token</td>
</tr>
</table>
      
      <h3 id="authuser" class="dep">authuser</h3>
      
      <div class="desc">Extra user properties related to auth</div>

<div class="extension">This is a merge schema</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>authType</td>
<td>string</td>
<td></td>
<td>Types of authentication used with this user</td>
</tr>
</table>
      
      <h3 id="contentassets" class="dep">contentassets</h3>
      
      <div class="desc">Tracks asset IDs referenced by content items</div>

<div class="extension">This is a merge schema</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_assetIds</td>
<td>array</td>
<td><pre>[]</pre></td>
<td> </td>
</tr>
</table>
      
      <h3 id="contentplugin" class="dep">contentplugin</h3>
      
      <div class="desc">An Adapt framework plugin</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>name</td>
<td>string</td>
<td></td>
<td>Unique name for the plugin</td>
</tr>
<tr class="">
<td>displayName</td>
<td>string</td>
<td></td>
<td>User-friendly name for the plugin</td>
</tr>
<tr class="required">
<td>version</td>
<td>string</td>
<td></td>
<td>Version number for the plugin</td>
</tr>
<tr class="required">
<td>framework</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="required">
<td>isLocalInstall</td>
<td>boolean</td>
<td></td>
<td>Whether the plugin has been installed locally (as opposed to with the CLI)</td>
</tr>
<tr class="">
<td>isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="required">
<td>type</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>targetAttribute</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>description</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>pluginDependencies</td>
<td>object</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>canBeUpdated</td>
<td>boolean</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>latestCompatibleVersion</td>
<td>boolean</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>isAddedByDefault</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Whether the plugin should be added by default for new courses</td>
</tr>
</table>
      
      <h3 id="coursethemepreset" class="dep">coursethemepreset</h3>
      
      <div class="desc">A reusable collection of theme settings</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>displayName</td>
<td>string</td>
<td></td>
<td>User-friendly name for the settings</td>
</tr>
<tr class="required">
<td>parentTheme</td>
<td>string</td>
<td></td>
<td>Name of the theme these settings should be applied to</td>
</tr>
<tr class="">
<td>properties</td>
<td>object</td>
<td></td>
<td>The theme settings</td>
</tr>
</table>
      
      <h3 id="localauthuser" class="dep">localauthuser</h3>
      
      <div class="desc">Local authentication user</div>

<div class="extension">Merges with <a href="#/schemas-reference?id=user">user</a></div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>isTempLocked</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Whether the user account has been temporarily locked</td>
</tr>
<tr class="">
<td>isPermLocked</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Whether the user account has been permanently locked</td>
</tr>
<tr class="required">
<td>password</td>
<td>string</td>
<td></td>
<td>Password for the user</td>
</tr>
<tr class="">
<td>failedLoginAttempts</td>
<td>number</td>
<td><pre>0</pre></td>
<td>The number of failed login attempts</td>
</tr>
<tr class="">
<td>lastFailedLoginAttempt</td>
<td>string</td>
<td></td>
<td>Timestamp of the last failed login attempt</td>
</tr>
</table>
      
      <h3 id="localpassword" class="dep">localpassword</h3>
      
      <div class="desc">Local authentication password</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>password</td>
<td>string</td>
<td></td>
<td>Password value</td>
</tr>
</table>
      
      <h3 id="log" class="dep">log</h3>
      
      <div class="desc">A system log message</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>level</td>
<td>string</td>
<td></td>
<td>The priority level of the log message</td>
</tr>
<tr class="">
<td>module</td>
<td>string</td>
<td></td>
<td>Module responsible for creating the log</td>
</tr>
<tr class="">
<td>timestamp</td>
<td>string</td>
<td></td>
<td>Time log was created</td>
</tr>
<tr class="">
<td>data</td>
<td>array</td>
<td></td>
<td>The data to be logged</td>
</tr>
</table>
      
      <h3 id="maildata" class="dep">maildata</h3>
      
      <div class="desc">Email data</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>to</td>
<td>string</td>
<td></td>
<td>Recipient email address</td>
</tr>
<tr class="required">
<td>from</td>
<td>string</td>
<td></td>
<td>Sender email address</td>
</tr>
<tr class="required">
<td>subject</td>
<td>string</td>
<td></td>
<td>Email subject</td>
</tr>
<tr class="required">
<td>text</td>
<td>string</td>
<td></td>
<td>Email text content</td>
</tr>
<tr class="">
<td>html</td>
<td>string</td>
<td></td>
<td>Email HTML content</td>
</tr>
</table>
      
      <h3 id="role" class="dep">role</h3>
      
      <div class="desc">A user role</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>shortName</td>
<td>string</td>
<td></td>
<td>Short name for the role</td>
</tr>
<tr class="required">
<td>displayName</td>
<td>string</td>
<td></td>
<td>Human-readable representation of the role</td>
</tr>
<tr class="">
<td>extends</td>
<td>string</td>
<td></td>
<td>The parent role that this role should inherit scopes from</td>
</tr>
<tr class="required">
<td>scopes</td>
<td>array</td>
<td></td>
<td>Scopes relevant to this role</td>
</tr>
</table>
      
      <h3 id="routeitem" class="dep">routeitem</h3>
      
      <div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>route</td>
<td>string</td>
<td></td>
<td>Express-style route path</td>
</tr>
<tr class="required">
<td>handlers</td>
<td>object</td>
<td></td>
<td>Keys are HTTP methods, values are handler name strings</td>
</tr>
<tr class="">
<td>internal</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Restrict route to localhost</td>
</tr>
<tr class="">
<td>permissions</td>
<td>object</td>
<td></td>
<td>Keys are HTTP methods, values are permission scope arrays or null for unsecured</td>
</tr>
<tr class="">
<td>meta</td>
<td>object</td>
<td></td>
<td>Keys are HTTP methods, values are OpenAPI operation objects</td>
</tr>
<tr class="">
<td>override</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>When true and a defaults template is in use, merges this route's properties onto the matching default route (by path) instead of adding a duplicate</td>
</tr>
</table>
      
      <h3 id="routes" class="dep">routes</h3>
      
      <div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>root</td>
<td>string</td>
<td></td>
<td>Router root path</td>
</tr>
<tr class="">
<td>routes</td>
<td>array</td>
<td></td>
<td>Route definitions</td>
</tr>
</table>
      
      <h3 id="tag" class="dep">tag</h3>
      
      <div class="desc">Tag metadata applied to other objects</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>title</td>
<td>string</td>
<td></td>
<td>The tag title</td>
</tr>
</table>
      
      <h3 id="tags" class="dep">tags</h3>
      
      <div class="desc">Extra properties to define tags</div>

<div class="extension">This is a merge schema</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>tags</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>Add tags by entering one or more words, separated with a comma (,)</td>
</tr>
</table>
      
      <h3 id="user" class="dep">user</h3>
      
      <div class="desc">A system user</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>email</td>
<td>string</td>
<td></td>
<td>Email address for the user</td>
</tr>
<tr class="">
<td>firstName</td>
<td>string</td>
<td><pre>"Adapt"</pre></td>
<td>First name of the user</td>
</tr>
<tr class="">
<td>lastName</td>
<td>string</td>
<td><pre>"User"</pre></td>
<td>Last name of the user</td>
</tr>
<tr class="">
<td>isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Whether the user is able to access the system</td>
</tr>
<tr class="">
<td>lastAccess</td>
<td>string</td>
<td></td>
<td>Timestamp of the last access</td>
</tr>
</table>
      
      <h3 id="userroles" class="dep">userroles</h3>
      
      <div class="desc">Extra user properties for specifying roles</div>

<div class="extension">Patches <a href="#/schemas-reference?id=user">user</a></div><table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>roles</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>Roles assigned to this user</td>
</tr>
</table>
      
      