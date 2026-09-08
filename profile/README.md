# di-framework

<p align="center">
  <img src="https://avatars.githubusercontent.com/u/311964013?v=4" width="128" height="128" alt="di-framework Logo" />
</p>

<p align="center">
  <strong>Lightweight, zero-dependency TypeScript Dependency Injection framework & modular ecosystem.</strong>
</p>

<p align="center">
  <a href="https://docs.di-framework.dev"><img src="https://img.shields.io/badge/docs-docs.di--framework.dev-blue.svg" alt="Documentation" /></a>
  <a href="https://github.com/di-framework/di-framework/actions"><img src="https://github.com/di-framework/di-framework/actions/workflows/ci.yml/badge.svg" alt="CI Status" /></a>
  <a href="https://www.npmjs.com/package/@di-framework/core"><img src="https://img.shields.io/npm/v/@di-framework/core.svg" alt="npm version" /></a>
  <a href="https://github.com/di-framework/di-framework/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT%20OR%20Apache--2.0-blue.svg" alt="License" /></a>
</p>

---

## 🚀 Overview

`di-framework` is a modern, decorator-driven TypeScript Dependency Injection container and comprehensive suite of application companion packages. Designed for maximum performance, minimal footprint, and zero third-party runtime dependencies in core modules, it works seamlessly with TypeScript's native decorator support, `SWC`, `bun`, and `esbuild`.

### Key Highlights

- ⚡ **Zero External Dependencies**: `@di-framework/core` and `@di-framework/auth` carry zero third-party runtime dependencies.
- 🎯 **Native Decorator First**: Elegant `@Container()`, `@Component()`, `@Publisher()`, `@Subscriber()`, and `@Telemetry()` decorators.
- 🔒 **Type-Safe Resolution**: Complete TypeScript type inference across singletons, transient services, and factory registrations.
- 🌐 **Modular Ecosystem**: Dedicated companion packages for HTTP, GraphQL, WebSockets/Sockets, RPC, AI, Auth, AuthZ, Configuration, Events, and Repositories.
- 🛠️ **Developer Experience**: Built-in CLI (`@di-framework/cli`) for scaffolding, typechecking (`init`, `check`, `build`), and custom `ttsc` emit-time parameter guards (`@di-framework/tsc`).

---

## 🗂️ Organization Projects

Public repositories in the organization:

