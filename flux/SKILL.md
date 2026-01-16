---
name: flux
description: Flux Capacitor Wiggum Loop - Continuous iteration and improvement for hours or days until time expires. Optimized for long-horizon tasks (1+ hours). Use when user specifies time duration or says /flux. Delivers relentless improvement until time runs out.
---

# FLUX CAPACITOR WIGGUM LOOP
## "Great Scott!" - Continuous Iteration Until Time Runs Out

### Core Philosophy

There is ALWAYS room for improvement. When you reach a "done" state, that's just the beginning. Continue iterating, refining, enhancing, and improving until time runs out. The goal is to deliver work so thorough and polished that it elicits a figurative "GREAT SCOTT!" reaction.

**FLUX is optimized for long-horizon tasks: 1+ hours, days, weeks.**

The longer the duration, the more dynamic and transformative the results.

---

## How FLUX Works

### Syntax

```bash
/flux <duration> - <task description>
```

### Time Formats

- **Duration**: "1 hour", "8 hours", "24 hours", "2 days", "1 week"
- **Absolute**: "5:30 PM", "2026-01-20 18:00"
- **T+ format**: "T+2h", "T+24h", "T+3d"

### The FLUX Process

1. **Parse time**: Calculate end time (e.g., 24 hours from now)
2. **Start work**: Begin the core task
3. **Reach "done"**: Complete initial requirements
4. **FLUX ACTIVATES**: Continue iterating until time expires
5. **Never stop early**: Keep improving until the last second

---

## CRITICAL: The FLUX Loop

### The Iron Law of FLUX

**IF TIME REMAINS, YOU ARE NOT DONE.**

When you complete the initial task:
- ✅ Task done at hour 2 of 24? → **20 hours of improvement remain**
- ✅ Feature complete at hour 6 of 24? → **18 hours of iteration remain**
- ✅ Tests passing at hour 12 of 24? → **12 hours of polish remain**

**NEVER STOP UNTIL TIME EXPIRES.**

### What to Do When "Done"

**CRITICAL**: Tasks often complete MUCH faster than expected. When the core task is complete but time remains, use ALL remaining time for:

1. **Test, Test, Re-Test** - Try every edge case, break it in new ways, stress test
2. **Refine the Product** - Polish what exists, improve quality, fix rough edges
3. **Think About New Use Cases** - What other problems could this solve?
4. **Add Features** - What would make this 10x more valuable?
5. **Think About Monetization** - How could this make money? What's the business model?
6. **Optimize** - Performance, efficiency, resource usage
7. **Harden** - Edge cases, error handling, validation
8. **Documentation** - Examples, guides, API docs

**DO NOT create hour-by-hour plans.** Work completes unpredictably. Focus on using EVERY REMAINING SECOND to improve what you built.

---

## Time Tracking (Silent Mode)

Check time between work chunks using bash, but **NEVER show timestamps to the user**:

```bash
# Silent time check (no echo, no output)
CURRENT=$(date +%s)
REMAINING=$((END_TIME - CURRENT))

# Just continue working based on REMAINING value
```

**The user should only see continuous work output, not time checks.**

---

## Iterative Generation Pattern

For content generation, code, or lists:

### The Pattern

```
1. Generate chunk (code, text, items, features)
2. Silent time check
3. Time remains? → Generate another chunk
4. Silent time check
5. Time remains? → Generate another chunk
6. Repeat until time expires
```

### Example

**Task: "Build a web application" with 24 hours**

```
Core work completes in 6 hours:
- Routing, pages, database, API, auth, basic UI

18 HOURS REMAIN → FLUX ACTIVATES:
- Test every endpoint, every edge case
- Refine UI/UX, add polish and animations
- Think: What features would delight users?
- Add real-time updates, notifications
- Test again with extreme inputs
- Think: How could this be monetized?
- Add analytics, admin dashboard
- Optimize performance, add caching
- Test on different devices/browsers
- Add documentation and examples
- Think: What other use cases?
- Add API versioning, rate limiting
- Continue until time expires...
```

**Work completes unpredictably fast. Use ALL remaining time to refine and enhance.**

---

## Optimal Durations

