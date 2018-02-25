# Security Playbook for Cryptoasset Investors

> **Contributors:** Gabriel Bianconi (Airlock Capital), Viraj Mehta (Airlock Capital)

> **Note:** This document is still an early draft. Exercise caution and do your own research.


This document describes a set of enterprise-grade security best practices for cryptoasset investors. Implementing some of these measures might require substantial technical expertise, time investment, and financial resources. The playbook is a work in progress, and cannot guarantee perfect security. 

We welcome and encourage contributions from the public. Please [send a pull request](https://github.com/GabrielBianconi/cryptoasset-security-playbook/pulls) or [open an issue](https://github.com/GabrielBianconi/cryptoasset-security-playbook/issues).


## Overview & Motivation

Cryptoassets are at great risk of theft given the difficulty in tracking and recovering stolen funds. In particular, large investors might be targeted by organized crime and rogue governments. The attacker profile and large attack surface makes it necessary for investors to be extremely careful in their security practices.

The nature of cryptoassets makes them very susceptible to cyber attacks. Some examples include malware, phishing, and social engineering. Third-party services and software (such as exchanges and wallets) present another set of challenges. For example, a number of exchanges have had their funds stolen. There have also been a number of cases in which attackers relied on physical violence to steal cryptoassets. Examples include armed robberies and ransoms for kidnappings. Refer to [this article](https://www.nytimes.com/2018/02/18/technology/virtual-currency-extortion.html) for a number of anecdotes.

This playbook covers cybersecurity and physical security. Both of them are relevant to investors, especially since they are often intertwined. We present a number of [Potential Attacks](#potential-attacks) and [Best Practices](#best-practices) for prevention and remediation. Finally, we present a [Checklist](#checklist) to help investors implement the strategies that are most relevant to their needs.


## Potential Attacks


### Stolen Credentials

- **Threat:** An attacker steals credentials to third-party services (e.g. exchanges) in an attempt to steal cryptoassets.
- **Prevention:** Follow [Password](#passwords) best practices. Enable [Two-Factor Authentication](#two-factor-authentication) and avoid services that do not support it.
- **Remediation:** TODO


### Stolen API Keys

- **Threat:** An attacker steals API keys to third-party services (e.g. exchanges) in an attempt to steal cryptoassets.
  - ***Note:** Trading privileges are enough to steal the funds. Refer to [Trading Privileges](#trading-privileges) for details.*
- **Prevention:** Do not generate API keys unless necessary. Assign the minimum amount of privileges necessary to the keys. If the key has withdrawal or trading privileges, treat it as a wallet's private key (refer to TODO).
- **Remediation:** Revoke the API keys. If other API keys are stored in the same location, revoke them as well.


### Trading Privileges

- **Threat:** An attacker can steal funds in exchanges using only trading privileges by selling back and forth between your account and theirs, profiting the spread on each trade. This technique is particularly profitable (and therefore dangerous) in exchanges with large spreads. Attackers can also deplete your account by accruing massive trading fees. Therefore, funds are at risk even if the attacker cannot perform an withdrawal.
- **Prevention:** Refer to [Stolen Credentials](#stolen-credentials) and [Stolen API Keys](#stolen-api-keys), as appropriate.
- **Remediation:** Refer to [Stolen Credentials](#stolen-credentials) and [Stolen API Keys](#stolen-api-keys), as appropriate.


### Stolen Devices

- **Threat:** An attacker steals devices (such as computers and mobile devices) in an attempt to to gain access to logged-in services or stored information and credentials.
- **Prevention:** Ensure every device is hardened so its data cannot be accessed without credentials. Refer to [Hardening Computers](#hardening-computers) and [Hardening Mobile Devices](#hardening-mobile-devices). 
- **Remediation:** TODO


## Best Practices

### Passwords

The following password policy should be adopted:

- Use a unique password for each service. Shared passwords will make an otherwise limited attack have a much wider effect.
- Use strong passwords. A sequence of common words (e.g. "securityforcryptoassets") tends to be highly secure and memorable (unlike short sequences of random characters, e.g. "w7Ro2mcA"). Refer to [this](https://baekdal.com/thoughts/password-security-usability/) and [this](https://xkcd.com/936/) for more details.

### Two-Factor Authentication

Two-factor authentication (2FA), or more broadly, multi-factor authenticator (MFA), prevents attackers from gaining access to your services by only stealing your credentials.

TODO

### Hardening Computers

Depending on your platform, refer to the following resources:

- **macOS (OS X):** A comprehensive guide for hardening macOS devices is available [here](https://github.com/drduh/macOS-Security-and-Privacy-Guide).

### Hardening Mobile Devices

Depending on your platform, refer to the following resources:

- **iOS:** Simple checklists suitable for individuals and small organizations can be found [here](https://security.utexas.edu/handheld-hardening-checklists/ios) and [here](https://ecn.io/ios-hardening-guide-df60535c6c5). A more comprehensive guide can be found [here](https://www.asd.gov.au/publications/protect/ios-hardening-guide.htm).



## Checklist

- [ ] Use secure [Passwords](#passwords).
- [ ] Enable [Two-Factor Authentication](#two-factor-authentication-2fa) (2FA/MFA).
- [ ] Ensure that every device that contains sensitive information or interacts with cryptoassets is hardened. Refer to [Hardening Computers](#hardening-computers) and [Hardening Mobile Devices](#hardening-mobile-devices).
- [ ] Revoke any unused API keys and make sure the remaining keys have the mininum amount of privileges required for the task. Refer to [Stolen API Keys](#stolen-api-keys).
