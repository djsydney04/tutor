# Cloudflare source and import notes

The 19 Cloudflare skill directories in this repository are adapted from
[Cloudflare's official skills repository](https://github.com/cloudflare/skills),
at commit
[`1a33048817d06df12882cb881dfc754e7039954a`](https://github.com/cloudflare/skills/tree/1a33048817d06df12882cb881dfc754e7039954a).
The source is licensed under Apache License 2.0; the complete upstream
[LICENSE](LICENSE) is preserved alongside this file. No upstream `NOTICE` file
was present in this snapshot. Original notices inside the imported files remain.

Imported skill directories:

- `agents-sdk`
- `basin`
- `cf-cli`
- `cloudflare`
- `cloudflare-email-service`
- `cloudflare-one`
- `cloudflare-one-migrations`
- `durable-objects`
- `gateway-workers`
- `k2`
- `nextjs-on-cloudflare`
- `sandbox-migrate-to-next`
- `sandbox-next`
- `sandbox-stable`
- `turnstile-spin`
- `web-perf`
- `workers-best-practices`
- `workers-profiling`
- `wrangler`

## Local changes

Each imported `SKILL.md` adds an `Apache-2.0` license field and a prominent
adaptation notice linking the [host guidance](host-adapter.md) and this file.
The upstream names and discovery descriptions remain unchanged. Supporting
references retain their relative layout. Markdown hard breaks use explicit
backslashes instead of trailing spaces, and incidental trailing whitespace was
normalized in six Markdown files for this repository's whitespace check. Shell
scripts and the Turnstile offline regression tests retain their source contents. No unsupported metadata fields were
present in the imported entrypoints.

The Basin SQL troubleshooting checklist uses a non-revealing token-presence
check instead of printing the authentication token into terminal or agent output.

The upstream plugin manifests and MCP configuration were not copied. Importing
these skills does not install or configure a plugin, browser, account, CLI,
scheduled job, or project dependency.

## Dependencies used by particular workflows

- A browser or documentation-fetching tool for current official documentation.
- `cf` for supported CLI workflows, using its current documented Node.js
  requirement (22.18 or later at this snapshot); `cf` is currently beta.
- The project's pinned Wrangler and package manager for existing Wrangler apps.
- Chrome DevTools MCP, or an equivalent source of actual browser captures, for
  `web-perf`; installing that server is a separate setup task.
- Separately maintained `cloudflare/vinext` skills for relevant Next.js setup or
  migration work. They are not included in this collection.
- A pprof reader, optionally Go's `pprof`, for `workers-profiling` captures.
- Bash, Python 3, and curl for Turnstile helpers; jq for widget validation and
  orchestration; Git for the optional upstream persistence helper. Live helpers
  require an authorized Cloudflare account and appropriate token scope.
- Project-specific SDKs, containers, and test runners when building the actual
  application. Their examples are guidance, not installed dependencies here.

To refresh this collection, review a new pinned upstream snapshot and retain
the local adaptation notices, host guidance, attribution, and license. The
shared repository updater pulls reviewed commits from this repository; it does
not independently track or execute upstream Cloudflare changes.
