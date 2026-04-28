# Security Review Prompts

Use these questions during a focused security pass.

- What untrusted input enters this path?
- Where can that input cross a privilege boundary?
- Could a secret be exposed through logs, docs, prompts, or generated files?
- Does this change make file, network, or execution authority broader than before?
- If configuration is missing or malformed, does the system fail safely?
- Is there any path where the user would assume consent but the code acts without it?
