# Meeting

It is a process for organizing and conducting meetings effectively, ensuring clear communication, documentation, and follow-up actions.

## Workflow Process

```mermaid
stateDiagram-v2
  s1: 👩‍💼<br/>**Preparation**<br/>The Meeting Moderator organizes relevant participants and communicates the meeting agenda in sequence.
  s2: 👩‍💼👨‍👩‍👧‍👦<br/>**Minute of Meeting**<br/>Conduct the meeting by following the agenda. The Meeting Moderator manages time control and ensures key points are recorded.
  s3: 👩‍💼<br/>**Summary**<br/>The Meeting Moderator summarizes discussion points for acknowledgment by participants and sets the next meeting (if any).
  s4: 👩‍💼<br/>**Distribute Notes**<br/>The summary is shared in the Telegram group “TheS Meeting” and a new event is created in Google Calendar (if any).

  [*] --> s1: At scheduled time
  s1 --> s2
  s2 --> s3
  s3 --> s4
  s4 --> [*]

  note right of s2:
    **NOTE:** If some topics remain unaddressed or key participants cannot attend, the Meeting Moderator should reschedule a new meeting time and skip those topics for now.
  end note
```

## Relevant Roles

| Role               | Description                                                                 | Duties                                                                                                    |
|--------------------|-----------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
| 👩‍💼 Meeting Moderator  | Person responsible for organizing and controlling the meeting.              | Set topics, invite participants, moderate the session, summarize outcomes, schedule the next meeting.     |
| 👨‍👩‍👧‍👦 Participants       | Individuals related to the meeting topics or invited to join the meeting. | Prepare in advance, review documents, draft questions or suggestions, contribute to actionable outcomes.  |

### Meeting Moderator Assignment
คนที่ทำหน้าที่เป็น Meeting Moderator ในแต่ละกระประชุมจะแตกต่างกันออกไป ขึ้นอยู่กับว่าเป็นประชุมอะไร เช่น

| NO | Meeting Type        | Meeting Moderator        |
|----|---------------------|--------------------------|
| 1  | Team Meeting        | Team Leader              |
| 2  | Cross-team Meeting  | Monthly Assigned Person  |
| 3  | Team Leader Meeting | Weekly Assigned Leader   |

## Base KPIs

| NO | KPI                     | Description                                                     | Target |
|----|-------------------------|-----------------------------------------------------------------|--------|
| 1 | Punctuality   | Meetings start and end on the scheduled time                    | 90%    |
| 2 | Attendance Rate | Percentage of participants attending the meeting                | 90%    |
| 3 | Notes Delivery  | Meeting Moderator delivers meeting notes within 24 hours after the session         | 100%   |