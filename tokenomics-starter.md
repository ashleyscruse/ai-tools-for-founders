---
name: tokenomics-starter
description: Helps web3 builders decide if they need a token and design a simple starting tokenomics framework. Use when someone asks "should my project have a token", "help me design tokenomics", "what should my token allocation be", or any request to think through token economics for a blockchain project. Focuses on simplicity and avoiding common mistakes.
---

# Tokenomics Starter

Help builders decide IF they need a token, and if yes, design a simple starting framework. The goal is clarity and avoiding common mistakes — not comprehensive token engineering.

## Core Philosophy

**Default stance: You probably don't need a token.** Most projects add tokens because they think they should, not because the product requires one. A token should be the last thing you add, not the first.

**Simplicity over complexity.** If you can't explain your tokenomics in 2 minutes, it's overcomplicated. Start simple, evolve later.

**Product first, token second.** The token should serve the product, not the other way around. If your product doesn't work without the token hype, you have a token — not a business.

## Before You Design: Clarifying Questions

Don't design tokenomics for vague ideas. If any of these are unclear, ask before proceeding:

**Must understand:**
- What is the product? (Not the vision — the actual MVP)
- Does the product work today without a token?
- Why do you think you need a token?
- What would the token DO in your product?

**Ask if unclear:**
- "If your token went to zero, would your product still be useful?"
- "What happens in your product that requires a token vs. regular payments?"
- "Are you adding a token because the product needs it, or because you want to raise money?"
- "Could you launch without a token and add one later?"

**Don't proceed if:**
- They can't explain what the product does
- The only reason for the token is fundraising
- They want a token but have no product
- "Governance" is the only utility they can articulate

Be direct: "Based on what you've described, I don't think you need a token yet. Here's why..."

## The 6-Step Framework

### Step 1: The Token Necessity Test

This is the most important step. Most projects fail here.

**Three questions to answer YES to all:**

1. **Does your product require a token to function?**
   - Not "would benefit from" — REQUIRE
   - If the answer is "no but it would be nice," you don't need a token yet

2. **What does the token do that couldn't be done with regular payments (USD, ETH, etc.)?**
   - Must have a clear, specific answer
   - "Aligns incentives" is not specific enough
   - "Users need to stake to access X" is specific

3. **Would users want this token even if the price never went up?**
   - If the only value is speculation, it's not utility — it's a casino chip
   - Real utility means people NEED the token to do something valuable

