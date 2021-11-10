# Incident Response Plan

This document offers guidance for employees or incident responders who
believe they have discovered or are responding to a security incident.

## Escalation

- Message #triage-bugs on Slack.

- Make sure the current exterminator is aware.

- Include as many specifics and details as you can.

## Severity

| **Severity level**     | **Description**                                                                                                                                    | **Examples**                                                                                                          | **Remediation**                                                                                              |
| :--------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| Low or Medium Severity | Most issues fall under this category. These do not require someone to be paged or woken up in the middle of the night.                             | Suspicious emails, outages, strange activity on a laptop                                                              | File a ticket in Shortcut for triage and notify the current exterminator.                        |
| High severity          | These are problems where an adversary or active exploitation hasn't been proven yet, and an attack may not have happened, but is likely to happen. | Backdoors, malware, malicious access of business data (e.g. passwords, payment information, vulnerability data, etc.) | Notify both the current exterminator and the CTO |
| Critical severity      | The attackers were successful, and something was lost.                                                                                             |                                                                                                                       |  Notify both the current exterminator and the CTO                                                        |

## Internal Issues

When the malicious actor is an employee, contractor, vendor, or partner,
please contact the CTO directly.
Do not discuss the issue with other employees.

## Compromised Communications

If there are IT communication risks (i.e. company phones, laptops, email
accounts, etc. are compromised) the team will announce an out-of-band
communication tool within the office.

## Response Steps

For critical issues, the response team will follow an iterative response
process designed to investigate, contain the exploitation, remediate the
vulnerability, and write post mortem and lessons learned documents.

1.  The CTO should determine if a
    lawyer should be involved with attorney-client privilege

2.  A private "War Room" Slack channel will be designated

3.  The following meeting will take place at regular intervals, starting
    with twice per day, until the incident is resolved

### Response Meeting -- Agenda

- Update the **Breach Timeline** with all known data related to the
  incident. The timeline should detail what you're sure the attacker
  did at what times.

- Review new **Indicators of Compromise** with the entire group.
  Indicators of Compromise are anything you know belongs to the
  attacker: an IP address that sent data, a compromised account, a
  malicious file used to spearphish, etc.

- Add new data (knowns and unknowns) to the **Investigative Q&A**,
  which is a list of questions to which, if you had answers, you'd
  understand everything the attacker did.

- Update the list of **Emergency Mitigations**: passwords to be reset,
  laptops to be wiped, IPs to be banned, etc.

- Long Term Mitigations (including Root Cause Analysis): record
  everything you'll start doing so this crisis doesn't happen again.

- Everything Else: communications, legal issues, blog posts, status
  pages, etc.

## Response Team Members

Nick Santos (nick@tilt.dev), CTO
L Körbes (l@tilt.dev), Head of Product

## Required Retrospective

All incidents classified as "High" or above require a retrospective meeting and a "lessons learned" document.

## Follow-ups must be completed

All incidents classified as "High" or above require follow-ups to be tasked in a task tracker and completed within a pre-defined time period.

## Disciplinary Action

Employees who violate this policy may face disciplinary consequences in
proportion to their violation. Windmill Engineering management will determine how
serious an employee's offense is and take the appropriate action.

## Responsibility

The CTO of Windmill Engineering is responsible for ensuring this policy is
followed.
