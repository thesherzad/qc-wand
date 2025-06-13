AI-Assisted QC for Clinical Analysis Ready Datasets

In order to run this project on your own device, you need to have an API Key from an LLM provider (OpenAI is recommended). Store the key in your .Renviron file as `OPENAI_API_KEY`. Read `ellmer` package documentation how to setup a key here: https://ellmer.tidyverse.org/

This repository demonstrates how to use Large Language Models (LLMs) like ChatGPT to automate and assist with Quality Control (QC) tasks in creating clinical Analysis Ready Datasets (ARDs), particularly in highly regulated environments such as the pharmaceutical industry.

It includes examples of:

Creating structured prompts based on CDISC-compliant data specifications

Generating reproducible, tidy R code for common variable derivations

Interacting with LLMs programmatically (e.g., via OpenAI API and the ellmer R package)

Improving QC efficiency while maintaining human oversight and auditability

💡 Note: This work assumes familiarity with clinical trial datasets (SDTM/ADaM), CDISC standards, and R programming.

📌 Why AI for QC?

QC of ARDs often involves repetitive, labor-intensive coding based on structured specs. While AI cannot fully replace human validation (especially in regulated contexts), it can:

Accelerate code generation

Help maintain consistency across studies

Reduce manual errors

Improve documentation and transparency

🔧 Features

⚙️ Prompt Engineering: How to create effective prompts using data specs

🤖 Code Generation: Use LLMs to write R code for derivations

🧪 Imputation Handling: Code examples for missing data (e.g., EXSTDTC, PCSTRESN)

🔍 Comparison Utilities: Compare AI-generated output with source datasets using arsenal::comparedf

📦 Integration with RStudio using rstudioapi::insertText for seamless code insertion

🛠 Technologies Used

R with packages: dplyr, stringr, admiral, skimr, arsenal, Hmisc

ellmer package for interacting with LLMs via API

OpenAI GPT-4 (or other LLMs)

R Markdown for documentation and automation

📎 Disclaimer

This repository is for educational and prototyping purposes only. Any AI-generated output must be reviewed and validated by a qualified clinical programmer or statistician before use in regulated workflows. And thanks to ChatGPT for assisting me to generate this README content :)

