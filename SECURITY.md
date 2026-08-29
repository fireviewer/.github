# FireViewer Security Policy

## Reporting a vulnerability

Please report suspected security vulnerabilities privately.

Use GitHub private vulnerability reporting when it is enabled for the affected
repository.

Otherwise contact:

**unicornwhodev@gmail.com**

Do not publish vulnerability details in a normal GitHub issue before the report
has been reviewed.

## Useful information

When possible, include:

- the affected repository or component;
- the relevant version or commit;
- a description of the issue;
- reproduction steps;
- the expected impact;
- any mitigation you have already identified.

A minimal proof of concept is useful, but please do not access or copy
information that is unnecessary to demonstrate the problem.

## Sensitive information

Never put the following in a public security report:

- credentials, API keys or tokens;
- private incident evidence;
- personal data;
- private contributor information;
- unpublished infrastructure identifiers;
- sensitive geographic information;
- third-party private data.

Contact the project privately if that information is necessary to explain the
issue.

## Security scope

Relevant issues include traditional software vulnerabilities such as:

- authentication or authorisation bypass;
- unintended access to private evidence;
- credential exposure;
- injection vulnerabilities;
- remote code execution;
- supply-chain compromise;
- unsafe file or media processing.

For FireViewer, **evidence integrity is also part of security**.

Please report vulnerabilities that could allow somebody to:

- replace evidence without preserving revision history;
- bypass provenance or integrity checks;
- alter an immutable spatial reference;
- make a modified artifact appear to have a trusted identity;
- remove required uncertainty;
- bypass a review or publication gate.

## What is normally not a security issue

Model false positives or false negatives, scientific disagreement, ordinary UI
bugs, performance problems and missing features should normally be reported as
technical or research issues.

They become security-relevant when an attacker can exploit them to bypass a
trust, access or integrity boundary.

## Responsible disclosure

Please allow reasonable time to investigate and mitigate a reported
vulnerability before publishing technical details.

FireViewer is still a small open-source research project and does not provide a
guaranteed security-response SLA.

Reports are handled on a best-effort basis, with priority given to issues that
could expose people, credentials, private evidence or the integrity of
published artifacts.

## Supported code

Security work is primarily focused on actively maintained code and current
interfaces.

Historical research artifacts and superseded experimental branches may not
receive security updates.

## Emergencies

FireViewer is not an emergency reporting service.

Do not use the security channel to report an active wildfire or request
emergency assistance.
