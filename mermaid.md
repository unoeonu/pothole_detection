```mermaid
flowchart TD
    A[Autonomous Vehicle Driving] --> B{Is the road damaged?}
    B -- No --> A
    B -- Yes --> C[Vehicle Stops]
    C --> D[Record Location on Raspberry Pi and Send Image to Server]
    C --> E[Change Direction]
    E --> F[Resume Driving]
    F --> A
