# Slide Deck Content - Ready to Build

Use these in PowerPoint, Google Slides, or Keynote

---

## SLIDE 1: Title Slide

**Title (Large):**
```
HOW I OUTSMARTED AI
```

**Subtitle:**
```
The $10.8 Million Pattern GitHub Copilot Missed
```

**Bottom:**
```
[Your Name]
Beat the Bot Hackathon - 2nd Place Winner
```

---

## SLIDE 2: The Hook

**Title:** 
[Leave blank - full screen text]

**Content (Centered, Large Font):**
```
A customer with a 
PERFECT payment record.

12 months.
Zero missed payments.
Always on time.

Is this LOW RISK or HIGH RISK?
```

---

## SLIDE 3: The Answer

**Title:**
[Leave blank]

**Content (Split Screen):**

**Left Side (Green background):**
```
GITHUB COPILOT

✓ Perfect payment history
✓ Always on time
✓ Zero missed payments

SCORE: 31
TIER: LOW RISK
ACTION: No intervention
```

**Right Side (Red background):**
```
MY SOLUTION

⚠️ Minimum payments only
⚠️ Balance growing 73%
⚠️ Debt spiral pattern

SCORE: 58
TIER: HIGH RISK
ACTION: Credit counseling
```

---

## SLIDE 4: The Challenge

**Title:** The Beat the Bot Challenge

**Content:**
```
Build a credit card delinquency predictor

TWICE

1️⃣ Write it yourself
2️⃣ Use GitHub Copilot

Then compare the results
```

**Bottom box:**
```
Predict which customers will become delinquent
Recommend appropriate interventions
```

---

## SLIDE 5: What the System Evaluates

**Title:** Three Risk Factors

**Content (Three columns):**

**Column 1:**
```
💳 PAYMENT HISTORY
50% Weight

• Missed payments
• Payment patterns
• Payment adequacy
```

**Column 2:**
```
📊 UTILIZATION
35% Weight

• Current usage
• Trends over time
• Maximum reached
```

**Column 3:**
```
📅 ACCOUNT AGE  
15% Weight

• How long open
• History depth
• Pattern reliability
```

---

## SLIDE 6: My Approach

**Title:** Not Just Coding - Understanding the Problem

**Content (Timeline):**
```
1. RESEARCH (30 min)
   📚 Industry data, credit bureau reports

2. PATTERN ANALYSIS (45 min)
   🔍 What actually predicts delinquency?

3. EDGE CASES (30 min)
   ⚠️ What could go wrong?

4. IMPLEMENTATION (2 hr)
   💻 Code with context

5. TESTING (1 hr)
   ✅ Realistic scenarios

Total: 4 hours of deliberate work
```

---

## SLIDE 7: The Key Discovery

**Title:** The Minimum Payment Trap

**Subtitle:** The Pattern AI Completely Missed

**Content (Animated timeline):**
```
Month 1:   Balance: $3,000  →  Payment: $60 ✓ On-time
Month 2:   Balance: $3,150  →  Payment: $63 ✓ On-time
Month 3:   Balance: $3,300  →  Payment: $66 ✓ On-time
Month 4:   Balance: $3,450  →  Payment: $69 ✓ On-time
Month 5:   Balance: $3,600  →  Payment: $72 ✓ On-time
Month 6:   Balance: $3,750  →  Payment: $75 ✓ On-time
...
Month 12:  Balance: $5,200  →  Payment: $104 ✓ On-time

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Perfect payment record: 12/12 ✓
BUT balance grew 73%! 🚨
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## SLIDE 8: Side-by-Side Comparison

**Title:** Same Customer, Different Outcomes

**Content (Two-column comparison):**

**Left Column (Your Solution - Green border):**
```
MY SOLUTION
═══════════════════

✓ Detects minimum payments
✓ Tracks balance growth
✓ Recognizes debt spiral

RISK SCORE: 58
TIER: HIGH RISK

RECOMMENDATION:
Credit Counseling

