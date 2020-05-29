# PlantUML stdlib snippets for vscode

[![Version](https://vsmarketplacebadge.apphb.com/version/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/version-short/voronenko.vscode-plantuml-stdlib-snippets.svg)
[![Install](https://vsmarketplacebadge.apphb.com/installs/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/installs-short/voronenko.vscode-plantuml-stdlib-snippets.svg)
[![Downloads](https://vsmarketplacebadge.apphb.com/downloads/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/downloads-short/voronenko.vscode-plantuml-stdlib-snippets.svg)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating-short/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/rating-short/voronenko.vscode-plantuml-stdlib-snippets.svg)

This extension provides you number of the dummy code snippets for PlantUML standard library https://plantuml.com/stdlib

Supported stdlib extensions

| StdLib name  |  Required common macros  |  Folder include macros supported  |  Snippets prefix  |   |   |
|---|---|---|---|---|---|
| aws  | i-aws-common  | N/A  |   |   |   |
| awslib  | N/A  | i-all  |   |   |   |
| azure  | i-azure-common  |   |   |   |   |
| cloudinsight  | N/A  |   |   |   |   |
| cloudogu  | i-co-common  |   |   |   |   |
| elastic  | i-elastic-common  |   |   |   |   |
| logo  |   |   |   |   |   |
| material  |   |   |   |   |   |
| office  | i-off-common  |   |   |   |   |
| osa  | N/A  |   |   |   |   |
| tupadr3  | i-t3-common  |   |   |   |   |


Idea for the snippets is to speedup time needed to recall how is called your favorite icon from stdlib and use it in your plantuml diagram.
Depending on a stdlib library used you might need to invoke following steps:

a) Invoke required "include-common" macros which initializes diagram for subsequent library objects.

Usually you are starting to type `i-` (which is shortened for `include-`) followed by library and word common. Note that VSCode is smart enough
to do a fuzzy search, thus you could just time smth like `iawscommon` in one word

b) Include icons that will be used in your diagram

On that moment you should briefly recall what kind of object you want to draw in your diagram.
Thus you could look for either part of the object name  `i-aws-efsfilesystem_large`, group and object name `i-aws-Storage-efsfilesystem`.

c) Now you can insert object itself

usual text to be used in fuzzy search would be library code - object name  `aws-amazonefs`.  As usually vscode smart enough, thus you can use quite fuzzy combination of words.
