# Security Playbook for Cryptoasset Investors

> **Note:** This document is still an early draft. Exercise caution and do your own research.

> **Contributors:** Gabriel Bianconi (Airlock Capital), Viraj Mehta (Airlock Capital)

This document describes a set of enterprise-grade security best practices for cryptoasset investors. Implementing some of these measures might require substantial technical expertise, time investment, and financial resources. The playbook is a work in progress, and cannot guarantee perfect security. 

We welcome and encourage contributions from the public. Please [send a pull request](https://github.com/GabrielBianconi/cryptoasset-security-playbook/pulls) or [open an issue](https://github.com/GabrielBianconi/cryptoasset-security-playbook/issues).


## Overview & Motivation

Cryptoassets are at great risk of theft given the difficulty in tracking and recovering stolen funds. In particular, large investors might be targeted by organized crime and rogue governments. The attacker profile and large attack surface makes it necessary for investors to be extremely careful in their security practices.

The nature of cryptoassets makes them very susceptible to cyber attacks. Some examples include malware, phishing, and social engineering. Third-party services and software (such as exchanges and wallets) present another set of challenges. For example, a number of exchanges have had their funds stolen. There have also been a number of cases in which attackers relied on physical violence to steal cryptoassets. Examples include armed robberies and ransoms for kidnappings. Refer to [this article](https://www.nytimes.com/2018/02/18/technology/virtual-currency-extortion.html) for a number of anecdotes.

This playbook is split into two sections: [Cybersecurity](#cybersecurity) and [Physical Security](#physical-security). Both of them are relevant to investors, especially as attacks and best practices are often hybrid. In each section, we present a number of potential attacks and best practices for prevention and remediation.


## Cybersecurity

### Potential Attacks

#### Stolen Devices

- **Threat:** An attacker steals devices (such as computers and mobile devices) in an attempt to to gain access to logged-in services or stored information and credentials.
- **Prevention:** Ensure every device is hardened so its data cannot be accessed without credentials. Refer to [Hardening Computers](#hardening-computers) and [Hardening Mobile Devices](#hardening-mobile-devices). 
- **Remediation:** TODO

### Best Practices

#### Hardening Computers

Depending on your platform, refer to the following resources:

- **macOS (OS X):** A comprehensive guide for hardening macOS devices is available [here](https://github.com/drduh/macOS-Security-and-Privacy-Guide).

#### Hardening Mobile Devices

Depending on your platform, refer to the following resources:

- **iOS:** Simple checklists suitable for individuals and small organizations can be found [here](https://security.utexas.edu/handheld-hardening-checklists/ios) and [here](https://ecn.io/ios-hardening-guide-df60535c6c5). A more comprehensive guide can be found [here](https://www.asd.gov.au/publications/protect/ios-hardening-guide.htm).


## Physical Security

### Potential Attacks

#### Property Theft

- **Threat:** An attacker steals property such as electronic devices and data stored offline.
- **Prevention:** Refer to [Stolen Devices](#stolen-devices). TODO: prevention for offline data
- **Remediation:** TODO
