========================================
Source Code (between the arrows)
========================================

🡆A vertical tab character (ASCII 11) ->

	A form feed character (ASCII 12),
	A next line (NEL) character (Unicode character U+0085),

	A non-breaking space (Unicode character U+00A0), 
	An ogham space mark (Unicode character U+1680), 
	En Quad (U+2000), 
	Em Quad (U+2001), 
	En Space (U+2002), 
	Em Space (U+2003), 
	Three-Per-Em Space (U+2004), 
	Four-Per-Em Space (U+2005), 
	Six-Per-Em Space (U+2006), 
	Punctuation Space (U+2008), 
	Thin Space (U+2009), 
	Hair Space (U+200A), 
	A paragraph separator (Unicode character U+2029),

	A narrow no-break space (Unicode character U+202F), 
	A medium mathematical space (Unicode character U+205F), 
	An ideographic space (Unicode character U+3000),　
	Figure Space; 🡄

========================================
Logged text
========================================

🡆Verbosity set to: High
Language version set to: Describe Lines - v1.0
Describe Transpiler initialized.
Starting a 'File -> AST' operation...
------------------------
Starting a parse operation on file: "C:\Users\Viktor Chernev\Desktop\testing\TestFiles\TestFilesFor10\B_exotic_spaces.ds"
Fetched file contents - 736 characters long

Parsing sequence: T(DATA|'A vertical tab character (ASCII 11) ') T(HYPHEN|'-') T(PRODUCTION_ARROW|'>\r\n\r\n\t') T(DATA|'A form feed character (ASCII 12)') T(SEPARATOR|',\r\n\t') T(DATA|'A next line (NEL) character (Unicode character U+0085)') T(SEPARATOR|',\r\n\r\n\t') T(DATA|'A non') T(HYPHEN|'-') T(DATA|'breaking space (Unicode character U+00A0)') T(SEPARATOR|', \r\n\t') T(DATA|'An ogham space mark (Unicode character U+1680)') T(SEPARATOR|', \r\n\t') T(DATA|'En Quad (U+2000)') T(SEPARATOR|', \r\n\t') T(DATA|'Em Quad (U+2001)') T(SEPARATOR|', \r\n\t') T(DATA|'En Space (U+2002)') T(SEPARATOR|', \r\n\t') T(DATA|'Em Space (U+2003)') T(SEPARATOR|', \r\n\t') T(DATA|'Three') T(HYPHEN|'-') T(DATA|'Per') T(HYPHEN|'-') T(DATA|'Em Space (U+2004)') T(SEPARATOR|', \r\n\t') T(DATA|'Four') T(HYPHEN|'-') T(DATA|'Per') T(HYPHEN|'-') T(DATA|'Em Space (U+2005)') T(SEPARATOR|', \r\n\t') T(DATA|'Six') T(HYPHEN|'-') T(DATA|'Per') T(HYPHEN|'-') T(DATA|'Em Space (U+2006)') T(SEPARATOR|', \r\n\t') T(DATA|'Punctuation Space (U+2008)') T(SEPARATOR|', \r\n\t') T(DATA|'Thin Space (U+2009)') T(SEPARATOR|', \r\n\t') T(DATA|'Hair Space (U+200A)') T(SEPARATOR|', \r\n\t') T(DATA|'A paragraph separator (Unicode character U+2029)') T(SEPARATOR|',\r\n\r\n\t') T(DATA|'A narrow no') T(HYPHEN|'-') T(DATA|'break space (Unicode character U+202F)') T(SEPARATOR|', \r\n\t') T(DATA|'A medium mathematical space (Unicode character U+205F)') T(SEPARATOR|', \r\n\t') T(DATA|'An ideographic space (Unicode character U+3000)') T(SEPARATOR|',　\r\n\t') T(DATA|'Figure Space') T(TERMINATOR|'; ') T(EOF|'<EOF>') Ok

File parsed successfully
Parser red 736 characters, into 58 tokens.
Those were translated to an AST.
All Files: 1, Succeeded: 1, Failed: 0, Errors: 0🡄

========================================
Produced AST
========================================

{"filename":"C:\\Users\\Viktor Chernev\\Desktop\\testing\\TestFiles\\TestFilesFor10\\B_exotic_spaces.ds","nspace":null,"expressions":[{"title":{"tilde":null,"text":{"leafType":"Text","text":"A vertical tab character (ASCII 11)","leadingTrivia":"","trailingTrivia":" "},"tag":null,"links":null,"decorators":null},"arrow":{"leafType":"ProductionArrow","text":"->","leadingTrivia":"","trailingTrivia":"\u000b\r\n\r\n\t"},"lines":[{"body":{"tilde":null,"text":{"leafType":"Text","text":"A form feed character (ASCII 12)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":"\f\r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"A next line (NEL) character (Unicode character U+0085)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":"\r\n\r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"A non-breaking space (Unicode character U+00A0)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"An ogham space mark (Unicode character U+1680)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"En Quad (U+2000)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Em Quad (U+2001)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"En Space (U+2002)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Em Space (U+2003)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Three-Per-Em Space (U+2004)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Four-Per-Em Space (U+2005)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Six-Per-Em Space (U+2006)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Punctuation Space (U+2008)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Thin Space (U+2009)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Hair Space (U+200A)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"A paragraph separator (Unicode character U+2029)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":"\r\n\r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"A narrow no-break space (Unicode character U+202F)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"A medium mathematical space (Unicode character U+205F)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":" \r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"An ideographic space (Unicode character U+3000)","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":",","leadingTrivia":"","trailingTrivia":"　\r\n\t"}},{"body":{"tilde":null,"text":{"leafType":"Text","text":"Figure Space","leadingTrivia":"","trailingTrivia":""},"tag":null,"links":null,"decorators":null},"punctuation":{"leafType":"Text","text":";","leadingTrivia":"","trailingTrivia":" "}}]}],"exception":null}