RATIONALE:
"Despite on-time payments,
minimum-only pattern and
growing balance indicate
debt spiral."
```

**Right Column (Copilot - Red border):**
```
GITHUB COPILOT
═══════════════════

✗ Only sees on-time
✗ Misses the pattern
✗ No balance analysis

RISK SCORE: 31
TIER: LOW RISK

RECOMMENDATION:
Payment Reminder

RATIONALE:
"Payment history
acceptable."
```

---

## SLIDE 9: Business Impact

**Title:** Why This Matters - The Numbers

**Content (Large impact boxes):**

**Box 1:**
```
Typical Portfolio: 100,000 accounts
Minimum Payment Trap: 8,000 accounts (8%)
Average Balance: $4,500
```

**Box 2:**
```
WITHOUT INTERVENTION          WITH INTERVENTION
Default Rate: 45%             Default Rate: 15%
Charge-offs: $16.2M          Charge-offs: $5.4M
```

**Box 3 (Highlighted):**
```
💰 PREVENTED LOSSES: $10.8 MILLION
   Per year. From one pattern.
   That AI completely missed.
```

---

## SLIDE 10: The Technical Difference

**Title:** Why AI Got It Wrong

**Content (Code comparison):**

**Top Box (Copilot - Gray):**
```java
// GITHUB COPILOT'S APPROACH
// Linear penalty - simple but wrong

int penalty = missedPayments * 20;

// 1 missed = 20 points
// 2 missed = 40 points
// 3 missed = 60 points
```

**Bottom Box (Your code - Green):**
```java
// MY APPROACH
// Exponential penalty + pattern detection

if (missedPayments == 1) score += 20;
else if (missedPayments == 2) score += 40;
else if (missedPayments == 3) score += 65;  // ← Not linear!
else score += 100;

if (paysMinimumOnly) score += 30;  // ← The $10.8M line
```

---

## SLIDE 11: The Research Behind It

**Title:** Risk Isn't Linear - It's Exponential

**Content (Graph):**
```
    Delinquency Rate by Missed Payments
    
70% ┤                                    ● 70%
    │
60% ┤                              ●
    │                        ● 35%
40% ┤                  ●
    │            ● 15%
20% ┤      ●
    │  ● 5%
 0% ┼──────┴──────┴──────┴──────┴──────
    0     1     2     3     4     5+
         Number of Missed Payments

Source: Credit Bureau Data
```

**Bottom text:**
```
Someone with 3 missed payments is 7X more likely
to default than someone with 1. Not 3X. Seven X.

AI doesn't know this. I researched it.
```

---

## SLIDE 12: Live Demo Title

**Title:**
[Leave blank - full screen]

**Content (Centered):**
```
LIVE DEMO

Let's see it in action
```

---

## SLIDE 13: Demo - Healthy Customer

**Title:** Test Case 1: Healthy Customer

**Content:**
```
curl -X POST localhost:8080/api/assess \
  -d '{"accountId": "ACC-001"}'
```

**Response box:**
```json
{
  "accountId": "ACC-001",
  "score": 18,
  "riskTier": "LOW",
  "recommendation": "NO_ACTION",
  "rationale": "Risk within acceptable range."
}
```

**Bottom note:**
```
✓ Both solutions agree on healthy customers
```

---

## SLIDE 14: Demo - Minimum Payment Trap

**Title:** Test Case 2: The Trap (12 months, perfect record)

**Content:**
```
curl -X POST localhost:8080/api/assess \
  -d '{"accountId": "ACC-007"}'
