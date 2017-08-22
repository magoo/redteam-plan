# The Red Team Planning Guide

#### Intro
This is a project manager's approach to designing a red team using a very specific method as described in [Red Teams](https://medium.com/starting-up-security/red-teams-6faa8d95f602). This specific method expresses several biases to optimize for blue team value, not red team dominance.

Review the questions below to test if your red team planning has been thorough and will give you the best results.

## Checklists

#### Time
- Planning: Planning the overall execution, filling in the gaps of this document. Weeks/Months
- Attack: Onboarding of red team and active creation of the incident. Minutes/Weeks
- Response: If the incident is discovered, the length of the immediate response. Hours/Weeks
- Tabletop: If the incident is not discovered, the length of the forced response or tabletop. Days / Weeks  
- Incident Response (Short Term): The time to remove red team access, plug any discovered vulnerability, elimination of the adversary. Days / Weeks
- Red Team Reveal: Displaying the Red Team's actions to calibrate on IR realities.
- Incident Response (Post Mortem): Organization of the lessons learned and wide presentation. Hours / Days
- Long Term Mitigation: Completion of harder lessons learned, refactoring, and growth before you consider the next red team. Weeks / Months

#### People  
- Consulting firms: Will you be hiring an external party as the red team?
- Internal resources: Will internal employees act as the red team?
- Who is responsible for calling (and withholding) a call to the police?
- Who is responsible for inbound PR / Communications?
- Who is responsible for customer interactions?
- Who is the breach notification resource? (In house counsel / firm)
- Who is the overall "Game Master"

#### Strategy
- Are potential defenders aware that a red team is expected, ever?
- Will you also announce a window in which a red team should be expected?
- Will the red team be heavily guided with cheating, or will it be freeform?
- Has the team been informed that there will be strict rules about shaming?
- Has the team been informed that this is meant to be a gift to a blue team, not to punish bad security? IE, this is not a test, this is sparring?
- Has a specific "kill chain" been selected for targeting? Is it a practical risk?
- Is your goal to simulate an incident in a heavily mitigated risk, or a risk with much less telemetry / preventative measures?

#### Attack Design
- Does the attack actually need a lot of expertise and effort, or can you have simple recreations of an attack to discover?
- Where should the attack begin in the kill chain? (IE, early: spear phishing, or late: lateral movement with domain admin)
- What credentials / physical access / documentation are required to support the initiation of the attack? Who will provide them? Are there security implications that need to be followed up on later?
- If the red team succeeds early, should they begin penetration testing or vulnerability assessment? Should they try to be caught?
- Should the attacker impersonate a specific adversary, or attack method?
- If the red team is detected, will there be a backup plan or second attack?
- Where and how will the red team be documenting their behaviors? These need to be captured for any follow up tabletop and to confirm remediation and lesson learned.
- Are the Red Team's methods going to be based in reality? Are they using methods that are not available to a realistic attacker?

#### Incident Response
- Is there a specific coordination method or plan that incident response should follow? For instance, the agenda and method described in [Security Breach 101](https://medium.com/starting-up-security/security-breach-101-b0f7897c027c) or [An Incident Response Plan for Startups](https://github.com/magoo/Incident-Response-Plan/blob/master/EXAMPLE.md)
- Will Incident Response need to come together naturally to weed out friction, or will this come together artificially to force the intended response as practice?
- Who will bridge communications with the Red Team, if there are honest questions from the Blue Team? (For example: "We think we found a separate breach")
- Who will document the Red Team's pain points as the Blue Team mitigates? ("You kept removing our beacons and it was hard to get back, we didn't expect you'd find them all at once!")
- If Incident Response is not progressing in a timely manner, who or how will indicators be leaked to the Blue Team?
- Are short term mitigations / long term preventative measures being collected as part of your incident response?

#### Red Team Reveal
- Are the Red Team's actions during the attack phase very well documented and understood?
- Has the incident response process missed any substantial Red Team actions?
- Are there any IOC's or artifacts that are still beaconing or discoverable in the future?
- Have any backdoors or other at risk changes survived incident response?
- How thorough was the Blue Team's investigation and containment?

#### Post Mortem
- Has a thorough interviewing process or debrief happened with all participants in the exercise?
- Have all follow up mitigation items been collected centrally and prioritized based on the value sentiment of the participants?
- Are these sentiments being concluded and presented back to the participants?
- Do you have a meeting blocked to present them?
- Who is presenting them?
- Is the Red Team available to comment on these sentiments, or available to answer questions?
- Are participants being rewarded for participating?
- Are they given plenty of time to debrief and discuss?
- Is this a valuable calibration towards practical risks?

