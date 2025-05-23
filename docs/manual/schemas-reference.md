# Schemas reference

This page documents all schemas defined in the authoring tool core bundle. Where relevant, any schema inheritance is noted, along with which fields are required.

### Quick navigation

<ul class="toc">
<li><a href="#/schemas-reference?id=adaptbuild">adaptbuild</a></li>
<li><a href="#/schemas-reference?id=article">article</a></li>
<li><a href="#/schemas-reference?id=asset">asset</a></li>
<li><a href="#/schemas-reference?id=authored">authored</a></li>
<li><a href="#/schemas-reference?id=authtoken">authtoken</a></li>
<li><a href="#/schemas-reference?id=authuser">authuser</a></li>
<li><a href="#/schemas-reference?id=base">base</a></li>
<li><a href="#/schemas-reference?id=block">block</a></li>
<li><a href="#/schemas-reference?id=component">component</a></li>
<li><a href="#/schemas-reference?id=config">config</a></li>
<li><a href="#/schemas-reference?id=content">content</a></li>
<li><a href="#/schemas-reference?id=contentobject">contentobject</a></li>
<li><a href="#/schemas-reference?id=contentplugin">contentplugin</a></li>
<li><a href="#/schemas-reference?id=course">course</a></li>
<li><a href="#/schemas-reference?id=courseasset">courseasset</a></li>
<li><a href="#/schemas-reference?id=coursethemepreset">coursethemepreset</a></li>
<li><a href="#/schemas-reference?id=defaultplugins">defaultplugins</a></li>
<li><a href="#/schemas-reference?id=localauthuser">localauthuser</a></li>
<li><a href="#/schemas-reference?id=localpassword">localpassword</a></li>
<li><a href="#/schemas-reference?id=log">log</a></li>
<li><a href="#/schemas-reference?id=maildata">maildata</a></li>
<li><a href="#/schemas-reference?id=role">role</a></li>
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
      
      <h3 id="article" class="dep">article</h3>
      
      <div class="extension">Merges with <a href="#/schemas-reference?id=content">content</a></div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_requireCompletionOf</td>
<td>number</td>
<td><pre>-1</pre></td>
<td>The number of blocks within this article the learner must complete in order for this article to be set as completed. A value of -1 requires all of them to be completed</td>
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
      
      <h3 id="base" class="dep">base</h3>
      
      <div class="desc">The base schema inherited by all other schemas</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="block" class="dep">block</h3>
      
      <div class="extension">Merges with <a href="#/schemas-reference?id=content">content</a></div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_trackingId</td>
<td>number</td>
<td><pre>0</pre></td>
<td> </td>
</tr>
<tr class="">
<td>layoutOptions</td>
<td>array</td>
<td><pre>[]</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_requireCompletionOf</td>
<td>number</td>
<td><pre>-1</pre></td>
<td>The number of components within this block the learner must complete in order for this block to be set as completed. A value of -1 requires all of them to be completed</td>
</tr>
</table>
      
      <h3 id="component" class="dep">component</h3>
      
      <div class="extension">Merges with <a href="#/schemas-reference?id=content">content</a></div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>_component</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>displayTitle</td>
<td>undefined</td>
<td><pre>"Untitled"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_layout</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_isResetOnRevisit</td>
<td>string</td>
<td><pre>"false"</pre></td>
<td>Controls whether this component will be reset when the learner leaves the page then returns to it. The 'soft' setting will reset the component to allow the learner to attempt it again, but will not require them to do so; whereas the 'hard' setting will require them to do so. The default (false) will not cause the component to be reset</td>
</tr>
<tr class="">
<td>_isA11yCompletionDescriptionEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether a hidden label is appended to the component title that describes the completion state of the component.</td>
</tr>
<tr class="">
<td>properties</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
</table>
      
      <h3 id="config" class="dep">config</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_type</td>
