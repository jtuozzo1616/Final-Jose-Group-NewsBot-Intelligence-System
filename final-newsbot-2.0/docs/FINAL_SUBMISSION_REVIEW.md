# Final submission review and evidence map

The final capstone extends the original midterm in this repository; the midterm is preserved. The prior final CI [run 42949516096](https://github.com/jtuozzo1616/Mid-Term-Jose-Group-NewsBot-Intelligence-System/actions/runs/42949516096) completed successfully. New changes require a fresh run.

| Requirement | Where to inspect |
|---|---|
| Advanced classification, topic modeling, sentiment | newsbot2/analysis.py, Article Lab, Research Lab |
| Understanding, generation, semantic search | newsbot2/retrieval.py, analysis.py; extractive summarization, templated headlines, LSA, optional multilingual embeddings |
| Multilingual | language.py; pivot, language filter, optional Argos packages |
| Conversational interface | chat.py; citations, follow-up, abstention |
| Web bonus | app.py; five interactive tabs |
| Research bonus | run_research.py; run_robustness.py; artifacts/ |
| Contributions | docs/CONTRIBUTIONS_TO_VERIFY.md; actual student verification required |

The 30 demo articles are fictional. The historical BBC score (96.18% accuracy, 0.9605 macro-F1) belongs exclusively to the midterm. The existing 24 controlled probes achieved MRR@3/Recall@3 1.0 with pivot and 0.625 without; these are in-corpus, selected probes and not an independent benchmark. The 30-item synthetic CV accuracy 0.5667 and macro-F1 0.5371 indicate real weaknesses: do not hide them. The added paired feature and language-holdout experiment is executable but results must be generated and inspected, not presumed.

Canvas requires separately downloaded final instructions and web bonus instructions; those were not supplied. Verify naming, group approval, contribution record, video version and all requirements before submitting. No production deployment or neural translation inference is claimed without evidence.
