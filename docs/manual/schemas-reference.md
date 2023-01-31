# Schemas reference

This page documents all schemas defined in the authoring tool core bundle. Where relevant, any schema inheritance is noted, along with which fields are required.

### Quick navigation

<ul class="toc">
<li><a href="#/schemas-reference?id=accordion-component">accordion-component</a></li>
<li><a href="#/schemas-reference?id=accordion-course">accordion-course</a></li>
<li><a href="#/schemas-reference?id=adaptbuild">adaptbuild</a></li>
<li><a href="#/schemas-reference?id=article">article</a></li>
<li><a href="#/schemas-reference?id=assessment-article">assessment-article</a></li>
<li><a href="#/schemas-reference?id=assessment-block">assessment-block</a></li>
<li><a href="#/schemas-reference?id=assessment-course">assessment-course</a></li>
<li><a href="#/schemas-reference?id=assessmentResults-component">assessmentResults-component</a></li>
<li><a href="#/schemas-reference?id=assessmentResults-course">assessmentResults-course</a></li>
<li><a href="#/schemas-reference?id=asset">asset</a></li>
<li><a href="#/schemas-reference?id=authored">authored</a></li>
<li><a href="#/schemas-reference?id=authtoken">authtoken</a></li>
<li><a href="#/schemas-reference?id=authuser">authuser</a></li>
<li><a href="#/schemas-reference?id=base">base</a></li>
<li><a href="#/schemas-reference?id=blank-component">blank-component</a></li>
<li><a href="#/schemas-reference?id=block">block</a></li>
<li><a href="#/schemas-reference?id=bookmarking-contentobject">bookmarking-contentobject</a></li>
<li><a href="#/schemas-reference?id=bookmarking-course">bookmarking-course</a></li>
<li><a href="#/schemas-reference?id=boxMenu-contentobject">boxMenu-contentobject</a></li>
<li><a href="#/schemas-reference?id=boxMenu-course">boxMenu-course</a></li>
<li><a href="#/schemas-reference?id=component">component</a></li>
<li><a href="#/schemas-reference?id=config">config</a></li>
<li><a href="#/schemas-reference?id=content">content</a></li>
<li><a href="#/schemas-reference?id=contentobject">contentobject</a></li>
<li><a href="#/schemas-reference?id=contentplugin">contentplugin</a></li>
<li><a href="#/schemas-reference?id=course">course</a></li>
<li><a href="#/schemas-reference?id=courseasset">courseasset</a></li>
<li><a href="#/schemas-reference?id=coursethemepreset">coursethemepreset</a></li>
<li><a href="#/schemas-reference?id=defaultplugins">defaultplugins</a></li>
<li><a href="#/schemas-reference?id=gmcq-component">gmcq-component</a></li>
<li><a href="#/schemas-reference?id=gmcq-course">gmcq-course</a></li>
<li><a href="#/schemas-reference?id=graphic-component">graphic-component</a></li>
<li><a href="#/schemas-reference?id=graphic-course">graphic-course</a></li>
<li><a href="#/schemas-reference?id=hotgraphic-component">hotgraphic-component</a></li>
<li><a href="#/schemas-reference?id=hotgraphic-course">hotgraphic-course</a></li>
<li><a href="#/schemas-reference?id=languagePicker-config">languagePicker-config</a></li>
<li><a href="#/schemas-reference?id=languagePicker-course">languagePicker-course</a></li>
<li><a href="#/schemas-reference?id=localauthuser">localauthuser</a></li>
<li><a href="#/schemas-reference?id=log">log</a></li>
<li><a href="#/schemas-reference?id=matching-component">matching-component</a></li>
<li><a href="#/schemas-reference?id=matching-course">matching-course</a></li>
<li><a href="#/schemas-reference?id=mcq-component">mcq-component</a></li>
<li><a href="#/schemas-reference?id=mcq-course">mcq-course</a></li>
<li><a href="#/schemas-reference?id=media-component">media-component</a></li>
<li><a href="#/schemas-reference?id=media-course">media-course</a></li>
<li><a href="#/schemas-reference?id=narrative-component">narrative-component</a></li>
<li><a href="#/schemas-reference?id=narrative-course">narrative-course</a></li>
<li><a href="#/schemas-reference?id=pageLevelProgress-article">pageLevelProgress-article</a></li>
<li><a href="#/schemas-reference?id=pageLevelProgress-block">pageLevelProgress-block</a></li>
<li><a href="#/schemas-reference?id=pageLevelProgress-component">pageLevelProgress-component</a></li>
<li><a href="#/schemas-reference?id=pageLevelProgress-contentobject">pageLevelProgress-contentobject</a></li>
<li><a href="#/schemas-reference?id=pageLevelProgress-course">pageLevelProgress-course</a></li>
<li><a href="#/schemas-reference?id=resources-contentobject">resources-contentobject</a></li>
<li><a href="#/schemas-reference?id=resources-course">resources-course</a></li>
<li><a href="#/schemas-reference?id=role">role</a></li>
<li><a href="#/schemas-reference?id=slider-component">slider-component</a></li>
<li><a href="#/schemas-reference?id=slider-course">slider-course</a></li>
<li><a href="#/schemas-reference?id=spoor-config">spoor-config</a></li>
<li><a href="#/schemas-reference?id=spoor-course">spoor-course</a></li>
<li><a href="#/schemas-reference?id=spoorcontent">spoorcontent</a></li>
<li><a href="#/schemas-reference?id=spoorcourse">spoorcourse</a></li>
<li><a href="#/schemas-reference?id=tag">tag</a></li>
<li><a href="#/schemas-reference?id=tags">tags</a></li>
<li><a href="#/schemas-reference?id=text-component">text-component</a></li>
<li><a href="#/schemas-reference?id=text-course">text-course</a></li>
<li><a href="#/schemas-reference?id=textinput-component">textinput-component</a></li>
<li><a href="#/schemas-reference?id=textinput-course">textinput-course</a></li>
<li><a href="#/schemas-reference?id=trickle-article">trickle-article</a></li>
<li><a href="#/schemas-reference?id=trickle-block">trickle-block</a></li>
<li><a href="#/schemas-reference?id=trickle-config">trickle-config</a></li>
<li><a href="#/schemas-reference?id=trickle-course">trickle-course</a></li>
<li><a href="#/schemas-reference?id=user">user</a></li>
<li><a href="#/schemas-reference?id=userroles">userroles</a></li>
<li><a href="#/schemas-reference?id=vanilla-article">vanilla-article</a></li>
<li><a href="#/schemas-reference?id=vanilla-block">vanilla-block</a></li>
<li><a href="#/schemas-reference?id=vanilla-component">vanilla-component</a></li>
<li><a href="#/schemas-reference?id=vanilla-contentobject">vanilla-contentobject</a></li>
<li><a href="#/schemas-reference?id=vanilla-theme">vanilla-theme</a></li>
</ul>


<h3 id="accordion-component" class="dep">accordion-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="accordion-course" class="dep">accordion-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="adaptbuild" class="dep">adaptbuild</h3>
      
      <div class="desc">An Adapt course build instance</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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
<td>Author of the data</td>
</tr>
<tr class="">
<td>versions</td>
<td>object</td>
<td></td>
<td>Versions of framework and plugins used in the build</td>
</tr>
<tr class="required">
<td>createdAt</td>
<td>string</td>
<td></td>
<td>Date that the data was created</td>
</tr>
<tr class="required">
<td>updatedAt</td>
<td>string</td>
<td></td>
<td>Date that the data was last modified</td>
</tr>
</table>
      
      <h3 id="article" class="dep">article</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
