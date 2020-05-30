# PlantUML stdlib snippets for vscode

[![Version](https://vsmarketplacebadge.apphb.com/version/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/version-short/voronenko.vscode-plantuml-stdlib-snippets.svg)
[![Install](https://vsmarketplacebadge.apphb.com/installs/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/installs-short/voronenko.vscode-plantuml-stdlib-snippets.svg)
[![Downloads](https://vsmarketplacebadge.apphb.com/downloads/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/downloads-short/voronenko.vscode-plantuml-stdlib-snippets.svg)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating-short/voronenko.vscode-plantuml-stdlib-snippets.svg)](https://vsmarketplacebadge.apphb.com/rating-short/voronenko.vscode-plantuml-stdlib-snippets.svg)

This extension provides you number of the dummy code snippets for PlantUML standard library https://plantuml.com/stdlib

Supported stdlib extensions

| StdLib name  |  Required common macros  |  Folder include macros supported  |  Snippets include prefix  |   |   |
|---|---|---|---|---|---|
| aws  | i-aws-common  | N/A  | ia  |   |   |
| awslib  | N/A  | i-all  | i-  |   |   |
| azure  | i-azure-common  | i-all-  | i-  |   |   |
| cloudinsight  | N/A  |   | i-cloudinsight  |   |   |
| cloudogu  | i-co-common  |   |  i-co  |   |   |
| elastic  | i-elastic-common  |   | i-es  |   |   |
| logo  |   |   | i-logo  |   |   |
| material  |   |   | i-material  |   |   |
| office  | i-off-common  |   |  i-off |   |   |
| osa  | N/A  |   |  i-osa |   |   |
| tupadr3  | i-t3-common  |   | i-t3  |   |   |


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

## Notes on a specific libraries

### aws

As seen on a screen recording below, usually you are supposed to have some prototype of the future diagram in raw plant uml, and use stdlib/aws to provide greater visualization 
to the diagram. On a moment when you want to include some icon, you start snippet search with `ia` followed by icon topic or name. On a moment, when you want to use icon itself,
you just start typing approximate icon name. The one in appercase will be the needed one

![AWS classic](docs/stdlib-aws.gif)


## awslib

That extension is kind of official "icons" released under https://github.com/awslabs/aws-icons-for-plantuml ; It appeared later than `aws` and the most notible difference
from classic `aws` lib is presence of the cumulative include all files with sprites divided in a limited set of areas. You could also distinguish icons from that set
by selecting AWS entity in a CamelCase.

|Section                             |snippet shortcut                   |
|--|--|
| Analytics/                         | iall-analytics                    |
| AWSCostManagement/                 | iall-awscostmanagement            |
| Compute/                           | iall-compute                      |
| Database/                          | iall-database                     |
| GameTech/                          | iall-gametech                     |  
| InternetOfThings/                  | iall-internetofthings             |
| MediaServices/                     | iall-mediaservices                |
| NetworkingAndContentDelivery/      | iall-networkingandcontentdelivery |
| Satellite/                         | iall-satellite                    |
| ApplicationIntegration/            | iall-applicationintegration       |
| Blockchain/                        | iall-blockchain                   |
| CustomerEnablement/                | iall-customerenablement           |
| DeveloperTools/                    | iall-developertools               |
| General/                           | iall-general                      |
| MachineLearning/                   | iall-machinelearning              |
| MigrationAndTransfer/              | iall-migrationandtransfer         |
| QuantumTechnologies/               | iall-quantumtechnologies          |
| SecurityIdentityAndCompliance/     | iall-securityidentityandcompliance|
| ARVR/                              | iall-arvr                         |
| BusinessApplications/              | iall-businessapplications         |
| CustomerEngagement/                | iall-customerengagement           |
| EndUserComputing/                  | iall-endusercomputing             |
| GroupIcons/                        | iall-groupicons                   |
| ManagementAndGovernance/           | iall-managementandgovernance      |
| Mobile/                            | iall-mobile                       |
| Robotics/                          | iall-robotics                     |
| Storage/                           | iall-storage                      |

For a simplicity, we introduce few additional "meta" snippets.

Diagrams constructed with this extension look like "Azure" ones

![AWS classic](docs/stdlib-awslib.gif
