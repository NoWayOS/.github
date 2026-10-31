<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/NoWayOS/.github/main/profile/nowayos-wordmark-reverse.png">
  <img alt="NoWayOS" src="https://raw.githubusercontent.com/NoWayOS/.github/main/profile/nowayos-wordmark-ink.png" width="300">
</picture>

## Single Purpose OS

**A computer with nothing else to do.**

One device. One job. Only the software it needs. NoWayOS brings deliberate simplicity to dedicated devices, built on the seL4 microkernel, in Rust.

A Single Purpose OS is built for one device's one job, rather than built to run anything and then locked down to one thing. Three things make it one:

- **Built for one job.** The device image holds its application, the drivers that application uses and the kernel. Nothing another job might need is there: no browser, desktop, shell, package manager or user account.
- **Sealed inside.** Each part (the screen, the input, the network, the application) runs in a compartment of its own and reaches only what it was granted. A fault in one part is designed to stay there.
- **Shows its working.** It comes with the evidence of what is inside and what each part may do: every grant written down, every component listed, and checks anyone can run.

Not kiosk mode, which locks a general-purpose system to one app and leaves everything else in place. Not a single-user OS, which limits who uses a computer, not what is in it.

When everything depends on it, give it one job.

### The projects

| Project | What it is | Licence |
| --- | --- | --- |
| [**NoWayOS**](https://github.com/NoWayOS/nowayos) | The Single Purpose OS. Protection-domain patterns on seL4 and Microkit, typed messages, drivers, networking and a native user interface. | MIT OR Apache-2.0 (intended) |
| [**Screen Compiler**](https://github.com/NoWayOS/screen-compiler) | Design in React. Ship native Rust. No browser on the device. | MIT |
| [**Showcase**](https://github.com/NoWayOS/showcase) | Secure kiosks you can run on a Raspberry Pi. | MIT OR Apache-2.0 (intended) |

### Where it stands

In development and not ready for production. It runs in QEMU and on the Raspberry Pi 5; NXP i.MX8 is the intended production hardware. The projects are intended to be open source, and the repositories are being prepared for publication.

seL4 has machine-checked proofs of correctness and security for specific configurations. NoWayOS uses seL4's mixed-criticality configuration, whose AArch64 proofs are in progress, so no NoWayOS image is inside seL4's completed proofs today.

To report a vulnerability, please write privately, as each repository's `SECURITY.md` describes, and not in a public issue.

### Find out more

[www.nowayos.com](https://www.nowayos.com) · [Getting started](https://www.nowayos.com/docs/getting-started) · [Security and evidence](https://www.nowayos.com/security) · [Glossary](https://www.nowayos.com/glossary) · [Questions](https://www.nowayos.com/faq)

NoWayOS is sponsored by Adappt.
