# :fire: :fire_engine: Planning a Red Team exercise
This document helps inform red team planning by contrasting against the very specific red team style described in [Red Teams](https://medium.com/starting-up-security/red-teams-6faa8d95f602). This method expresses several biases to optimize for blue team value and enthusiasm. It specifically avoids attempts to motivate by red team punishment.

Review the questions below to test if your red team planning has been thoroughly thought out for your blue team's value.

### :x: Negative motivations
The following are common reasons to drive a red team exercise. These have damaging qualities to morale or team cohesion. An exercise may be the wrong tool for your goals.
- Prove the insecurity of another organization
- Display dominance over a group of people
- Prove or make a point through shock and awe
- Enumerate and discover as many vulnerabilities as possible
- Test if simple detection mechanisms are working

### :thumbsup: Stakeholders
Nothing could be more wasteful than an exercise without any sponsorship or follow up from leadership or influencers. Make sure the learnings of an exercise are championed by an enthusiastic group of stakeholders. Make sure this group is informed and can generate momentum.
- Set expectations and a known home / owner to drive outcomes of the exercise
- Ensure there is openness to change, and have sponsorship lined up to drive the change.
- Is the organization a willing participant in this exercise?
- Would participants be open *any* calibration on risk, or a revisitation of their current roadmap?
- Is there significant debt that would take precedence over any Red Team findings?
- Will the Red Team's findings be so predictable that an exercise wasn't needed to begin with?

### :date: Time estimations
You can project the amount of time to allocate from this planning phase, to the end of a mitigation phase, or something in between. Time expectations are highly dependent on decisions made for each phase.

- *Planning* (Weeks/Months): Planning the overall execution, filling in the gaps of this document.
- *Attack* (Minutes/Weeks): Onboarding of red team and active creation of the incident.
- *Response* (Hours/Weeks): If the incident is discovered, the length of the immediate response.
- *Tabletop* (Days / Weeks): If the incident is not discovered, the length of the forced response or tabletop.  
- *Incident Response (Short Term)* (Days / Weeks): The time to remove red team access, plug any discovered vulnerability, elimination of the adversary.
- *Red Team Reveal* (Hours): Displaying the Red Team's actions to calibrate on IR realities.
- *Incident Response (Post Mortem)* (Hours / Days): Organization of the lessons learned and wide presentation.
- *Long Term Mitigation* (Weeks / Months): Completion of harder lessons learned, refactoring, and growth before you consider the next red team.

### :family: People
Identify all the people who may need to know the Red Team's plans and secrets. This is where you'll want to mitigate any "Break Glass" risk, and have contact details ready for a pivot away from an exercise due to any emergencies.
- Consulting firms: Will you be hiring an external party as the red team?
- Internal resources: Will internal employees act as the red team?
- Who is responsible for (in this case, withholding) a call to the police?
- Who is responsible for inbound PR / Communications?
- Who is responsible for customer interactions?
- Who is the breach notification resource? (in-house / outside counsel)
- Who is the overall "Game Master" that will steer issues and be the ultimate source of good judgement?

### :chart_with_downwards_trend: Strategy
Decide where you are going to accumulate your value from this experience. There are tradeoffs everywhere that may not scratch what you're trying to itch with an exercise.
- Are potential defenders aware that a red team should be expected at some point?
  - Should they be? Do you need to set this expectation?
- Will you also announce a window in which a red team should be expected?
  - Will this cause healthy excitement and a preparation sprint?
- Will the attackers be heavily guided with cheating, or will it be freeform?
  - This tradeoff is about incident response value and the discovery of vulnerabilities.
- Has the team been informed that there will be strict rules about shaming?
  - You want to avoid any feeling that this is a punishment for bad security.
- Has the team been informed that this is meant to be a gift to a blue team, not to punish bad security? IE, this is not a test, this is sparring?
  - Doubling down on this point. Make sure it's known that this is a valuable feedback loop, not an employee performance cycle.
- Has a specific [method](https://attack.mitre.org/wiki/Main_Page) or realistic "kill chain" been selected to frame the exercise?
- Is your goal to simulate an incident in a heavily mitigated risk, or a risk with much less telemetry / preventative measures?
- During each phase, what is the "break glass"? How do you announce widely what the truth is, and what needs to happen next, in case a red team goes awry and causes an outage?
- Under what circumstances do you want to "call off" the red team?
  - Consider when it is naturally complete, outside interference requires a shut down, or when the experience is no longer valuable for participants.

### :wrench: Attack Design
An attack represents the risks you're trying to mitigate, the incident you're trying to handle, or the individuals you're hoping to include on the response. These decisions all have planning burdens that are helpful to identify as early as possible.
- Does the attack actually need a lot of expertise and effort, or can you have simple recreations of an attack to discover? Are external parties even necessary?
- Where should the attack begin in the kill chain? (IE, early: spear phishing, or late: lateral movement with domain admin)
- What credentials / physical access / documentation are required to support the initiation of the attack? Who will provide them? Are there security implications that need to be followed up on later?
- If the red team succeeds early, should they begin penetration testing or vulnerability assessment? Should they try to be caught?
- Should the attacker impersonate a specific adversary, or attack method?
- If the red team is detected, will there be a backup plan or second attack? Will the red team resort to a penetration test?
- Where and how will the red team be documenting their behaviors? These need to be captured for any follow up tabletop and to confirm remediation and lesson learned. Can you collect a bash history? A TCP dump? Manual notes?
- Are the Red Team's methods going to be based in reality? Are they using methods that are not available to a realistic attacker?

### :rotating_light: Incident Response
If you can foresee how mature your response process will be, you can manipulate the response for greater benefit. An immature response team can be heavily guided by the Game Master, or a mature response team can be left alone to identify friction points in coordination and communication.
- Is there a specific coordination method or plan that incident response should follow? For instance, the agenda and method described in [Security Breach 101](https://medium.com/starting-up-security/security-breach-101-b0f7897c027c) or [An Incident Response Plan for Startups](https://github.com/magoo/Incident-Response-Plan/blob/master/EXAMPLE.md)
- Will Incident Response need to come together naturally, so you can to weed out friction in its process?
- Will Incident Response come together artificially to force the intended response as practice?
- Will you want to escalate the incident artificially so you can control the Incident Response?
- Who will bridge communications with the Red Team, if there are honest questions from the Blue Team? (For example: "We think we found a separate breach")
- Who will document the Red Team's pain points as the Blue Team mitigates? ("You kept removing our beacons and it was hard to get back, we didn't expect you'd find them all at once!")
- If Incident Response is not progressing in a timely manner, who or how will indicators be leaked to the Blue Team?
  - Will this be done in a tabletop format?
- Are short term mitigations / long term preventative measures being collected as part of your incident response?

### :mag: Red Team Reveal
The Blue Team will have all kinds of questions for the red team. This can be a moment of excitement if done correctly. Keeping this relationship healthy is critical. The red team should be viewed as an invaluable sparring partner. Better yet, a rabbit to chase.
- Are the Red Team's actions during the attack phase very well documented and understood?
- Has the incident response process missed any substantial Red Team actions?
- Are there any IOC's or artifacts that are still beaconing or discoverable in the future?
- Have any backdoors or other at risk changes survived incident response?
- How thorough was the Blue Team's investigation and containment?

### :skull: Post Mortem
A high quality post mortem will inform months of roadmap'd security work, and calibrate everyone on a mission through a shared experience.
- Has a thorough interviewing process or debrief happened with all participants in the exercise?
- Have all follow up mitigation items been collected centrally and prioritized based on the value sentiment of the participants?
- Are these sentiments being concluded and presented back to the participants?
- Do you have a meeting blocked to present them?
- Who is presenting them?
- Is the Red Team available to comment on these sentiments, or available to answer questions?
- Are participants being rewarded for participating?
- Are they given plenty of time to debrief and discuss?
- Is this a valuable calibration towards practical risks?

## :baby: Small Exercises
You can keep an exercise small and with minimal involvement of others. Be creative.

Simply have a team member simulate an incident that you think you could successfully respond to. For instance, you can install a piece of software that has auto-update functionality, and pretend it is malware. Then you'd "hunt" for the "C&C" which would just be its update beacon. For instance, can you prove that it is isolated to this host, and not others?

Or, have a team member make an "unauthorized change", and pull together an incident timeline that documents the event and what follow ups would matter.

Just be sure to document your findings, your lessons, and your follow ups to present to others. Red teams are not valuable if their lessons are isolated, and they don't need to be complicated.