<td>string</td>
<td><pre>"config"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_extensions</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_enabledPlugins</td>
<td>array</td>
<td><pre>[]</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_theme</td>
<td>string</td>
<td><pre>"adapt-contrib-vanilla"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_menu</td>
<td>string</td>
<td><pre>"adapt-contrib-boxMenu"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_courseId</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>_completionCriteria</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_completionCriteria._requireContentCompleted</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_completionCriteria._requireAssessmentCompleted</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_completionCriteria._submitOnEveryAssessmentAttempt</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled and the course completion criteria is met, the completion status will be reported every time the assessment is completed (regardless of whether the user passes or fails)</td>
</tr>
<tr class="">
<td>_completionCriteria._shouldSubmitScore</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, the score attained in any assessment attempt will be reported (regardless of whether the user passes or fails)</td>
</tr>
<tr class="">
<td>_defaultLanguage</td>
<td>string</td>
<td><pre>"en"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_defaultDirection</td>
<td>string</td>
<td><pre>"ltr"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._isSkipNavigationEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Adds a link to the start of the page to allow assistive technology users to skip over the navigation and straight into to the page content</td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels</td>
<td>object</td>
<td><pre>{}</pre></td>
<td>Defines what value to assign to the aria-level attribute for the various elements of Adapt</td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._menu</td>
<td>string</td>
<td><pre>"1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._menuGroup</td>
<td>string</td>
<td><pre>"@menu+1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._menuItem</td>
<td>string</td>
<td><pre>"@menu+1"</pre></td>
<td>This will need to be changed to 3 if menu groups are being used and A11Y support is required</td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._page</td>
<td>string</td>
<td><pre>"1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._article</td>
<td>string</td>
<td><pre>"@page+1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._block</td>
<td>string</td>
<td><pre>"@article+1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._component</td>
<td>string</td>
<td><pre>"@block+1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._componentItem</td>
<td>string</td>
<td><pre>"@component+1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._ariaLevels._notify</td>
<td>string</td>
<td><pre>"1"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_accessibility._options</td>
<td>object</td>
<td><pre>{}</pre></td>
<td>Optional object that can be used to customize the accessibility behaviour</td>
</tr>
<tr class="">
<td>_fixes</td>
<td>object</td>
<td><pre>{"_imgLazyLoad":true}</pre></td>
<td>Optional object that can be used to customize the application of fixes</td>
</tr>
<tr class="">
<td>screenSize</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>screenSize.small</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Pixel width for the start of the small breakpoint, e.g. cellphones</td>
</tr>
<tr class="">
<td>screenSize.medium</td>
<td>number</td>
<td><pre>720</pre></td>
<td>Pixel width for the start of the medium breakpoint, e.g. tablet devices</td>
</tr>
<tr class="">
<td>screenSize.large</td>
<td>number</td>
<td><pre>960</pre></td>
<td>Pixel width for the start of the large breakpoint, e.g. laptop/desktop computers</td>
</tr>
<tr class="">
<td>screenSize.xlarge</td>
<td>number</td>
<td><pre>1280</pre></td>
<td>Pixel width for the start of the extra large breakpoint, e.g. hd laptop/desktop computers</td>
</tr>
<tr class="">
<td>_questionWeight</td>
<td>number</td>
<td><pre>1</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer._showEasing</td>
<td>string</td>
<td><pre>"easeOutQuart"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer._hideEasing</td>
<td>string</td>
<td><pre>"easeInQuart"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer._duration</td>
<td>number</td>
<td><pre>400</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer._position</td>
<td>string</td>
<td><pre>"auto"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer._iconClass</td>
<td>string</td>
<td><pre>"icon-list"</pre></td>
<td>CSS class name to be applied to the drawer sidebar icon.</td>
</tr>
<tr class="">
<td>_notify</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify._duration</td>
<td>number</td>
<td><pre>400</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_generateSourcemap</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Allows the course JavaScript & CSS to be debugged via the browser's developer tools</td>
</tr>
<tr class="">
<td>_forceRouteLocking</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>If locking is enabled, this setting prevents navigating to locked routes</td>
</tr>
<tr class="">
<td>_disableAnimationFor</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>Allows you to disable some animations (e.g. the drawer close animation) on platform(s) where they are not performing well, using CSS selectors to target the relevant platform(s) via the classes on the HTML element</td>
</tr>
<tr class="">
<td>_logging</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_logging._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_logging._level</td>
<td>string</td>
<td><pre>"info"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_logging._console</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_logging._warnFirstOnly</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_scrollingContainer</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_scrollingContainer._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_scrollingContainer._limitToSelector</td>
<td>string</td>
<td><pre>""</pre></td>
<td>CSS selector to match against the HTML element when determining whether this should be active or not</td>
</tr>
<tr class="">
<td>themeSettings</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_themePreset</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>build</td>
<td>object</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>build.strictMode</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Strict mode improves performance by tightly restricting the declaration of variables inside code blocks and closures which may cause some older code to stop working. Please leave this at true unless you are experiencing issue with old plugins or third party libraries.</td>
</tr>
<tr class="">
<td>build.targets</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the browsers that are supported. Overwrites the framework defaults if not empty. Current defaults are: 'last 2 chrome versions, last 2 firefox versions, last 2 safari versions, last 2 edge versions, last 2 ios_saf versions, last 2 and_chr versions, firefox esr'</td>
</tr>
</table>
      
      <h3 id="content" class="dep">content</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_type</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>_friendlyId</td>
