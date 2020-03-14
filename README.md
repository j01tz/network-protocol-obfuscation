# Network Protocol Obfuscation Research

This repository helps organize research about the current state of network protocol obfuscation, particularly with regard to usability against active censors utilizing deep packet inspection (DPI) techniques.

If you have more research to add or notice outdated or wrong information please open a PR. The network protocol obfuscation landscape is constantly changing as the latest DPI techniques and obfuscation research chase each other.

* Existing known well-researched techniques with well-tested implementations are tracked in the [obfuscation techniques document](obfuscation_techniques.md).

* Attacks on the obfuscation techniques are tracked in the [obfuscation attacks document](obfuscation_attacks.md).

Unique applications of obfuscation techniques may be required for different use cases. Below are notes on obfuscating specific protocols.

| Project | Obfuscation Technique(s) | Obfuscation Quality |
| --- | --- | --- |
| [Tor](https://2019.www.torproject.org/docs/pluggable-transports.html.en) | Obfs4, Meek, FTE (all optional) | Medium |
| [Bitcoin](https://github.com/bitcoin/bitcoin/blob/master/doc/tor.md) | Tor (optional, proxy + bitcoin hidden servers) | Medium/Low |
| [Grin](grin_obfuscation.md) | Tor (optional, transactions only) | Low |

_Note: Tor's "Obfuscation Quality" score is not in reference to the ability of Tor to obfuscate the data it is transporting, it is referencing the ability to obfuscate the fact that a packet flow is using the Tor protocol while using one of the available "Obfuscation Techniques"_
