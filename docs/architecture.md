# TeamUp — Architecture (Planned)

```mermaid
flowchart LR
  A[Client: React + React Flow] -- REST / WS --> B(API: FastAPI)
  B -- pub/sub --> C[Redis]
  B -- SQL --> D[(PostgreSQL)]
  B -- logs --> E[Monitoring (Grafana/CloudWatch)]
