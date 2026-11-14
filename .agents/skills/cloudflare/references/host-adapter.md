# Shared-library host guidance

Apply the Cloudflare workflow within the user's request and the current host's
instructions. Use tools actually available here. The skills are instructions,
references, and optional scripts; installing them does not connect a Cloudflare
account or grant permission to deploy, change DNS, write secrets, send email,
post feedback, or change account resources.

Prefer an available connected Cloudflare tool when it supports the requested
operation. Otherwise use the project's existing CLI and package manager. Fetch
the linked official documentation when a named MCP or documentation tool is
unavailable. Report a missing capability when no equivalent can produce the
needed evidence. Do not claim to have measured performance without a capture.

Setup examples apply when setup is part of the task. Check installed tools
before installing packages, authenticating, adding upstream skills, or changing
global agent instructions or MCP configuration. Preserve the existing project's
Wrangler or `cf` choice. The upstream `nextjs-on-cloudflare` workflow may require
skills maintained separately in `cloudflare/vinext`; they are not bundled here.

For Turnstile, resolve the bundled scripts from the skill's own directory before
invoking them. The repository already installs this bundle for reuse, so the
upstream per-project persistence step is optional and applies only if the user
wants another project-local copy. Keep the upstream widget, hostname, secret,
and live-validation safeguards when executing an authorized setup.

These skills overlap the separately installed Cloudflare plugin. Prefer one
current source for a task rather than loading duplicate versions. Read only
the product references required by the assignment.
