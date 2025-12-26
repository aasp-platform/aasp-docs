# CLAUDE.md

This file provides context to AI coding assistants (Claude Code, Cursor, etc.) when working with this codebase.

## Project Overview

AASP Docs is the documentation site for the AI Agent Security Platform. It provides guides, API reference, tutorials, and examples for users and developers.

## Tech Stack

- **Framework**: Next.js (App Router)
- **Content**: MDX (Markdown with React components)
- **Styling**: Tailwind CSS
- **Code Highlighting**: Shiki

## Commands

```bash
# Development
pnpm dev          # Start dev server at http://localhost:3000
pnpm build        # Production build
pnpm start        # Start production server

# Content
pnpm lint         # Lint code and content
```

## Directory Structure

```
docs/
├── getting-started/
│   ├── introduction.md
│   ├── quickstart.md
│   └── concepts.md
├── sdk/
│   ├── installation.md
│   ├── langchain.md
│   └── custom-agents.md
├── policies/
│   ├── creating-policies.md
│   └── rule-syntax.md
├── api/
│   ├── authentication.md
│   ├── ingest.md
│   └── policies.md
└── deployment/
    └── self-hosted.md
```

## Writing Guidelines

### Content Style

- **Be concise**: Developers skim, every word counts
- **Show code**: Examples > explanations
- **Test snippets**: All code must work
- **Use headers**: Enable easy navigation

### MDX Components

```mdx
import { Callout } from '@/components/Callout'
import { CodeBlock } from '@/components/CodeBlock'

<Callout type="warning">
  Important warning message here.
</Callout>

<CodeBlock language="python" filename="example.py">
{`from aasp_sdk import AASPCallback`}
</CodeBlock>
```

### Code Examples

Always include:
- Language identifier
- Filename when relevant
- Complete, runnable code
- Comments for complex logic

```python
# Install the SDK
pip install aasp-sdk

# Basic usage
from aasp_sdk import AASPCallback

callback = AASPCallback(api_key="aasp_live_xxx")
```

## Common Tasks

### Adding a new doc page

1. Create `.md` or `.mdx` file in appropriate directory
2. Add frontmatter with title and description
3. Update navigation in `src/config/navigation.ts`

### Adding a code example

1. Test the code works with current SDK version
2. Use appropriate language highlighting
3. Include error handling for production examples

### Updating API reference

1. Sync with actual API endpoints in aasp-server
2. Include request/response examples
3. Document error responses

## Important Notes

- Keep in sync with aasp-server and aasp-sdk changes
- All code examples should work with latest SDK version
- Test links before publishing
- Images should be optimized and in `/public/`
