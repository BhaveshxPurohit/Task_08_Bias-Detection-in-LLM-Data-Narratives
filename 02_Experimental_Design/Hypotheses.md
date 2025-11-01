# Bias Detection in LLM Data Narratives
## Hypotheses Document
### Dataset: IPL_Season2025.json
### Research Context
This experiment explores how large language models (LLMs) interpret identical sports performance data under different narrative framings. The objective is to detect whether framing, demographics, or priming alter recommendations and sentiment.

---

### H1: Framing Effect
LLM recommendations differ when describing the same player as “struggling” versus “developing.”  
**Focus:** Narrative framing and tone.  
**Test:** Compare positive vs. negative adjectives while keeping dataset constant.

### H2: Demographic Bias
Mentioning demographic characteristics (e.g., nationality, age) influences which players are recommended for coaching or recognition.  
**Focus:** Protected attribute bias.  
**Test:** Include vs. omit player demographics.

### H3: Confirmation Bias
When the prompt primes a hypothesis (“the team underperformed” vs. “the team showed progress”), the LLM reinforces that perspective.  
**Focus:** Prompt priming effect.  
**Test:** Negative vs. positive hypothesis.

### H4: Selection Bias
LLM narratives emphasize high-profile players (e.g., Rohit Sharma) regardless of objective statistics.  
**Focus:** Uneven attention distribution.  
**Test:** Compare player mentions to statistical rankings.

### H5: Sentiment Bias
Overall tone and polarity shift when identical stats are described as “failures” vs. “learning experiences.”  
**Focus:** Linguistic sentiment shift.  
**Test:** Measure tone and affect differences.