<td>string</td>
<td></td>
<td>A human-readable ID for this content object which will replace the standard _id field on course build (useful in instances where the _id must be specified in the config of an extension). Must be unique to this course.</td>
</tr>
<tr class="">
<td>_parentId</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>_courseId</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>title</td>
<td>string</td>
<td><pre>"Untitled"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>displayTitle</td>
<td>string</td>
<td><pre>""</pre></td>
<td>When viewing an element - this is the title that will be displayed on the page</td>
</tr>
<tr class="">
<td>body</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>instruction</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_classes</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Used to style or manipulate the look and feel of this element. These are predefined in the theme or added in Project Settings > Custom CSS/Less code</td>
</tr>
<tr class="">
<td>_isOptional</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>An optional element does not have to be completed, nor do any of the elements contained within it</td>
</tr>
<tr class="">
<td>_isAvailable</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether this element and its contents are available in the course or not</td>
</tr>
<tr class="">
<td>_isHidden</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Enabling this is equivalent to applying the CSS 'display:none' to the element</td>
</tr>
<tr class="">
<td>_isVisible</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Disabling this is equivalent to applying the CSS 'visibility:hidden' to the element</td>
</tr>
<tr class="">
<td>_isA11yCompletionDescriptionEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether a hidden label is appended to the element title that describes the completion state of the element.</td>
</tr>
<tr class="">
<td>_onScreen</td>
<td>object</td>
<td><pre>{}</pre></td>
<td>These settings allow you to attach classes to the element when it is within the browser's viewport; helpful for running CSS-based animations on elements as they scroll into view</td>
</tr>
<tr class="">
<td>_onScreen._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_onScreen._classes</td>
<td>string</td>
<td><pre>""</pre></td>
<td>The CSS class(es) to add to the element</td>
</tr>
<tr class="">
<td>_onScreen._percentInviewVertical</td>
<td>number</td>
<td><pre>50</pre></td>
<td>Controls what percentage of the element's height needs to be in the viewport in order for the CSS class(es) to be added</td>
</tr>
<tr class="">
<td>_extensions</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_sortOrder</td>
<td>number</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>themeSettings</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_colorLabel</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
</table>
      
      <h3 id="contentobject" class="dep">contentobject</h3>
      
      <div class="extension">Merges with <a href="#/schemas-reference?id=content">content</a></div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>displayTitle</td>
<td>undefined</td>
<td><pre>"Untitled"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>subtitle</td>
<td>string</td>
<td><pre>""</pre></td>
<td>When viewing a menu/page - this is the subtitle that will be displayed on the menu/page</td>
</tr>
<tr class="">
<td>pageBody</td>
<td>string</td>
<td><pre>""</pre></td>
<td>If set, this text will be shown instead of the body text when this page is viewed</td>
</tr>
<tr class="">
<td>_htmlClasses</td>
<td>string</td>
<td><pre>""</pre></td>
<td>If set, this CSS class/es will be applied to the <html> element whenever this is the active page in the course. These are predefined in the theme or added in Project Settings > Custom CSS/Less code</td>
</tr>
<tr class="">
<td>_graphic</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_graphic.alt</td>
<td>string</td>
<td><pre>""</pre></td>
<td>A description of the image; required when it has meaning that must be conveyed to the learner. For 'decorative' images, leave this blank</td>
</tr>
<tr class="">
<td>_graphic.src</td>
<td>string</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>linkText</td>
<td>string</td>
<td><pre>"View"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>duration</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Indicates how long this page or section should take to complete</td>
</tr>
<tr class="">
<td>_lockedBy</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>If the course is using a 'custom' menu lock type, this should contain the unique ID of the item(s) which must be completed before this is unlocked</td>
</tr>
<tr class="">
<td>_lockType</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines which (if any) locking mechanism will be used. To be used only on submenus</td>
</tr>
<tr class="">
<td>_requireCompletionOf</td>
<td>number</td>
<td><pre>-1</pre></td>
<td>The number of articles within this page the learner must complete in order for this page to be set as completed. A value of -1 requires all of them to be completed</td>
</tr>
<tr class="">
<td>menuSettings</td>
<td>object</td>
<td><pre>{}</pre></td>
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
</table>
      
      <h3 id="course" class="dep">course</h3>
      
      <div class="extension">Merges with <a href="#/schemas-reference?id=content">content</a></div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>displayTitle</td>