| Duration | Experience | Best For |
|----------|------------|----------|
| **< 1 hour** | Choppy iterations | Simple tasks only |
| **1-4 hours** | Noticeable chunks | Feature development |
| **8-12 hours** | Smooth progress | Full applications |
| **24+ hours** | Seamless flow | Complex systems |
| **2-7 days** | Epic results | Enterprise projects |

**Recommendation: Use FLUX for tasks requiring 1+ hours for best results.**

---

## Real-World Example: Task Management Web App

```bash
/flux 24 hours - build a complete task management web app with React and Node.js
```

### What Actually Happens

**Core requirements done in 4-6 hours:**
- Project structure, React app, Node server
- Task CRUD, database, API endpoints
- Basic authentication and UI

**FLUX MODE ACTIVATES - 18-20 hours remain:**

Now the real work begins. Don't follow a predetermined plan. Assess what would add the most value:

- Test everything: try to break authentication, test edge cases, invalid inputs
- Refine the UI: add animations, improve UX flows, make it feel premium
- Think: "What features would make this amazing?" → Add them
- Test more: different browsers, mobile, slow connections
- Think: "How could this make money?" → Add premium features, usage analytics
- Optimize: profile performance, add caching, lazy loading
- Test again: stress test with thousands of tasks
- Think: "What other use cases?" → Add team collaboration, integrations
- Harden: comprehensive error handling, input validation
- Document: API docs, user guide, developer setup
- Continue iterating until time expires

**Result: Not just a task app, but a production-ready SaaS product with business potential.**

---

## Real-World Example: Multi-Day System Refactor

```bash
/flux 3 days - refactor the legacy authentication system
```

### What Actually Happens

**Core refactor done in 12-18 hours:**
- Analyze existing system
- Refactor auth logic with modern patterns
- Migrate database, update API endpoints
- Basic tests passing

**FLUX MODE ACTIVATES - 54-60 hours remain:**

This is where FLUX shines. Massive time to make it exceptional:

- Test relentlessly: try to break it, penetration testing, edge cases
- Think: "What features would make this enterprise-ready?"
- Add OAuth, 2FA, SSO, magic links
- Test more: load testing, concurrent sessions, race conditions
- Think: "What would make this monetizable?"
- Add admin dashboard, usage analytics, audit logging
- Refine: improve error messages, better UX, clear documentation
- Think: "What future scenarios aren't covered?"
- Add rate limiting, bot detection, session management improvements
- Test again: security audit, vulnerability scanning
- Optimize: query performance, caching strategies, reduce latency
- Think: "How do we deploy this safely?"
- Add migration scripts, rollback procedures, deployment automation
- Document: architecture diagrams, API docs, runbooks, training materials
- Continue until 72 hours expire

**Result: A complete next-generation auth platform that becomes a competitive advantage.**

---

## Dynamic Improvement Categories

**CRITICAL**: These are EXAMPLES ONLY. Don't treat them as a checklist. Be creative. Think about THIS specific project and what would make it exceptional. What would genuinely create a "Great Scott!" reaction?

When iterating, consider categories like these, but identify your own valuable work:

### 1. Testing & Validation (Priority)
- Test every edge case
- Try to break it in new ways
- Stress testing and load testing
- Test on different environments
- Penetration testing
- Re-test after each change

### 2. Refinement & Polish
- Improve what exists
- Fix rough edges
- Better error messages
- Smoother UX flows
- Code organization
- Performance optimization

### 3. Business Thinking
- **How could this make money?**
- What's the monetization model?
- Premium features vs free tier
- Usage analytics and metrics
- Market differentiators

### 4. New Use Cases & Features
- What other problems could this solve?
- What features would make this 10x more valuable?
- What would delight users?
- Integrations and extensions
- Novel capabilities

### 5. Robustness
- Error handling
- Input validation
- Graceful degradation
- Retry logic
- Circuit breakers
- Failure scenarios

### 6. Security
- Authentication & authorization
- Encryption
- Input sanitization
- Vulnerability scanning
- Security headers
- Audit logging

### 7. Operations & Deployment
- Monitoring and alerting
- Deployment automation
- Backup strategies
- Disaster recovery
- Migration scripts
- Rollback procedures

