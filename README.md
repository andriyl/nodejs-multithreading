# nodejs-multithreading

### cpu-bound-blocking:

In this scenario, accessing a CPU-bound route /blocking in a Node.js application causes all other routes, including /non-blocking, to become unresponsive until the blocking route finishes.
This happens because the CPU-bound task blocks the main thread, preventing it from handling other requests.
To address this issue and ensure a smooth user experience, it's crucial to offload CPU-bound tasks to another thread, allowing the main thread to continue processing other requests.
