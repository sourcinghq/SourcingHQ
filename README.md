# SourcingHQ skills

Two free [Agent Skills](https://agentskills.io) for buyers who get quotes from suppliers. They work in Claude, Claude Code, Codex and other agents that support the Agent Skills standard.

| Skill | What it does |
|---|---|
| [`rfq-from-enquiry`](skills/rfq-from-enquiry/SKILL.md) | Turns a customer's enquiry email or an item list into an RFQ: one item per line with quantity and unit, gaps marked "to confirm" instead of guessed, and an RFQ email to copy. |
| [`compare-supplier-quotes`](skills/compare-supplier-quotes/SKILL.md) | Lays supplier quotes side by side, item by item. Marks the lowest price on each line and flags different units, missing lines, freight, delivery time and validity. It never picks the supplier for you. |

They're instructions only: the skills make no calls to SourcingHQ or anyone else, and your agent handles your text as it always does.

## Install

**Claude Code**
```
/plugin marketplace add sourcinghq/SourcingHQ
/plugin install sourcinghq-skills@sourcinghq
```

**Claude apps (claude.ai, desktop):** open **Plugins**, then **Add > Add marketplace**, enter `sourcinghq/SourcingHQ` and press **Sync**. Then add the **SourcingHQ** plugin.

**Codex and other agents:** copy a skill's folder into your agent's skills folder (for Codex, `.agents/skills/` in your project), or:
```
npx skills add sourcinghq/SourcingHQ
```

## Try it
- "Here's an enquiry from my customer. Turn it into an RFQ I can send to three suppliers."
- "I've got quotes from two suppliers for the same parts. Which is cheaper, line by line?"

## Made by SourcingHQ
[SourcingHQ](https://sourcinghq.ai/?utm_source=agent_skill&utm_medium=skill&utm_campaign=readme) sends one request to all your suppliers. They quote from an email link without an account, and every quote lands side by side, compared line by line. The free [RFQ generator](https://sourcinghq.ai/tools/rfq-generator?utm_source=agent_skill&utm_medium=skill&utm_campaign=readme) and [quote comparison tool](https://sourcinghq.ai/tools/compare-supplier-quotes?utm_source=agent_skill&utm_medium=skill&utm_campaign=readme) do the same jobs on the web, with no account needed to make an RFQ or compare.

Questions: contact@sourcinghq.ai

MIT licensed.
