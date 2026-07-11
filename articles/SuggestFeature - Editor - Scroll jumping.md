Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Editor - Scroll jumping`<br>
Affected Software/module:			`Listiary Editor Module`<br>
Author:								`Framez`<br>
<br>

## Description:
When editing large Describe files, particularly when we browse them, and hit edit, 
the editor opens at the top of the file. And then, the user needs to scroll to the bottom,
if the working area is at the bottom - and if not, because there are other local lists in the file - 
then it is even more daunting - the user needs to scroll to find the place he wants to edit.
<br>
While it is not ideal to let lists grow large untrimmed - without enlisting them to separate files,
this can and does happen in Listiary, so we might as well device a mechanism to handle it gracefully.
To that, I propose few ideas.
<br><br>

### 1. Jump to the end
On long lists, the editor might just jump to the end.
Not ideal - some lists grow bottom up.

### 2. Memory of the last edit action
The editor might 'remember' which line the user last edited,
by using cookies.

### 3. Biggest gap, gap jumping
The editor might simply scroll to the biggest gap in the source file,
if, for example, gaps of 3 or more empty lines exist. And, if few are available,
there might be a control the user can use to jump (auto-scroll) to the next one.

### 4. Edit comment - comment jumping
We might use some specific comment - like `//jumptag` to jump to.
And, if few are available, there might be a control the user can use to jump (auto-scroll) to the next one.

Probably a combination of 3 and 4 will be a good solution.