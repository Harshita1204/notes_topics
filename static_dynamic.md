# Static vs Dynamic Websites

---

# Static Website

## Definition

A static website serves pre-built HTML, CSS, and JS files directly 
to the browser.

Content does NOT change per user unless files are manually updated.

Server Role:
Only serves files. No runtime processing required.

---

## How It Works

Client → Request → Server → Returns same HTML file

No database interaction.
No server-side rendering logic.

---

## Examples

- Portfolio website
- Company landing page
- Documentation site

---

## Advantages

1. Very fast (no backend processing)
2. Highly secure (no server-side logic)
3. Cheap hosting (CDN friendly)
4. Easy to deploy
5. Excellent scalability

---

## Disadvantages

1. Hard to manage large content
2. No personalization
3. Manual updates required
4. No real-time data

---

## Hosting Architecture

- CDN (Content Delivery Network)
- Object storage (like S3)
- Static hosting platforms

---

# Dynamic Website

## Definition

A dynamic website generates content at runtime based on:

- User input
- Database data
- Business logic
- Authentication state

Server processes request before sending response.

---

## How It Works

Client → Request → Server → Business Logic → Database → Response

Content varies per user.

---

## Examples

- E-commerce website
- Social media platform
- Banking portal
- SaaS dashboard

---

## Advantages

1. Personalized content
2. Real-time data
3. Database integration
4. Scalable business logic
5. User authentication & sessions

---

## Disadvantages

1. Slower than static (processing required)
2. Requires backend infrastructure
3. More security risks
4. More complex scaling

---

# Static vs Dynamic Comparison

| Feature | Static Website | Dynamic Website |
|----------|----------------|----------------|
| Content | Fixed | Generated at runtime |
| Backend | Not required | Required |
| Speed | Very Fast | Moderate |
| Scalability | Extremely easy | Requires architecture |
| Personalization | No | Yes |
| Cost | Low | Higher |

---

# Modern Hybrid Approach (Important)

Modern frameworks combine both:

- Static Site Generation (SSG)
- Server-Side Rendering (SSR)
- Client-Side Rendering (CSR)
- Incremental Static Regeneration (ISR)

Example:
Static product page + Dynamic cart system

---

# Scalability Perspective (20 LPA Insight)

Static websites scale easily because:

- Served via CDN
- No database bottleneck
- No backend processing

Dynamic websites need:

- Load balancer
- Caching
- Database scaling
- Auto scaling

---

# SEO Perspective

Static:
- Excellent SEO (pre-rendered content)

Dynamic:
- Needs SSR or pre-rendering for SEO optimization

---

# When to Use What

Use Static When:
- Content rarely changes
- SEO priority
- High traffic landing page

Use Dynamic When:
- User accounts required
- Real-time data
- Complex business logic

---

# Interview-Level Insight

Modern large systems rarely use purely static or purely dynamic.

They use hybrid architecture:

- Static for performance-critical pages
- Dynamic APIs for personalized content

Understanding rendering strategy 
is more important than labeling website as static or dynamic.