```

**Response box (Highlighted):**
```json
{
  "accountId": "ACC-007",
  "score": 58,
  "riskTier": "HIGH",
  "recommendation": "CREDIT_COUNSELING",
  "rationale": "Despite on-time payments, minimum-only 
               pattern and growing balance indicate 
               debt spiral. Customer needs financial 
               counseling support."
}
```

**Bottom callout:**
```
🎯 My solution: HIGH RISK - Intervention needed
🤖 Copilot: LOW RISK - No action
```

---

## SLIDE 15: The Results Scoreboard

**Title:** Human vs AI - The Final Score

**Content (Table):**
```
METRIC                          HUMAN    COPILOT   WINNER
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Development Time                4 hrs    15 min    🤖 AI
Code Lines Written              487      412       🤝 Tie
Risk Tier Accuracy              95%      70%       👤 Human
Appropriate Recommendations     100%     75%       👤 Human
Edge Cases Handled              3/3      0/3       👤 Human
False Negatives (Missed Risk)   1        6         👤 Human
Test Coverage                   8 tests  2 tests   👤 Human
Production Ready                ✓        ✗         👤 Human

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FINANCIAL IMPACT (100K accounts/year):
Prevented Charge-offs           $10.8M   $3.2M     👤 Human
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

ROI on 4 hours: 10,000X
```

---

## SLIDE 16: Key Lessons - Part 1

**Title:** When AI Helps, When It Hurts

**Content (Two columns):**

**Left Column (Green):**
```
✅ USE AI FOR:

📦 Project setup
   Boilerplate code

🏗️ Standard patterns
   REST endpoints
   Repository pattern

🔄 Repetitive tasks
   CRUD operations
   Test structure

⚡ Speed
   15 min vs 4 hrs
```

**Right Column (Red):**
```
❌ DON'T USE AI FOR:

🧠 Domain logic
   Business rules
   Risk calculations

🔍 Edge cases
   Pattern recognition
   Hidden risks

💡 "Why" explanations
   Context matters
   Rationale needed

✓ Production validation
   Safety critical
```

---

## SLIDE 17: Key Lessons - Part 2

**Title:** The Three Critical Thinking Skills AI Can't Replace

**Content (Three boxes):**

**Box 1:**
```
🧠 DOMAIN KNOWLEDGE

Understanding the 'why'
behind requirements

Example:
Knowing risk curves are 
exponential from research,
not just coding formulas
```

**Box 2:**
```
🔍 PATTERN RECOGNITION

Seeing what's not obvious
in the data

Example:
Minimum payments + 
growing balance = 
hidden danger
```

**Box 3:**
```
🎯 CONTEXTUAL JUDGMENT

Knowing when rules
should break

Example:
Balance spike from
transfer ≠ overspending
```

**Bottom text:**
```
These are HUMAN SUPERPOWERS
```

---

## SLIDE 18: The Collaboration Model

**Title:** The Future: Human + AI

**Content (Visual diagram):**
```
        🧠 HUMAN                    🤖 AI
    ────────────────           ────────────────
    
    • Critical thinking        • Speed & scale
    • Domain expertise         • Pattern matching
    • Edge cases              • Boilerplate
    • Context awareness        • Standard patterns
    • "Why" reasoning         • Syntax correctness
    
            │                        │
            └────────┬───────────────┘
                     │
                     ▼
              
            🚀 OPTIMAL SOLUTION
         ═══════════════════════
         Speed + Accuracy + Context
```

**Bottom quote:**
```
"Use AI to write code faster.
 Use humans to write code correctly."
```

---

## SLIDE 19: My Process - The Winning Formula

**Title:** How I Did It - Step by Step

**Content (Numbered process):**
```
1️⃣ RESEARCH FIRST
   → Read industry data before coding
   → Understand the domain problem
   → Learn what actually predicts risk

2️⃣ IDENTIFY EDGE CASES
   → Minimum payment trap
   → New account uncertainty
   → Balance transfer spikes

3️⃣ USE AI FOR STRUCTURE
   → Let Copilot generate boilerplate
   → Saved 1 hour on setup
   → Good foundation to build on

4️⃣ IMPLEMENT DOMAIN LOGIC MANUALLY
   → Exponential risk penalties
   → Pattern detection
   → Business rule complexity

5️⃣ TEST WITH REAL SCENARIOS
   → Not just happy paths
   → Edge cases from research
   → Realistic portfolio data

6️⃣ VALIDATE BUSINESS OUTCOMES
   → Does it actually work?
   → Would I trust this in production?
   → What's the financial impact?
