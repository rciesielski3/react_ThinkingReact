# ${pkg}: Dependabot upgrade review

This PR is a placeholder for reviewing and applying Dependabot advisories affecting `${pkg}`.

Action items:
- Review the repository Dependabot alerts: https://github.com/rciesielski3/react_ThinkingReact/security/dependabot
- For each alert affecting `${pkg}`, upgrade to the `first_patched_version` listed in the advisory.
- Run the full build and smoke test:

```bash
npm install
npm run build
npm run dev  # manual smoke test
```

- If the upgrade is breaking, document the required code changes and test steps in this PR.

Notes:
- This placeholder was created by automation to collect reviewers and testing notes.
