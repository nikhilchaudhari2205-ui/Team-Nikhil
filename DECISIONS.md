# Architectural & Design Decisions

### Decision Point 1: Client-Side State Management via LocalStorage
We selected browser LocalStorage paired with vanilla JavaScript instead of a remote database. This decision eliminates setup latency, guarantees instant reads and writes for gig listings and client bookings, and ensures evaluators can immediately test the full workflow without database provisioning or credentials.

### Decision Point 2: Dual Role Toggle Instead of Traditional Authentication
We implemented a dynamic role switcher ('Client' vs 'Creator') directly in the global navigation bar. This decision strictly aligns with the hackathon policy prohibiting login barriers, allowing graders to test both buyer commissions and creator studio dashboards seamlessly without sign-up friction.

### Decision Point 3: Single-Page Architecture with Pure Tailwind CSS CDN
We chose a unified single-page HTML architecture utilizing the Tailwind CSS and Lucide icon CDNs. This removes complex build and bundler dependencies, enabling zero-config deployment to Vercel and instant browser rendering on any device.
