# Security policy

This policy covers every NoWayOS repository that has no security policy of its own.

NoWayOS is the Single Purpose OS: a computer with nothing else to do. If you find a security flaw in
any NoWayOS project, please tell us privately, so that it can be fixed before anyone else can use it.

## Reporting a vulnerability

**Please do not open a public issue, pull request or discussion.** Report it privately, either:

- through GitHub's private vulnerability reporting: **Report a vulnerability** on the repository's
  **Security** tab; or
- by email to **security@nowayos.com**.

Please tell us what is affected (the repository, and the crate, system, commit or release), how to
reproduce it, and what an attacker could do with it. Use synthetic test cases only: never send
personal data or anyone's real files.

## Scope

In scope: the code in NoWayOS's repositories, on `main` and in each supported release, built as its
documentation says.

Out of scope:

- **Third-party code**, including the seL4 kernel, Microkit and the projects' dependencies. Please
  report those to their maintainers, and tell us too if a NoWayOS project's use of them is affected.
- **Configurations the documentation calls development-only**, such as debug kernels and test
  systems.
- **Physical attacks on a Raspberry Pi 5.** The Pi is NoWayOS's prototype target, not a hardened
  one: it is not expected to resist invasive hardware attacks, glitching, or anyone with debug
  access.

## Supported versions

Until the first release, only `main` is supported.
