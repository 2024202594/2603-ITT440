# MUHAMMAD ARIFF BIN MOHD FAUZI
## Problem Statement 
Streaming platforms like Netflix manage millions of watch events daily. Calculating global trends (Top 10) and personalized user recommendations (similarity scores) requires massive computational power. Executing these tasks sequentially on a single CPU core is simply unachievable as it is insufficient. This project explores how Parallelism (Multiprocessing) and Concurrency (Threading) can be used to optimize these calculations, providing a scalable solution for big-data streaming analytics.

## System Requirements

 Python 3.8+, Multi-core CPU (recommended for parallel testing).

## Type Of Methods Used


Sequential Execution: The "Baseline." It processes one user at a time. If user A takes 2 seconds and user B takes 2 seconds, the total is 4 seconds.

Concurrency (Threading): Uses ThreadPoolExecutor. Explain that while it manages multiple tasks, it is limited by the Global Interpreter Lock (GIL) in Python, meaning it doesn't truly run math in parallel on multiple cores.

Parallelism (Multiprocessing): Uses ProcessPoolExecutor. This is the "Winner." It creates a separate memory instance for each CPU core, allowing the computer to perform 4 or 8 calculations at the exact same millisecond.
## Analysis
''' ssh
