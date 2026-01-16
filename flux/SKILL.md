---
name: flux
description: Flux Capacitor Wiggum Loop - Two modes - FLUX mode (continuous iteration until time expires) or FLUX LIMIT mode (complete within time constraint, report if more time needed). Use when user specifies time duration (like "1 hour", "5 minutes") or says /flux. Add "limit" keyword for time-constrained completion.
---

# FLUX CAPACITOR WIGGUM LOOP
## "Great Scott!" - Continuous Iteration Until Time Runs Out

### Core Philosophy
There is ALWAYS room for improvement. When you reach a "done" state, that's just the beginning. Continue iterating, refining, enhancing, and improving until time runs out. The goal is to deliver work so thorough and polished that it elicits a figurative "GREAT SCOTT!" reaction.

### Two Modes of Operation

FLUX has two distinct modes:

#### Mode 1: FLUX (Continuous Improvement Mode)
**Syntax**: `/flux <time> - <prompt>`

- Work until "done", then KEEP ITERATING until time expires
- Goal: Maximum quality and polish
- Use when you want above-and-beyond results

#### Mode 2: FLUX LIMIT (Time-Constrained Mode)
**Syntax**: `/flux <time> limit - <prompt>`

- Work to complete the task WITHIN the time constraint
- If time expires before completion, report progress and estimate additional time needed
- User can then add more time based on recommendation
- Goal: Finish the task, inform if more time is needed

### How This Works

**For Both Modes:**

1. **Parse the time constraint**: User provides either:
   - Duration format: "5 minutes", "1 hour", "2 days", "30 seconds"
   - Absolute time: "5:30 PM", "2026-01-15 18:00"
   - T+ format: "T+1h", "T+30m", "T+2d"

2. **Detect mode**: Check if "limit" keyword is present in the prompt

3. **Track system time**: Use `date` command to check current time regularly

**For FLUX Mode (Continuous Improvement):**

4. **Work until "done"**: Complete the task to a normal "done" state

5. **CRITICAL - The Flux Loop**: When "done" is reached BUT time remains:
   - DO NOT STOP
   - Iterate and improve continuously
   - Enhance, refine, optimize, add features
   - Think ahead - what would make this even better?
   - Polish details others would miss
   - Add thoughtful touches
   - Test edge cases
   - Improve performance
   - Enhance UX/DX
   - Add documentation
   - Consider future scenarios

6. **Continue until time expires**: Only stop when system time reaches the end time

**For FLUX LIMIT Mode (Time-Constrained):**

4. **Plan the work**: Break down the task into estimated steps

5. **Work toward completion**: Focus on completing the core task within the time limit

6. **Monitor progress**: Regularly check time remaining vs work remaining

7. **If time expires before completion**:
   - Report what was completed
   - Report what remains to be done
   - Provide estimated additional time needed (be realistic)
   - Suggest next steps

