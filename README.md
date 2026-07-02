ML-Generic Project

A production-ready, opinionated template for building, training, evaluating, and deploying machine learning projects. Use this as a starting point for new ML work so every project ships with the same solid foundation: reproducibility, testing, configuration management, experiment tracking, and deployment tooling built in from day one.



Table of Contents


Why This Template
Features
Project Structure
Getting Started
Configuration
Data
Training
Evaluation
Experiment Tracking
Serving / Inference
Testing
Code Quality
CI/CD
Docker
Reproducibility
Using This as a Template
Contributing
License



Why This Template

Most ML projects start as a notebook and never grow the scaffolding they need to be trustworthy in production: pinned dependencies, config-driven experiments, tests, logging, monitoring hooks, and a repeatable path from raw data to a served model. ML-Generic bakes those practices in up front so teams can focus on modeling instead of re-solving infrastructure problems on every new project.

Features


Config-driven pipelines — every run (data prep, training, evaluation, inference) is controlled by versioned YAML configs, not hardcoded values.
Reproducible environments — pinned dependencies, lockfiles, and a Dockerfile so "works on my machine" isn't a risk.
Modular source layout — clear separation between data, features, models, training, and serving code.
Experiment tracking — integrated hooks for tools like MLflow / Weights & Biases (swap in whichever your team uses).
Testing from day one — unit tests for data transforms and model logic, plus a smoke test for the full pipeline.
Linting, formatting, and type checking pre-configured and enforced via pre-commit hooks.
CI/CD pipeline — lint, test, and build steps ready to plug into GitHub Actions (or your CI of choice).
Model packaging & serving — a minimal, extensible inference service (FastAPI-based) with a Dockerfile for deployment.
Structured logging & config validation to make debugging production issues tractable.


