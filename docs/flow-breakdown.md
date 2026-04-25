# Flow Breakdown

## Flow 1: Candidate Intake

Trigger:

- New response submitted in Microsoft Forms

Actions:

- Get response details
- Create item in SharePoint List
- Store candidate submission metadata
- Start downstream automations

Purpose:

- Convert unstructured form submission into a trackable internal record

## Flow 2: HTML Snapshot Archiving

Trigger:

- New SharePoint list item created

Actions:

- Generate HTML representation of the submission
- Save the file in SharePoint

Purpose:

- Preserve a readable version of the application for review or audit

## Flow 3: Security Review Task Creation

Trigger:

- New application record created

Actions:

- Calculate due date
- Create Planner task for security team
- Populate task details with candidate information
- Post message to Teams

Purpose:

- Route candidate screening to the responsible team without manual handoff

## Flow 4: Completion-Based Notification

Trigger:

- Planner task completed

Actions:

- Read outcome from task details or process convention
- Notify HR in Teams
- Notify HR by email

Purpose:

- Close the loop between security review and HR action

## Flow 5: Offer Preparation

Trigger:

- Candidate approved by security and ready for next hiring step

Actions:

- Load offer template
- Populate predefined fields
- Leave only minimal editable inputs for HR

Purpose:

- Reduce repetitive document preparation work

## Flow 6: E-Signature Delivery

Trigger:

- Offer finalized by HR

Actions:

- Send document to candidate using Adobe Sign
- Track signature process

Purpose:

- Speed up offer acceptance and reduce manual document handling

## Reporting Layer

Planner data supports metrics such as:

- Number of closed tasks per person
- Average completion time
- Backlog size
- SLA adherence
- Team throughput trends

In a public portfolio, these metrics can be described conceptually without exposing production dashboards.
