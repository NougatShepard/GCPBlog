---
title: Use gsutil to deploy local contents to gcs
abbrlink: 4a17b156
date: 2020-11-23 21:21:49
tags: GCP
---
Install gsutil from PyPI.

```
pip install gsutil
```

Open google cloud sdk shell.

gsutil commands:

Do not use uniform bucket-level access.

The "defacl set" command:

```
gsutil defacl set public-read gs://www.example.com
```

The gsutil rsync command:

```
gsutil -m rsync -R local-dir gs://www.example.com
```

References:
<https://cloud.google.com/storage/docs/gsutil>