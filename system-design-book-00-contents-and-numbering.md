# Contents and Chapter Numbering

This is the authoritative chapter map for the book. Every cross-reference from Chapter 3 onward uses these numbers. Total: 194 chapters across 9 parts.

## Conventions used throughout

- No em dashes or en dashes anywhere in the text.
- Headings use `#` for chapter, `##` for section, `###` for subsection, so Google Docs maps them to Heading 1, 2, and 3 on paste.
- Every diagram appears as Mermaid, with an ASCII version alongside it when the diagram carries load, because Mermaid does not render inside Google Docs.
- Every chapter follows the same 20 numbered sections.
- Code examples are Java and Spring Boot unless the topic demands otherwise (SQL, Redis commands, JSON, YAML).
- Terminology is fixed on first use in Chapter 1 (client, instance, service, request path, state, stateless, SPOF, fan-out) and reused without redefinition.

## Part 1: System Design Fundamentals (Chapters 1 to 85)

| Ch | Title | Ch | Title |
|---|---|---|---|
| 1 | What Is System Design? | 44 | Leader-Follower Replication |
| 2 | High Level Design (HLD) | 45 | Multi-Leader Replication |
| 3 | Low Level Design (LLD) | 46 | Leaderless Databases |
| 4 | HLD vs LLD | 47 | Read Replicas |
| 5 | Functional Requirements | 48 | Database Failover |
| 6 | Non-Functional Requirements | 49 | Bloom Filters |
| 7 | Latency | 50 | Consistent Hashing |
| 8 | Throughput | 51 | Distributed Locks |
| 9 | Scalability | 52 | Distributed Transactions |
| 10 | Availability | 53 | Kafka |
| 11 | Reliability | 54 | RabbitMQ |
| 12 | Durability | 55 | Pub/Sub |
| 13 | Fault Tolerance | 56 | Event Driven Architecture |
| 14 | CAP Theorem | 57 | CQRS |
| 15 | PACELC | 58 | Event Sourcing |
| 16 | ACID | 59 | Saga Pattern |
| 17 | BASE | 60 | Circuit Breaker |
| 18 | Eventual Consistency | 61 | Retry Patterns |
| 19 | Strong Consistency | 62 | Rate Limiting |
| 20 | Idempotency | 63 | Token Bucket |
| 21 | Horizontal Scaling | 64 | Leaky Bucket |
| 22 | Vertical Scaling | 65 | Sliding Window |
| 23 | Stateless Services | 66 | Service Discovery |
| 24 | Stateful Services | 67 | Monitoring |
| 25 | Monolith | 68 | Logging |
| 26 | Microservices | 69 | Metrics |
| 27 | Service Mesh | 70 | Distributed Tracing |
| 28 | API Gateway | 71 | Authentication |
| 29 | Reverse Proxy | 72 | Authorization |
| 30 | Load Balancer | 73 | OAuth2 |
| 31 | DNS | 74 | JWT |
| 32 | CDN | 75 | API Keys |
| 33 | Caching | 76 | HTTPS |
| 34 | Cache Invalidation | 77 | Encryption |
| 35 | Redis | 78 | REST |
| 36 | Memcached | 79 | gRPC |
| 37 | SQL | 80 | GraphQL |
| 38 | NoSQL | 81 | HTTP/1 |
| 39 | Database Indexing | 82 | HTTP/2 |
| 40 | Query Optimization | 83 | HTTP/3 |
| 41 | Replication | 84 | WebSockets |
| 42 | Sharding | 85 | Server Sent Events |
| 43 | Partitioning | | |

## Part 2: Back of the Envelope Calculations (86 to 96)

86 Capacity Planning · 87 Traffic Estimation · 88 QPS · 89 Storage · 90 Memory · 91 Bandwidth · 92 CPU · 93 Cache Size · 94 Database Size · 95 Read Write Ratio · 96 Growth Estimation

## Part 3: Low Level Design (97 to 122)

97 Object-Oriented Programming · 98 SOLID Principles · 99 Singleton · 100 Factory · 101 Builder · 102 Observer · 103 Strategy · 104 Decorator · 105 Adapter · 106 Facade · 107 Proxy · 108 Repository · 109 Dependency Injection · 110 Class Diagrams · 111 Sequence Diagrams · 112 Entity Relationships

LLD case studies: 113 Parking Lot · 114 ATM · 115 Hotel · 116 Library · 117 BookMyShow · 118 Chess · 119 Snake Game · 120 Elevator · 121 Vending Machine · 122 Food Delivery

