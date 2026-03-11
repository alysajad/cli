---
"gws": patch
---

Resolve TOCTOU race condition in `fs_util::atomic_write` and `atomic_write_async` to securely enforce 0600 file permissions upon file creation, preventing intermediate local read access to secrets.
