# Zaka Red Hackers Team

A small terminal launcher for OpenAI Codex CLI. It runs Codex in the current project folder, using the existing ChatGPT sign-in instead of an `OPENAI_API_KEY` environment variable.

## Requirements

- Codex CLI installed and signed in with ChatGPT (`codex login`).
- A ChatGPT plan/account with Codex access. Usage limits still apply.

## Run

From the project you want Codex to work on:

```sh
~/zaka-red-hackers-team-project/zaka-red-hackers-team
```

Or pass a starting request:

```sh
~/zaka-red-hackers-team-project/zaka-red-hackers-team "Explain this project, then fix the login bug"
```

The launcher keeps Codex's normal sandbox and approval behavior. It removes `OPENAI_API_KEY` from the child process so this launcher uses the saved ChatGPT login rather than API-key billing.

## Install from this repository

```sh
git clone https://github.com/zakakingpapa-pixel/zaka-red-hackers-team.git
cd zaka-red-hackers-team
chmod +x zaka-red-hackers-team
```

Then run `./zaka-red-hackers-team` from the project folder you want Codex to edit, or call the launcher by its full path.

## License

MIT. See [LICENSE](LICENSE).