| Project | Description | Site |
| :--- | :--- | :--- |
| [`di-framework`](https://github.com/di-framework/di-framework) | Core monorepo and npm packages | [di-framework.dev](https://di-framework.dev) |
| [`di-framework-kube`](https://github.com/di-framework/kube) | CLI for provisioning isolated Kubesolo clusters with the wasmCloud runtime operator | — |
| [`docs`](https://github.com/di-framework/docs) | Versioned documentation and search | [docs.di-framework.dev](https://docs.di-framework.dev) |
| [`plugin`](https://github.com/di-framework/plugin) | Agent plugin and MCP server for coding assistants | — |
| [`.github`](https://github.com/di-framework/.github) | Organization profile and community health defaults | — |

---

## 📦 Ecosystem Packages

| Package | Description | Version |
| :--- | :--- | :--- |
| [`@di-framework/core`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-core) | Core DI container, decorator metadata, and service resolver | [![npm](https://img.shields.io/npm/v/@di-framework/core.svg)](https://www.npmjs.com/package/@di-framework/core) |
| [`@di-framework/cli`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-cli) | Developer CLI tool (`init`, `check`, `build`, maintainer `mx`) | [![npm](https://img.shields.io/npm/v/@di-framework/cli.svg)](https://www.npmjs.com/package/@di-framework/cli) |
| [`@di-framework/cli-extension`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-cli-extension) | CLI extension authoring API, command types, and manifest contract | [![npm](https://img.shields.io/npm/v/@di-framework/cli-extension.svg)](https://www.npmjs.com/package/@di-framework/cli-extension) |
| [`@di-framework/cli-plugin-wasmcloud`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-cli-plugin-wasmcloud) | CLI extension to build, serve, and deploy apps as wasmCloud WebAssembly components | [![npm](https://img.shields.io/npm/v/@di-framework/cli-plugin-wasmcloud.svg)](https://www.npmjs.com/package/@di-framework/cli-plugin-wasmcloud) |
| [`@di-framework/tsc`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-tsc) | TypeScript compiler transform (`ttsc`) for emit-time type guards | [![npm](https://img.shields.io/npm/v/@di-framework/tsc.svg)](https://www.npmjs.com/package/@di-framework/tsc) |
| [`@di-framework/http`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-http) | Type-safe HTTP routing & build-time OpenAPI 3.1 generation | [![npm](https://img.shields.io/npm/v/@di-framework/http.svg)](https://www.npmjs.com/package/@di-framework/http) |
| [`@di-framework/graphql`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-graphql) | Object-oriented, decorator-driven GraphQL schema generation | [![npm](https://img.shields.io/npm/v/@di-framework/graphql.svg)](https://www.npmjs.com/package/@di-framework/graphql) |
| [`@di-framework/events`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-events) | Event bus bridging `@Publisher`/`@Subscriber` to Kafka, NATS, Memory | [![npm](https://img.shields.io/npm/v/@di-framework/events.svg)](https://www.npmjs.com/package/@di-framework/events) |
| [`@di-framework/socket`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-socket) | Security-first WebCrypto WebSocket, TCP, and UDP communication | [![npm](https://img.shields.io/npm/v/@di-framework/socket.svg)](https://www.npmjs.com/package/@di-framework/socket) |
| [`@di-framework/rpc`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-rpc) | Decorator-generated JSON-RPC & per-method gRPC with typed clients | [![npm](https://img.shields.io/npm/v/@di-framework/rpc.svg)](https://www.npmjs.com/package/@di-framework/rpc) |
| [`@di-framework/config`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-config) | Typed, validated configuration injection from env/files | [![npm](https://img.shields.io/npm/v/@di-framework/config.svg)](https://www.npmjs.com/package/@di-framework/config) |
| [`@di-framework/cloudfoundry`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-cloudfoundry) | Cloud Foundry service discovery, application metadata, and automatic DI bindings | [![npm](https://img.shields.io/npm/v/@di-framework/cloudfoundry.svg)](https://www.npmjs.com/package/@di-framework/cloudfoundry) |
| [`@di-framework/auth`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-auth) | Sessions, JWT, OAuth2/OIDC, and WebAuthn passkeys on WebCrypto | [![npm](https://img.shields.io/npm/v/@di-framework/auth.svg)](https://www.npmjs.com/package/@di-framework/auth) |
| [`@di-framework/authz`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-authz) | Resource-level authorization policies, EBNF rules & HTTP bindings | [![npm](https://img.shields.io/npm/v/@di-framework/authz.svg)](https://www.npmjs.com/package/@di-framework/authz) |
| [`@di-framework/ai`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-ai) | Annotation-driven Chat, Tools, RAG, MCP, and AI Agents | [![npm](https://img.shields.io/npm/v/@di-framework/ai.svg)](https://www.npmjs.com/package/@di-framework/ai) |
| [`@di-framework/ai-utils`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-ai-utils) | Agent Skills (`SKILL.md`) toolbox (`SkillsAgent.builder`) | [![npm](https://img.shields.io/npm/v/@di-framework/ai-utils.svg)](https://www.npmjs.com/package/@di-framework/ai-utils) |
| [`@di-framework/repo`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-repo) | Storage-agnostic repository abstractions and standardized data access | [![npm](https://img.shields.io/npm/v/@di-framework/repo.svg)](https://www.npmjs.com/package/@di-framework/repo) |
| [`@di-framework/codegen`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-codegen) | Contract-driven code generation for typed service interfaces | [![npm](https://img.shields.io/npm/v/@di-framework/codegen.svg)](https://www.npmjs.com/package/@di-framework/codegen) |

---

## 💻 Quick Example

```typescript
import { Container, Publisher, Subscriber } from '@di-framework/core/decorators';

@Container()
class UserService {
  @Publisher('user.created')
  createUser(name: string) {
    return { id: 1, name };
  }
}

@Container()
class AuditService {
  @Subscriber('user.created')
  onUserCreated(event: any) {
    console.log('User created:', event.result);
  }
}
```

---

## 🛠️ Getting Started

Scaffold a new project in seconds using the CLI:

```bash
bun x @di-framework/cli init my-app
# or
npx @di-framework/cli init my-app
```

Check and build your application:

```bash
bun run check
bun run build
```

---

## 📚 Documentation & Resources

- 📖 **Documentation**: [docs.di-framework.dev](https://docs.di-framework.dev)
- 🏠 **Website**: [di-framework.dev](https://di-framework.dev)
- 📦 **Monorepo Repository**: [github.com/di-framework/di-framework](https://github.com/di-framework/di-framework)
- 📝 **Migration Guide**: [MIGRATION_GUIDE.md](https://github.com/di-framework/di-framework/blob/main/packages/di-framework-core/MIGRATION_GUIDE.md)
- 📄 **Packaging Policy**: [PACKAGING.md](https://github.com/di-framework/di-framework/blob/main/PACKAGING.md)
- 🔒 **Security Policy**: [SECURITY.md](https://github.com/di-framework/di-framework/blob/main/SECURITY.md)

---

## 📄 License

Dual-licensed under either the [MIT License](https://opensource.org/licenses/MIT) or the [Apache License (Version 2.0)](https://www.apache.org/licenses/LICENSE-2.0).
