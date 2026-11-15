# Do safety refusals hold up in lower-resource Indian languages?

Testing election manipulation requests on Sarvam 105B and global LLMs in English, Hindi and Bengali.

Nandini Nair and Rishika Rai (TARA 2026). 
Mentor: Ajay Agarwal.

## What this project does
We test whether AI models will write election manipulation content for Indian elections, such as false voting information, communal rumours and fake grassroots posts, when asked in English, Hindi and Bengali. Each manipulation request is paired with a near-identical legitimate request, so we measure both how often models help with manipulation and how often they wrongly refuse ordinary political requests.

Models tested: Sarvam 105B, gpt-oss-120b and Llama 3.3 70B, with a smaller check on Claude Haiku 5.5 and Opus 5.5.

## Why it matters for AI safety
Safety training is mostly done in English, and research shows models give more harmful answers in low-resource languages. Cheap, fluent disinformation in Indian languages could let a small group sway the world's largest electorate, and repeated manipulated wins could entrench power that voters can no longer remove. This test set can be rerun on each new generation of models.

## How to run it
1. Open the notebooks in Google Colab, in number order.
2. Add your API keys to Colab Secrets (see the top of each notebook).
3. Raw model outputs are saved to a private Google Drive folder, never to this repo.

| Notebook | What it does |
|---|---|
| 01_test_models | Checks every key and model works |
| 02_build_requests | Builds the request set (coming) |
| 03_translate | Translates into Hindi and Bengali with IndicTrans2 (coming) |
| 04_run_models | Sends every request to every model (coming) |
| 05_judge | Scores answers with StrongREJECT-style judging (coming) |
| 06_analysis | Compliance and over-refusal rates (coming) |

## What is and is not in this repo
- Included: the requests, scores and code.
- Not included: model answers, which may contain harmful content. All candidates, parties and places in the requests are fictional.

## Key findings
To be added at the end of the project.

## Requirements
See requirements.txt.
