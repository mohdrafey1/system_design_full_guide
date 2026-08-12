# System Design: The Complete Guide

A full-length System Design book, written from first principles for engineers who know how to build a service but have never been taught how to design one.

Not a summary. Not an interview cheat sheet. Every chapter opens with a real production failure, explains why the failure was structural rather than accidental, and builds the concept from there.

**Current state: 37 chapters written of 118 planned.** See [Chapters written](#chapters-written) below.

## Who this is for

You will get the most from this if you:

- write Java and Spring Boot, or can read them
- know enough SQL to write a join and read an `EXPLAIN`
- have one to three years of engineering experience
- have never sat down and studied distributed systems properly

Nothing is assumed beyond that. Terminology is defined on first use in Chapter 1 and reused without redefinition afterward.

## How the book is organised

| Part | Chapters | What it covers |
|---|---|---|
| 1. Fundamentals | 1 to 74 | Requirements, the non-functional properties, consistency models, scaling, the network layer, data, messaging, resilience, observability, security, protocols |
| 2. Back of the Envelope | 75 to 79 | Capacity planning, QPS, storage, memory, bandwidth, worked end to end |
| 3. Low Level Design | 80 to 96 | OOP, SOLID, design patterns, UML, then ten case studies from Parking Lot to Food Delivery |
| 4. Interview Framework | 97 to 101 | A reusable method for a forty-five minute design interview |
| 5. Case Studies | 102 to 129 | URL Shortener, WhatsApp, Instagram, News Feed, YouTube, Netflix, Drive, Uber, Stripe, Google Docs, ChatGPT and more |
| 6. Comparison Cheat Sheets | 130 to 132 | The consolidated decision tables |
| 7. Visual Learning | 133 | Every diagram in the book, with Mermaid source |
| 8. Practice | 134 to 137 | 400 questions with worked explanations |
| 9. Revision | 138 to 145 | Cheat sheets, formulas, checklists, glossary, ninety-day roadmap |

The authoritative chapter map, including which original chapters were merged and why, is in [contents-and-numbering.md](contents-and-numbering.md).

## Every chapter has the same twenty sections

Consistent structure means you can read a chapter end to end, or jump straight to section 12 when you only need the trade-offs.

| # | Section | # | Section |
|---|---|---|---|
| 1 | Problem Statement | 11 | Limitations |
| 2 | Why This Problem Exists | 12 | Trade-offs |
| 3 | Real World Analogy | 13 | Common Mistakes |
| 4 | Simple Explanation | 14 | Interview Questions |
| 5 | Technical Deep Dive | 15 | Production Best Practices |
| 6 | Architecture Diagram | 16 | Summary |
| 7 | Request Flow | 17 | Quick Revision Notes |
| 8 | Internal Components | 18 | Mini Quiz |
| 9 | Production Example | 19 | Hands-on Exercise |
| 10 | Advantages | 20 | Further Reading |

Section 1 is always a specific failure with numbers attached, usually from the same running system, so the concepts accumulate rather than arriving as a list.

## How to read it

**Studying from scratch.** Chapters 1 to 20 in order, no skipping. They establish the vocabulary everything else uses. After that you can move around freely.

**Preparing for an interview in a hurry.** Part 4 first (the framework), then two or three case studies from Part 5, then Chapter 138 Quick Revision Notes. Do the section 19 exercises in the case studies. Reading a design and being able to produce one are different skills, and only the second one gets tested.

**Looking something up.** Every chapter is self-contained enough to read alone. Cross-references point to where a dependency is explained properly rather than repeating it.

**Reading on paper or in Google Docs.** Headings map to Heading 1, 2 and 3 on paste. Mermaid diagrams do not render in Google Docs, so every diagram that carries real weight has an ASCII version beside it.

## Conventions

- Chapter files are named `topic-name-ch-N.md`, one chapter per file, so the topic is visible in the filename.
- Mermaid for diagrams, with ASCII alongside where the diagram matters.
- Java and Spring Boot for code, except where the topic demands SQL, Redis commands, JSON, or YAML.
- No em dashes or en dashes anywhere, so the text pastes cleanly into any editor.
- Production examples are drawn from published engineering work by Netflix, Google, Amazon, Uber, Meta, Stripe, Cloudflare, Discord, Shopify and others, cited in section 20.

## Chapters written

**37 of 118.** All of Part 1 so far, taking the book from "what is system design" through requirements, the non-functional properties, consistency models, scaling, the network layer, the full caching tier, and into the relational database.

| # | Chapter | # | Chapter |
|---|---|---|---|
| 1 | [What Is System Design?](what-is-system-design-ch-1.md) | 20 | [Idempotency](idempotency-ch-20.md) |
| 2 | [High Level Design](high-level-design-ch-2.md) | 21 | [Horizontal Scaling](horizontal-scaling-ch-21.md) |
| 3 | [Low Level Design](low-level-design-ch-3.md) | 22 | [Vertical Scaling](vertical-scaling-ch-22.md) |
| 4 | [HLD vs LLD](hld-vs-lld-ch-4.md) | 23 | [Stateless Services](stateless-services-ch-23.md) |
| 5 | [Functional Requirements](functional-requirements-ch-5.md) | 24 | [Stateful Services](stateful-services-ch-24.md) |
| 6 | [Non-Functional Requirements](non-functional-requirements-ch-6.md) | 25 | [Monolith](monolith-ch-25.md) |
| 7 | [Latency](latency-ch-7.md) | 26 | [Microservices](microservices-ch-26.md) |
| 8 | [Throughput](throughput-ch-8.md) | 27 | [Service Mesh](service-mesh-ch-27.md) |
| 9 | [Scalability](scalability-ch-9.md) | 28 | [API Gateway](api-gateway-ch-28.md) |
| 10 | [Availability](availability-ch-10.md) | 29 | [Reverse Proxy](reverse-proxy-ch-29.md) |
| 11 | [Reliability](reliability-ch-11.md) | 30 | [Load Balancer](load-balancer-ch-30.md) |
| 12 | [Durability](durability-ch-12.md) | 31 | [DNS](dns-ch-31.md) |
| 13 | [Fault Tolerance](fault-tolerance-ch-13.md) | 32 | [CDN](cdn-ch-32.md) |
| 14 | [CAP Theorem](cap-theorem-ch-14.md) | 33 | [Caching](caching-ch-33.md) |
| 15 | [PACELC](pacelc-ch-15.md) | 34 | [Cache Invalidation](cache-invalidation-ch-34.md) |
| 16 | [ACID](acid-ch-16.md) | 35 | [Redis](redis-ch-35.md) |
| 17 | [BASE](base-ch-17.md) | 36 | [Memcached](memcached-ch-36.md) |
| 18 | [Eventual Consistency](eventual-consistency-ch-18.md) | 37 | [SQL](sql-ch-37.md) |
| 19 | [Strong Consistency](strong-consistency-ch-19.md) | | |

**Next: Chapter 38, NoSQL.**

### Why 118 chapters and not 194

The original outline had 194. Many of those entries were sub-topics rather than chapters: Token Bucket, Leaky Bucket and Sliding Window are three algorithms compared inside one rate-limiting chapter, and separating them makes the comparison impossible. TinyURL and Bitly are the same design as URL Shortener under different constraints. Monitoring, Logging and Metrics are three signals of one discipline, and split apart each chapter repeats the same instrumentation material.

Merging them produces chapters where section 12, Trade-offs, has something real to say, because the alternatives are on the same page. The full merge table and the cross-reference errata are in the contents file.

## A note on the writing

The book is written the way a senior engineer explains something to a teammate at a whiteboard: the problem first, then why the obvious fix does not work, then the mechanism, then what it costs you. Intuition before terminology, and why before how.

If a paragraph is not teaching something, it should not be there.
