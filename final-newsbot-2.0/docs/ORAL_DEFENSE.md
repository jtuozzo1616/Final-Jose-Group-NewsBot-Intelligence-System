# Final oral defense — rehearsal guide

**Goal:** demonstrate what you actually understand, not memorize unsupported claims. Suggested 8 minutes; adjust to the instructor's time limit.

| Time | Demonstration | Explanation |
|---|---|---|
| 0:00–0:45 | Open final GitHub README | Midterm classifier became a source-grounded, modular NLP system. |
| 0:45–1:30 | Command Center | Corpus schema, source IDs and synthetic markers; no live news claims. |
| 1:30–2:30 | Article Lab | TF-IDF, classifier origin, NMF and MMR; score is not calibrated probability. |
| 2:30–3:30 | Search & Languages | Spanish or German query; filter sources; explain lexical pivot vs learned vectors. |
| 3:30–4:30 | Grounded Chat | Ask about AI chip researchers; inspect cited source; ask unrelated query to test abstention. |
| 4:30–5:30 | Research Lab | Run CV; discuss macro-F1 and class weaknesses; contrast historical BBC with fictional final corpus. |
| 5:30–6:30 | Executed notebook and evidence | Show real outputs and tests. Show neural evidence only if the run succeeded. |
| 6:30–8:00 | Limitations and personal reflection | Human review, external benchmark, translation validation, calibration and deployment safeguards. |

## Questions to practice (answer in your own words)

1. **Why is the 96.18% not the final model's accuracy?** It is the historical BBC holdout from 288 records; the final fixture is a different task and dataset.
2. **Why use macro-F1?** It weights classes equally, exposing weak minority or hard classes; accuracy alone can conceal them.
3. **How did you prevent leakage?** Feature fitting and classification occur within training folds; held-out predictions use the same partition strategy across alternatives.
4. **What does MMR do?** Selects relevant source sentences while penalizing redundancy; preserves source wording and order.
5. **What is the difference between pivot and embeddings?** A fixed dictionary maps selected terms; learned embeddings map semantic contexts to dense vectors, allowing comparison beyond exact words.
6. **Does a citation make an answer true?** No; it establishes provenance, not accuracy or publisher reliability.
7. **What if a model is missing?** The system reports unavailable or falls back explicitly; no neural success claim is made from the fallback.
8. **Why is 1.0 MRR not definitive?** The 24 selected probes were created with corpus knowledge, not independent annotation.
9. **How would you improve production readiness?** Licensed data, time/publisher holdouts, human evaluation, calibration, access controls, monitoring and editorial review.
10. **What did you personally do?** Describe actual implementation, experimentation, testing, documentation and assistance honestly, following course policy.

## Rehearsal checklist

- Explain one source file and one test without reading notes.
- Run the app and reproduce one cited response and one abstention.
- Explain one incorrect prediction and how you would evaluate a proposed fix.
- Open notebook outputs and the latest evidence run; distinguish verified and pending capabilities.
- Confirm official group label and detailed Canvas instructions with the instructor.
