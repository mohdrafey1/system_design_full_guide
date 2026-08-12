# Contents and Chapter Numbering

This is the authoritative chapter map for the book. Every cross-reference from Chapter 3 onward uses these numbers. Total: 118 chapters across 9 parts.

**Revision note.** The original plan listed 194 chapters. Many of those were sub-topics of a single idea rather than chapters in their own right: Token Bucket, Leaky Bucket, and Sliding Window are three algorithms inside one rate-limiting chapter, not three chapters. TinyURL and Bitly are the same design as URL Shortener with different constraints. Splitting them produced chapters that could not follow the twenty-section structure honestly, because sections like "Trade-offs" and "Failure Handling" only become meaningful when the alternatives sit side by side.

The map below merges those. Chapters 1 to 61 keep their original numbers, so every cross-reference written in Chapters 1 to 33 up to number 61 remains correct. Numbering diverges from 62 onward. The errata section at the end maps every affected reference.

## Conventions used throughout

- No em dashes or en dashes anywhere in the text.
- Headings use `#` for chapter, `##` for section, `###` for subsection, so Google Docs maps them to Heading 1, 2, and 3 on paste.
- Every diagram appears as Mermaid, with an ASCII version alongside it when the diagram carries load, because Mermaid does not render inside Google Docs.
- Every chapter follows the same 20 numbered sections.
- Code examples are Java and Spring Boot unless the topic demands otherwise (SQL, Redis commands, JSON, YAML).
- Terminology is fixed on first use in Chapter 1 (client, instance, service, request path, state, stateless, SPOF, fan-out) and reused without redefinition.

## Part 1: System Design Fundamentals (Chapters 1 to 74)

| Ch | Title | Ch | Title |
|---|---|---|---|
| 1 | What Is System Design? | 38 | NoSQL |
| 2 | High Level Design (HLD) | 39 | Database Indexing |
| 3 | Low Level Design (LLD) | 40 | Query Optimization |
| 4 | HLD vs LLD | 41 | Replication |
| 5 | Functional Requirements | 42 | Sharding |
| 6 | Non-Functional Requirements | 43 | Partitioning |
| 7 | Latency | 44 | Leader-Follower Replication |
| 8 | Throughput | 45 | Multi-Leader Replication |
| 9 | Scalability | 46 | Leaderless Databases |
| 10 | Availability | 47 | Read Replicas |
| 11 | Reliability | 48 | Database Failover |
| 12 | Durability | 49 | Bloom Filters |
| 13 | Fault Tolerance | 50 | Consistent Hashing |
| 14 | CAP Theorem | 51 | Distributed Locks |
| 15 | PACELC | 52 | Distributed Transactions |
| 16 | ACID | 53 | Kafka |
| 17 | BASE | 54 | RabbitMQ |
| 18 | Eventual Consistency | 55 | Pub/Sub |
| 19 | Strong Consistency | 56 | Event Driven Architecture |
| 20 | Idempotency | 57 | CQRS |
| 21 | Horizontal Scaling | 58 | Event Sourcing |
| 22 | Vertical Scaling | 59 | Saga Pattern |
| 23 | Stateless Services | 60 | Circuit Breaker |
| 24 | Stateful Services | 61 | Retry Patterns |
| 25 | Monolith | 62 | Rate Limiting |
| 26 | Microservices | 63 | Service Discovery |
| 27 | Service Mesh | 64 | Observability |
| 28 | API Gateway | 65 | Distributed Tracing |
| 29 | Reverse Proxy | 66 | Authentication and Authorization |
| 30 | Load Balancer | 67 | OAuth2 and JWT |
| 31 | DNS | 68 | Transport Security and Encryption |
| 32 | CDN | 69 | REST |
| 33 | Caching | 70 | gRPC |
| 34 | Cache Invalidation | 71 | GraphQL |
| 35 | Redis | 72 | The HTTP Protocol Family |
| 36 | Memcached | 73 | WebSockets |
| 37 | SQL | 74 | Server Sent Events |

**Merges applied in Part 1**

