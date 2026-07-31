# *Describe Markup Language*  
![242452146-26dc5f4b-a676-41b8-837a-ac2fad29e556aa3](https://github.com/viktorchernev/DescribeCompiler/assets/72315339/b043a521-cdfc-494b-9267-f7a5d5d2dd06)

_Maintaining large data lists, made easy_  
  
  
![GitHub release (latest by date)](https://img.shields.io/github/v/release/viktorchernev/DescribeCompiler?color=green&logo=github)
[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)

Describe is a markup language designed to write and maintain complex data lists that are compiled on demand to various formats, such as html, xml, sql and json. It is simple to use, intuitive and easy to master. Describe is readily extendible - implementing support for new target languages or customizing the transpilation process is straightforward, making it adaptable to a wide range of projects.

Built on the reliable ANTLR 4.13, Describe offers a robust grammar. The Describe Compiler is currently in beta. It is available for free under the AGPL v3 license, but commercial licenses are negotiable as well.

While ANTLR ensures strong grammar handling, please note that the compiler is still under active development, and occasional bugs may occur. We appreciate your patience as we continue to improve the tool.


## How to
The Describe Compiler is a project written in C#, in Visual Studio 2022. It targets DotNet 8.0, which is the cross-platform open source version of DotNet. It can be built for various platforms, like Linux. 

There are several ways to use the compiler, but we will focus on the three most common: referencing it as a DLL, running it from the Windows command line, and deploying it as an Amazon Lambda function (AWS).







There is a command line version - a front for the compiler, and an Amazon Lambda project for hosting as a microservice on Amazon cloud.

You can download the source code and use it in visual studio, and possibly compile it for other OS like Linux, or use it like that. You can also reference the dll in your projects. You can also run the command line executable on a windows machine, or host the lambda project and use it as a microservice in your websites.

The release includes the dll library and the CLI front end, that can be used on any Windows machine. I will show you how to use the dll API version, the CLI interface, and the Amazon AWS, as most common use cases. Other use cases you will need to figure out for yourself, but it should be straight forward.

So, In order to run the `DescribeCompiler.CLI.exe` you need a Windows PC with DotNet framework version 8.0 or higher. In order to reference the `DescribeCompiler.dll` in your DotNet projects, you need to target DotNet framework version 8.0 or higher. There are no other dependencies. 

Also, be sure to check out our [wiki](https://github.com/viktorchernev/DescribeCompiler/wiki) for the complete documentation.  
  
  
### 0. Set up highlighting
In order to highlight Describe code, you can download the xml files for Notepad++ from the folder [Highlighting](https://github.com/viktorchernev/DescribeCompiler/tree/master/%23DescribeLanguage/Highlighting), or use the instructions provided in said folder to set up your preferred text editor.
  
### 1. Write Describe code  
Write a title of each list, followed by an arrow `->` and the elements, one on a line, separated by comma `,` and end with a semicolon `;`. Add `[links]` in square brackets, and `<tag>` items in order to piece lists together. Add additional data as `{decorators}` in curly brackets or as tilde inversions - `~`. For more info visit the [documentation](https://documentation.listiary.com/)/[github](https://github.com/viktorchernev/DescribeCompiler/wiki/Grammar-How-To) or explore Describe source codes and test cases in this [huge collection](https://library.listiary.com/)/[github](https://github.com/viktorchernev/DataLists/tree/master/Lists). 
  
![pic1a](https://github.com/viktorchernev/DescribeCompiler/assets/72315339/d5a71183-33ff-4e21-b6a1-db3ed7ac5967)


### 2a. [Compile (using CLI)](https://github.com/viktorchernev/DescribeCompiler/wiki/CliCompiler-how-to)  
Run the CLI compiler by specifying the target folder (or file) as first argument and output file (or folder) as second argument.  Add [options](https://github.com/viktorchernev/DescribeCompiler/wiki/CliCompiler-how-to) after that, if needed.  

![pic2a](https://github.com/viktorchernev/DescribeCompiler/assets/72315339/d8f6ac78-2cbc-4056-b560-16273474fa4d)

### 2b. [Compile (using API)](https://github.com/viktorchernev/DescribeCompiler/wiki/ApiCompiler-how-to)
### 2c. [Compile (using AWS)](https://github.com/viktorchernev/DescribeCompiler/wiki/AwsCompiler-how-to)


### 3. Result  
The final output will depend on the translator used - and you can easily write your own translator, or use the ones that are prebuilt for you. Here we are using a set of particular HTML templates to build a bare-bone website. The JSON translator is one of the particularly usefull ones. With that tanslator you produce JSON that can be consumed from web applications.
  
![pic3a](https://github.com/viktorchernev/DescribeCompiler/assets/72315339/36ae6997-82df-467e-b490-b7b9d63a860c)

## Get in touch  
- Use GitHub's issue reporter on the right
- Send me an email vchernev91@abv.bg (might take a few days)
- You can reach me on Viber as well: +359-885-18-05-86

## Releases
We are working on testing the Transpiler v1.0, as it is in alpha - pre release phase. It is finished but contains bugs here and there, and once those have been removed, it will be released.

* 1.0 (Coming up soon)
* [0.9.3](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9.3) (Support for Describe Language v1.0 - Official)  
* [0.9.2](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9.2) (Added features and bugfixes)
* [0.9.1](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9.1) (Refactoring, added features and bugfixes)
* [0.9](https://github.com/viktorchernev/DescribeCompiler/releases/tag/0.9) (Initial release - Open beta)

## Notes
* We currently have inbuilt translators for HTML and JSON. If you need to target other languages, you'd have to write your own translator - it is very easy. I will give updates here when more translators are available.