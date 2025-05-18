
[[Flows and Tasks in Prefect]] support the ability to cache their return value. Caching allows you to efficiently reuse [results](https://docs.prefect.io/concepts/results/) of tasks that may be expensive to reproduce with every flow run, or reuse cached results if the inputs to a task have not changed.

To enable caching, specify a `cache_key_fn` — a function that returns a cache key — on your task. You may optionally provide a `cache_expiration` timedelta indicating when the cache expires. You can define a task that is cached based on its inputs by using the Prefect [`task_input_hash`](https://docs.prefect.io/api-ref/prefect/tasks/#prefect.tasks.task_input_hash)

Example in my [repo_info_print.py](https://github.com/Filbog/prefect-practice) in this GH repo