| New chapter | Absorbs the original chapters | Why |
|---|---|---|
| 62 Rate Limiting | 62 Rate Limiting, 63 Token Bucket, 64 Leaky Bucket, 65 Sliding Window | The four algorithms only make sense compared against each other. Chapter 62 covers all four plus distributed enforcement. |
| 64 Observability | 67 Monitoring, 68 Logging, 69 Metrics | Logs, metrics, and traces are three signals of one discipline. Split apart, each chapter repeats the same instrumentation and cardinality material. |
| 66 Authentication and Authorization | 71 Authentication, 72 Authorization, 75 API Keys | Who you are and what you may do are one request-path decision. API keys are a credential type, covered here. |
| 67 OAuth2 and JWT | 73 OAuth2, 74 JWT | JWT is the token format OAuth2 hands you. Explaining either alone forces forward references in both directions. |
| 68 Transport Security and Encryption | 76 HTTPS, 77 Encryption | HTTPS is TLS applied to HTTP. One chapter covers the primitives, then the protocol that uses them. |
| 72 The HTTP Protocol Family | 81 HTTP/1, 82 HTTP/2, 83 HTTP/3 | The versions are one evolutionary story: head-of-line blocking solved twice, at two layers. |

Chapter 70 Distributed Tracing keeps a chapter of its own despite being an observability signal, because propagation, sampling, and span design carry enough weight to stand alone. It is now Chapter 65.

## Part 2: Back of the Envelope Calculations (75 to 79)

| Ch | Title | Absorbs |
|---|---|---|
| 75 | Capacity Planning and Traffic Estimation | 86 Capacity Planning, 87 Traffic Estimation, 96 Growth Estimation |
| 76 | QPS and the Read Write Ratio | 88 QPS, 95 Read Write Ratio |
| 77 | Storage and Database Sizing | 89 Storage, 94 Database Size |
| 78 | Memory, Cache Sizing, and CPU | 90 Memory, 92 CPU, 93 Cache Size |
| 79 | Bandwidth | 91 Bandwidth |

Every chapter in this part is worked examples end to end, not formulas in isolation.

## Part 3: Low Level Design (80 to 96)

| Ch | Title | Absorbs |
|---|---|---|
| 80 | Object-Oriented Programming | 97 |
| 81 | SOLID Principles | 98 |
| 82 | Creational Patterns: Singleton, Factory, Builder | 99, 100, 101 |
| 83 | Behavioural Patterns: Observer, Strategy | 102, 103 |
| 84 | Structural Patterns: Decorator, Adapter, Facade, Proxy | 104, 105, 106, 107 |
| 85 | Repository and Dependency Injection | 108, 109 |
| 86 | UML for Engineers: Class, Sequence, and ER Diagrams | 110, 111, 112 |

LLD case studies, one chapter each, unchanged in scope:

| Ch | Case study | Ch | Case study |
|---|---|---|---|
| 87 | Parking Lot | 92 | Chess |
| 88 | ATM | 93 | Snake Game |
| 89 | Hotel Booking | 94 | Elevator |
| 90 | Library Management | 95 | Vending Machine |
| 91 | BookMyShow | 96 | Food Delivery |

## Part 4: System Design Interview Framework (97 to 101)

| Ch | Title | Absorbs |
|---|---|---|
| 97 | The Framework and Clarifying Requirements | 123 Clarify Requirements, 124 Estimate Scale |
| 98 | API and Database Design in an Interview | 125 Design APIs, 127 Database Design |
| 99 | High Level Design, Caching, and Scaling | 126, 128, 129 |
| 100 | Reliability, Failure Handling, and Security | 130, 131, 132 |
| 101 | Trade-offs and Future Improvements | 133, 134 |

The original twelve were the twelve steps of one method. As chapters they repeated the same worked example twelve times. As five, each covers a contiguous phase of a real forty-five minute interview.

## Part 5: Real World Case Studies (102 to 129)

