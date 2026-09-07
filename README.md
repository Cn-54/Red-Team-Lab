# Red Team Lab

A collection of isolated, reproducible environments for researching and reproducing known vulnerabilities.

Each vulnerability is split into two components:

- **Exploit** -- a custom proof-of-concept demonstrating the vulnerability.
- **Lab** -- an intentionally vulnerable Docker environment used to safely reproduce it.

The goal of this project is to understand vulnerabilities at a technical level by studying their behaviour, reproducing them in controlled environments, and implementing the exploitation logic independently.

> ⚠️ **Disclaimer**
>
> These exploits are intended for authorised security research and isolated lab environments only.
> Do not use them against systems you do not own or have explicit permission to test.

---

## Structure

```text
red-team-lab/
├── README.md
├── exploits
│   ├── CVE-2018-15473
│   │   ├── README.md
│   │   └── exploit.py
│   └── CVE-2021-41773
│       ├── README.md
│       └── exploit.py
└── labs
    ├── CVE-2018-15473
    │   ├── Dockerfile
    │   └── README.md
    └── CVE-2021-41773
        ├── Dockerfile
        └── README.md
