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
├── CVE-2014-6271
│   ├── Exploit
│   │   ├── README.md
│   │   ├── exploit.py
│   │   └── images
│   │       ├── after.png
│   │       └── before.png
│   └── Lab
│       ├── Dockerfile
│       ├── Packages
│       │   └── bash_4.2%2Bdfsg-0.1_amd64.deb
│       ├── README.md
│       ├── end-point
│       └── index.html
├── CVE-2018-15473
│   ├── Lab
│   │   ├── Dockerfile
│   │   └── README.md
│   └── exploits
│       ├── README.md
│       └── exploit.py
├── CVE-2021-41773
│   ├── Exploit
│   │   ├── README.md
│   │   └── exploit.py
│   └── Lab
│       ├── Dockerfile
│       └── README.md
└── README.md