| Ch | Case study | Absorbs / note |
|---|---|---|
| 102 | URL Shortener | 135 URL Shortener, 136 TinyURL, 137 Bitly. Same system. Bitly's analytics and custom domains appear as extensions. |
| 103 | WhatsApp | 138 |
| 104 | Instagram | 139 |
| 105 | News Feed: Facebook and Twitter Timeline | 140, 141. One fan-out problem, two answers. |
| 106 | YouTube | 142 |
| 107 | Netflix | 143 |
| 108 | Video Streaming Infrastructure | 162. The delivery layer under Chapters 106 and 107. |
| 109 | Google Drive and Dropbox | 144, 145. Same sync problem. |
| 110 | Distributed File Storage | 160 |
| 111 | Gmail | 146 |
| 112 | Slack | 147 |
| 113 | Reddit | 148 |
| 114 | Bluesky and Federated Social | 149 |
| 115 | Spotify | 150 |
| 116 | Airbnb | 151 |
| 117 | Uber and Ride Sharing | 152, 163. Same system. |
| 118 | Tinder | 153 |
| 119 | Amazon E-commerce | 154 |
| 120 | Search Engine | 155 |
| 121 | Payment Gateway and the Stripe Flow | 156, 157 |
| 122 | Notification Service | 158 |
| 123 | Distributed Cache | 159 |
| 124 | Ticket Booking | 161 |
| 125 | Online Multiplayer Game | 164 |
| 126 | Google Docs: Real-time Collaboration | 165 |
| 127 | Zoom | 166 |
| 128 | Apple AirTags | 167 |
| 129 | ChatGPT Architecture, Meta Serverless, Cloudflare PostgreSQL Scaling | 168, 169, 170. Three modern architectures, one chapter, each a self-contained study. |

## Part 6: Comparison Cheat Sheets (130 to 132)

The eleven planned comparison chapters were tables that belong beside the topics they compare, and every one of them already appears inside its own chapter's Trade-offs section. What remains here is the consolidated reference.

| Ch | Title | Covers |
|---|---|---|
| 130 | Data Layer Comparisons | SQL vs NoSQL, Redis vs Memcached, Strong vs Eventual Consistency, Leader-Follower vs Leaderless Replication |
| 131 | Communication Comparisons | REST vs GraphQL, REST vs gRPC, HTTP vs WebSockets, WebSockets vs SSE, Kafka vs RabbitMQ |
| 132 | Architecture Comparisons | Monolith vs Microservices, Horizontal vs Vertical Scaling, plus the decision trees for choosing between them |

## Part 7: Visual Learning (133)

133 Diagram Catalogue: architecture, component, sequence, data flow, network, and request lifecycle diagrams, with the Mermaid source for every major topic in the book.

## Part 8: Practice (134 to 137)

134 One Hundred Beginner Questions · 135 One Hundred Intermediate Questions · 136 One Hundred Advanced Questions · 137 One Hundred FAANG-style Interview Questions

## Part 9: Revision (138 to 145)

138 Quick Revision Notes · 139 Interview Cheat Sheets · 140 Important Formulas · 141 Architecture Checklist · 142 Technology Selection Guide · 143 Common Interview Mistakes · 144 Glossary · 145 Ninety-Day Learning Roadmap

## Errata: cross-references in Chapters 1 to 33

Two rounds of correction apply. Chapters 1 and 2 were written before any map existed. Chapters 3 to 33 match the original map exactly, so only their references to Chapter 62 and above have moved.

### Round 1: Chapters 1 and 2, written before the map

**Chapter 1**

| Written as | Should be | Topic |
|---|---|---|
| Chapter 21 | Chapter 23 | Stateless Services |
| Chapter 27 | Chapter 31 | DNS |
| Chapters 76 and 79 | Chapters 68 and 72 | HTTPS and HTTP/2 |
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
| Chapter 108 (Netflix) | Chapter 107 | Netflix case study |

**Chapter 2**

| Written as | Should be | Topic |
|---|---|---|
| Chapter 83 onward | Chapter 75 onward | Capacity Planning and estimation |
| Chapter 47 | Chapter 53 | Kafka |
| Chapter 114 | Chapter 105 | Twitter Timeline |
| Chapter 108 (all three mentions) | Chapter 102 | URL Shortener |
| Chapter 3, Chapter 20, Chapter 1 | unchanged | already correct |

### Round 2: the merge. Applies to every chapter, 1 to 33

References to Chapters 1 to 61 are unaffected. References at 62 and above move as follows.