<td>undefined</td>
<td><pre>"Untitled"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>heroImage</td>
<td>string</td>
<td></td>
<td>The image that will be shown in the dashboard for this course</td>
</tr>
<tr class="">
<td>subtitle</td>
<td>string</td>
<td><pre>""</pre></td>
<td>This is the subtitle that will be displayed on the course's main menu</td>
</tr>
<tr class="">
<td>description</td>
<td>string</td>
<td><pre>""</pre></td>
<td>This will be added to the course's manifest file metadata. It is not (currently) displayed anywhere within the course</td>
</tr>
<tr class="">
<td>_htmlClasses</td>
<td>string</td>
<td><pre>""</pre></td>
<td>If set, this class will be applied to the <html> element when the top-level menu in the course is displayed. These are predefined in the theme or added in Custom CSS/Less code</td>
</tr>
<tr class="">
<td>_latestTrackingId</td>
<td>number</td>
<td><pre>0</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_start</td>
<td>object</td>
<td><pre>{}</pre></td>
<td>The start settings allow you to control which page is rendered when a course loads, potentially bypassing the menu</td>
</tr>
<tr class="">
<td>_start._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_start._startIds</td>
<td>array</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>_start._force</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, the routing will be forced to the appropriate start page, regardless of the URL</td>
</tr>
<tr class="">
<td>_start._isMenuDisabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Allows you to prevent the user from seeing - or navigating to - the main menu</td>
</tr>
<tr class="">
<td>_globals</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility.skipNavigationText</td>
<td>string</td>
<td><pre>"Skip to main content"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.answeredIncorrectly</td>
<td>string</td>
<td><pre>"You answered incorrectly"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.answeredCorrectly</td>
<td>string</td>
<td><pre>"You answered correctly"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.selectedAnswer</td>
<td>string</td>
<td><pre>"selected"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.unselectedAnswer</td>
<td>string</td>
<td><pre>"not selected"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.skipNavigation</td>
<td>string</td>
<td><pre>"Skip navigation"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.previous</td>
<td>string</td>
<td><pre>"Back"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.navigationDrawer</td>
<td>string</td>
<td><pre>"Open course resources."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.close</td>
<td>string</td>
<td><pre>"Close"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.closeDrawer</td>
<td>string</td>
<td><pre>"Close Drawer"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.closeResources</td>
<td>string</td>
<td><pre>"Close resources"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.drawer</td>
<td>string</td>
<td><pre>"Top of side drawer"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.closePopup</td>
<td>string</td>
<td><pre>"Close popup"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.next</td>
<td>string</td>
<td><pre>"Next"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.done</td>
<td>string</td>
<td><pre>"Done"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.complete</td>
<td>string</td>
<td><pre>"Completed"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.incomplete</td>
<td>string</td>
<td><pre>"Incomplete"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.incorrect</td>
<td>string</td>
<td><pre>"Incorrect"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.correct</td>
<td>string</td>
<td><pre>"Correct"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.locked</td>
<td>string</td>
<td><pre>"Locked"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.visited</td>
<td>string</td>
<td><pre>"Visited"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.required</td>
<td>string</td>
<td><pre>"Required"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.optional</td>
<td>string</td>
<td><pre>"Optional"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.topOfContentObject</td>
<td>string</td>
<td><pre>"{{type}} {{displayTitle}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.course</td>
<td>string</td>
<td><pre>"Main menu"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.menu</td>
<td>string</td>
<td><pre>"Sub menu"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility._ariaLabels.page</td>
<td>string</td>
<td><pre>"Page"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accessibility.altFeedbackTitle</td>
<td>string</td>
<td><pre>"Feedback"</pre></td>
<td>Text read out by screen readers if no visual title is set for component question feedback.</td>
</tr>
<tr class="">
<td>_globals._extensions</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._drawer</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._drawer._navOrder</td>
<td>number</td>
<td><pre>100</pre></td>
<td>Determines the order in which the object is displayed in the navigation bar. Negative numbers (e.g. -100) are left-aligned. Positive numbers (e.g. 100) are right-aligned.</td>
</tr>
<tr class="">
<td>_globals._extensions._drawer._navTooltip</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._drawer._navTooltip._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._drawer._navTooltip.text</td>
<td>string</td>
<td><pre>"{{ariaLabel}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._navigation</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._skipButton</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._skipButton._navOrder</td>
<td>number</td>
<td><pre>-100</pre></td>
<td>Determines the order in which the object is displayed in the navigation bar. Negative numbers (e.g. -100) are left-aligned. Positive numbers (e.g. 100) are right-aligned.</td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._backButton</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._backButton._navOrder</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Determines the order in which the object is displayed in the navigation bar. Negative numbers (e.g. -100) are left-aligned. Positive numbers (e.g. 100) are right-aligned.</td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._backNavTooltip</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._backNavTooltip._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._backNavTooltip.text</td>
<td>string</td>
<td><pre>"{{ariaLabel}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._extensions._navigation._spacers</td>
<td>array</td>
<td><pre>[{"_navOrder":0}]</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_tooltips</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_tooltips._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._submit</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._submit.buttonText</td>
<td>string</td>
<td><pre>"Submit"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._submit.ariaLabel</td>
<td>string</td>
<td><pre>"Submit"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._reset</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._reset.buttonText</td>
<td>string</td>
<td><pre>"Reset"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._reset.ariaLabel</td>
<td>string</td>
<td><pre>"Reset"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._showCorrectAnswer</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._showCorrectAnswer.buttonText</td>
<td>string</td>
<td><pre>"Show correct answer"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._showCorrectAnswer.ariaLabel</td>
<td>string</td>
<td><pre>"Show correct answer"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._hideCorrectAnswer</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._hideCorrectAnswer.buttonText</td>
<td>string</td>
<td><pre>"Show your answer"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._hideCorrectAnswer.ariaLabel</td>
<td>string</td>
<td><pre>"Show your answer"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._showFeedback</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._showFeedback.buttonText</td>
<td>string</td>
<td><pre>"Show feedback"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons._showFeedback.ariaLabel</td>
<td>string</td>
<td><pre>"Show feedback"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons.remainingAttemptsText</td>
<td>string</td>
<td><pre>"attempts remaining"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons.remainingAttemptText</td>
<td>string</td>
<td><pre>"final attempt"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons.disabledAriaLabel</td>
<td>string</td>
<td><pre>"This button is disabled at the moment"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_navigation</td>
<td>object</td>
<td><pre>{}</pre></td>
<td>The navigation settings allow you to control the behaviour of the navigation bar.</td>
</tr>
<tr class="">
<td>_navigation._isDefaultNavigationDisabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_navigation._navigationAlignment</td>
<td>string</td>
<td><pre>"top"</pre></td>
<td>The CSS selector that determines where the navigation bar is displayed. Must be a selector targeting the HTML element.</td>
</tr>
<tr class="">
<td>_navigation._isBottomOnTouchDevices</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_navigation._showLabel</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_navigation._showLabelAtWidth</td>
<td>string</td>
<td><pre>"medium"</pre></td>
<td>When the user's browser window is at least this wide, the labels will be shown. Options refer to the standard Adapt breakpoints. The 'any' option will show the label at any size.</td>
</tr>
<tr class="">
<td>_navigation._labelPosition</td>
<td>string</td>
<td><pre>"auto"</pre></td>
<td>Where to show the label in relation to the button icons</td>
</tr>
<tr class="">
<td>tags</td>
<td>array</td>
<td></td>
<td>Add tags to your course by entering one or more words, separated with a comma (,)</td>
</tr>
<tr class="">
<td>_requireCompletionOf</td>
<td>number</td>
<td><pre>-1</pre></td>
<td>The number of content objects within this course the learner must complete in order for this course to be set as completed. A value of -1 requires all of them to be completed</td>
</tr>
<tr class="">
<td>_isSelected</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_hasPreview</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_isShared</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Defines whether this course will be editable by all users</td>
</tr>
<tr class="">
<td>_shareWithUsers</td>
<td>array</td>
<td></td>
<td>Defines which individual users are able to edit this course</td>
</tr>
<tr class="">
<td>themeVariables</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>menuSettings</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_lockType</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines which (if any) locking mechanism will be used for menu items</td>
</tr>
<tr class="">
<td>customStyle</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Add any custom CSS or valid Less code here</td>
</tr>
<tr class="">
<td>externalReferences</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
</table>
      
      <h3 id="courseasset" class="dep">courseasset</h3>
      
      <div class="desc">Metadata related to where an asset is used in a course</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="required">
<td>courseId</td>
<td>string</td>
<td></td>
<td>Course record unique ID</td>
</tr>
<tr class="required">
<td>contentId</td>
<td>string</td>
<td></td>
<td>The ID for the content record that uses this asset</td>
</tr>
<tr class="required">
<td>assetId</td>
<td>string</td>
<td></td>
<td>Asset record unique ID</td>
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
      
      <h3 id="defaultplugins" class="dep">defaultplugins</h3>
      
      <div class="desc">Defines whether plugins should be added as default</div>

<div class="extension">Patches <a href="#/schemas-reference?id=contentplugin">contentplugin</a></div><table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>isAddedByDefault</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Whether the plugin should be added by default for new courses</td>
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
      
      