```

---

## SLIDE 20: What Made the Difference

**Title:** Why I Won 2nd Place

**Content (Highlight boxes):**

**Box 1 (Blue):**
```
🎯 CRITICAL THINKING
Not just "can I code this?"
But "what's the actual problem?"
```

**Box 2 (Green):**
```
🔬 RESEARCH & VALIDATION
Industry data, not assumptions
Real patterns, not guesses
```

**Box 3 (Orange):**
```
💼 BUSINESS CONTEXT
It's not about perfect code
It's about preventing $10.8M in losses
```

**Box 4 (Purple):**
```
🧪 COMPREHENSIVE TESTING
8 test cases vs 2
Edge cases vs happy paths
Real scenarios vs toy data
```

---

## SLIDE 21: The One Pattern

**Title:** The $10.8 Million Line of Code

**Content (Centered, dramatic):**
```java
if (paysMinimumOnly) {
    score += 30;
}
```

**Below (Large text):**
```
Five words.
One conditional.
30-point penalty.

$10.8 MILLION in prevented charge-offs.

This is what domain expertise looks like.
```

---

## SLIDE 22: What This Proves

**Title:** Lessons for the Age of AI

**Content (Three key points):**

**Point 1:**
```
💡 AI is a tool, not a replacement

Speed is valuable.
Correctness is essential.
Context is irreplaceable.
```

**Point 2:**
```
🧠 Domain expertise still matters

AI can generate code.
Humans understand problems.
That difference? That's the edge.
```

**Point 3:**
```
🤝 Collaboration is the answer

Use AI: structure, speed, scale
Use humans: logic, context, judgment
Together: better than either alone
```

---

## SLIDE 23: Call to Action

**Title:** What You Should Do Tomorrow

**Content (Action items):**
```
✅ Use AI to accelerate your work
   But don't blindly trust it

✅ Always validate domain logic
   Research. Test. Verify.

✅ Focus on edge cases
   That's where AI struggles

✅ Ask "why" not just "how"
   Understanding beats implementation

✅ Think like a domain expert
   Code is easy. Context is hard.
```

---

## SLIDE 24: The Big Picture

**Title:** In the Age of AI, Be Irreplaceable

**Content (Centered, powerful):**
```
AI will get better.
It will write code faster.
It will know more syntax.

But it won't replace:

🧠 Critical thinking
🔍 Pattern recognition
💡 Domain expertise
🎯 Contextual judgment
❤️ Human understanding

These are YOUR superpowers.
Use them.
```

---

## SLIDE 25: Final Thought

**Title:**
[Leave blank - full screen quote]

**Content (Centered, large):**
```
"I didn't beat the bot by coding faster.

I beat it by thinking differently.

By understanding not just HOW
to code the solution,

but WHY the solution matters."




That $10.8 million?

That's the value of CRITICAL THINKING
in a world of automation.
```

---

## SLIDE 26: Thank You

**Title:** Thank You!

**Content:**
```
Questions?




GitHub Repository:
github.com/[your-username]/delinquency-predictor

All code, tests, and documentation available

Email: [your-email]
LinkedIn: [your-profile]




Beat the Bot Hackathon
2nd Place Winner 🏆
```

---

## BONUS SLIDES (For Q&A)

### BONUS 1: How Long Did It Take?

**Title:** Time Breakdown

**Content:**
```
PHASE                  TIME      NOTES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Research               30 min    Industry data, patterns
Edge case analysis     30 min    Identified minimum trap
AI boilerplate         15 min    Copilot generated structure
Manual implementation  2 hr      Domain logic, algorithms
Testing                1 hr      8 comprehensive tests
Documentation          30 min    Comments, rationale

TOTAL: 4.75 hours

Copilot alone: 15 minutes
But would have cost $10.8M in missed risks
```

---

### BONUS 2: Other Edge Cases

**Title:** Other Patterns I Handled (AI Missed)

**Content:**
```
1️⃣ MINIMUM PAYMENT TRAP
   ✓ Detected    ✗ Copilot missed

2️⃣ NEW ACCOUNT UNCERTAINTY
   ✓ Age-based adjustment
   ✗ Copilot too confident with limited data