| Written as | Now | Topic |
|---|---|---|
| 62, 63, 64, 65 | 62 | Rate Limiting and its four algorithms |
| 66 | 63 | Service Discovery |
| 67, 68, 69 | 64 | Monitoring, Logging, Metrics, now Observability |
| 70 | 65 | Distributed Tracing |
| 71, 72, 75 | 66 | Authentication, Authorization, API Keys |
| 73, 74 | 67 | OAuth2 and JWT |
| 76, 77 | 68 | HTTPS and Encryption |
| 78 | 69 | REST |
| 79 | 70 | gRPC |
| 80 | 71 | GraphQL |
| 81, 82, 83 | 72 | HTTP/1, HTTP/2, HTTP/3 |
| 84 | 73 | WebSockets |
| 85 | 74 | Server Sent Events |
| 86 to 96 | 75 to 79 | Back of the envelope, see Part 2 table |
| 97 | 80 | Object-Oriented Programming |
| 98 | 81 | SOLID Principles |
| 99, 100, 101 | 82 | Creational patterns |
| 102, 103 | 83 | Behavioural patterns |
| 104 to 107 | 84 | Structural patterns |
| 108, 109 | 85 | Repository and Dependency Injection |
| 110, 111, 112 | 86 | UML diagrams |
| 113 to 122 | 87 to 96 | LLD case studies, subtract 26 |
| 123 to 134 | 97 to 101 | Interview framework, see Part 4 table |
| 135, 136, 137 | 102 | URL Shortener |
| 138 | 103 | WhatsApp |
| 140, 141 | 105 | News Feed and Twitter Timeline |
| 143 | 107 | Netflix |
| 159 | 123 | Distributed Cache |
| 160 | 110 | Distributed File Storage |
| 162 | 108 | Video Streaming |
| 163 | 117 | Ride Sharing, now inside Uber |
| 165 | 126 | Google Docs |
| 171 to 181 | 130 to 132 | Comparison cheat sheets |

**The specific stale references present in the existing text of Chapters 1 to 33**, listed so they can be found and fixed:

| File | Written as | Should be |
|---|---|---|
| Chapter 1 | Chapter 108 (Netflix) | Chapter 107 |
| Chapter 2 | Chapter 83 onward, 114, 108 | 75 onward, 105, 102 |
| Chapters 3 to 33 | Chapter 67 (Monitoring) | Chapter 64 |
| Chapters 3 to 33 | Chapter 69 (Metrics) | Chapter 64 |
| Chapters 3 to 33 | Chapter 70 (Tracing) | Chapter 65 |
| Chapters 3 to 33 | Chapter 72 (Authorization) | Chapter 66 |
| Chapters 3 to 33 | Chapter 79 (gRPC) | Chapter 70 |
| Chapters 3 to 33 | Chapter 83 (HTTP/3) | Chapter 72 |
| Chapters 3 to 33 | Chapter 84 (WebSockets) | Chapter 73 |
| Chapters 3 to 33 | Chapter 92 (CPU) | Chapter 78 |
| Chapters 3 to 33 | Chapter 97 (OOP) | Chapter 80 |
| Chapters 3 to 33 | Chapter 98 (SOLID) | Chapter 81 |
| Chapters 3 to 33 | Chapter 100 (Factory) | Chapter 82 |
| Chapters 3 to 33 | Chapter 103 (Strategy) | Chapter 83 |
| Chapters 3 to 33 | Chapter 104 (Decorator) | Chapter 84 |
| Chapters 3 to 33 | Chapters 108, 109 (Repository, DI) | Chapter 85 |
| Chapters 3 to 33 | Chapters 110, 111, 112 (UML) | Chapter 86 |
| Chapters 3 to 33 | Chapter 134 (Future Improvements) | Chapter 101 |
| Chapters 3 to 33 | Chapter 138 (WhatsApp) | Chapter 103 |
| Chapters 3 to 33 | Chapter 141 (Twitter) | Chapter 105 |
| Chapters 3 to 33 | Chapter 159 (Distributed Cache) | Chapter 123 |
| Chapters 3 to 33 | Chapter 160 (File Storage) | Chapter 110 |
| Chapters 3 to 33 | Chapter 165 (Google Docs) | Chapter 126 |
| Chapters 3 to 33 | Chapter 173 (Kafka vs RabbitMQ) | Chapter 131 |
