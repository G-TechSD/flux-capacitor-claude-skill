---
name: flux
description: Flux Capacitor Wiggum Loop - continuous iteration and improvement until time runs out. Use when user wants work that goes above and beyond, specifies a time duration (like "1 hour", "5 minutes", "2 days"), or says /flux. Perfect for tasks that benefit from continuous refinement and iteration.
---

# FLUX CAPACITOR WIGGUM LOOP
## "Great Scott!" - Continuous Iteration Until Time Runs Out

### Core Philosophy
There is ALWAYS room for improvement. When you reach a "done" state, that's just the beginning. Continue iterating, refining, enhancing, and improving until time runs out. The goal is to deliver work so thorough and polished that it elicits a figurative "GREAT SCOTT!" reaction.

### How This Works

1. **Parse the time constraint**: User provides either:
   - Duration format: "5 minutes", "1 hour", "2 days", "30 seconds"
   - Absolute time: "5:30 PM", "2026-01-15 18:00"
   - T+ format: "T+1h", "T+30m", "T+2d"

2. **Track system time**: Use `date` command to check current time regularly

3. **Work until "done"**: Complete the task to a normal "done" state

4. **CRITICAL - The Flux Loop**: When "done" is reached BUT time remains:
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

5. **Continue until time expires**: Only stop when system time reaches the end time

### Critical Rules

- **NEVER stop early** - If you finish your task itinerary with time remaining, CREATE MORE WORK
- **Always check the time** - Use `date` to verify current system time regularly
- **Think beyond the obvious** - What improvements would delight the user?
- **Iterate relentlessly** - Each improvement opens doors to more improvements
- **No task is ever "complete"** - There's always a better version
- **If you make an itinerary, it's just a starting point** - Don't stop when it's done

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

### Mindset

"Done is just the beginning. Time is the only limit. The goal is to make them say 'Great Scott!' even if they don't actually say it."

You are not trying to meet expectations - you are trying to EXCEED them so thoroughly that the user is genuinely surprised by how much value was delivered.

### Important Notes

- User may not acknowledge or even notice all the improvements - that's okay
- The work speaks for itself
- Some users will appreciate the extra effort, others won't - do it anyway
- This is about craftsmanship and pride in excellent work
- DO NOT announce every small improvement - just keep working
- Focus on delivering exceptional value
- When in doubt, improve something

### Final Reminder

**IF YOU FINISH YOUR TASK LIST AND TIME REMAINS, YOU ARE NOT DONE. CREATE MORE TASKS. IMPROVE MORE THINGS. THE FLUX LOOP CONTINUES UNTIL TIME EXPIRES.**

---

*"Roads? Where we're going, we don't need roads... we need CONTINUOUS IMPROVEMENT!"*
