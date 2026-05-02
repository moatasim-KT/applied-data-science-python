# Week 4: Concurrency & Asynchronous I/O for Data Ingestion

## Overview
I/O is often the bottleneck in data science. This week covers techniques to parallelize and overlap I/O operations to significantly speed up data ingestion workflows.

## Key Concepts
### 1. Multi-threading vs. Multi-processing
- **The GIL**: Python’s Global Interpreter Lock (GIL) serializes execution of Python bytecode. Multi-threading helps for I/O-bound tasks (e.g., waiting for API responses), while multi-processing is necessary for CPU-bound tasks (e.g., parallelizing data processing across CPU cores).
- **Executor Pattern**: `concurrent.futures` provides a high-level, consistent interface for managing both types of concurrency.

### 2. Asynchronous Programming with `asyncio`
- **Non-blocking I/O**: `asyncio` allows building highly concurrent programs using an event loop, where one thread manages multiple I/O-bound tasks simultaneously, significantly increasing efficiency compared to standard multi-threading.
- **Async/Await**: Using `async def` and `await` makes asynchronous code readable and easy to reason about, which is essential for building scalable, high-performance data scrapers and API ingestors.
