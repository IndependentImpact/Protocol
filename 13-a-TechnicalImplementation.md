## Technical implementation

This section is still a W.I.P.

Every entity (other than actions) on the platform has a Hedera topic. Posting to a topic costs HBAR, as per HIP-991. The Hedera topic of an entity is its ID in the Independent Impact ecosystem, i.e., the value that will be used for the “@id” field in the Fluree ledger. 

Every action on the II platform is recorded as a transaction on the Hedera network. The message ID of the transaction is the “@id” value for the action.

Every action on the platform is recorded on the Hedera hashgraph and therefore incurs transaction fees. To create a new activity, for example, will cost something; to cast a vote, or to post a comment or a question to a topic, will also cost something. These costs will be generally very small as they will largely be determined by the Hedera network transaction fees  – which are famously very low.

Every review request will have a discussion Hedera topic associated with it which will provide a space for the reviewers on the panel, including the trainee reviewer, to communicate with each other and the activity owner regarding the subject of the review. This topic will be publicly visible.

Bounties vs review requests: A review request is a type of bounty; it is just a lot more “specialised”. For example, a bounty could specify minimum reputation requirements, but is not required to do so; a review request, on the other hand, must specify such requirements. What are the rules for bounties? How many bounties is an agent allowed to pursue simultaneously?

All reputation stuff, including CR, must be tokens, because then we can let them interact with smart contracts etc. Yes, all of them are tokens – fungible and divisible, but not tradable.

The owner of an activity must be able to allow or disallow free (unsolicited) public contribution of information about/to their activity. 

Furthermore, the platform is intentionally designed to maximise transparency, traceability and verifiability. Every action performed on the platform is transparently recorded on the Hedera network. All information provided about activities, and any changes made thereto, along with the authors of the information and the changes, are captured in a publicly accessible, time-travelable Fluree ledger.

In addition, the platform is designed to maximise the accessibility, accountability and comparability of information by capturing all information in a public, semantic ledger with a complete history of authorship. 