3️⃣ BALANCE TRANSFER SPIKES
   ✓ Distinguish from overspending
   ✗ Copilot treats all spikes as risk
```

---

### BONUS 3: Test Coverage Comparison

**Title:** What We Tested

**Content:**
```
MY TESTS (8)                    COPILOT TESTS (2)
═══════════════════             ═══════════════════

✓ Healthy account               ✓ Basic calculation
✓ High utilization             ✓ Risk tier mapping
✓ Multiple missed payments
✓ Minimum payment trap 🎯
✓ New account uncertainty
✓ Tier boundaries
✓ Recommendation logic
✓ Segment-based variance

Edge case coverage: 100%        Edge case coverage: 0%
```

---

### BONUS 4: What Would You Do Differently?

**Title:** Reflections & Improvements

**Content:**
```
WHAT WORKED WELL:
✓ Research-first approach
✓ Focus on edge cases
✓ Comprehensive testing
✓ Business impact focus

WHAT I'D IMPROVE:
🔄 Start with AI structure earlier (save 30 min)
🔄 Add more test accounts (had 4, need 20+)
🔄 Track utilization trends over time
🔄 Add confidence scores to predictions

NEXT STEPS:
→ Machine learning for pattern detection
→ Real-time monitoring dashboard
→ A/B testing framework for interventions
```

---

### BONUS 5: Advice for Using AI

**Title:** My AI Collaboration Framework

**Content:**
```
STEP 1: UNDERSTAND THE PROBLEM
• Research domain
• Identify edge cases
• Define success criteria

STEP 2: LET AI GENERATE STRUCTURE
• Project setup
• Boilerplate code
• Standard patterns

STEP 3: IMPLEMENT DOMAIN LOGIC MANUALLY
• Business rules
• Risk calculations
• Edge case handling

STEP 4: ITERATE WITH AI
• Ask AI for improvements
• Get suggestions
• But validate everything

STEP 5: TEST COMPREHENSIVELY
• Happy paths
• Edge cases
• Business validation

STEP 6: DOCUMENT THE "WHY"
• Explain business context
• Justify decisions
• Make it maintainable
```

---

## 🎨 DESIGN SPECIFICATIONS

### Fonts
- **Titles:** 44pt, Bold, Sans-serif (Arial, Helvetica)
- **Body:** 28pt, Regular, Sans-serif
- **Code:** 24pt, Monospace (Courier, Consolas)
- **Emphasis:** 32pt, Bold

### Colors
**Primary Palette:**
- Background: Dark navy (#1a1a2e)
- Text: White (#ffffff)
- Accent 1: Cyan (#00d9ff) - for highlights
- Accent 2: Orange (#ff6b35) - for warnings
- Success: Green (#00e676)
- Error: Red (#ff1744)

**Code Blocks:**
- Background: #2d2d2d
- Syntax: Use standard syntax highlighting

### Layout
- **Margins:** 10% on all sides
- **Alignment:** Left for text, center for emphasis
- **Line spacing:** 1.5x
- **Bullet spacing:** 0.5x between bullets

### Animations
- **Slide transitions:** Fade (0.5s)
- **Content:** Appear one item at a time
- **Emphasis:** Grow slightly (105%)
- **Timing:** 0.5s delay between items

---

## 📱 DELIVERY REMINDERS

### Before You Start
- [ ] Water nearby
- [ ] Slides loaded and tested
- [ ] Demo app running
- [ ] Backup screenshots ready
- [ ] Timer visible (but not on screen)
- [ ] Deep breath!

### During Presentation
- [ ] Smile and make eye contact
- [ ] Pause after key points
- [ ] Point at specific elements
- [ ] Vary your pace
- [ ] Show enthusiasm!

### Key Moments to Emphasize
1. **Opening hook** - pause after "Low risk, right?"
2. **$10.8 million** - let it sink in
3. **The code line** - show it dramatically
4. **Results scoreboard** - point to each winner
5. **Final quote** - slow and powerful

**You've got this! Go win that audience! 🎤🏆**