<td>_assessment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment._id</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Unique name for the assessment. This is required by other plugins such as the 'Assessment Results' component to identify the assessment and display its variables</td>
</tr>
<tr class="">
<td>_assessment._attempts</td>
<td>number</td>
<td><pre>-1</pre></td>
<td>Controls the number of attempts the user is allowed to have on this assessment. Set to -1 (or 0) to allow infinite attempts</td>
</tr>
<tr class="">
<td>_assessment._isPercentageBased</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Determines whether the pass mark values should be treated as percentages (default) or as the raw score and correctness</td>
</tr>
<tr class="">
<td>_assessment._scoreToPass</td>
<td>number</td>
<td><pre>60</pre></td>
<td>The minimum score required by the learner to pass the assessment or the minimum percentage score if percentage-based</td>
</tr>
<tr class="">
<td>_assessment._correctToPass</td>
<td>number</td>
<td><pre>60</pre></td>
<td>The minimum number of correct questions required by the learner to pass the assessment or the minimum percentage correct if percentage-based</td>
</tr>
<tr class="">
<td>_assessment._includeInTotalScore</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Determines if the score from this assessment should be sent to the LMS. The score sent is a percentage according to 'Assessment weight'</td>
</tr>
<tr class="">
<td>_assessment._assessmentWeight</td>
<td>number</td>
<td><pre>1</pre></td>
<td>If there are multiple assessments in the course, this value controls the proportion of the LMS score which is attributed to this assessment, i.e. 1 equals 100%, 0.5 is 50%, etc.</td>
</tr>
<tr class="">
<td>_assessment._suppressMarking</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Determines whether question marking should be delayed until completion of the assessment or until all attempts have been exhausted</td>
</tr>
<tr class="">
<td>_assessment._isResetOnRevisit</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether the assessment should be reset automatically (up to the number of available attempts) when a user revisits the page</td>
</tr>
<tr class="">
<td>_assessment._allowResetIfPassed</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether the assessment may be reset after it has been passed (whilst there are attempts remaining)</td>
</tr>
<tr class="">
<td>_assessment._scrollToOnReset</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether to scroll to the assessment after reset or to stay at the top of the assessment page</td>
</tr>
<tr class="">
<td>_assessment._randomisation</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment._randomisation._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If randomisation is enabled, a specified number of blocks will be displayed to the user in a random order</td>
</tr>
<tr class="">
<td>_assessment._randomisation._blockCount</td>
<td>number</td>
<td><pre>-1</pre></td>
<td>The number of blocks to present to the learner. Set to -1 (or 0) to display all blocks</td>
</tr>
<tr class="">
<td>_assessment._banks</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment._banks._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Enables associating blocks of question components with a 'bank', allowing questions to be grouped then rendered via the 'Question counts' property</td>
</tr>
<tr class="">
<td>_assessment._banks._split</td>
<td>string</td>
<td><pre>""</pre></td>
<td>This is a comma-separated list of numbers corresponding to the number of questions to be drawn from each question bank. The position of the number in the list corresponds to the 'Bank ID' assigned, e.g. "3,2" would display three questions from Bank 1 and two from Bank 2</td>
</tr>
<tr class="">
<td>_assessment._banks._randomisation</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether the questions will be displayed in a random order</td>
</tr>
<tr class="">
<td>_assessment._questions</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment._questions._resetType</td>
<td>string</td>
<td><pre>"hard"</pre></td>
<td>Determines whether the question will register as completed when reset. When assigned a value of 'soft', the learner may continue to interact with it, but the complete attribute remains set to true. When assigned 'hard', complete is set to false, and the learner will be forced to complete it again if it is reset. For 'soft', when using trickle, please set the trickle Completion Attribute to `_isInteractionComplete'.</td>
</tr>
<tr class="">
<td>_assessment._questions._canShowFeedback</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Allows the user to view feedback on their answer</td>
</tr>
<tr class="">
<td>_assessment._questions._canShowMarking</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Displays ticks and crosses on question completion</td>
</tr>
<tr class="">
<td>_assessment._questions._canShowModelAnswer</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Allows the user to view the 'model answer' should they answer the question incorrectly</td>
</tr>
<tr class="">
<td>_trickle</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._autoScroll</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._scrollDuration</td>
<td>number</td>
<td><pre>500</pre></td>
<td>Duration of the scroll animation in milliseconds</td>
</tr>
<tr class="">
<td>_trickle._onChildren</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Set to false on the article to use trickle at article level</td>
</tr>
<tr class="">
<td>_trickle._scrollTo</td>
<td>string</td>
<td><pre>"@block +1"</pre></td>
<td>Set how trickle scrolls</td>
</tr>
<tr class="">
<td>_trickle._completionAttribute</td>
<td>string</td>
<td><pre>"_isComplete"</pre></td>
<td>Set which attribute is used to determine completion</td>
</tr>
<tr class="">
<td>_trickle._button</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._styleBeforeCompletion</td>
<td>string</td>
<td><pre>"hidden"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._styleAfterClick</td>
<td>string</td>
<td><pre>"hidden"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._isFullWidth</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._autoHide</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Hides the button when it scrolls from view; not recommended for use in courses that need to be screenreader compatible</td>
</tr>
<tr class="">
<td>_trickle._button._showEndOfPage</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._className</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._hasIcon</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Displays an icon alongside, or in place of, the Trickle button text. Default icon is a small downwards arrow</td>
</tr>
<tr class="">
<td>_trickle._button.text</td>
<td>string</td>
<td><pre>"Continue"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button.ariaLabel</td>
<td>string</td>
<td><pre>"Continue"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button.startText</td>
<td>string</td>
<td><pre>"Begin"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button.startAriaLabel</td>
<td>string</td>
<td><pre>"Begin"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button.finalText</td>
<td>string</td>
<td><pre>"Finish"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button.finalAriaLabel</td>
<td>string</td>
<td><pre>"Finish"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button._component</td>
<td>string</td>
<td><pre>"trickle-button"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking._isCompletionRequired</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking._isLockedOnRevisit</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isCompletionIndicatorEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._textAlignment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._title</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the article title. Left: Aligns the title to the left of the container. Center: Aligns the title to the center of the container. Right: Aligns the title to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._body</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the article body. Left: Aligns the body to the left of the container. Center: Aligns the body to the center of the container. Right: Aligns the body to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._instruction</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the article instruction. Left: Aligns the instruction to the left of the container. Center: Aligns the instruction to the center of the container. Right: Aligns the instruction to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._large</td>
<td>string</td>
<td></td>
<td>Large background image - used on desktop</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._medium</td>
<td>string</td>
<td></td>
<td>Medium background image - used on tablet</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._small</td>
<td>string</td>
<td></td>
<td>Small background image - used on mobile</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundRepeat</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Repeat-x: The background image is repeated only horizontally. Repeat-y: The background image is repeated only vertically</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundSize</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Auto: The background image is displayed in its original size. Cover: Resize the background image to cover the entire container, even if it has to stretch or crop the image. Contain: Resize the background image to make sure the image is fully visible. 100% 100%: Resize the background image to match the dimensions of the container</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundPosition</td>
<td>string</td>
<td><pre>""</pre></td>
<td>The first value is the horizontal position and the second value is the vertical</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._large</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Large CSS class - used on desktop</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._medium</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Medium CSS class - used on tablet</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._small</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Small CSS class - used on mobile</td>
</tr>
</table>
      
      <h3 id="assessment-article" class="dep">assessment-article</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="assessment-block" class="dep">assessment-block</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="assessment-course" class="dep">assessment-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="assessmentresults-component" class="dep">assessmentResults-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="assessmentresults-course" class="dep">assessmentResults-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="asset" class="dep">asset</h3>
      
      <div class="desc">An Adapt assets.json file</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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
<tr class="required">
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
<tr class="">
<td>tags</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>Add tags by entering one or more words, separated with a comma (,)</td>
</tr>
</table>
      
      <h3 id="authored" class="dep">authored</h3>
      
      <div class="desc">Adds properties relating to authoring</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="authtoken" class="dep">authtoken</h3>
      
      <div class="desc">An authorisation token</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
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
      
      <h3 id="blank-component" class="dep">blank-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="block" class="dep">block</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
<td>_assessment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment._quizBankID</td>
<td>number</td>
<td><pre>1</pre></td>
<td>Used to group blocks of question components into associated banks. This works in conjunction with the 'Question counts' property when question banks are in use</td>
</tr>
<tr class="">
<td>_trickle</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._isInherited</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._autoScroll</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._scrollDuration</td>
<td>number</td>
<td><pre>500</pre></td>
<td>Duration of the scroll animation in milliseconds</td>
</tr>
<tr class="">
<td>_trickle._scrollTo</td>
<td>string</td>
<td><pre>"@block +1"</pre></td>
<td>Set how trickle scrolls</td>
</tr>
<tr class="">
<td>_trickle._completionAttribute</td>
<td>string</td>
<td><pre>"_isComplete"</pre></td>
<td>Set which attribute is used to determine completion</td>
</tr>
<tr class="">
<td>_trickle._button</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._styleBeforeCompletion</td>
<td>string</td>
<td><pre>"hidden"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._styleAfterClick</td>
<td>string</td>
<td><pre>"hidden"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._isFullWidth</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._autoHide</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Hides the button when it scrolls from view; not recommended for use in courses that need to be screenreader compatible</td>
</tr>
<tr class="">
<td>_trickle._button._showEndOfPage</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._className</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button._hasIcon</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Displays an icon alongside, or in place of, the Trickle button text. Default icon is a small downwards arrow</td>
</tr>
<tr class="">
<td>_trickle._button.text</td>
<td>string</td>
<td><pre>"Continue"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button.ariaLabel</td>
<td>string</td>
<td><pre>"Continue"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._button.startText</td>
<td>string</td>
<td><pre>"Begin"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button.startAriaLabel</td>
<td>string</td>
<td><pre>"Begin"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button.finalText</td>
<td>string</td>
<td><pre>"Finish"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button.finalAriaLabel</td>
<td>string</td>
<td><pre>"Finish"</pre></td>
<td>Only on articles when 'Enable on child blocks' set to true</td>
</tr>
<tr class="">
<td>_trickle._button._component</td>
<td>string</td>
<td><pre>"trickle-button"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking._isCompletionRequired</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._stepLocking._isLockedOnRevisit</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isCompletionIndicatorEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._textAlignment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._title</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the block title. Left: Aligns the title to the left of the container. Center: Aligns the title to the center of the container. Right: Aligns the title to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._body</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the block body. Left: Aligns the body to the left of the container. Center: Aligns the body to the center of the container. Right: Aligns the body to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._instruction</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the block instruction. Left: Aligns the instruction to the left of the container. Center: Aligns the instruction to the center of the container. Right: Aligns the instruction to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._large</td>
<td>string</td>
<td></td>
<td>Large background image - used on desktop</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._medium</td>
<td>string</td>
<td></td>
<td>Medium background image - used on tablet</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._small</td>
<td>string</td>
<td></td>
<td>Small background image - used on mobile</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundRepeat</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Repeat-x: The background image is repeated only horizontally. Repeat-y: The background image is repeated only vertically</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundSize</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Auto: The background image is displayed in its original size. Cover: Resize the background image to cover the entire container, even if it has to stretch or crop the image. Contain: Resize the background image to make sure the image is fully visible. 100% 100%: Resize the background image to match the dimensions of the container</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundPosition</td>
<td>string</td>
<td><pre>""</pre></td>
<td>The first value is the horizontal position and the second value is the vertical</td>
</tr>
<tr class="">
<td>_vanilla._minimumHeights</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._minimumHeights._large</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the block height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_vanilla._minimumHeights._medium</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the block height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_vanilla._minimumHeights._small</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the block height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._large</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Large CSS class - used on desktop</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._medium</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Medium CSS class - used on tablet</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._small</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Small CSS class - used on mobile</td>
</tr>
<tr class="">
<td>_vanilla._isDividerBlock</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, applies a divider class to the block</td>
</tr>
<tr class="">
<td>_vanilla._paddingTop</td>
<td>string</td>
<td><pre>"standard"</pre></td>
<td>Changes the value of the blocks top spacing. Double: Doubles the blocks top spacing. Standard: Retains the standard blocks top spacing. Half: Halves the blocks top spacing. Remove: Removes the blocks top spacing. The default value is `standard`.</td>
</tr>
<tr class="">
<td>_vanilla._paddingBottom</td>
<td>string</td>
<td><pre>"standard"</pre></td>
<td>Changes the value of the blocks bottom spacing. Double: Doubles the blocks bottom spacing. Standard: Retains the standard blocks bottom spacing. Half: Halves the blocks bottom spacing. Remove: Removes the blocks bottom spacing. The default value is `standard`.</td>
</tr>
<tr class="">
<td>_vanilla._componentVerticalAlignment</td>
<td>string</td>
<td><pre>"top"</pre></td>
<td>Defines the vertical alignment of the child component(s) in relation to the block. Top: Aligns descendents to the top of the block. Center: Aligns descendents to the center of the block. Bottom: Aligns descendents to the bottom of the block. The default alignment is `top`.</td>
</tr>
</table>
      
      <h3 id="bookmarking-contentobject" class="dep">bookmarking-contentobject</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="bookmarking-course" class="dep">bookmarking-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="boxmenu-contentobject" class="dep">boxMenu-contentobject</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="boxmenu-course" class="dep">boxMenu-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="component" class="dep">component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
<td>_pageLevelProgress</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isCompletionIndicatorEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._textAlignment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._title</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the component title. Left: Aligns the title to the left of the container. Center: Aligns the title to the center of the container. Right: Aligns the title to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._body</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the component body. Left: Aligns the body to the left of the container. Center: Aligns the body to the center of the container. Right: Aligns the body to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._textAlignment._instruction</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the component instruction. Left: Aligns the instruction to the left of the container. Center: Aligns the instruction to the center of the container. Right: Aligns the instruction to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
</table>
      
      <h3 id="config" class="dep">config</h3>
      
      <div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
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
<td>_completionCriteria._shouldSubmitScore</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, the score attained in any assessment will be reported (regardless of whether the user passes or fails the assessment)</td>
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
<td><pre>520</pre></td>
<td>Pixel width for the small breakpoint, e.g. cellphones</td>
</tr>
<tr class="">
<td>screenSize.medium</td>
<td>number</td>
<td><pre>760</pre></td>
<td>Pixel width for the medium breakpoint, e.g. tablet devices</td>
</tr>
<tr class="">
<td>screenSize.large</td>
<td>number</td>
<td><pre>900</pre></td>
<td>Pixel width for the large breakpoint, e.g. laptop/desktop computers</td>
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
<tr class="required">
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
<tr class="">
<td>tags</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>Add tags by entering one or more words, separated with a comma (,)</td>
</tr>
<tr class="">
<td>_trickle</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_trickle._logState</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether the Trickle extension logs its state to the browser console.</td>
</tr>
<tr class="">
<td>_trickle._completionAttribute</td>
<td>string</td>
<td><pre>"_isComplete"</pre></td>
<td>Set which attribute is used to determine completion</td>
</tr>
<tr class="">
<td>_languagePicker</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_languagePicker._isEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether the Language Picker extension is enabled or disabled</td>
</tr>
<tr class="">
<td>_languagePicker.title</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Text to be shown in the browser's title bar when the language picker is displayed</td>
</tr>
<tr class="">
<td>_languagePicker.displayTitle</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Header text for the Language Picker</td>
</tr>
<tr class="">
<td>_languagePicker.body</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Introductory or explanatory text for the Language Picker</td>
</tr>
<tr class="">
<td>_languagePicker._showOnCourseLoad</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether the Language Picker should be displayed on course load or not</td>
</tr>
<tr class="">
<td>_languagePicker._languagePickerIconClass</td>
<td>string</td>
<td><pre>"icon-language-2"</pre></td>
<td>Your default options here are: icon-globe, icon-language-1, icon-language-2</td>
</tr>
<tr class="">
<td>_languagePicker._restoreStateOnLanguageChange</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Determines whether or not the language picker will try to restore the 'state' of the course when the user changes language. It is advised that you only enable this setting if all course languages have exactly the same structure; if they do not, some loss of tracking data will occur. If this setting is disabled, tracking data will be cleared when the user switches language - the 'Confirm Message' should be used to warn the user of this</td>
</tr>
<tr class="">
<td>_languagePicker._classes</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_languagePicker._languages</td>
<td>array</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>If enabled, the plugin will try to find and track to a SCORM conformant LMS. Uncheck to switch off SCORM tracking</td>
</tr>
<tr class="">
<td>_spoor._tracking</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor._tracking._shouldStoreResponses</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>If enabled, the user's responses to questions will be saved and restored in each session. Note: this setting should be enabled in the majority of cases</td>
</tr>
<tr class="">
<td>_spoor._tracking._shouldStoreAttempts</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, a history of the user's responses to questions will be saved and restored in each session. Note: this setting should be disabled in the majority of cases</td>
</tr>
<tr class="">
<td>_spoor._tracking._shouldRecordInteractions</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>If enabled, the course will record the user's responses to questions to the cmi.interactions SCORM data fields</td>
</tr>
<tr class="">
<td>_spoor._reporting</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor._reporting._onTrackingCriteriaMet</td>
<td>string</td>
<td><pre>"completed"</pre></td>
<td>What status to report back to the LMS when the tracking criteria are met</td>
</tr>
<tr class="">
<td>_spoor._reporting._onAssessmentFailure</td>
<td>string</td>
<td><pre>"incomplete"</pre></td>
<td>What status to report back to the LMS when the assessment is failed</td>
</tr>
<tr class="">
<td>_spoor._reporting._resetStatusOnLanguageChange</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, the the course status will be reset to 'incomplete' when the user changes the course language</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._scormVersion</td>
<td>string</td>
<td><pre>"1.2"</pre></td>
<td>The SCORM standard to use - SCORM 1.2 or SCORM 2004 4th Edition</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._showDebugWindow</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, a popup window will be shown on course launch that gives detailed information about what SCORM calls are being made. This can be very useful for debugging SCORM issues. Note that this popup window will appear automatically if the SCORM code encounters an error, even if this is set to false</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._commitOnStatusChange</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>If enabled, a 'commit' call will be made any time the lesson_status is changed</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._commitOnAnyChange</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, a 'commit' (save all data) call will be made any time a value is changed. Note that enabling this setting may have a detrimental impact on the server and should only be used if absolutely necessary and only after careful load testing. Consider trying a lower value for 'Frequency of automatic commits' before changing this setting</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._timedCommitFrequency</td>
<td>number</td>
<td><pre>10</pre></td>
<td>The frequency (in minutes) at which a 'commit' call should be made automatically. Set to 0 to disable automatic commits altogether</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._maxCommitRetries</td>
<td>number</td>
<td><pre>5</pre></td>
<td>If a 'commit' call fails, this setting controls how many times it should be retried before giving up and throwing an error</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._commitRetryDelay</td>
<td>number</td>
<td><pre>2000</pre></td>
<td>How much of a delay (in milliseconds) to leave between commit retries</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._suppressErrors</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, error messages will not be displayed when SCORM tracking problems occur</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._commitOnVisibilityChangeHidden</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>If enabled, a 'commit' call will be made whenever the course window is hidden/minimised. Requires a browser that supports the 'visibilitychange' event</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._manifestIdentifier</td>
<td>string</td>
<td><pre>"adapt_manifest"</pre></td>
<td>Sets the 'identifier' attribute in the imsmanifest.xml</td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._exitStateIfIncomplete</td>
<td>string</td>
<td><pre>"auto"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._exitStateIfComplete</td>
<td>string</td>
<td><pre>"auto"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor._advancedSettings._setCompletedWhenFailed</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>If enabled, `cmi.completion_status` will be set to "completed" if the assessment is "failed". Only valid for SCORM 2004, where the logic for completion and success is separate.</td>
</tr>
<tr class="">
<td>_spoor._showCookieLmsResetButton</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>If enabled, a reset button will be available to relaunch the course and optionally clear tracking data (scorm_test_harness.html only).</td>
</tr>
</table>
      
      <h3 id="content" class="dep">content</h3>
      
      <div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
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
<td>_ariaLevel</td>
<td>number</td>
<td><pre>0</pre></td>
<td>If you need to override the default element ARIA level (as defined in Configuration Settings), set this to any number greater than 0</td>
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
<tr class="required">
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
<tr class="">
<td>tags</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>Add tags by entering one or more words, separated with a comma (,)</td>
</tr>
</table>
      
      <h3 id="contentobject" class="dep">contentobject</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
<td>_bookmarking</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_bookmarking._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether Bookmarking is enabled or disabled for this page of the course</td>
</tr>
<tr class="">
<td>_bookmarking._level</td>
<td>string</td>
<td><pre>"inherit"</pre></td>
<td>Whether you want to inherit the 'Level' setting from Project settings or override it for this page of the course</td>
</tr>
<tr class="">
<td>_boxMenu</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._renderAsGroup</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Enable this option to render items into a group on the menu. Groups can display a title, body, and instruction text</td>
</tr>
<tr class="">
<td>_pageLevelProgress</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._showPageCompletion</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether the progress calculations for this page are based on all components and the overall page - or only the components that are set to be displayed in Page Level Progress</td>
</tr>
<tr class="">
<td>_pageLevelProgress._isCompletionIndicatorEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._excludeAssessments</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether the progress calculations will include assessments</td>
</tr>
<tr class="">
<td>_resources</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether the Resources extension is enabled or disabled</td>
</tr>
<tr class="">
<td>_resources._resourcesItems</td>
<td>array</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._large</td>
<td>string</td>
<td></td>
<td>Large background image - used on desktop</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._medium</td>
<td>string</td>
<td></td>
<td>Medium background image - used on tablet</td>
</tr>
<tr class="">
<td>_vanilla._backgroundImage._small</td>
<td>string</td>
<td></td>
<td>Small background image - used on mobile</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundRepeat</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Repeat-x: The background image is repeated only horizontally. Repeat-y: The background image is repeated only vertically</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundSize</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Auto: The background image is displayed in its original size. Cover: Resize the background image to cover the entire container, even if it has to stretch or crop the image. Contain: Resize the background image to make sure the image is fully visible. 100% 100%: Resize the background image to match the dimensions of the container</td>
</tr>
<tr class="">
<td>_vanilla._backgroundStyles._backgroundPosition</td>
<td>string</td>
<td><pre>""</pre></td>
<td>The first value is the horizontal position and the second value is the vertical</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._large</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Large CSS class - used on desktop</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._medium</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Medium CSS class - used on tablet</td>
</tr>
<tr class="">
<td>_vanilla._responsiveClasses._small</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Small CSS class - used on mobile</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._textAlignment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._textAlignment._title</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the page title. Left: Aligns the title to the left of the container. Center: Aligns the title to the center of the container. Right: Aligns the title to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._textAlignment._body</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the page body. Left: Aligns the body to the left of the container. Center: Aligns the body to the center of the container. Right: Aligns the body to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._textAlignment._instruction</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the page instruction. Left: Aligns the instruction to the left of the container. Center: Aligns the instruction to the center of the container. Right: Aligns the instruction to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundImage</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundImage._large</td>
<td>string</td>
<td></td>
<td>Large background image - used on desktop</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundImage._medium</td>
<td>string</td>
<td></td>
<td>Medium background image - used on tablet</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundImage._small</td>
<td>string</td>
<td></td>
<td>Small background image - used on mobile</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundStyles</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundStyles._backgroundRepeat</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Repeat-x: The background image is repeated only horizontally. Repeat-y: The background image is repeated only vertically</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundStyles._backgroundSize</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Auto: The background image is displayed in its original size. Cover: Resize the background image to cover the entire container, even if it has to stretch or crop the image. Contain: Resize the background image to make sure the image is fully visible. 100% 100%: Resize the background image to match the dimensions of the container</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._backgroundStyles._backgroundPosition</td>
<td>string</td>
<td><pre>""</pre></td>
<td>The first value is the horizontal position and the second value is the vertical</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._minimumHeights</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._minimumHeights._large</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the page header height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._minimumHeights._medium</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the page header height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_vanilla._pageHeader._minimumHeights._small</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the page header height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
</table>
      
      <h3 id="contentplugin" class="dep">contentplugin</h3>
      
      <div class="desc">An Adapt framework plugin</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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
<td>isAddedByDefault</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Whether the plugin should be added by default for new courses</td>
</tr>
</table>
      
      <h3 id="course" class="dep">course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
<td>_globals</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._text</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._text.ariaRegion</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._narrative</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._narrative.ariaRegion</td>
<td>string</td>
<td><pre>"Slide show. Select the next button to progress."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._narrative.previous</td>
<td>string</td>
<td><pre>"{{#if title}}Back to {{{title}}} (item {{itemNumber}} of {{totalItems}}){{else}}{{_globals._accessibility._ariaLabels.previous}}{{/if}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._narrative.next</td>
<td>string</td>
<td><pre>"{{#if title}}Forward to {{{title}}} (item {{itemNumber}} of {{totalItems}}){{else}}{{_globals._accessibility._ariaLabels.next}}{{/if}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._graphic</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._graphic.ariaRegion</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._hotgraphic</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._hotgraphic.ariaRegion</td>
<td>string</td>
<td><pre>"Image with selectable areas. Select each button to show more information."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._hotgraphic.item</td>
<td>string</td>
<td><pre>"Item {{{itemNumber}}} of {{{totalItems}}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._hotgraphic.previous</td>
<td>string</td>
<td><pre>"{{#if title}}Back to {{{title}}} (item {{itemNumber}} of {{totalItems}}){{else}}{{_globals._accessibility._ariaLabels.previous}}{{/if}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._hotgraphic.next</td>
<td>string</td>
<td><pre>"{{#if title}}Forward to {{{title}}} (item {{itemNumber}} of {{totalItems}}){{else}}{{_globals._accessibility._ariaLabels.next}}{{/if}}"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._hotgraphic.popupPagination</td>
<td>string</td>
<td><pre>"{{itemNumber}} / {{totalItems}}"</pre></td>
<td>This is the aria label for each item. Use {{itemNumber}} and {{totalItems}} in your text to tell the user which item they are viewing and how many items there are in total</td>
</tr>
<tr class="">
<td>_globals._assessmentResults</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._assessmentResults.ariaRegion</td>
<td>string</td>
<td><pre>"Assessment results."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accordion</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._accordion.ariaRegion</td>
<td>string</td>
<td><pre>"List of expandable sections. Select each button to expand the content."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._trickle</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._trickle.incompleteContent</td>
<td>string</td>
<td><pre>"There is incomplete content above. You must complete this before you can proceed through the course."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._gmcq</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._gmcq.ariaRegion</td>
<td>string</td>
<td><pre>"Multiple choice question"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._boxMenu</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._boxMenu.durationLabel</td>
<td>string</td>
<td><pre>"Duration:"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._mcq</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._mcq.ariaRegion</td>
<td>string</td>
<td><pre>"Multiple choice question"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._pageLevelProgress</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._pageLevelProgress.pageLevelProgress</td>
<td>string</td>
<td><pre>"Page sections"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._pageLevelProgress.pageLevelProgressIndicatorBar</td>
<td>string</td>
<td><pre>"Page progress. Use this to listen to the list of regions in this topic and whether they're completed. You can jump directly to any that are incomplete or which sound particularly interesting. {{percentageComplete}}%"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._pageLevelProgress.pageLevelProgressMenuBar</td>
<td>string</td>
<td><pre>"Page completion {{percentageComplete}}%"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._pageLevelProgress.pageLevelProgressEnd</td>
<td>string</td>
<td><pre>"You have reached the end of the list of page sections."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._pageLevelProgress.optionalContent</td>
<td>string</td>
<td><pre>"Optional content"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._pageLevelProgress._navOrder</td>
<td>number</td>
<td><pre>90</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._matching</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._matching.ariaRegion</td>
<td>string</td>
<td><pre>"Matching. Select from lists and then submit."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._languagePicker</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._languagePicker.navigationBarLabel</td>
<td>string</td>
<td><pre>"Select course language"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._languagePicker.languageSelector</td>
<td>string</td>
<td><pre>"Language selector"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._textinput</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._textinput.ariaRegion</td>
<td>string</td>
<td><pre>"Text input. Type your answer and then submit."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._slider</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._slider.ariaRegion</td>
<td>string</td>
<td><pre>"Slider. Respond to the question by selecting a value on the scale and then submit."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._slider.labelStart</td>
<td>string</td>
<td><pre>"Start of the scale"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._slider.labelEnd</td>
<td>string</td>
<td><pre>"End of the scale"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._resources</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._resources.resources</td>
<td>string</td>
<td><pre>"Additional resources."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.ariaRegion</td>
<td>string</td>
<td><pre>"Media player{{#any _transcript._inlineTranscript _transcript._externalTranscript}} and transcript{{/any}}."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.skipToTranscript</td>
<td>string</td>
<td><pre>"Skip to transcript"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.playText</td>
<td>string</td>
<td><pre>"Play"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.pauseText</td>
<td>string</td>
<td><pre>"Pause"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.stopText</td>
<td>string</td>
<td><pre>"Stop"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.audioPlayerText</td>
<td>string</td>
<td><pre>"Audio Player"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.videoPlayerText</td>
<td>string</td>
<td><pre>"Video Player"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.tracksText</td>
<td>string</td>
<td><pre>"Captions/Subtitles"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.timeSliderText</td>
<td>string</td>
<td><pre>"Time Slider"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.muteText</td>
<td>string</td>
<td><pre>"Mute Toggle"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.unmuteStatusText</td>
<td>string</td>
<td><pre>"Unmute"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.muteStatusText</td>
<td>string</td>
<td><pre>"Mute"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.volumeSliderText</td>
<td>string</td>
<td><pre>"Volume Slider"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.fullscreenText</td>
<td>string</td>
<td><pre>"Fullscreen"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.goFullscreenText</td>
<td>string</td>
<td><pre>"Go Fullscreen"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.turnOffFullscreenText</td>
<td>string</td>
<td><pre>"Turn off Fullscreen"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.noneText</td>
<td>string</td>
<td><pre>"None"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.skipBackText</td>
<td>string</td>
<td><pre>"Skip back %1 seconds"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.allyVolumeControlText</td>
<td>string</td>
<td><pre>"Use Up/Down Arrow keys to increase or decrease volume."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_globals._media.progessHelpText</td>
<td>string</td>
<td><pre>"Use Left/Right Arrow keys to advance one second, Up/Down arrows to advance ten seconds."</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_bookmarking</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_bookmarking._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether the Bookmarking extension is enabled or disabled</td>
</tr>
<tr class="">
<td>_bookmarking._level</td>
<td>string</td>
<td><pre>"component"</pre></td>
<td>Allows you to set whether Bookmarking is done at page, block or component level</td>
</tr>
<tr class="">
<td>_bookmarking._showPrompt</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether the Bookmarking prompt is enabled or disabled. If not enabled, the user will be returned to their bookmarked position automatically</td>
</tr>
<tr class="">
<td>_bookmarking.title</td>
<td>string</td>
<td><pre>"Bookmarking"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_bookmarking.body</td>
<td>string</td>
<td><pre>"Would you like to continue where you left off?"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_bookmarking._buttons</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_bookmarking._buttons.yes</td>
<td>string</td>
<td><pre>"Yes"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_bookmarking._buttons.no</td>
<td>string</td>
<td><pre>"No"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_assessment._isPercentageBased</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Determines whether the pass mark values should be treated as percentages (default) or as the raw score and correctness</td>
</tr>
<tr class="">
<td>_assessment._scoreToPass</td>
<td>number</td>
<td><pre>60</pre></td>
<td>The minimum score required by the learner to pass the assessment or the minimum percentage score if percentage-based</td>
</tr>
<tr class="">
<td>_assessment._correctToPass</td>
<td>number</td>
<td><pre>60</pre></td>
<td>The minimum number of correct questions required by the learner to pass the assessment or the minimum percentage correct if percentage-based</td>
</tr>
<tr class="">
<td>_boxMenu</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._backgroundImage</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._backgroundImage._large</td>
<td>string</td>
<td></td>
<td>Large background image - used on desktop</td>
</tr>
<tr class="">
<td>_boxMenu._backgroundImage._medium</td>
<td>string</td>
<td></td>
<td>Medium background image - used on tablet</td>
</tr>
<tr class="">
<td>_boxMenu._backgroundImage._small</td>
<td>string</td>
<td></td>
<td>Small background image - used on mobile</td>
</tr>
<tr class="">
<td>_boxMenu._backgroundStyles</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._backgroundStyles._backgroundRepeat</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Repeat-x: The background image is repeated only horizontally. Repeat-y: The background image is repeated only vertically</td>
</tr>
<tr class="">
<td>_boxMenu._backgroundStyles._backgroundSize</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Auto: The background image is displayed in its original size. Cover: Resize the background image to cover the entire container, even if it has to stretch or crop the image. Contain: Resize the background image to make sure the image is fully visible</td>
</tr>
<tr class="">
<td>_boxMenu._backgroundStyles._backgroundPosition</td>
<td>string</td>
<td><pre>""</pre></td>
<td>The first value is the horizontal position and the second value is the vertical</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._textAlignment</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._textAlignment._title</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the menu title. Left: Aligns the title to the left of the container. Center: Aligns the title to the center of the container. Right: Aligns the title to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._textAlignment._body</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the menu body. Left: Aligns the body to the left of the container. Center: Aligns the body to the center of the container. Right: Aligns the body to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._textAlignment._instruction</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Set the alignment of the menu instruction. Left: Aligns the instruction to the left of the container. Center: Aligns the instruction to the center of the container. Right: Aligns the instruction to the right of the container. The alignment automatically inverses for right-to-left languages. The default is `` which inherits the natural page direction.</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundImage</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundImage._large</td>
<td>string</td>
<td></td>
<td>Large background image - used on desktop</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundImage._medium</td>
<td>string</td>
<td></td>
<td>Medium background image - used on tablet</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundImage._small</td>
<td>string</td>
<td></td>
<td>Small background image - used on mobile</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundStyles</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundStyles._backgroundRepeat</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Repeat-x: The background image is repeated only horizontally. Repeat-y: The background image is repeated only vertically</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundStyles._backgroundSize</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Auto: The background image is displayed in its original size. Cover: Resize the background image to cover the entire container, even if it has to stretch or crop the image. Contain: Resize the background image to make sure the image is fully visible</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._backgroundStyles._backgroundPosition</td>
<td>string</td>
<td><pre>""</pre></td>
<td>The first value is the horizontal position and the second value is the vertical</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._minimumHeights</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._minimumHeights._large</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the menu header height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._minimumHeights._medium</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the menu header height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_boxMenu._menuHeader._minimumHeights._small</td>
<td>number</td>
<td><pre>0</pre></td>
<td>Minimum height should only be used in instances where the menu header height needs to be greater than the content e.g. to prevent a background image being cropped</td>
</tr>
<tr class="">
<td>_pageLevelProgress</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._showPageCompletion</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether the progress calculations are based on all components - or only those that are set to be displayed in Page Level Progress</td>
</tr>
<tr class="">
<td>_pageLevelProgress._isCompletionIndicatorEnabled</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._isShownInNavigationBar</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_pageLevelProgress._showAtCourseLevel</td>
<td>boolean</td>
<td><pre>false</pre></td>
<td>Controls whether to display all content objects and the current page components together, or just the current page components</td>
</tr>
<tr class="">
<td>_resources</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._isEnabled</td>
<td>boolean</td>
<td><pre>true</pre></td>
<td>Controls whether the Resources extension is enabled or disabled</td>
</tr>
<tr class="">
<td>_resources._drawerOrder</td>
<td>number</td>
<td><pre>0</pre></td>
<td>The order in which this extension should appear as a drawer item</td>
</tr>
<tr class="">
<td>_resources.title</td>
<td>string</td>
<td><pre>"Resources"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources.description</td>
<td>string</td>
<td><pre>"Select here to view resources for this course"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterButtons</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterButtons.all</td>
<td>string</td>
<td><pre>"All"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterButtons.document</td>
<td>string</td>
<td><pre>"Documents"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterButtons.media</td>
<td>string</td>
<td><pre>"Media"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterButtons.link</td>
<td>string</td>
<td><pre>"Links"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterAria</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterAria.allAria</td>
<td>string</td>
<td><pre>"View all resources"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterAria.documentAria</td>
<td>string</td>
<td><pre>"View document resources"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterAria.mediaAria</td>
<td>string</td>
<td><pre>"View media resources"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._filterAria.linkAria</td>
<td>string</td>
<td><pre>"View resource links"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_resources._resourcesItems</td>
<td>array</td>
<td></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_spoor._messages</td>
<td>object</td>
<td><pre>{}</pre></td>
<td>Optional object that can be used to amend/translate the error messages shown by the spoor extension</td>
</tr>
</table>
      
      <h3 id="courseasset" class="dep">courseasset</h3>
      
      <div class="desc">Metadata related to where an asset is used in a course</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="gmcq-component" class="dep">gmcq-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="gmcq-course" class="dep">gmcq-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="graphic-component" class="dep">graphic-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="graphic-course" class="dep">graphic-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="hotgraphic-component" class="dep">hotgraphic-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="hotgraphic-course" class="dep">hotgraphic-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="languagepicker-config" class="dep">languagePicker-config</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="languagepicker-course" class="dep">languagePicker-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="localauthuser" class="dep">localauthuser</h3>
      
      <div class="desc">Extra user properties related to local auth</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="log" class="dep">log</h3>
      
      <div class="desc">A system log message</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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
      
      <h3 id="matching-component" class="dep">matching-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="matching-course" class="dep">matching-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="mcq-component" class="dep">mcq-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="mcq-course" class="dep">mcq-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="media-component" class="dep">media-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="media-course" class="dep">media-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="narrative-component" class="dep">narrative-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="narrative-course" class="dep">narrative-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="pagelevelprogress-article" class="dep">pageLevelProgress-article</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="pagelevelprogress-block" class="dep">pageLevelProgress-block</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="pagelevelprogress-component" class="dep">pageLevelProgress-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="pagelevelprogress-contentobject" class="dep">pageLevelProgress-contentobject</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="pagelevelprogress-course" class="dep">pageLevelProgress-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="resources-contentobject" class="dep">resources-contentobject</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="resources-course" class="dep">resources-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="role" class="dep">role</h3>
      
      <div class="desc">A user role</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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
      
      <h3 id="slider-component" class="dep">slider-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="slider-course" class="dep">slider-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="spoor-config" class="dep">spoor-config</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="spoor-course" class="dep">spoor-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="spoorcontent" class="dep">spoorcontent</h3>
      
      <div class="desc">Extra properties related to spoor</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="spoorcourse" class="dep">spoorcourse</h3>
      
      <div class="desc">Extra properties related to spoor</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="tag" class="dep">tag</h3>
      
      <div class="desc">Tag metadata applied to other objects</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
<td>title</td>
<td>string</td>
<td></td>
<td>The tag title</td>
</tr>
</table>
      
      <h3 id="tags" class="dep">tags</h3>
      
      <div class="desc">Extra properties to define tags</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="text-component" class="dep">text-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="text-course" class="dep">text-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="textinput-component" class="dep">textinput-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="textinput-course" class="dep">textinput-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="trickle-article" class="dep">trickle-article</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="trickle-block" class="dep">trickle-block</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="trickle-config" class="dep">trickle-config</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="trickle-course" class="dep">trickle-course</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="user" class="dep">user</h3>
      
      <div class="desc">A system user</div>

<div class="required">Fields in bold are required.</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="required">
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
<tr class="">
<td>roles</td>
<td>array</td>
<td><pre>[]</pre></td>
<td>Roles assigned to this user</td>
</tr>
<tr class="required">
<td>authType</td>
<td>string</td>
<td></td>
<td>Types of authentication used with this user</td>
</tr>
</table>
      
      <h3 id="userroles" class="dep">userroles</h3>
      
      <div class="desc">Extra user properties for specifying roles</div>

<table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="vanilla-article" class="dep">vanilla-article</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="vanilla-block" class="dep">vanilla-block</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="vanilla-component" class="dep">vanilla-component</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="vanilla-contentobject" class="dep">vanilla-contentobject</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
</table>
      
      <h3 id="vanilla-theme" class="dep">vanilla-theme</h3>
      
      <table class="schema"><tr><th>Attribute</th><th>Type</th><th>Default</th><th>Description</th></tr><tr class="">
<td>_id</td>
<td>string</td>
<td></td>
<td>Unique identifier</td>
</tr>
<tr class="">
<td>_global</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_global.font-color</td>
<td>string</td>
<td><pre>"#4D4D4D"</pre></td>
<td>Global body font colour</td>
</tr>
<tr class="">
<td>_global.font-color-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Global body font colour inverted. Either a lightened/darkened alternative to Font colour</td>
</tr>
<tr class="">
<td>_global.link</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_global.link-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Global link font colour inverted. Either a lightened/darkened alternative to Link colour</td>
</tr>
<tr class="">
<td>_global.link-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_global.link-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Global link font colour when hovered over inverted. Either a lightened/darkened alternative to Link hover colour</td>
</tr>
<tr class="">
<td>_global.heading-color</td>
<td>string</td>
<td><pre>"#36CDE8"</pre></td>
<td>Global title colour</td>
</tr>
<tr class="">
<td>_global.heading-color-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Global title colour inverted. Either a lightened/darkened alternative to Title colour</td>
</tr>
<tr class="">
<td>_items</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_items.item-color</td>
<td>string</td>
<td><pre>"#36CDE8"</pre></td>
<td>Defines the clickable areas or points of interest in components</td>
</tr>
<tr class="">
<td>_items.item-color-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the item text/icon colour. Should be a colour that provides good contrast against the item colour</td>
</tr>
<tr class="">
<td>_items.item-color-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_items.item-color-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the item text/icon colour when hovered over. Should be a colour that provides good contrast against the item hover colour</td>
</tr>
<tr class="">
<td>_items.item-color-selected</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_items.item-color-inverted-selected</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the item text/icon colour when selected. Should be a colour that provides good contrast against the Item selected colour</td>
</tr>
<tr class="">
<td>_items.visited</td>
<td>string</td>
<td><pre>"#727272"</pre></td>
<td>Defines the item colour when it has been visited</td>
</tr>
<tr class="">
<td>_items.visited-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the item text/icon colour when visited. Should be a colour that provides good contrast against the item visited colour</td>
</tr>
<tr class="">
<td>_buttons</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons.btn-color</td>
<td>string</td>
<td><pre>"#4D4D4D"</pre></td>
<td>Defines component question buttons and navigational elements</td>
</tr>
<tr class="">
<td>_buttons.btn-color-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the button text/icon colour. Should be a colour that provides good contrast against the button colour</td>
</tr>
<tr class="">
<td>_buttons.btn-color-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons.btn-color-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the button text/icon colour when hovered over. Should be a colour that provides good contrast against the button hover colour</td>
</tr>
<tr class="">
<td>_buttons.btn-icon-color</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the standardised icon button background colour</td>
</tr>
<tr class="">
<td>_buttons.btn-icon-color-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the button icon colour. Should be a colour that provides good contrast against the button colour</td>
</tr>
<tr class="">
<td>_buttons.btn-icon-color-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons.btn-icon-color-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the button icon colour when hovered over. Should be a colour that provides good contrast against the button hover colour</td>
</tr>
<tr class="">
<td>_buttons.disabled</td>
<td>string</td>
<td><pre>"#DDDDDD"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_buttons.disabled-inverted</td>
<td>string</td>
<td><pre>"#000000"</pre></td>
<td>Defines the button text/icon colour when it is disabled. Should be a colour that provides good contrast against the button disabled colour</td>
</tr>
<tr class="">
<td>_validation</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_validation.validation-success</td>
<td>string</td>
<td><pre>"#065f28"</pre></td>
<td>Defines the question marking success colour</td>
</tr>
<tr class="">
<td>_validation.validation-success-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the question marking success text/icon colour. Should be a colour that provides good contrast against the question marking success colour</td>
</tr>
<tr class="">
<td>_validation.validation-error</td>
<td>string</td>
<td><pre>"#ff0000"</pre></td>
<td>Defines the question marking error colour</td>
</tr>
<tr class="">
<td>_validation.validation-error-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the question marking error text/icon colour. Should be a colour that provices good contrast against the question marking error colour</td>
</tr>
<tr class="">
<td>_progress</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_progress.progress</td>
<td>string</td>
<td><pre>"#9096A0"</pre></td>
<td>Defines the global progress width fill colour</td>
</tr>
<tr class="">
<td>_progress.progress-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the global progress fill background colour</td>
</tr>
<tr class="">
<td>_progress.progress-border</td>
<td>string</td>
<td><pre>"#9096A0"</pre></td>
<td>Defines the global border colour that appears around the progress fill bar</td>
</tr>
<tr class="">
<td>_menu</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_menu.menu-item</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_menu.menu-item-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the menu item text colour. Should be a colour that provides good contrast against the menu item colour</td>
</tr>
<tr class="">
<td>_menu.menu-item-border-color</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_menu.menu-item-progress</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the menu-item-specific progress width fill override colour</td>
</tr>
<tr class="">
<td>_menu.menu-item-progress-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the menu-item-specific progress fill background override colour</td>
</tr>
<tr class="">
<td>_menu.menu-item-progress-border</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_menu.menu-item-btn-color</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_menu.menu-item-btn-color-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the menu item button text colour. Should be a colour that provides good contrast against the menu item button colour</td>
</tr>
<tr class="">
<td>_menu.menu-item-btn-color-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_menu.menu-item-btn-color-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the menu item button text colour when hovered over. Should be a colour that provides good contrast against the menu item button hover colour</td>
</tr>
<tr class="">
<td>_nav</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_nav.nav</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_nav.nav-inverted</td>
<td>string</td>
<td><pre>"#9096A0"</pre></td>
<td>Defines the general navigation inverted colour. Should be a colour that provides good contrast against the navigation colour</td>
</tr>
<tr class="">
<td>_nav.nav-icon</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_nav.nav-icon-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the navigation button text/icon colour. Should be a colour that provides good contrast against the navigation button colour</td>
</tr>
<tr class="">
<td>_nav.nav-icon-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_nav.nav-icon-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the navigation button text/icon colour when hovered over. Should be a colour that provides good contrast against the navigation button hover colour</td>
</tr>
<tr class="">
<td>_nav.nav-progress</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the navigation-specific progress width fill override colour</td>
</tr>
<tr class="">
<td>_nav.nav-progress-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the navigation-specific progress fill background override colour</td>
</tr>
<tr class="">
<td>_nav.nav-progress-border</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_nav.nav-progress-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the navigation-specific progress width fill override colour when hovered over</td>
</tr>
<tr class="">
<td>_nav.nav-progress-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the navigation-specific progress fill background override colour when hovered over</td>
</tr>
<tr class="">
<td>_nav.nav-progress-border-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify</td>
<td>string</td>
<td><pre>"#36CDE8"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the notify text colour. Should be a colour that provides good contrast against the notify colour</td>
</tr>
<tr class="">
<td>_notify.notify-link</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify-link-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify-btn</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify-btn-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the notify button text/icon colour. Should be a colour that provides good contrast against the notify button colour</td>
</tr>
<tr class="">
<td>_notify.notify-btn-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify-btn-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the notify button text/icon colour when hovered over. Should be a colour that provides good contrast against the notify button hover colour</td>
</tr>
<tr class="">
<td>_notify.notify-icon</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify-icon-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the notify icon inverse colour. Should be a colour that provides good contrast against the notify icon colour</td>
</tr>
<tr class="">
<td>_notify.notify-icon-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_notify.notify-icon-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the notify icon colour when hovered over. Should be a colour that provides good contrast against the notify icon colour</td>
</tr>
<tr class="">
<td>_drawer</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer</td>
<td>string</td>
<td><pre>"#263944"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the drawer text colour. Should be a colour that provides good contrast against the drawer colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-link</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-link-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-icon</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-icon-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer icon button inverse colour. Should be a colour that provides good contrast against the drawer icon button colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-icon-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-icon-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer icon button inverse colour when hovered over. Should be a colour that provides good contrast against the drawer icon button hover colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-item</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-item-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer item text/icon colour. Should be a colour that provides good contrast against the drawer item colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-item-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-item-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer item text/icon colour when hovered over. Should be a colour that provides good contrast against the drawer item hover colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-item-selected</td>
<td>string</td>
<td><pre>""</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_drawer.drawer-item-inverted-selected</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer item text/icon colour when selected. Should be a colour that provides good contrast against the drawer item selected colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-progress</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer-specific progress width fill override colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-progress-inverted</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer-specific progress fill background override colour</td>
</tr>
<tr class="">
<td>_drawer.drawer-progress-border</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer-specific border override colour that appears around the progress fill bar</td>
</tr>
<tr class="">
<td>_drawer.drawer-progress-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer-specific progress width fill override colour when hovered over</td>
</tr>
<tr class="">
<td>_drawer.drawer-progress-inverted-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer-specific progress fill background override colour when hovered over</td>
</tr>
<tr class="">
<td>_drawer.drawer-progress-border-hover</td>
<td>string</td>
<td><pre>""</pre></td>
<td>Defines the drawer-specific border override colour that appears around the progress fill bar when hovered over</td>
</tr>
<tr class="">
<td>_misc</td>
<td>object</td>
<td><pre>{}</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_misc.background</td>
<td>string</td>
<td><pre>"#000000"</pre></td>
<td>Sets the generic background colour</td>
</tr>
<tr class="">
<td>_misc.background-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the background text/icon colour. Should be a colour that provides good contrast against the background colour</td>
</tr>
<tr class="">
<td>_misc.shadow</td>
<td>string</td>
<td><pre>"#000000"</pre></td>
<td> </td>
</tr>
<tr class="">
<td>_misc.shadow-inverted</td>
<td>string</td>
<td><pre>"#FFFFFF"</pre></td>
<td>Defines the shadow text/icon colour. Should be a colour that provides good contrast against the shadow colour</td>
</tr>
</table>
      
      