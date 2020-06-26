
To Future developer of LINZ:

The reason that this repo existed (before April 2019)
This library mainly supports OIDC, thus the typical use of id_token token. code is only for use in server-side web apps (until the spec committees make other recommendations, but that's beyond this conversation). That leaves them only supporting token, which is not OIDC.


Now it can be removed if you agree with the statment in the link below and implement correctly what they recommend. I hope I was able to implement this before closing the issue.

[This workaround of the repo is **NOT** needed if the following can be done](https://github.com/IdentityModel/oidc-client-js/issues/645)

The library is pretty well designed, so you can replace the ResponseValidator implementation through the oidcSettings :
gravedigging a bit, but I've found it easiest to work around this by constructing my UserManager and overrriding

