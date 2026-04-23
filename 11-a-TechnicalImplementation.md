## Technical implementation

This section is still a W.I.P.

Every entity (other than actions) on the platform has a Hedera topic. Posting to a topic costs HBAR, as per HIP-991. The Hedera topic of an entity is its ID in the Independent Impact ecosystem, i.e., the value that will be used for the “@id” field in the Fluree ledger. 

Every action on the II platform is recorded as a transaction on the Hedera network. The message ID of the transaction is the “@id” value for the action.

Every action on the platform is recorded on the Hedera hashgraph and therefore incurs transaction fees. To create a new activity, for example, will cost something; to cast a vote, or to post a comment or a question to a topic, will also cost something. These costs will be generally very small as they will largely be determined by the Hedera network transaction fees  – which are famously very low.

Every review request will have a discussion Hedera topic associated with it which will provide a space for the reviewers on the panel, including the trainee reviewer, to communicate with each other and the activity owner regarding the subject of the review. This topic will be made publicly visible when the review process concludes.

All reputation (Knowledge & Skills and Conduct) will be tokens - fungible and divisible, but not tradable. This will allow them to interact with smart contracts etc. 

