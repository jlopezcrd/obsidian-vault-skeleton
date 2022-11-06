---
tags: "#type/personal"
---

```bash
#!/bin/bash

git add .
git commit -m "vault manual backup: $(date +'%Y-%m-%d %H:%M:%S')"
git push
