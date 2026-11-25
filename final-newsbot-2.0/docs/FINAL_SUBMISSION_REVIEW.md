# Final submission review and evidence map

The final capstone extends the original midterm in this repository; the midterm is preserved. Final CI [run 45679903622](https://github.com/jtuozzo1616/Mid-Term-Jose-Group-NewsBot-Intelligence-System/actions/runs/45679903622) completed successfully for code revision `572edc9e6d9ac9c50f2d70315f57712e1e09d9c8`: 27 tests passed, 1 warning; CLI, both research experiments and artifact upload succeeded.

| Requirement | Where to inspect |
|---|---|
| Advanced classification, topic modeling, sentiment | newsbot2/analysis.py, Article Lab, Research Lab |
| Understanding, generation, semantic search | newsbot2/retrieval.py, analysis.py; extractive summarization, templated headlines, LSA, optional multilingual embeddings |
| Multilingual | language.py; pivot, language filter, optional Argos packages |
| Conversational interface | chat.py; citations, follow-up, abstention |
| Web bonus | app.py; five interactive tabs |
| Research bonus | run_research.py; run_robustness.py; artifacts/ |
| Contributions | docs/CONTRIBUTIONS_TO_VERIFY.md; actual student verification required |

The 30 demo articles are fictional. The historical BBC score (96.18% accuracy, 0.9605 macro-F1) belongs exclusively to the midterm. The existing 24 controlled probes achieved MRR@3/Recall@3 1.0 with pivot and 0.625 without; these are in-corpus, selected probes and not an independent benchmark. The 30-item synthetic CV accuracy 0.5667 and macro-F1 0.5371 indicate real weaknesses: do not hide them. The paired feature experiment executed successfully. Results from its CI log:

| Features | Accuracy | Macro-F1 |
|---|---:|---:|
| Word TF-IDF baseline | 0.5667 | 0.5371 |
| Pivot word TF-IDF | 0.6000 | 0.5720 |
| Pivot + character n-grams | 0.6667 | 0.6143 |

Absolute macro-F1 gain: 0.0772 on the same 30 fictional records and same splits. This is not external validation. The CI artifact includes per-record predictions and leave-one-language-out diagnostics.

Canvas requires separately downloaded final instructions and web bonus instructions; those were not supplied. Verify naming, group approval, contribution record, presentation version and all requirements before submitting. No production deployment or neural translation inference is claimed without evidence.
