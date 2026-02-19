# Monolithic Architecture

## Definition

Monolithic architecture is a software design pattern where the entire application
(UI, business logic, database access) is built and deployed as a single unit.

Everything runs inside one codebase and one deployment artifact.

---

## Structure

All modules exist inside one application:

- User Module
- Order Module
- Payment Module
- Inventory Module
- Authentication
- Database access layer

Single Deployment → Single Server (or replicated same app)

---

## Real-World Example

Early-stage companies like Flipkart and Facebook initially started with monolithic systems.

---

## Advantages

1. Simple to build and understand
2. Easy local development
3. Easy debugging (single codebase)
4. Lower infrastructure complexity
5. Good for small teams and startups

---

## Disadvantages

1. Entire app must scale even if only one module needs scaling
2. Codebase becomes tightly coupled
3. Deployment risk (one bug can affect whole system)
4. Slower CI/CD as project grows
5. Hard to adopt new technologies for specific modules

---

## Scaling Strategy

Horizontal scaling:
Deploy multiple instances of the same application behind a load balancer.

But still:
All modules scale together → Resource wastage.

---

## When to Use

- Early-stage startup
- Small team
- Limited traffic
- Fast MVP requirement


