# Fact source per control axis

**The pattern:** When an assessment scores risk along several axes, each axis is paired with one explicit, human-legible fact source that answers it.

| Control axis | Example fact source |
|---|---|
| Vendor posture | A completed security questionnaire |
| Internal control | Access telemetry, such as who holds which permissions and when they last used them |

**Why it matters:** An axis with no named fact source invites the agent, or the analyst, to fill the gap with judgment presented as evidence. Naming the source makes the gap visible, and it combines naturally with the [human-legible source](human-legible-source.md) pattern.

**Second application: a funnel.** The [Source-to-Start Reconciliation](../19_SourceToStart/) recipe treats each funnel stage as an axis and names its source of record:

| Stage | Fact source |
|---|---|
| Spend | Billing: ad platform and vendor invoices |
| Inquiry, application | The admissions CRM |
| Start | The registrar's census file |
| Channel of record | The CRM source code, read through a crosswalk both offices agree on |

When two sources answer the same axis, the pattern doesn't pick one quietly: it names one as the record and uses the other as a witness. There, platform counts witness the CRM's inquiries, and the gap between them is the tracking audit.

**Third application: internal control itself.** The [RCU Access Review](../test-kitchen/rcu-access-review/) demo answers the axis the pattern started with:

| Question | Fact source |
|---|---|
| Who should have access | The HR record: job, office, status, earlier jobs |
| Who does have access | The SIS security user list, with last sign-in |
| Why access falls outside a job | The access-request log: reason, approver, end date |
| What each job should hold | Nobody keeps it. The page proposes a first draft from the access people share. |

The HR record is the record and the security user list is what gets fixed. A question with no fact source is named as a gap, not filled with judgment.

*Status: draft, identified in governance-and-risk work and stated here in general form. Applied in recipe 19 and the Access Review demo.*
