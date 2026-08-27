<picture>
  <source media="(prefers-color-scheme: dark)" srcset="restless-init-dark.svg">
  <img width="100%" src="restless-init.svg" alt="Restless">
</picture>

Run in your codebase to get started:

```sh
npx restless init
```

This scans your project, figures out your framework, generates an OpenAPI spec, and automatically wires the SDK into your server.

## The SDKs

| repo | package | works with |
| --- | --- | --- |
| [node](https://github.com/restlesshq/node) | `@restlessai/sdk` | Express, Fastify, Koa, Hono, Next.js, bare `http` |
| [python](https://github.com/restlesshq/python) | `restless-sdk` | Flask, Django, FastAPI, Starlette, anything WSGI or ASGI |
| [ruby](https://github.com/restlesshq/ruby) | `restless-sdk` | Rails, Sinatra, Hanami, Grape, Roda, anything Rack |
| [go](https://github.com/restlesshq/go) | `github.com/restlesshq/go` | net/http, chi, gorilla/mux, Echo, Gin |

Every SDK captures the same thing in the same wire format, and every one of them logs asynchronously. An upload that fails never touches your request path.

[onboarding](https://github.com/restlesshq/onboarding) is what actually runs when you type `npx restless init`. [demo](https://github.com/restlesshq/demo) is a handful of small APIs to try it against.

---

**[restless.ai](https://restless.ai)**
