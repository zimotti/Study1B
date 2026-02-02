# A Framework for Verb Annotation of Spanish L2 Written Corpora Using Local LLMs (Study0B)

A specialized research tool for Applied Linguists to analyze Spanish Second Language Acquisition (SLA) data.

This pipeline connects local Large Language Models (via Ollama) to your participants data to automate the extraction of **Suppliance in Obligatory Contexts (SOC)**. It uses a sliding-window approach to correctly identify tense (Preterite vs. Imperfect) based on narrative context.

---

## Which LLM? 

| LLM | Detection Recall | Tense ID Accuracy | Error Status Accuracy | Cohen's Kappa | N. of Tense Disagreements |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **gpt-oss:120b** | 93.2% | 92.0% | 94.9% | 0.893 | 11 |
| **gemma3:27b** | 88.5% | 82.4% | 80.2% | 0.580 | 23 |
| **gemma3:12b** | 82.4% | 81.1% | 79.5% | 0.558 | 23 |
| **gemma3:1b** | 43.9% | 52.3% | 30.8% | -0.139 | 31 |
| **llama3.3:70b** | 87.8% | 90.0% | 88.5% | 0.742 | 13 |
| **llama3.3:70b-instruct-q4_K_M** | 87.2% | 91.5% | 86.0% | 0.684 | 11 |
| **llama3.1:8b** | 70.9% | 49.5% | 64.8% | 0.282 | 53 |
| **mistral-small3.2:24b** | 89.9% | 87.2% | 87.2% | 0.720 | 17 |
| **mixtral:8x22b** | 78% | 71.3% | 72.2% | 0.425 | 33 |
| **mistral-nemo:12b** | 45.3% | 47.8% | 47.8% | 0.000 | 35 |
