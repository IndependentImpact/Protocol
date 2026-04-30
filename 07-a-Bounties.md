
## Bounties

### Overview

Bounties on the Independent Impact platform function similarly to their real-world counterparts: they involve a sum of money locked in a smart contract, accompanied by a clearly defined task that agents can complete to receive the reward. Any agent with sufficient funds can create a bounty for various purposes, including data collection, information review, or indicator creation.

What distinguishes platform bounties from traditional ones is the controlled participation system. While traditional bounties often attract multiple competitors racing to complete the task, platform bounties limit the number of agents who can work on a bounty simultaneously. This approach serves two key purposes:

1. **Encouraging thoroughness over speed**: By limiting the number of participants, we ensure that those who do take on a bounty can focus on delivering high-quality results rather than rushing through the task.

2. **Optimizing resource allocation**: Preventing resource wastage by avoiding situations where multiple agents work on the same task simultaneously, which could lead to redundant efforts and inefficient use of human capital.

**Note**: Agents who participate in a bounty are collectively referred to as the "mission team."

## Bounty Creation and Participation Rules

### 1. Bounty Creation
Any agent can create a bounty for tasks listed in Appendix SWS. The process begins with the agent specifying the task details and locking the compensation funds in a smart contract escrow.

### 2. Compensation and Escrow
The compensation amount, typically in HBAR, is deducted from the bounty creator's account and placed in escrow at the time of bounty creation. This ensures that funds are available to reward successful completion of the task.

### 3. Bounty Phases
A bounty period consists of three distinct phases:

- **Team Assembly Phase**: During this initial phase, agents can claim seats on the mission team. The duration of this phase is determined by the bounty creator.

- **Mission Phase**: This is the active work period where the mission team completes the task. The duration is also set by the bounty creator.

- **Dispute Resolution Phase**: This final phase lasts between 7 to 30 days and is dedicated to resolving any disputes about the submitted work. The creator can request minor changes or corrections, and formal disputes can be adjudicated during this period.

The start and end dates for each phase must be clearly specified by the bounty creator when publishing the bounty.

### 4. Eligibility Requirements
Bounty creators may establish minimum KS (Knowledge Skills) or CR (Contribution Reputation) requirements for participants. These requirements help ensure that only qualified agents can participate in the bounty.

### 5. Compensation Distribution for Multi-Domain Bounties
When reputation requirements are specified across multiple KS domains, the bounty creator must clearly define how the compensation will be divided among these domains. For example, if a bounty requires expertise in both environmental science and data analysis, the creator might specify that 60% of the compensation will be allocated to the environmental science domain and 40% to the data analysis domain, based on the relative contributions of each domain to the task.

### 6. Mission Team Composition
The number of seats available on a mission team depends on the number of KS reputation domains with specified minimum score requirements:

- If no reputation requirements are specified, the mission team consists of a single agent.

- If reputation requirements are specified for multiple domains, the mission team can include one agent per KS domain, ensuring a diverse set of expertise for complex tasks.

### 7. Claiming a Seat
An agent who wishes to participate in a bounty signals their intent by claiming a seat on the mission team. Once a seat is claimed, it becomes unavailable to other agents, ensuring that each seat is occupied by only one agent.

### 8. Seat Eligibility
If reputation criteria are specified for a specific seat, an agent can only claim that seat if they meet the required reputation standards for that domain.

### 9. Multiple Seat Claims
An agent can claim multiple seats on a mission team, provided they meet the minimum reputation criteria for each seat they claim.

### 10. Seat Cancellation
An agent can cancel their claim on a mission team seat, but will lose CR points based on when the cancellation occurs:
- During the team assembly phase or first quarter of the mission phase: 1 CR point
- Second quarter of the mission phase: 2 CR points
- Third quarter of the mission phase: 3 CR points
- Fourth quarter of the mission phase: 4 CR points
A seat cannot be cancelled during the dispute resolution phase.

### 11. Seat Transfer
An agent can transfer their mission team seat claim to another agent if they cannot fulfill their responsibilities on time. The transfer rules are:
- Before the end of the second quarter of the mission phase: no CR loss for the original holder
- After the end of the second quarter: 1 CR point loss for the original holder
A seat transfer cannot occur during the dispute resolution phase.

### 12. Transfer Eligibility
An agent can only transfer their mission team seat to another agent who:
- Meets the domain-specific reputation criteria for the seat, if specified
- Does not hold seats on more than two other mission teams at the time of the transfer
- Formally agrees to the transfer

### 13. Transfer Consequences
An agent who transfers their seat will not receive any compensation at the end of the bounty period, regardless of when or why the transfer occurred.