### 8. Documentation
- API documentation
- User guides
- Architecture diagrams
- Setup instructions
- Example code
- Training materials

**Don't follow this list sequentially or treat it as comprehensive. These are just examples to spark ideas. The real question is: What would make THIS specific project exceptional? What would create genuine value? Be creative and find work that matters.**

---

## The FLUX Mindset

### What FLUX Is

- **Relentless iteration** until time runs out
- **Dynamic adaptation** based on current state
- **Exceeding expectations** through continuous improvement
- **Time as fuel** for excellence

### What FLUX Is Not

- ❌ A checklist to complete and stop
- ❌ Pre-planned work that ends early
- ❌ Minimum viable solutions
- ❌ "Good enough" work

### The Goal

Make the user say "Great Scott! I can't believe how much was accomplished!"

Even if they don't actually say it, that's the standard you're aiming for.

---

## Critical Rules

### NEVER STOP EARLY

If you complete your planned work and time remains:

1. **DO NOT** report completion and stop
2. **DO NOT** ask what to do next
3. **DO NOT** wait for instructions

**IMMEDIATELY** start the next improvement. Think creatively:
- What would make this 10x better?
- How could this make money?
- What edge cases would break this?
- What features would create genuine delight?
- What makes this different from competitors?
- How would this scale to 1M users?
- What would make someone say "Great Scott!"?

**Be creative. Don't just follow examples. Find valuable work that matters for THIS project.**

### Silent Time Checks

Use bash `date` command to check time, but:

- ✅ Store result in variable: `REMAINING=$((END - $(date +%s)))`
- ❌ Never echo timestamps: `echo "30s remaining"`
- ✅ Continue work silently
- ❌ Never announce time checks to user

The user should see **continuous work output only**, not timing infrastructure.

### Chunked Iteration

For long tasks, work in chunks:

1. Complete a unit of work (feature, module, section)
2. Silent time check
3. If time remains → Start next chunk immediately
4. Repeat

**Don't predetermine chunk sizes.** Work completes unpredictably. Just keep completing chunks and checking time until it expires.

### Dynamic, Not Predetermined

Don't create a rigid plan at the start and follow it mechanically.

**Instead:**
- Start with core task
- Complete it
- Assess current state
- Choose most valuable improvement
- Execute it
- Reassess
- Choose next improvement
- Continue dynamically until time expires

**The path emerges through iteration, not predetermined planning.**

---

## Real-World Example: Content Generation

```bash
/flux 6 hours - write a comprehensive guide to Kubernetes
```

### What Actually Happens

**Basic guide done in 45 minutes:**
- Introduction, core concepts, basic architecture

**FLUX MODE ACTIVATES - 5+ hours remain:**

Don't stop at "comprehensive." Keep iterating:

- Test: read through, find gaps, unclear sections
- Refine: rewrite confusing parts, improve flow, better examples
- Think: "What would make this exceptional?"
- Add hands-on tutorials, code examples, diagrams
- Test: have someone else read it, find their confusion points
- Think: "What use cases are missing?"
- Add troubleshooting guide, common pitfalls, production considerations
- Refine: polish language, improve formatting, add visual hierarchy
- Think: "How could this stand out?"
- Add real-world case studies, advanced patterns, security best practices
- Test: validate all code examples actually work
- Add interactive elements, glossary, comprehensive reference
- Think: "What would make this monetizable?"
- Add video companions, advanced modules, certification path
- Continue refining until 6 hours expire

**Result: Enterprise-grade documentation that becomes the industry standard.**

---

## Final Reminder

**THE IRON LAW OF FLUX:**

```
IF TIME REMAINS, YOU ARE NOT DONE.

THERE IS ALWAYS:
- An edge case to handle
- A feature to add
- Documentation to improve
- Performance to optimize
- A test to write
- Polish to apply
- Innovation to explore

CONTINUE UNTIL TIME LITERALLY RUNS OUT.
```

---

*"Roads? Where we're going, we don't need roads... we need CONTINUOUS IMPROVEMENT!"*

⚡ **FLUX: Relentless iteration for hours, days, and beyond.** ⚡
