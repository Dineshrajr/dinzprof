# SuperKart — Automated MLOps Sales Forecasting Pipeline

An end-to-end MLOps pipeline that predicts `Product_Store_Sales_Total` for
SuperKart, with automated data registration, preprocessing, model
training/tuning/evaluation, model registration, and deployment — wired
together with a GitHub Actions CI/CD workflow.

## Links

- **Live app (Streamlit Community Cloud):** `<add after deploying on share.streamlit.io>`
- **Hugging Face dataset:** `<add after first run>`
- **Hugging Face model:** `<add after first run>`
- **GitHub repo:** `<this repo>`

> **Note on hosting:** the deployment code targets a Hugging Face Space
> (Docker SDK) as originally designed. As of 2026, Hugging Face requires a
> **PRO subscription** to run any compute-backed Space (Gradio or Docker)
> on a free account — only static (no-backend) Spaces are free. Since this
> project uses a free HF account, `deployment/hosting.py`'s push to HF
> fails gracefully with a logged 402 (the CI step is marked
> `continue-on-error`, so it doesn't block the rest of the pipeline), and
> the live public demo is instead hosted for free on **Streamlit Community
> Cloud** (see setup below). The app and Dockerfile are unchanged either
> way — only *where* the container/app actually runs differs.

## Folder structure
