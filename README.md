# Doppy

Doppy is a minimal DSL for AI data pipelines.

It provides a declarative syntax to define datasets, models, and evaluation workflows with clarity and simplicity.

## Vision

Modern AI workflows are complex and fragmented.

Doppy introduces a minimal orchestration layer focused on readability, structure, and developer experience.

## Example

```doppy
dataset "tn_qa" {
  source: "data.csv"
  min_quality: 0.8
}

model "tn_model" {
  base: "qwen-7b"
  train_on: "tn_qa"
}