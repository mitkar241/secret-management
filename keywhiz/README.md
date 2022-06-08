# Keywhiz
---
`Keywhiz` is a tool built by `Square` and operated in production for some time. It has a lot of features for storing and managing application and infrastructure secrets. Square describes Keywhiz as follows:

> "Keywhiz makes managing secrets easier and more secure. Keywhiz servers in a cluster centrally store secrets encrypted in a database. Clients use mutually authenticated TLS (mTLS) to retrieve secrets they have access to. Authenticated users administer Keywhiz via CLI. To enable workflows, Keywhiz has automation APIs over mTLS."
