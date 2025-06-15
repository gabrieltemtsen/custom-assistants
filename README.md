
# 🧠 Crypto Agent Starter – Powered by ElizaOS

Kickstart your own crypto-native agent assistant with this ElizaOS starter template.

This template is designed to help you build intelligent, modular, and highly customizable agents capable of assisting users in web3 environments—from handling smart contract queries to surfacing onchain data and plugin-powered workflows.

## ✨ Features

- ⚙️ Pre-configured project structure for ElizaOS agent development
- 🧪 Built-in test suite: unit, integration, and end-to-end
- 🧠 Default character setup with plugin and action integration
- 🧩 Example service, provider, and action implementations
- 🛠 TypeScript-first developer experience
- 📘 Built-in examples and documentation for quick ramp-up

---

## 🚀 Getting Started

Create and launch your custom crypto assistant in seconds:

```bash
# Scaffold a new project using the ElizaOS CLI
elizaos create -t project my-agent

# Navigate to your project
cd my-agent

# Start the agent with hot-reloading
elizaos dev
```

---

## ⚒️ Development Workflow

```bash
# Recommended: Start in dev mode with live reload
elizaos dev

# Production-like runtime (no reload)
elizaos start

# Rebuild manually when using 'start':
bun run build

# Run full test suite
elizaos test
```

---

## ✅ Testing Your Agent

Testing is core to ElizaOS development. This starter supports:

### 🔬 Component Tests (`__tests__/`)
- **Unit Tests**: Validate logic in isolation
- **Integration Tests**: Verify plugin-character interaction
- Run with: `elizaos test component`

### 🌐 E2E Tests (`e2e/`)
- Run your agent in a full ElizaOS runtime
- Validate real-world interactions
- Run with: `elizaos test e2e`

### 💡 Example Test

```ts
// Unit test (__tests__/config.test.ts)
describe('Agent Config', () => {
  it('should load with defaults', () => {
    expect(config.debug).toBeDefined();
  });
});

// E2E test (e2e/project.test.ts)
export class ProjectTestSuite implements TestSuite {
  name = 'project_test_suite';
  tests = [
    {
      name: 'project_initialization',
      fn: async (runtime) => {
        // Simulate full agent runtime
      },
    },
  ];
}

export default new ProjectTestSuite();
```

> Utilities in `__tests__/utils/` simplify repetitive test patterns.

---

## 🧬 Customize Your Agent

Personalize your agent’s logic and behavior by editing:

- `src/index.ts` – Entry point to your assistant
- `src/character.ts` – Define your assistant's identity, skills, and voice
- Add new services, actions, and plugins to extend capabilities

---

## 🧠 Use Cases

Your ElizaOS agent can become:
- A DeFi companion that explains onchain actions
- A wallet assistant that summarizes activity
- A governance guide for DAOs
- A modular framework for multi-chain crypto agents

---

## 👾 Ready to Build?

Start creating your crypto-native assistant today, powered by ElizaOS.
