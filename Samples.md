
🧭 Mermaid Chart Types Overview
1. Flowchart (processes, logic, workflows)
flowchart TD
    A[Start] --> B{Login?}
    B -->|Yes| C[Dashboard]
    B -->|No| D[Show Error]
    C --> E[Logout]
    D --> A


📌 Shapes:

[ ] rectangle

{ } diamond (decision)

(( )) circle

2. Sequence Diagram (interactions over time)
sequenceDiagram
    participant User
    participant App
    participant Server

    User->>App: Click Login
    App->>Server: Send credentials
    Server-->>App: Success
    App-->>User: Show dashboard


📌 Use for message flows between actors.

3. Class Diagram (object-oriented models)
classDiagram
    class Animal {
      +String name
      +int age
      +makeSound()
    }

    class Dog {
      +String breed
      +bark()
    }

    Animal <|-- Dog


📌 Use for UML-style modeling.

4. State Diagram (state machines, lifecycle)
stateDiagram-v2
    [*] --> Idle
    Idle --> Running : Start
    Running --> Paused : Pause
    Paused --> Running : Resume
    Running --> [*] : Stop


📌 Great for lifecycle and state transitions.

5. Gantt Chart (timelines & schedules)
gantt
    title Project Plan
    dateFormat  YYYY-MM-DD
    section Phase 1
    Task A :a1, 2025-08-01, 5d
    Task B :after a1, 3d
    section Phase 2
    Task C :2025-08-10, 4d


📌 Use for project management.

6. ER Diagram (Entity–Relationship for databases)
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE_ITEM : contains
    CUSTOMER {
        string name
        string email
    }
    ORDER {
        int id
        date orderDate
    }


📌 Good for database modeling.

7. Pie Chart (simple data visualization)
pie title Favorite Fruits
    "Apple" : 40
    "Banana" : 25
    "Orange" : 20
    "Other" : 15


📌 For quick percentage breakdowns.

8. Mindmap (brainstorming)
mindmap
  root((Mermaid))
    Flowcharts
    Sequence Diagrams
    Gantt Charts
    ER Diagrams
    Class Diagrams
    State Machines


📌 Visual idea organization.

9. Timeline (historical events, milestones)
timeline
    title Space Exploration
    1969 : Moon Landing
    1998 : ISS Launched
    2021 : James Webb Telescope
    2024 : Artemis Mission


📌 For chronological events.
