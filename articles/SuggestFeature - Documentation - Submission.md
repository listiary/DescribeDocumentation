Article type: 						`Feature Suggestion`<br>
Article name:						`SuggestFeature - Documentation - Submission`<br>
Affected Software/module:			`Listiary Documentation Site`<br>
Author:								`Framez` 
<br>

## Description:
We need a data pipeline for these write-up articles, bug reports, etc.
<br><br>
It should be integrated in the Jekyll documentation site in the form of a sending form,
must be easy to use, not requiring login, be automated and resilient, even if domains fail.
Those write-ups must end up somewhere, where they can get reviewed and published
in a specific section on our documentation site, later, where they can even be vote on - 
if we choose to implement that feature, in time.
<br><br>
Few possibilities I have considered - adding the functionality to the site and using
the SQL database - which has a lot of problems in itself.
I also thought about those being sent as emails to editors in a mailing list, so that editors 
can upload them to the github repo for documentation. Which comes with issues of its own - spam blocking,
double uploading, etc.
<br><br>
Conversing with N (I call N - AI chatbots), I have come to believe that the best implementation
would be to create a dedicated repository in the Listiary organization - called something like
"ListiarySubmissions" and implement Google forms to that repo pipeline with a bit of JS on Google's part.
<br><br>
And, of course, we will have multiple forms for each write-up type, that end up in different folders
in that repository on Github.