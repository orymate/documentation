```yaml title="config.yaml"
# Main configuration flags : https://www.pomerium.com/docs/reference/
pomerium_debug: true
address: :80
cookie_secret: YVFTMIfW8yBJw+a6sYwdW8rHbU+IAAV/SUkCTg9Jtpo=
shared_secret: 80ldlrU2d7w+wVpKNfevk6fmb8otEx6CqOfshj2LwhQ=

idp_provider: "google"
idp_client_id: REPLACE_ME
idp_client_secret: REPLACE_ME

insecure_server: true
forward_auth_url: http://fwdauth.localhost.pomerium.io
authenticate_service_url: https://authenticate.localhost.pomerium.io

policy:
  - from: https://verify.localhost.pomerium.io
    to: https://httpbin
    allowed_domains:
      - pomerium.com
      - gmail.com
    pass_identity_headers: true
```
