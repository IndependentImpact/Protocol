--- a/Bounties.md
+++ b/Bounties.md
@@ -1,3 +1,48 @@
-TODO: Describe what happens during the dispute resolution phase.
-TODO: NB: What happens if an agent holds a seat on a bounty, but then their reputation scores drop below the seat's rep reqs while they are still holding it?
-TODO: How can someone contest someone else's vote?
+# Bounties
+
+A bounty is a scoped work item with explicit acceptance criteria, reputation requirements, and rewards. This chapter describes how bounty seats remain eligible, how disputes are resolved, and how votes can be contested.
+
+## Seat eligibility while holding a bounty
+
+A seat on a bounty has reputation requirements. Eligibility is checked continuously.
+
+If an agent's reputation falls below a seat's requirements after the agent has been assigned the seat:
+
+1. The seat enters a remediation state immediately.
+2. The agent may remain associated with the bounty for the purpose of completing in-flight work, but cannot exercise governance privileges that require the seat.
+3. The agent cannot cast new bounty votes, approve disbursements, or receive seat-based rewards while below the requirement.
+4. If the agent restores the required reputation before the remediation window ends, full seat privileges are restored.
+5. If the agent does not restore the required reputation, the seat is declared vacant and the bounty's replacement process begins.
+
+Votes cast while the agent was eligible remain valid unless separately invalidated by a successful contest or dispute.
+
+## Dispute resolution phase
+
+A dispute may be raised when a submission is rejected, when a vote is contested, or when a participant believes bounty rules were violated.
+
+During dispute resolution:
+
+1. The affected bounty action is frozen. Funds, rewards, and state changes tied to the disputed action cannot be finalized until the dispute is closed.
+2. The disputing party states the rule allegedly violated and provides supporting evidence.
+3. The opposing party may respond with evidence.
+4. Eligible reviewers evaluate the record against the bounty's published acceptance criteria and protocol rules.
+5. Reviewers vote to uphold the disputed action, reverse it, or apply a remedial action permitted by the protocol.
+
+A dispute is resolved when the required reviewer votes are recorded and any mandatory challenge window has passed. The outcome is final unless the protocol provides an explicit appeal path.
+
+If reviewers determine that a participant acted in bad faith, submitted false evidence, or attempted to manipulate the process, that participant may lose reputation, forfeit stake, or be removed from the bounty.
+
+## Contesting another participant's vote
+
+A participant with standing in the bounty may contest another participant's vote.
+
+To contest a vote, the challenger must:
+
+1. Submit a contest during the applicable challenge window.
+2. Identify the contested vote and the bounty action it affects.
+3. Provide evidence that the vote was invalid, coercive, fraudulent, conflicted, or otherwise violated bounty rules.
+4. Lock any contest bond required by the protocol.
+
+While a contest is open, the contested vote is marked provisional and is excluded from final settlement until the contest is resolved.
+
+If the contest is upheld, the vote is invalidated or re-weighted according to the resolution outcome, and the voter may be subject to reputation or stake penalties. If the contest is rejected, the vote is counted as cast, and the challenger may forfeit the contest bond if the contest was frivolous or abusive.