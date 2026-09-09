---
layout: page
title: Describe Markup Language
permalink: /listiary/outreach/dreadme/
exclude: true
---
<img src="{{ site.baseurl }}/assets/images/describe.png" alt="logo" style="height:100px;">

*Maintaining large data lists, made easy*<br>
*Release: v1.0.1-beta*<br>
*License: AGPL v3*<br>

Describe is a markup language designed to write and maintain complex data lists that are compiled on demand to various formats, such as html, xml, sql and json. It is simple to use, intuitive and easy to master. Describe is readily extendable - implementing support for new target languages or customizing the transpilation process is straightforward, making it adaptable to a wide range of projects.<br>

- [Describe Language - A quick overview](https://documentation.listiary.com/language/how-to-write/)
- [Describe Language - 1001 source files directory](https://library.listiary.com/)
- [Describe Language - Official documentation](https://documentation.listiary.com/)

Built on a state of the art parsing platform such as ANTLR 4.13, Describe offers a robust grammar, although the compiler is currently in beta and some bugs are to be expected. It is available for free under the AGPL v3 license, but commercial licenses are negotiable as well.<br>

While ANTLR ensures strong grammar handling, the compiler is still under active development, and occasional bugs may occur. We appreciate your patience and value your contributions, as we continue to improve the tool.<br>


<br>
### How to
In order to run the `DescribeCompilerCLI.exe` you need a Windows PC with DotNet framework version 8.0 or higher. In order to reference the `DescribeCompilerAPI.dll` in your DotNet projects, you need to target DotNet framework version 8.0 or higher. In order to use the Amazon Lambda project, on the other hand, you need to upload it to AWS. Also, be sure to check out our [wiki](https://github.com/viktorchernev/DescribeCompiler/wiki) for the complete documentation.

#### 0. Set up highlighting
To enable Describe code highlighting, you can download the XML files for Notepad++ from the [Highlighting](https://github.com/viktorchernev/DescribeCompiler/tree/master/!highlighting) folder, or follow the instructions there to set up another text editor of your choice. This method uses user-defined languages for highlighting, which is a bit limited and makeshift, but it works reasonably well. A more refined solution using editor plugins is preferable, but isn’t available yet.

#### 1. Write Describe code
Write a title of each list, followed by an arrow `->` and the elements, one on a line, separated by comma `,` and end with a semicolon `;`. Add `[links]` in square brackets, and `<tag>` items in order to piece lists together. Add additional data as `{decorators}` in curly brackets or as tilde inversions - `~`. For more info visit the [documentation](https://documentation.listiary.com/)/[github](https://github.com/viktorchernev/DescribeCompiler/wiki/Grammar-How-To) or explore Describe source codes and test cases in this [huge collection](https://library.listiary.com/)/[github](https://github.com/viktorchernev/DataLists/tree/master/Lists).

<img src="{{ site.baseurl }}/assets/images/describe-example1.png" alt="Example 1" style="border:3px solid black; height:300px; margin-bottom: 5px;"><br>


#### 2a. [Compile (using CLI)](https://github.com/viktorchernev/DescribeCompiler/wiki/CliCompiler-how-to)
Run the CLI compiler by specifying the command as the first argument, the target folder (or file) as second argument and output file (or folder) as third argument. Add [options](https://github.com/viktorchernev/DescribeCompiler/wiki/CliCompiler-how-to) after that, if needed.

<img src="{{ site.baseurl }}/assets/images/describe-example2.png" alt="Example 2" style="border:3px solid black; height:300px; margin-bottom: 5px;"><br>


#### 2b. [Compile (using API)](https://github.com/viktorchernev/DescribeCompiler/wiki/ApiCompiler-how-to)
#### 2c. [Compile (using AWS)](https://github.com/viktorchernev/DescribeCompiler/wiki/AwsCompiler-how-to)

#### 3. Result
The final output will depend on the translator used - and you can easily write your own translator, or use the ones that are prebuilt for you. Here we are using a set of particular HTML templates to build a bare-bone website. The JSON translator is one of the particularly useful ones. With that translator you produce JSON that can be consumed from web applications.<br>

<img src="{{ site.baseurl }}/assets/images/describe-example3.png" alt="Example 3" style="border:3px solid black; height:300px; margin-bottom: 5px;"><br>


<br>
### Get in touch

Start a discussion in the GitHub discussions<br>
Send an email [contact@listiary.org](mailto:contact@listiary.org)<br>
Or, contact me - the founder, directly at [vchernev91@abv.bg](mailto:vchernev91@abv.bg) (might take a few days)<br>
You can reach me on Viber as well: +359-885-18-05-86<br>


<br>
## Sponsor
<!-- Listiary and Describe are designed to give everyone open, modular, and accessible tools for knowledge management. We’re currently setting up an Open Collective page where you’ll be able to contribute in the near future. Your support helps keep the project free, sustainable, and continuously evolving. -->
You can now support Listiary directly through <a href="https://opencollective.com/listiary" target="_blank">Open Collective</a> - a transparent platform for community funding. Your donation helps keep the project free, sustainable, and continuously evolving.


<br>
## Releases
We are excited to present the Describe Markup Language Transpiler v1.0.<br>

* [1.0.1-beta](https://github.com/viktorchernev/DescribeCompiler/releases/tag/1.0.1-beta) (CLI argument - auto)<br>
* [1.0.0-beta](https://github.com/viktorchernev/DescribeCompiler/releases/tag/1.0-beta) (ANTLR4, Describe v1.1)<br>
* [0.9.3](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9.3) (Support for Describe Language v1.0 - Official)<br>
* [0.9.2](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9.2) (Added features and bugfixes)<br>
* [0.9.1](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9.1) (Refactoring, added features and bugfixes)<br>
* [0.9.0](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9) (Initial release - Open beta)<br>

<br>
## Notes
* We currently have inbuilt translators for HTML, XML, JSON and SQL (although the SQL one is just for uploading whole parsed files to a database). If you need to target other languages, or need specific functionality, you'd have to write your own translator class - it is very easy. I will give updates here when more translators are available.<br>


<br>
### Links
[Back](/listiary/outreach/)<br>
