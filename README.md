# RAG Evaluation Tools Benchmark

A comparison of W&B Weave, Ragas, DeepEval, TruLens, and UpTrain on how they score the relevance of retrieved passages for retrieval-augmented generation.

[Read the benchmark on AIMultiple](https://aimultiple.com/rag-evaluation-tools).

Each question is paired with five passages, including a relevant passage and adversarial alternatives. Some alternatives retain the topic while changing an entity or fact needed to answer the question. The evaluation examines whether each tool can distinguish useful evidence from these close matches.

The tools use GPT-4o with their default evaluation prompts and receive the same question and context inputs. Reported metrics include Top-1 accuracy and ranking quality across the five passages.

Tie handling matters because the tools return scores on different scales. The article distinguishes ordinary Top-1 accuracy from the stricter requirement that the reference passage receive the unique highest score. The results apply to this evaluation task. They do not measure every aspect of a complete RAG system.

The benchmark implementation was developed for AIMultiple and belongs to AIMultiple. This repository is a documentation summary. Source code and benchmark datasets are not distributed here.
