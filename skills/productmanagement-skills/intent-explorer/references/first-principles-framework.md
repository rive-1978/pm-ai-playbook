# First Principles Framework Reference

## Core Method

"Boil things down to the most fundamental truths and then reason up from there." — Elon Musk

### The Battery Example

- **Conventional**: "Batteries are expensive ($600/kWh), always have been"
- **First Principles**: What are batteries made of? Carbon, nickel, aluminum, polymers
- **Atomic Question**: What do those materials cost on the London Metal Exchange?
- **Discovery**: Raw materials = $80/kWh
- **Rebuild**: Engineer better manufacturing → Tesla's cost breakthrough

## The Process

### Phase 1: Identify Assumptions

Ask: "What am I assuming to be true that might not be?"
List every assumption embedded in the current approach.

### Phase 2: Break to Atoms

For each assumption, ask: "What is the most fundamental truth here?"
Keep asking "why?" until you hit bedrock facts.

### Phase 3: Rebuild From Truth

Starting ONLY from verified fundamentals, ask:
"What's the simplest solution that addresses the core need?"

## The Decomposition Ladder

### Level 1: Surface Problem

"We need better parent engagement"

### Level 2: Functional Need

"Parents need to feel connected to their child's day"

### Level 3: Emotional Core

"Parents feel guilt about not being present"

### Level 4: Fundamental Truth

"Humans need proof of wellbeing for those they love"

### Level 5: Atomic Solution

Photo + timestamp + child's face = proof of wellbeing
Everything else is decoration.

## Common Assumption Traps

### 1. The "Industry Standard" Trap

"Everyone does it this way" → WHY does everyone do it this way?
Often: legacy, not logic

### 2. The "Customer Said" Trap

"Customers asked for X" → What PROBLEM were they trying to solve?
Often: they're describing solutions, not needs

### 3. The "Technology Exists" Trap

"We should use [tech] because it exists" → What fundamental need does this serve?
Often: solution seeking a problem

### 4. The "Competitor Does It" Trap

"Competitor has this feature" → Does it actually solve a real problem?
Often: feature bloat, not value

## Questions That Cut Through

1. "If we were starting from scratch today, would we build it this way?"
2. "What would a complete outsider think is weird about this?"
3. "If this cost 10x more, would we still do it?"
4. "If this was illegal, what would we do instead?"
5. "What's the version of this that a child could understand?"

## Output Format

```
PROBLEM: [stated problem]

ASSUMPTIONS IDENTIFIED:
1. [assumption] → Challenge: [why this might be wrong]
2. [assumption] → Challenge: [why this might be wrong]

FUNDAMENTAL TRUTHS:
• [bedrock fact 1]
• [bedrock fact 2]
• [bedrock fact 3]

REBUILT SOLUTION:
[New approach built only from fundamentals]

VS CONVENTIONAL:
[How this differs from the obvious approach]
```

## Integrated Framework: First Principles + Design Thinking + Systems Engineering

For deep problem solving, combine three complementary frameworks:

### Phase 1: First Principles (Musk Method)

**Core Question**: What is fundamentally true?

1. Identify assumptions
2. Break to atomic truths
3. Rebuild from fundamentals

**Best For:** Challenging conventional wisdom, finding non-obvious solutions, cost reduction / efficiency

### Phase 2: Stanford Design Thinking (IDEO Method)

**Core Question**: What do humans actually need?

The Five Stages:

1. **Empathize** - Deeply understand user needs, pain, context
2. **Define** - Frame the real problem (often different from stated problem)
3. **Ideate** - Generate many solutions without judgment
4. **Prototype** - Build quick, cheap versions to test
5. **Test** - Learn from real user feedback, iterate

Key Practices:

- **Beginner's Mind**: Approach without assumptions
- **How Might We**: Reframe problems as opportunities
- **Rapid Prototyping**: Learn fast, fail cheap
- **User-Centered**: Always return to user needs

**Best For:** User-facing products, innovation and new concepts, understanding unmet needs

### Phase 3: MIT Systems Engineering

**Core Question**: How do the parts interact?

Systems Thinking Principles:

1. **Holistic View**: System behavior emerges from interactions
2. **Feedback Loops**: Outputs affect inputs (positive/negative)
3. **Boundaries**: Define system vs environment
4. **Hierarchy**: Systems contain subsystems
5. **Emergence**: Whole > sum of parts

Key Questions:

- What are the system boundaries?
- Where are the feedback loops?
- What are the leverage points?
- What are the unintended consequences?

