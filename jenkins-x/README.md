## Overview

Attempted to setup Jenkins X using Minikube following [this](https://jenkins-x.io/v3/admin/platforms/minikube/) getting started guide.

When getting to the step labelled ['Install the git operator'](https://jenkins-x.io/v3/admin/setup/operator/), after running:

`$ jx admin operator --username <user> --token <token>`

The command hung on the output (last 5 lines):

```bash
jx-basic-auth-user-password: valid: password/password, username/username
lighthouse-hmac-token: valid: hmac/hmac
lighthouse-oauth-token: valid: oauth/oauth
tekton-container-registry-auth: valid: .dockerconfigjson/.dockerconfigjson
tekton-git: valid: password/password, username/username
```

