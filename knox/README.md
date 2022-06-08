# Knox
---
`Pinterest` also built its own secrets management tool and open sourced it, calling it `Knox` (as in Fort Knox). Here were the problems Pinterest was facing which led to the creation of Knox:

> "Pinterest has a plethora of keys or secrets doing things like signing cookies, encrypting data, protecting our network via TLS, accessing our AWS machines, communicating with our third parties, and many more. If these keys become compromised, rotating (or changing our keys) used to be a difficult process generally involving a deploy and likely a code change. Keys/secrets within Pinterest were stored in git repositories. This means they were copied all over our company’s infrastructure and present on many of our employees laptops. There was no way to audit who accessed or who has access to the keys. Knox was built to solve these problems."

Per Pinterest, the goals of Knox are:

> "Ease of use for developers to access/use confidential secrets, keys, and credentials
Confidentiality for secrets, keys, and credentials
Provide mechanisms for key rotation in case of compromise
Create audit log to keep track of what systems and users access confidential data"
