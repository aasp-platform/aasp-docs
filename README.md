<p align="center">
  <img src="https://harbyx.com/logos/harbyx_logo.jpeg" alt="AASP Logo" width="120" />
</p>

<h1 align="center">AASP Documentation</h1>

<p align="center">
  <strong>Complete documentation for the AI Agent Security Platform</strong><br>
  Guides, API reference, tutorials, and examples.
</p>

<p align="center">
  <a href="https://aasp-mvp.aminereg.com/docs"><img src="https://img.shields.io/badge/docs-live-brightgreen?style=for-the-badge" alt="Live Docs"></a>
  <a href="https://github.com/aasp-platform/aasp-docs/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="License"></a>
  <a href="https://github.com/aasp-platform/aasp-docs/issues"><img src="https://img.shields.io/github/issues/aasp-platform/aasp-docs?style=for-the-badge" alt="Issues"></a>
</p>

---

## Documentation Structure

```
docs/
├── getting-started/
│   ├── introduction.md      # What is AASP?
│   ├── quickstart.md        # 5-minute setup
│   └── concepts.md          # Core concepts
├── sdk/
│   ├── installation.md      # SDK installation
│   ├── langchain.md         # LangChain integration
│   ├── crewai.md            # CrewAI integration
│   └── custom-agents.md     # Custom agent integration
├── policies/
│   ├── creating-policies.md # Policy creation guide
│   ├── rule-syntax.md       # Rule syntax reference
│   └── templates.md         # Policy templates
├── dashboard/
│   ├── overview.md          # Dashboard features
│   ├── approvals.md         # Human-in-the-loop
│   └── audit-log.md         # Action audit trail
├── api/
│   ├── authentication.md    # API key management
│   ├── ingest.md            # Ingest endpoint
│   ├── policies.md          # Policy API
│   └── approvals.md         # Approval API
├── deployment/
│   ├── self-hosted.md       # Self-hosted deployment
│   ├── docker.md            # Docker deployment
│   └── production.md        # Production best practices
└── security/
    ├── best-practices.md    # Security guidelines
    └── compliance.md        # SOC2, GDPR compliance
```

---

## Quick Links

| Section | Description | Link |
|---------|-------------|------|
| **Quickstart** | Get running in 5 minutes | [View](https://aasp-mvp.aminereg.com/docs#quickstart) |
| **SDK Reference** | Python SDK documentation | [View](https://aasp-mvp.aminereg.com/docs#sdk) |
| **API Reference** | REST API documentation | [View](https://aasp-mvp.aminereg.com/docs#api) |
| **Policy Templates** | Ready-to-use policies | [View](https://github.com/aasp-platform/policy-library) |

---

## Local Development

### Prerequisites

- Node.js 20+
- pnpm

### Setup

```bash
# Clone the repository
git clone https://github.com/aasp-platform/aasp-docs.git
cd aasp-docs

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

Visit `http://localhost:3000` to view the docs locally.

### Building

```bash
# Production build
pnpm build

# Preview production build
pnpm start
```

---

## Contributing

We love documentation improvements! Here's how to contribute:

### Quick Edits

1. Click "Edit this page" on any documentation page
2. Make your changes
3. Submit a pull request

### Adding New Content

1. Fork the repository
2. Create a new branch: `git checkout -b docs/my-improvement`
3. Add your content following the existing structure
4. Submit a pull request

### Writing Guidelines

- **Be concise** — Developers skim, make every word count
- **Show, don't tell** — Include code examples
- **Test your examples** — All code snippets should work
- **Use consistent formatting** — Follow existing patterns

### Good First Issues

Look for issues labeled [`good-first-issue`](https://github.com/aasp-platform/aasp-docs/labels/good-first-issue) or [`documentation`](https://github.com/aasp-platform/aasp-docs/labels/documentation).

---

## Documentation Stack

| Tool | Purpose |
|------|---------|
| **Next.js** | Documentation site framework |
| **MDX** | Markdown with React components |
| **Tailwind CSS** | Styling |
| **Shiki** | Code syntax highlighting |

---

## Related Projects

| Project | Description |
|---------|-------------|
| [aasp-server](https://github.com/aasp-platform/aasp-server) | Main AASP server |
| [aasp-sdk](https://github.com/aasp-platform/aasp-sdk) | Python SDK |
| [policy-library](https://github.com/aasp-platform/policy-library) | Policy templates |

---

## License

MIT License - see [LICENSE](LICENSE) for details.

Documentation content is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

<p align="center">
  <strong>Built by <a href="https://harbyx.com">Harbyx</a></strong><br>
  <sub>Making AI agent security accessible to everyone.</sub>
</p>
