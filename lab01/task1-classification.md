# Task 1: Project, Operation, or Programme?

| #  | Initiative | Temporary? | Unique? | Coordinated? | Class | Justification |
|----|------------|------------|---------|--------------|-------|---------------|
| 1  | Build the Realtime Quiz platform and pilot it with 50 students in week 14 | Yes | Yes | Yes | Programme | The platform launch combines several related initiatives (platform build, LMS integration, grade export) that only deliver value together.
| 2  | Run the nightly backup of the gicitc.com PostgreSQL database | No | No | No | Operation | Repeating nightly backups are ongoing maintenance to keep the service running.
| 3  | Move the department's three web servers to a new Linode region before 15 December | Yes | Yes | No | Project | A one‑off migration with a fixed deadline produces a new state that did not exist before.
| 4  | Answer helpdesk tickets within the 4-hour service level | No | No | No | Operation | Ticket handling is a continuous support activity without a defined end.
| 5  | "Digital classroom": Realtime Quiz, LMS upgrade and lecture capture sharing one login and one grade export | Yes | Yes | Yes | Programme | Multiple coordinated deliverables (quiz, LMS, capture) depend on each other to create the classroom solution.
| 6  | Apply the monthly security patches to the VPS | No | No | No | Operation | Ongoing security patching is routine maintenance.
| 7  | Add multi-node scaling (RabbitMQ relay, Redis registry) to Realtime Quiz next semester | Yes | Yes | No | Project | A one‑time scaling effort creates a new capability for the platform.
| 8  | Operate the Realtime Quiz platform after go-live: password resets, restarts, monitoring | No | No | No | Operation | Day‑to‑day operational tasks keep the platform available after launch.
| 9  | Write and publish the department's annual IT report for the dean by 31 January | Yes | Yes | No | Project | Each annual report is a unique deliverable with a fixed deadline.
| 10 | Replace 40 wireless access points in two buildings during the summer break | Yes | Yes | No | Project | The installation is a one‑off deployment with a set timeframe.

## Grey zones
- **Row 7 – Multi-node scaling**: Could be seen as a **Project** (new capability) or an **Operation** (ongoing capacity improvement). Additional information about whether the scaling is funded as a separate initiative would settle it.
- **Row 9 – Annual IT report**: Might be classified as a **Project** (annual unique deliverable) or an **Operation** (repeating yearly activity). Knowing if the report is part of a continuous reporting process or a one‑off strategic review would resolve the ambiguity.

## What our project hands over
1. After week 14 the **operations team** will take charge of routine platform maintenance (password resets, service restarts, and health monitoring).
2. They will also manage **incident response** for any downtime or performance issues that arise during live sessions.
3. Finally, the team will handle **regular updates** and minor enhancements, ensuring the platform remains compliant with security patches and university policies.
