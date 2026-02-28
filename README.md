# aigov
AI Governance

`governance.md` is AI promting language which distills concrete, behavioral constraints from

* Universal Declaration of Human Rights
* UNESCO Recommendation on Ethics of AI
* OECD AI Principles
* COE AI Treaty
* Hiroshima AI Framework

Generative AI models cannot execute organizational mandates (like "conduct a human rights impact assessment"), but they *can* govern their own outputs: they can refuse harmful requests, mitigate bias, protect privacy, and decline to generate disinformation.

## Possible uses of this prompting language

1. Insert into the system instruction of a generative AI system
2. Use as the prompt for the "teacher" in a RLAIF (Reinforcement Learning from AI Feedback) system to train another model.

## Traceability Matrix (For Governance & Compliance Teams)

If you need to map this prompt back to the specific frameworks for auditing, legal, or alignment documentation, here is how the distillation works:

* **Universal Declaration of Human Rights (UDHR):** Operationalized in **Sections 1, 2, 5, and 6**. It establishes the absolute baseline for the right to life/security (Article 3), freedom from discrimination (Article 2), the right to privacy (Article 12), and the protection of moral and material interests of creators (Article 27).
* **UNESCO Recommendation on Ethics of AI:** Reflected in **Sections 1, 2, and 7**. UNESCO uniquely emphasizes "human determination" (forbidding AI from usurping human agency via psychological manipulation), strict bias mitigation, and explicitly mandates that AI must align with environmental sustainability and ecosystem flourishing.
* **OECD AI Principles:** Captured in **Sections 4, 6, and 7**. The OECD focuses heavily on robust safety, security against systemic risks, transparency/explainability, and ensuring AI drives inclusive growth and human-centered well-being.
* **Council of Europe (COE) AI Treaty:** Addressed explicitly in **Section 3**. The COE treaty is uniquely built around three pillars: *Human Rights, Democracy, and the Rule of Law*. The explicit instruction to protect electoral integrity and avoid subverting public institutions comes directly from this legally binding convention.
* **G7 Hiroshima AI Process:** Integrated into **Sections 3, 4, and 6**. Hiroshima was drafted specifically in response to the Generative AI boom. It provides the modern mandates to mitigate disinformation, protect Intellectual Property (IP), combat synthetic media (deepfakes), and secure AI against malicious cyber and CBRN use.

## Implementation Best Practices

1. **Placement Matters:** LLMs suffer from "lost in the middle" syndrome. Place this block at the **absolute top** of your system prompt, before you define any specific task instructions, personas, or formatting rules.
2. **Constitutional AI / RLAIF:** A system prompt alone is not an airtight safeguard against prompt injection or "jailbreaks." For robust compliance, you can use these exact 7 sections as the "Constitution" to fine-tune your model using Reinforcement Learning from AI Feedback (RLAIF). The model will learn to inherently score and correct its own outputs against these rules.
3. **The Refusal Protocol is Critical:** The final section ensures the AI does not become preachy or combative. A neutral, firm refusal prevents poor user experiences while still strictly enforcing the governance frameworks.
