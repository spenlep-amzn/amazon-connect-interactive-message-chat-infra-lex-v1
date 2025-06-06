> ### **📢 Annoucement:** This repository is no longer maintained. Amazon Lex V1 will reach end of life on September 15, 2025. Please follow this migration guide: https://docs.aws.amazon.com/lexv2/latest/dg/migration.html
> ![Maintenance](https://img.shields.io/badge/repo-inactive-red)

---

# Amazon Connect Interactive Message Chat Infra [Lex V1]

Example setup for Amazon Connect chat interactive message feature [Lex Bot V1]

## Links

* Documentation: https://docs.aws.amazon.com/connect/latest/adminguide/interactive-messages.html
* Blog Post: https://aws.amazon.com/blogs/contact-center/easily-set-up-interactive-messages-for-your-amazon-connect-chatbot/
* (old) Workshop: https://catalog.us-east-1.prod.workshops.aws/workshops/638d00f5-2248-488f-b7ca-903e8b966bf8/en-US/2-workshop/400-lex-chat

## Files

[![Download Lambda ZIP](https://img.shields.io/badge/Download-ZIP-blue.svg?logo=aws-lambda&logoColor=orange&label=Download%20Lambda&color=orange)](https://github.com/spencerlepine/amazon-connect-interactive-message-chat-infra-lex-v1/blob/main/exports/InteractiveMessge_LambdaCodeHook_LexV1Export.zip)

[![Download Lex Bot ZIP](https://img.shields.io/badge/Download-ZIP-blue.svg?logo=amazon-aws&logoColor=lightgray&label=Download%20Lex%20Bot%20Export&color=blue)](https://github.com/spencerlepine/amazon-connect-interactive-message-chat-infra-lex-v1/blob/main/exports/InteractiveMessge_LambdaCodeHook_LexV1Export.zip)

[![Download Contact Flow JSON](https://img.shields.io/badge/Download-JSON-blue.svg?logo=amazon-aws&logoColor=lightgray&label=Download%20Contact%20Flow&color=green)](https://github.com/spencerlepine/amazon-connect-interactive-message-chat-infra-lex-v1/blob/main/exports/InteractiveMessaging_ContactFlow_LexV1.json)

## Screenshots

### Architecture

![image](./InteractiveMessageArchitecture.png)

### Flow Chart

![image](./InteractiveMessageFlowChart.png)

### Chat Usage

![image](./InteractiveMessageChatFlow.png)

## Specifications

- Lex Bot V1 support
- Node v16+

## Deployment

### Connect Instace

Create an Amazon Connect Instance to use, follow [documentation](https://docs.aws.amazon.com/connect/latest/adminguide/amazon-connect-instances.html) for more details.

| Region | Launch Button |
| ------ | ------------- |
| us-east-1 (N. Virginia)  | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://us-east-1.console.aws.amazon.com/connect/v2/app/onboarding?region=us-east-1)  |
| us-west-2 (Oregon)       | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://us-west-2.console.aws.amazon.com/connect/v2/app/onboarding?region=us-west-2)       |
| ap-southeast-2 (Sydney)  | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-southeast-2.console.aws.amazon.com/connect/v2/app/onboarding?region=ap-southeast-2)  |
| ap-northeast-1 (Tokyo)   | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-northeast-1.console.aws.amazon.com/connect/v2/app/onboarding?region=ap-northeast-1)   |
| eu-central-1 (Frankfurt) | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://eu-central-1.console.aws.amazon.com/connect/v2/app/onboarding?region=eu-central-1) |
| eu-west-2 (London)       | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://eu-west-2.console.aws.amazon.com/connect/v2/app/onboarding?region=eu-west-2)       |
| ap-southeast-1 (Singapore) | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-southeast-1.console.aws.amazon.com/connect/v2/app/onboarding?region=ap-southeast-1) |
| ca-central-1 (Canada)    | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ca-central-1.console.aws.amazon.com/connect/v2/app/onboarding?region=ca-central-1)    |
| ap-northeast-2 (South Korea) | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-northeast-2.console.aws.amazon.com/connect/v2/app/onboarding?region=ap-northeast-2) |
| af-south-1 (Cape Town)   | [![Create Instance](https://img.shields.io/badge/Create%20Instance-%20-green.svg?logo=amazon-aws&logoColor=white)](https://af-south-1.console.aws.amazon.com/connect/v2/app/onboarding?region=af-south-1)   |


### Lambda [![Download Lambda ZIP](https://img.shields.io/badge/Download-ZIP-blue.svg?logo=aws-lambda&logoColor=orange&label=Download%20Lambda&color=orange)](https://github.com/spencerlepine/amazon-connect-interactive-message-chat-infra-lex-v1/blob/main/exports/InteractiveMessge_LambdaCodeHook_LexV1Export.zip)

Upload the Lambda [InteractiveMessge_LambdaCodeHook_LexV1Export.zip](./exports/InteractiveMessge_LambdaCodeHook_LexV1Export.zip) file, follow the [documentation](https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-package.html#gettingstarted-package-zip) for instructions.

| Region | Launch Button |
| ------ | ------------- |
| us-east-1 (N. Virginia) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://us-east-1.console.aws.amazon.com/lambda/home?region=us-east-1#/create/function?intent=authorFromScratch) |
| us-west-2 (Oregon) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://us-west-2.console.aws.amazon.com/lambda/home?region=us-west-2#/create/function?intent=authorFromScratch) |
| ap-southeast-2 (Sydney) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-southeast-2.console.aws.amazon.com/lambda/home?region=ap-southeast-2#/create/function?intent=authorFromScratch) |
| ap-northeast-1 (Tokyo) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-northeast-1.console.aws.amazon.com/lambda/home?region=us-east-1#/create/function?intent=authorFromScratch) |
| eu-central-1 (Frankfurt) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://eu-central-1.console.aws.amazon.com/lambda/home?region=us-east-1#/create/function?intent=authorFromScratch) |
| eu-west-2 (London) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://eu-west-2.console.aws.amazon.com/lambda/home?region=eu-west-2#/create/function?intent=authorFromScratch) |
| ap-southeast-1 (Singapore) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-southeast-1.console.aws.amazon.com/lambda/home?region=ap-southeast-1#/create/function?intent=authorFromScratch) |
| ca-central-1 (Canada) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ca-central-1.console.aws.amazon.com/lambda/home?region=ca-central-1#/create/function?intent=authorFromScratch) |
| ap-northeast-2 (South Korea) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-northeast-2.console.aws.amazon.com/lambda/home?region=ap-northeast-2#/create/function?intent=authorFromScratch) |
| af-south-1 (Cape Town) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lambda-%20-green.svg?logo=amazon-aws&logoColor=white)](https://af-south-1.console.aws.amazon.com/lambda/home?region=af-south-1#/create/function?intent=authorFromScratch) |

### Lex Bot [![Download Lex Bot ZIP](https://img.shields.io/badge/Download-ZIP-blue.svg?logo=amazon-aws&logoColor=lightgray&label=Download%20Lex%20Bot%20Export&color=blue)](https://github.com/spencerlepine/amazon-connect-interactive-message-chat-infra-lex-v1/blob/main/exports/InteractiveMessageBot_LEX_V1.zip)

Create a bot and import the [InteractiveMessageBot_LEX_V1.zip](./exports/InteractiveMessageBot_LEX_V1.zip) file, follow the [documentation](https://docs.aws.amazon.com/lexv2/latest/dg/import-console.html) for instructions.

| Region | Launch Button |
| ------ | ------------- |
| us-east-1 (N. Virginia) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://us-east-1.console.aws.amazon.com/lexv2/home?region=us-east-1#importBot) |
| us-west-2 (Oregon) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://us-west-2.console.aws.amazon.com/lexv2/home?region=us-west-2#importBot) |
| ap-southeast-2 (Sydney) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-southeast-2.console.aws.amazon.com/lexv2/home?region=ap-southeast-2#importBot) |
| ap-northeast-1 (Tokyo) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-northeast-1.console.aws.amazon.com/lexv2/home?region=ap-northeast-1#importBot) |
| eu-central-1 (Frankfurt) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://eu-central-1.console.aws.amazon.com/lexv2/home?region=eu-central-1#importBot) |
| eu-west-2 (London) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://eu-west-2.console.aws.amazon.com/lexv2/home?region=eu-west-2#importBot) |
| ap-southeast-1 (Singapore) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-southeast-1.console.aws.amazon.com/lexv2/home?region=ap-southeast-1#importBot) |
| ca-central-1 (Canada) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ca-central-1.console.aws.amazon.com/lexv2/home?region=ca-central-1#importBot) |
| ap-northeast-2 (South Korea) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://ap-northeast-2.console.aws.amazon.com/lexv2/home?region=ap-northeast-2importBot) |
| af-south-1 (Cape Town) | [![Deploy Lambda](https://img.shields.io/badge/Create%20Lex%20Bot-%20-green.svg?logo=amazon-aws&logoColor=white)](https://af-south-1.console.aws.amazon.com/lexv2/home?region=af-south-1#importBot) |

### Contact Flow [![Download Contact Flow JSON](https://img.shields.io/badge/Download-JSON-blue.svg?logo=amazon-aws&logoColor=lightgray&label=Download%20Contact%20Flow&color=green)](https://github.com/spencerlepine/amazon-connect-interactive-message-chat-infra-lex-v1/blob/main/exports/InteractiveMessaging_ContactFlow_LexV1.json)

Import the [InteractiveMessaging_ContactFlow_LexV1.json](./exports/InteractiveMessaging_ContactFlow_LexV1.json) file to create an inbound contact flow, follow the [documentation](https://docs.aws.amazon.com/connect/latest/adminguide/contact-flow-import-export.html) for more details



---

![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Famazon-connect-interactive-message-chat-infra-lex-v1&label=VIEWS&countColor=%23263759)

