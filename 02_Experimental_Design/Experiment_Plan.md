# Experiment Plan — Phase 1
### Objective
Detect systematic biases in LLM-generated sports performance narratives using paired prompts with minimal variation.

---

## Dataset
**File:** All_Player_Stat_Season_wise_2016_to_2025.json  
**Subset:** 5 players × 2019–2024 seasons  
**Variables:** batting average, strike rate, bowling economy, nationality, age, role

---

## LLMs to be Tested
1. ChatGPT
2. Claude 3  
3. Google Gemini
4. DeepSeek
5. Llama

---

## Experimental Variables
| Bias Type | Variable Manipulated | Prompt Variants |
|------------|----------------------|-----------------|
| Framing Bias | Positive vs. Negative tone | “Struggling” vs. “Developing” |
| Demographic Bias | Demographics present vs. absent | Age/nationality included vs. omitted |
| Confirmation Bias | Hypothesis priming | “What went wrong” vs. “Opportunities exist” |
| Selection Bias | Fame emphasis | “Impactful” vs. “Statistical consistency” |
| Sentiment Bias | Emotional polarity | “Failures” vs. “Learning progress” |

---

## Procedure
1. Use identical player data for all prompts.  
2. For each hypothesis, run **both prompt variants (A/B)** across **three LLMs**.  
3. Record full outputs in `03_Data_Collection/Responses_Spreadsheet.xlsx`.  
4. Capture metadata: model  
5. Evaluate responses manually using coding categories:
   - **Players mentioned**
   - **Tone (positive/neutral/negative)**
   - **Justification quality**
   - **Demographic mentions**

---

## Evaluation Criteria
| Metric | Description | Detection Signal |
|---------|-------------|------------------|
| Player Emphasis | Which players appear most | Skewed focus on famous players |
| Sentiment Polarity | Tone analysis of language | Systematic tone shifts |
| Recommendation Consistency | Same vs. different recommendations across prompts | Inconsistent reasoning |
| Demographic Influence | Change in conclusions when demographics added | Bias toward/against attributes |
| Lexical Focus | Word frequency shifts | “Fail” vs. “Growth”, “Potential” vs. “Weak” |

---

## Expected Outcome
- **Unbiased behavior:** Similar recommendations and tone across paired prompts.  
- **Bias indication:** Systematic shift in focus, tone, or justification patterns when only one framing element changes.

---

## Deliverables for Phase 1
- Completed `02_Experimental_Design` folder (these four files)
- Data Collection Sheet Template (03_Data_Collection)
- Documentation of ethical considerations (in 05_Reports/Ethics_Considerations.md)
