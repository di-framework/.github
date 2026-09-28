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
| [`di-framework`](https://github.com/di-framework/di-framework) | Core monorepo: DI, HTTP, GraphQL, events, auth, RPC, queues, actors, and the app CLI | [di-framework.dev](https://di-framework.dev) |
| [`ai`](https://github.com/di-framework/ai) | AI clients, tools, agents, and Agent Skills (`@di-framework/ai`, `@di-framework/ai-utils`) | — |
| [`platform`](https://github.com/di-framework/platform) | Operated wasmCloud platform: Pulumi installer, guest bindings, and the Cloud Foundry adapter | — |
| [`cli-extensions`](https://github.com/di-framework/cli-extensions) | Installable command groups (`@di-framework/cli-plugin-platform`) | — |
| [`examples`](https://github.com/di-framework/examples) | Sample applications for the framework, platform, and adapters | — |
| [`kube`](https://github.com/di-framework/kube) | CLI for provisioning isolated Kubesolo clusters with the wasmCloud runtime operator | — |
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
| [`@di-framework/cli-plugin-platform`](https://github.com/di-framework/cli-extensions/tree/main/packages/cli-plugin-platform) | CLI extension to build, serve, and deploy apps as wasmCloud WebAssembly components (`di-framework platform`) | [![npm](https://img.shields.io/npm/v/@di-framework/cli-plugin-platform.svg)](https://www.npmjs.com/package/@di-framework/cli-plugin-platform) |
| [`@di-framework/platform`](https://github.com/di-framework/platform/tree/main/platform/platform) | Cluster install: Pulumi, CRDs, controller, tenancy, and backing services | [![npm](https://img.shields.io/npm/v/@di-framework/platform.svg)](https://www.npmjs.com/package/@di-framework/platform) |
| [`@di-framework/bindings`](https://github.com/di-framework/platform/tree/main/platform/bindings) | Application guest bindings and workload metadata. Through 5.x this was `@di-framework/wasmcloud` | [![npm](https://img.shields.io/npm/v/@di-framework/bindings.svg)](https://www.npmjs.com/package/@di-framework/bindings) |
| [`@di-framework/tsc`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-tsc) | TypeScript compiler transform (`ttsc`) for emit-time type guards | [![npm](https://img.shields.io/npm/v/@di-framework/tsc.svg)](https://www.npmjs.com/package/@di-framework/tsc) |
| [`@di-framework/http`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-http) | Type-safe HTTP routing & build-time OpenAPI 3.1 generation | [![npm](https://img.shields.io/npm/v/@di-framework/http.svg)](https://www.npmjs.com/package/@di-framework/http) |
| [`@di-framework/graphql`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-graphql) | Object-oriented, decorator-driven GraphQL schema generation | [![npm](https://img.shields.io/npm/v/@di-framework/graphql.svg)](https://www.npmjs.com/package/@di-framework/graphql) |
| [`@di-framework/events`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-events) | Event bus bridging `@Publisher`/`@Subscriber` to Kafka, NATS, Memory | [![npm](https://img.shields.io/npm/v/@di-framework/events.svg)](https://www.npmjs.com/package/@di-framework/events) |
| [`@di-framework/socket`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-socket) | Security-first WebCrypto WebSocket, TCP, and UDP communication | [![npm](https://img.shields.io/npm/v/@di-framework/socket.svg)](https://www.npmjs.com/package/@di-framework/socket) |
| [`@di-framework/rpc`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-rpc) | Decorator-generated JSON-RPC & per-method gRPC with typed clients | [![npm](https://img.shields.io/npm/v/@di-framework/rpc.svg)](https://www.npmjs.com/package/@di-framework/rpc) |
| [`@di-framework/config`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-config) | Typed, validated configuration injection from env/files | [![npm](https://img.shields.io/npm/v/@di-framework/config.svg)](https://www.npmjs.com/package/@di-framework/config) |
| [`@di-framework/cloudfoundry`](https://github.com/di-framework/platform/tree/main/adapters/cloudfoundry) | Cloud Foundry service discovery, application metadata, and automatic DI bindings | [![npm](https://img.shields.io/npm/v/@di-framework/cloudfoundry.svg)](https://www.npmjs.com/package/@di-framework/cloudfoundry) |
| [`@di-framework/auth`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-auth) | Sessions, JWT, OAuth2/OIDC, and WebAuthn passkeys on WebCrypto | [![npm](https://img.shields.io/npm/v/@di-framework/auth.svg)](https://www.npmjs.com/package/@di-framework/auth) |
| [`@di-framework/authz`](https://github.com/di-framework/di-framework/tree/main/packages/di-framework-authz) | Resource-level authorization policies, EBNF rules & HTTP bindings | [![npm](https://img.shields.io/npm/v/@di-framework/authz.svg)](https://www.npmjs.com/package/@di-framework/authz) |
| [`@di-framework/ai`](https://github.com/di-framework/ai/tree/main/ai) | Annotation-driven Chat, Tools, RAG, MCP, and AI Agents | [![npm](https://img.shields.io/npm/v/@di-framework/ai.svg)](https://www.npmjs.com/package/@di-framework/ai) |
| [`@di-framework/ai-utils`](https://github.com/di-framework/ai/tree/main/ai-utils) | Agent Skills (`SKILL.md`) toolbox (`SkillsAgent.builder`) | [![npm](https://img.shields.io/npm/v/@di-framework/ai-utils.svg)](https://www.npmjs.com/package/@di-framework/ai-utils) |
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

## 🤖 Build AI Applications

The [AI repository](https://github.com/di-framework/ai) contains chat clients, tool calling, conversation memory, RAG, MCP, and agent workflows. Use the fluent APIs directly or wire them into the DI container. Add `@di-framework/ai-utils` for Agent Skills and repository tools.

### Chat with a model

Install the AI package and its peers. AI packages use version 6; core and auth peers remain on version 5.

```bash
bun add @di-framework/ai@^6 @di-framework/core@^5 @di-framework/auth@^5
bun add --dev typescript@^5
```

Save this as `chat.ts`:

```typescript
import { ChatClient, createChatModel } from '@di-framework/ai';

const client = ChatClient.builder(createChatModel())
  .defaultSystem('You are a concise, helpful assistant.')
  .build();

const answer = await client
  .prompt('Explain dependency injection in two sentences.')
  .call()
  .content();

console.log(answer);
```

Set your provider's API key in the environment, then run with Bun:

```bash
# Requires OPENAI_API_KEY:
PROVIDER=openai AUTH=api bun chat.ts

# Or, with ANTHROPIC_API_KEY:
PROVIDER=anthropic AUTH=api bun chat.ts
```

Set `MODEL` to select a model explicitly. To try the client without credentials, import `FakeChatModel` and replace `createChatModel()` with `new FakeChatModel('Hello!')`.

### Give an agent a skill

```bash
bun add @di-framework/ai-utils@^6
```

Create `.agents/skills/code-reviewer/SKILL.md` in your project:

```markdown
---
name: code-reviewer
description: Review TypeScript code for correctness. Use when asked to review code.
---

# Code review

1. Read the requested file.
2. Identify correctness issues and explain their impact.
3. Suggest a concrete fix for each issue.
```

Save this as `review.ts` and run it from your project directory with the same provider environment as the chat example. Replace `src/index.ts` with the file you want reviewed.

```typescript
import { createChatModel } from '@di-framework/ai';
import { SkillsAgent } from '@di-framework/ai-utils';

const agent = SkillsAgent.builder()
  .chatModel(createChatModel())
  .system('Help review TypeScript code. Use the code-reviewer skill when reviewing.')
  .workspace(process.cwd())
  .addSkillsDirectory('.agents/skills')
  .build();

const reply = await agent.chat('Review src/index.ts.');
console.log(reply.content);
```

Skills expose descriptions first and load their full instructions when activated. The default toolbox includes file-reading tools; writing, editing, and shell execution are opt-in.

See the [AI usage guide](https://github.com/di-framework/ai#readme), [AI package documentation](https://github.com/di-framework/ai/blob/main/ai/README.md), and [skills and utilities documentation](https://github.com/di-framework/ai/blob/main/ai-utils/README.md) for more examples. The `di-framework agent` and `di-framework skills` CLI commands remain in the [core monorepo](https://github.com/di-framework/di-framework).

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