**Best For:** Complex multi-component problems, long-term strategic thinking, avoiding unintended consequences

### When to Use Which

| Situation                  | Primary          | Supporting       |
| -------------------------- | ---------------- | ---------------- |
| Challenging industry norms | First Principles | Design Thinking  |
| New product/feature        | Design Thinking  | Systems          |
| Complex org problem        | Systems          | First Principles |
| Optimization task          | First Principles | Systems          |
| Innovation sprint          | Design Thinking  | First Principles |

### Combined Output Format

```markdown
## First Principles Analysis

**Assumptions Challenged:**

- [assumption] → [fundamental truth]

## Design Thinking Synthesis

**User Need:** [What they really need]
**How Might We:** [Reframed problem]
**Solution Concepts:** [Top 3 ideas]

## Systems View

**Key Feedback Loops:**

- [loop 1]
- [loop 2]

**Leverage Points:**

- [where small changes have big effects]

**Potential Unintended Consequences:**

- [second-order effects to monitor]
```

## Examples

### Example 1: TeddySnaps Photo System

**Surface Problem:** "We need to send more photos to parents"

**Assumptions Challenged:**

1. ❌ Parents want MORE photos → Actually: they want the RIGHT photos
2. ❌ All moments are equal → Actually: moments with THEIR child matter
3. ❌ Staff should curate → Actually: staff time is expensive and inconsistent

**Fundamental Truths:**

- Parents want proof their specific child is safe/happy
- Face = identity = "that's MY child"
- Time = context = "this happened today"
- Automatic > Manual for consistency

**Rebuilt Solution:**
AI face recognition + automatic tagging + parent-specific feed
Staff takes photos freely → System sorts and delivers automatically

---

### Example 2: TISA Enrollment Process

**Surface Problem:** "Our enrollment process is too slow"

**Assumptions Challenged:**

1. ❌ We need all info upfront → Actually: we need enough to make a decision
2. ❌ Forms must be comprehensive → Actually: forms create friction
3. ❌ Parents want to give info → Actually: parents want to RECEIVE confirmation

**Fundamental Truths:**

- Enrollment = exchange of commitment (parent commits child, school commits spot)
- Minimum viable info: child name, age, parent contact
- Everything else can come later
- Speed of response = perception of quality

**Rebuilt Solution:**
Phase 1: Name + age + email (30 seconds) → Instant spot reservation
Phase 2: Detailed forms (after commitment)
Result: 10x faster, higher conversion

---

### Example 3: GolfTab Ordering

**Surface Problem:** "Golfers need to order food on the course"

**Assumptions Challenged:**

1. ❌ Need full restaurant menu → Actually: simplified menu works better
2. ❌ Need precise delivery time → Actually: "by hole X" is enough
3. ❌ Complex payment flow → Actually: charge to room/tab, settle later

**Fundamental Truths:**

- Golfer's hands are often dirty/gloved
- Attention span on course = minimal
- Location = hole number (already known via tee time)
- Speed > options

**Rebuilt Solution:**
5-tap ordering: Item → Quantity → Hole → Confirm → Done
No menu browsing, no payment friction, no address entry

---

### Example 4: Staff Scheduling (TeddyKids)

**Surface Problem:** "Staff scheduling is complex and time-consuming"

**Assumptions Challenged:**

1. ❌ Manager must create schedule → Actually: AI can draft, manager approves
2. ❌ Staff preferences are unpredictable → Actually: patterns emerge over time
3. ❌ Ratio compliance is manual → Actually: this is pure math

**Fundamental Truths:**

- Child:staff ratios are legally mandated (deterministic)
- Staff availability has patterns (learnable)
- Cost optimization is mathematical
- Human oversight needed for exceptions only

**Rebuilt Solution:**
Algorithm generates schedule → Manager reviews exceptions → Staff confirms
80% automated, 20% human judgment

## Template

```
PROBLEM: [What are you trying to solve?]

CURRENT APPROACH: [How is it done now?]

ASSUMPTIONS (list 3-5):
1. We assume [X] → But what if [challenge]?
2. We assume [Y] → But what if [challenge]?

FUNDAMENTAL TRUTHS:
• [Irreducible fact 1]
• [Irreducible fact 2]
• [Irreducible fact 3]

REBUILT SOLUTION:
[Solution built only from truths above]

VALIDATION:
- Does this solve the core need? [Y/N]
- Is it simpler than current approach? [Y/N]
- Can we build this? [Y/N]
```