### 14. Bounty Cancellation
A bounty can be cancelled by its creator, but the creator will lose CR points and potentially some of their escrowed funds:
- During the team assembly phase or first quarter of the mission phase: 1 CR point
- Second quarter: 2 CR points
- Third quarter: 3 CR points
- Fourth quarter: 4 CR points
A bounty cannot be cancelled during the dispute resolution phase.

### 15. Partial Compensation for Cancellation
If a bounty is cancelled, agents who had held a seat for at least one quarter will receive:
- 25% of the compensation for holding a seat for at least one quarter
- 50% for at least two quarters
- 75% for at least three quarters

### 16. Work Submission
Each agent who holds a seat on a bounty’s mission team must submit their work before the mission deadline specified by the creator of the bounty.

### 17. Late Submission Consequences
If an agent fails to submit their work on time, they will lose CR points according to the seat cancellation rules and will not receive any part of the bounty.

### 18. Bounty Accessibility
A bounty is by default open to all agents on the platform. However, the creator can choose to follow an invitation-only approach, meaning that seats on the mission team will only be available to agents who were specifically invited by the creator.

### 19. Unfilled Bounty
If a bounty reaches the end of its team assembly period and none of the seats on the mission team have been filled, the bounty will automatically be cancelled by the platform. The creator will not lose any CR, and the full bounty will be returned to their account.

### 20. Partially Filled Bounty
If a bounty reaches the end of its team assembly period and only some of the seats have been filled, the creator has three options:
- Republish the bounty with new dates for the different phases and possibly adjust reputation requirements and bounty size
- Continue with the bounty, allowing the existing mission team to move into the mission phase
- Cancel the bounty, returning the full bounty to the creator

### 21. Dispute Resolution Phase
During the dispute resolution phase:
- The creator can request minor changes or corrections to the submitted work
- Formal disputes can be adjudicated by an independent third party
- Team members can lodge complaints about each other's contributions

### 22. Bounty Payout
The bounty will be paid out to the mission team at the end of the dispute resolution phase.

### 23. Creator Reputation Gain
The creator of a bounty will earn CR points proportionate to the size of the bounty. The formula for calculating CR gain is:
\[ \text{CR Gain} = \frac{\text{Bounty Amount}}{\text{Total Platform Bounty Amounts}} \times \text{Constant Factor} \]

**Note**: Every bounty will have its own discussion topic to facilitate communication between the creator and the mission team. Only the creator and mission team members can post to the discussion topic, but it will be made publicly visible once the bounty period has ended.

### Reputation-based Reviewing

An agent can publish a request for the review of some claim or information. A review request is a type of bounty and is therefore governed by the rules provided in Section Bounty. However, several additional rules apply to review requests:

**Note**: The mission team of a review request is referred to here as the "review panel."

**Note**: When a bounty is a review request, its dispute resolution phase doubles up as the "Q&A phase" of the review request.

1. **Permission Requirement**: If an agent who wishes to publish a review request is neither the owner nor the contributor of the information, they must obtain permission from the owner to create the review request.

2. **Review Subject**: A review request must clearly specify the subject of the review, such as "Review of statistical robustness of activity XYZ's planned sampling strategy for impact monitoring."

3. **Review Mandate**: A review request must clearly state the mandate of the review, i.e., whether the objective is to validate, to verify, or both.

4. **Review Standard**: A review request must specify the standard against which the review should be carried out.

5. **Reviewer Eligibility**: The creator of the review request must specify at least one minimum KS reputation requirement for at least one relevant KS domain that must be met by agents who wish to act as reviewers.

6. **Conflict of Interest**: Every reviewer must sign a declaration of conflicts of interest.

7. **Reviewer Restrictions**: An agent cannot review information contributed by or related to them or their activities.

8. **Review Submission**: Each reviewer who holds a seat on a review request’s panel must submit a review before the review deadline. Reviewers are encouraged to communicate with each other during the review period to complement each other's expertise.

9. **Trainee Review**: Every review request provides the opportunity for one "ineligible" agent to submit a "training" review. The trainee’s review must be reviewed and graded by every eligible reviewer on the review panel during the Q&A phase.

10. **Trainee Grading**: An "expert" reviewer who fails to grade the trainee reviewer’s review at the end of a review process will lose 2 CR points.

11. **Q&A Response**: A reviewer who fails to respond to final questions from the review requester during the Q&A phase will lose 1 CR point.

12. **Review Contestation**: Review outcomes can be contested during the dispute resolution phase. The rules for contestation and the process for retracting a review will be specified in the platform's dispute resolution guidelines.

**Note**: It is advisable to restrict the scope of a review request as much as possible to avoid requiring collaboration among too many reviewers.

**Note**: The trainee seat in the review system is a core feature that cannot be disabled by the creator of the review request. It is designed to promote knowledge sharing and learning on the platform.