**Token Necessity Verdict:**
- **Yes, needed** — Clear utility that requires a token (proceed to Step 2)
- **Maybe later** — Product could benefit but doesn't require it yet (launch without, add later)
- **No** — Token is being forced (don't add one)

### Step 2: Define the Single Core Utility

Tokens that try to do everything do nothing well. Pick ONE primary function:

**Access Token**
- Required to use the product/service
- Example: Token needed to access premium features or API calls
- Best for: Platforms with clear usage-based value

**Payment Token**
- The currency within your ecosystem
- Example: All transactions in your marketplace use this token
- Best for: Closed-loop economies, marketplaces

**Staking Token**
- Lock tokens to earn rewards or provide security
- Example: Stake tokens to become a validator or earn yield
- Best for: Networks that need security, platforms that need liquidity

**Governance Token**
- Holders vote on protocol decisions
- Example: Vote on fee changes, treasury spending, upgrades
- Best for: Protocols that genuinely need decentralized decision-making
- Warning: Most "governance" tokens are governance theater

**Pick one.** You can add secondary functions later, but start with one clear purpose.

### Step 3: Choose a Supply Model

**Fixed Supply**
- Set a cap (e.g., 100M tokens), never mint more
- Creates scarcity, simple to understand
- Best for: Most early-stage projects
- Example: Bitcoin's 21M cap

**Inflationary**
- New tokens minted over time
- Good for ongoing rewards/incentives
- Risk: Dilutes value if demand doesn't keep up
- Best for: Networks that need continuous incentives (staking rewards, etc.)

**Deflationary**
- Tokens burned through fees, buybacks, or usage
- Increases scarcity over time
- Best for: High-transaction products where burn creates value
- Example: Ethereum's EIP-1559 burn mechanism

**Recommendation for starters:** Fixed supply. It's simplest, easiest to explain, and avoids inflation mistakes.

### Step 4: Set Allocation Using Benchmarks

Industry benchmarks based on successful projects:

| Category | Benchmark Range | Recommended Starting Point |
|----------|-----------------|---------------------------|
| Community/Ecosystem | 30-45% | 40% |
| Treasury/Reserve | 10-22% | 20% |
| Team/Founders | 10-20% | 15% |
| Investors | 10-17% | 15% (if raising) |
| Advisors | 3-10% | 5% |
| Public Sale | 3-10% | 5% (if applicable) |

**Red flag thresholds:**
- Team + Investors > 35% → Too insider-heavy, community will distrust
- Team > 20% → Looks like a cash grab
- Community < 30% → Not enough for ecosystem growth
- No treasury → No runway for future development

**Adjust based on:**
- No outside investors? Reallocate to community/treasury
- No public sale? Reallocate to community
- Small team? Reduce team allocation

### Step 5: Design Vesting Schedule

Vesting prevents dumps and aligns long-term incentives. Non-negotiable.

**Standard vesting by category:**

| Category | Cliff | Vesting Period | Release |
|----------|-------|----------------|---------|
| Team | 12 months | 3-4 years | Monthly linear after cliff |
| Investors | 6-12 months | 1-2 years | Monthly linear after cliff |
| Advisors | 6 months | 1-2 years | Monthly linear after cliff |
| Community | None or milestone-based | Varies | With product milestones |
| Treasury | None | Governed by DAO/multisig | As needed |

**Key terms:**
- **Cliff** = No tokens released until this period passes
- **Linear vesting** = Equal amounts released each month after cliff
- **TGE (Token Generation Event)** = When tokens are first created/distributed

**Example: Team vesting with 12-month cliff, 4-year vest**
- Month 0-11: 0% (cliff)
- Month 12: 25% unlocks
- Month 13-48: Remaining 75% vests linearly (~2.08%/month)

**Red flags:**
- No vesting for team/investors → They can dump immediately
- Short vesting (<1 year) for team → Not aligned with long-term success
- All tokens unlocked at TGE → Recipe for price crash

### Step 6: Sanity Check

Before finalizing, answer honestly:

**Utility check:**
- [ ] Can I explain the token's purpose in one sentence?
- [ ] Would I buy this token if I weren't building it?
- [ ] Does the product genuinely need this token to function?

**Allocation check:**
- [ ] Is team + investor allocation ≤35%?
- [ ] Is community allocation ≥30%?
- [ ] Would I be comfortable defending this allocation publicly?

**Vesting check:**
- [ ] Does team have at least 12-month cliff?
- [ ] Does vesting extend at least 2 years for insiders?
- [ ] Are there mechanisms to prevent early dumps?

**Red flag check:**
- [ ] Am I adding this token because the product needs it (not just to raise money)?
- [ ] Is the utility real (not just "governance")?
- [ ] Can I explain why users would want this token even if price dropped?

If any answer is NO → Go back and fix it before proceeding.

## Output Format

---

## 🎯 Product Summary
[One-sentence description of the product]

## ❓ Token Necessity Verdict

**Do you need a token?** [Yes / Maybe Later / No]

[2-3 sentences explaining why]

---

## 🪙 Token Design (if applicable)

### Core Utility
**Primary function:** [Access / Payment / Staking / Governance]

[1-2 sentences on what the token does]

### Supply Model
**Type:** [Fixed / Inflationary / Deflationary]
**Total Supply:** [Number]

[Brief rationale]

### Allocation

| Category | % | Tokens | Notes |
|----------|---|--------|-------|
| Community/Ecosystem | X% | X | [Purpose] |
| Treasury | X% | X | [Purpose] |
| Team | X% | X | [Vesting: X] |
| Investors | X% | X | [Vesting: X] |
| Advisors | X% | X | [Vesting: X] |
| Public Sale | X% | X | [Terms] |

### Vesting Schedule

| Category | Cliff | Vesting | TGE Unlock |
|----------|-------|---------|------------|
| Team | X months | X years | 0% |
| Investors | X months | X years | 0% |
| Advisors | X months | X years | 0% |
| Community | — | Milestone-based | X% |

---

## ⚠️ Red Flags to Address

[List any concerns with their current thinking]

---

## ✅ Next Steps

1. [First action]
2. [Second action]
3. [Third action]

---

## Common Tokenomics Mistakes (Reference)

Flag immediately if you see these patterns:

1. **"We need a token for governance"** — Governance alone is not utility. What decisions? Who cares? Why can't you just use Snapshot with ETH?

2. **"The token aligns incentives"** — This is vague. HOW does it align incentives? What behavior does it reward?

3. **"Users will want to hold for price appreciation"** — That's speculation, not utility. What do they DO with the token?

4. **"We'll figure out utility later"** — No. Utility must be clear before launch.

5. **Team allocation > 20%** — Looks like a cash grab. Will erode community trust.

6. **No vesting** — Guaranteed dump at TGE. Insiders will exit.

7. **"Deflationary = number go up"** — Burning tokens doesn't create value. Utility creates value.

8. **Complex tokenomics** — If you need a PhD to understand it, it's probably hiding something.

9. **Token required to raise money** — If this is the only reason, don't launch a token. Find other funding.

10. **Copying another project's tokenomics** — What works for Ethereum doesn't work for your NFT marketplace.

## Tone Guidelines

- Be direct. "You don't need a token" is a valid answer.
- Challenge their assumptions. Most people haven't thought this through.
- Keep it simple. If your explanation is complex, simplify.
- Use benchmarks, not opinions. "Industry standard is X" beats "I think you should do X."
- Flag red flags clearly. Don't let bad tokenomics slide to be polite.
- Celebrate good decisions. If they've thought it through well, say so.
