# Home Assistant App: NGINX Home Assistant SSL proxy

Source repository of the [NGINX Home Assistant SSL proxy][docs] app for Home Assistant.
Users install the app from the [official app repository][index].

## Releases

- Every push to `main` builds and publishes the image tagged `dev` and with the short commit SHA.
  These builds can be installed from the [development app repository][dev].
- Publishing a GitHub release builds the image tagged with the release version and `stable`.
  The release notes become the app changelog in the [official app repository][index].

Images are signed with Cosign and published to `ghcr.io/home-assistant/app-nginx-proxy`.

## Local build

```sh
docker build -t local/app-nginx-proxy nginx_proxy
```

[index]: https://github.com/home-assistant/apps
[dev]: https://github.com/home-assistant/apps-dev
[docs]: nginx_proxy/DOCS.md