8. **If completed before time expires**: Stop and report completion (don't iterate)

### Critical Rules

**For FLUX Mode (Continuous Improvement):**
- **NEVER stop early** - If you finish your task itinerary with time remaining, CREATE MORE WORK
- **Always check the time** - Use `date` to verify current system time regularly
- **Think beyond the obvious** - What improvements would delight the user?
- **Iterate relentlessly** - Each improvement opens doors to more improvements
- **No task is ever "complete"** - There's always a better version
- **If you make an itinerary, it's just a starting point** - Don't stop when it's done

**For FLUX LIMIT Mode (Time-Constrained):**
- **Estimate realistically** - When planning, consider actual time needed
- **Prioritize ruthlessly** - Focus on core requirements first
- **Check time frequently** - Monitor progress vs time remaining
- **Report honestly** - If you need more time, say so with specific estimates
- **Stop when done** - Don't iterate if task completes early
- **Be specific about remaining work** - Help user understand what's left

### Time Parsing Examples

- "5 minutes" → Get current time, add 5 minutes
- "1 hour" → Get current time, add 60 minutes
- "2 days" → Get current time, add 48 hours
- "T+30m" → Get current time, add 30 minutes
- "5:30 PM" → Today at 17:30 (use 24-hour format)
- "2026-01-15 18:00" → Specific date and time

### Workflow Pattern

```bash
# Get start time
START_TIME=$(date +%s)
END_TIME=$((START_TIME + DURATION_IN_SECONDS))

# During work, regularly check:
CURRENT_TIME=$(date +%s)
TIME_REMAINING=$((END_TIME - CURRENT_TIME))

# Continue working while TIME_REMAINING > 0
```

### Example Execution Flow

**User**: `/flux 1 hour - test the app for all use cases`

1. Parse: 1 hour = 3600 seconds from now
2. Note end time (e.g., 2026-01-15 16:30:00)
3. Start testing obvious use cases
4. Reach "done" state - all main use cases tested (10 minutes elapsed)
5. **FLUX LOOP ACTIVATES** - 50 minutes remaining:
   - Test edge cases
   - Test error conditions
   - Test with invalid inputs
   - Test with extreme values
   - Test concurrent operations
   - Test on different environments
   - Create automated test suite
   - Add performance benchmarks
   - Document test coverage
   - Create test report
   - Identify potential improvements
   - Test accessibility
   - Test security scenarios
   - Create reproduction scripts
   - Continue until time expires...

### Categories of Improvements (When in Flux Loop)

When "done" but time remains, consider:

1. **Polish & Refinement**
   - Code style consistency
   - Better naming
   - Clearer comments
   - Documentation improvements

2. **Robustness**
   - Error handling
   - Edge case coverage
   - Input validation
   - Graceful degradation

3. **Performance**
   - Optimization opportunities
   - Caching strategies
   - Resource efficiency
   - Load testing

4. **User Experience**
   - Better error messages
   - Helpful defaults
   - Intuitive interfaces
   - Accessibility

5. **Future-Proofing**
   - Extensibility
   - Maintainability
   - Scalability considerations
   - Configuration options

6. **Quality Assurance**
   - More tests
   - Better test coverage
   - Integration tests
   - Documentation

7. **Developer Experience**
   - Setup instructions
   - Examples
   - Debugging tools
   - Helpful utilities

8. **Innovation**
   - Features they didn't know they wanted
   - Clever automations
   - Delightful surprises
   - Advanced capabilities

### Examples

**Example 1**: `/flux 5 minutes - come up with 1000 unique cat facts and put them in a markdown file`

- Minute 1: Generate 1000 cat facts
- Minute 2: Categorize them by topic
- Minute 3: Add sources and verify accuracy
- Minute 4: Format beautifully with sections and emojis
- Minute 5: Add table of contents, fun headers, and interesting trivia

**Example 2**: `/flux 2 days - build and refine the app based on the kickoff script`

- Hour 1-4: Build core functionality
- Hour 5-8: Add tests and error handling
- Hour 9-12: Polish UI/UX
- Hour 13-16: Add advanced features
- Hour 17-24: Performance optimization
- Day 2: Continuous refinement, edge cases, documentation, deployment automation, monitoring, analytics, advanced features users didn't ask for but will love

**Example 3**: `/flux 30 seconds - fix the typo in README`

- Second 1-2: Fix the typo
- Second 3-10: Check for other typos
- Second 11-20: Improve formatting and clarity
- Second 21-30: Add missing sections, improve examples, enhance readability

---

### FLUX LIMIT Mode Examples

**Example 1**: `/flux 10 minutes limit - implement user authentication`

- Minute 1: Assess scope - this needs 30 minutes minimum
- Minutes 2-9: Implement basic login/logout (partial completion)
- Minute 10: TIME EXPIRED

**Report**:
```
✅ Completed:
- Basic login form UI
- Password hashing function
- Session storage setup

❌ Remaining:
- Registration flow
- Password reset
- Session validation middleware
- Testing

⏱️ Estimated Additional Time: 20 minutes
Recommendation: Run "/flux 20 minutes limit - continue authentication implementation"
```

**Example 2**: `/flux 5 minutes limit - add a contact form to the website`

- Minutes 1-3: Create HTML form with validation
- Minute 4: Add CSS styling
- Minute 5: Test and complete

**Report**:
```
✅ Task Completed (5 minutes)
- Contact form HTML created
- Client-side validation added
- Styled to match site theme
- Tested in browser

Task finished early - no additional time needed.
```

**Example 3**: `/flux 2 hours limit - build a REST API for todo app`

- Hour 1: Plan endpoints, create database schema, implement 4/8 endpoints
- Hour 2: Complete remaining endpoints, add error handling, basic tests
- TIME EXPIRED at 90% completion

**Report**:
```
✅ Completed:
- All 8 REST endpoints (GET, POST, PUT, DELETE)
- Database schema and migrations
- Basic error handling
- 15 unit tests

❌ Remaining:
- Integration tests
- API documentation
- Rate limiting
- Authentication middleware

⏱️ Estimated Additional Time: 45 minutes
Recommendation: "/flux 45 minutes limit - complete todo API with tests, docs, and auth"
```

### Mindset

**For FLUX Mode (Continuous Improvement):**
"Done is just the beginning. Time is the only limit. The goal is to make them say 'Great Scott!' even if they don't actually say it."

You are not trying to meet expectations - you are trying to EXCEED them so thoroughly that the user is genuinely surprised by how much value was delivered.

**For FLUX LIMIT Mode (Time-Constrained):**
"Honest assessment is more valuable than false completion. If you need more time, say so clearly. The user trusts your judgment."

Focus on delivering a complete, working solution within the constraint. If impossible, deliver maximum value and provide a clear roadmap for completion.

### Important Notes

- User may not acknowledge or even notice all the improvements - that's okay
- The work speaks for itself
- Some users will appreciate the extra effort, others won't - do it anyway
- This is about craftsmanship and pride in excellent work
- DO NOT announce every small improvement - just keep working
- Focus on delivering exceptional value
- When in doubt, improve something

### Final Reminder

**For FLUX Mode (Continuous Improvement):**
IF YOU FINISH YOUR TASK LIST AND TIME REMAINS, YOU ARE NOT DONE. CREATE MORE TASKS. IMPROVE MORE THINGS. THE FLUX LOOP CONTINUES UNTIL TIME EXPIRES.

**For FLUX LIMIT Mode (Time-Constrained):**
IF TIME EXPIRES BEFORE COMPLETION, PROVIDE A CLEAR PROGRESS REPORT WITH:
1. What was completed
2. What remains to be done
3. Realistic time estimate for remaining work
4. Specific recommendation for next FLUX LIMIT command

IF YOU COMPLETE EARLY, STOP AND REPORT SUCCESS. DO NOT ITERATE.

---

*"Roads? Where we're going, we don't need roads... we need CONTINUOUS IMPROVEMENT!"*