## Part 4: System Design Interview Framework (123 to 134)

123 Clarify Requirements · 124 Estimate Scale · 125 Design APIs · 126 High Level Design · 127 Database Design · 128 Caching · 129 Scaling · 130 Reliability · 131 Failure Handling · 132 Security · 133 Trade-offs · 134 Future Improvements

## Part 5: Real World Case Studies (135 to 170)

135 URL Shortener · 136 TinyURL · 137 Bitly · 138 WhatsApp · 139 Instagram · 140 Facebook News Feed · 141 Twitter Timeline · 142 YouTube · 143 Netflix · 144 Google Drive · 145 Dropbox · 146 Gmail · 147 Slack · 148 Reddit · 149 Bluesky · 150 Spotify · 151 Airbnb · 152 Uber · 153 Tinder · 154 Amazon E-commerce · 155 Search Engine · 156 Payment Gateway · 157 Stripe Payment Flow · 158 Notification Service · 159 Distributed Cache · 160 Distributed File Storage · 161 Ticket Booking · 162 Video Streaming · 163 Ride Sharing · 164 Online Multiplayer Game · 165 Google Docs Real-time Collaboration · 166 Zoom · 167 Apple AirTags · 168 ChatGPT Architecture · 169 Meta Serverless · 170 Cloudflare PostgreSQL Scaling

## Part 6: Comparison Cheat Sheets (171 to 181)

171 SQL vs NoSQL · 172 Redis vs Memcached · 173 Kafka vs RabbitMQ · 174 REST vs GraphQL · 175 REST vs gRPC · 176 HTTP vs WebSockets · 177 WebSockets vs SSE · 178 Monolith vs Microservices · 179 Strong vs Eventual Consistency · 180 Leader-Follower vs Leaderless Replication · 181 Horizontal vs Vertical Scaling

## Part 7: Visual Learning (182)

182 Diagram Catalogue: architecture, component, sequence, data flow, network, and request lifecycle diagrams, with the Mermaid source for every major topic in the book.

## Part 8: Practice (183 to 186)

183 One Hundred Beginner Questions · 184 One Hundred Intermediate Questions · 185 One Hundred Advanced Questions · 186 One Hundred FAANG-style Interview Questions

## Part 9: Revision (187 to 194)

187 Quick Revision Notes · 188 Interview Cheat Sheets · 189 Important Formulas · 190 Architecture Checklist · 191 Technology Selection Guide · 192 Common Interview Mistakes · 193 Glossary · 194 Ninety-Day Learning Roadmap

## Errata: cross-references in Chapters 1 and 2

Chapters 1 and 2 were written before this map existed and their forward references drift. Corrections below. Everything from Chapter 3 onward matches the map.

### Chapter 1

| Written as | Should be | Topic |
|---|---|---|
| Chapter 21 | Chapter 23 | Stateless Services |
| Chapter 27 | Chapter 31 | DNS |
| Chapters 76 and 79 | Chapters 76 and 82 | HTTPS and HTTP/2 |
| Chapter 28 | Chapter 32 | CDN |
| Chapter 26 | Chapter 30 | Load Balancer |
| Chapters 24 and 61 | Chapters 28 and 62 | API Gateway and Rate Limiting |
| Chapters 29 to 31 | Chapters 33 to 35 | Caching, Cache Invalidation, Redis |
| Chapters 34 and 35 | Chapters 39 and 40 | Database Indexing and Query Optimization |
| Chapter 30 | Chapter 34 | Cache Invalidation |
| Chapter 35 (data model) | Chapter 39 | Database Indexing |
| Chapter 15 (CAP) | Chapter 14 | CAP Theorem |
| Chapters 56 and 20 | Chapters 61 and 20 | Retry Patterns and Idempotency |
| Chapter 55 | Chapter 60 | Circuit Breaker |
| Chapter 23 (monolith) | Chapters 25 and 26 | Monolith and Microservices |
| Chapter 108 (Netflix) | Chapter 143 | Netflix case study |

### Chapter 2

| Written as | Should be | Topic |
|---|---|---|
| Chapter 83 onward | Chapter 86 onward | Capacity Planning and estimation |
| Chapter 47 | Chapter 53 | Kafka |
| Chapter 114 | Chapter 141 | Twitter Timeline |
| Chapter 108 (all three mentions) | Chapter 135 | URL Shortener |
| Chapter 3, Chapter 20, Chapter 1 | unchanged | already correct |
