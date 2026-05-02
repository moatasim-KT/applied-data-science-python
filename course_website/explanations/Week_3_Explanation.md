
## Practice
Practice functional programming techniques by tackling the higher-order function and closure exercises on [Exercism](https://exercism.org/tracks/python). These challenges will help you become comfortable using functional idioms to write concise and modular data transformation code.
# Week 3: Functional Programming & Decorators

## Overview
Functional programming simplifies data transformations, while decorators allow for clean, non-intrusive extension of existing functionality—key for data pipelines.

## Key Concepts
### 1. Lambda, Map, and Filter
- **Declarative Style**: `lambda` functions, `map`, and `filter` allow for concise, functional data transformations. They are especially powerful when applied to iterables, helping to keep code focused on the "what" rather than the "how" of iteration.

### 2. Decorators
- **Behavioral Extension**: Decorators allow you to wrap functions to add side-effect behavior (e.g., timing execution, logging data ingress/egress, caching results) without changing the core function logic.
- **DRY Principle**: They help prevent code duplication across different parts of a project, such as applying the same validation logic to multiple functions in a pipeline.
