# TP DNS — Windows Server `wilders.lan`

**Serveur DNS :** `172.16.10.5`  
**Zone directe :** `wilders.lan`  
**Zone indirecte :** `10.16.172.in-addr.arpa`

---

## 1. Zone directe

![Zone directe](https://github.com/JeMa9701/install_dns_win_serv/commit/c3a3d8c3716c7a13dcaa7e9ebef5c7976dbb1127#diff-d529c52a4038a6738b4fee952afdae8f306c7bbd89506ef79c2beb587a828d3f)

> Configuration de la zone directe `wilders.lan` avec les enregistrements A (`srv-dns`) et CNAME (`dns`).

---

## 2. Zone indirecte

![Zone indirecte]()

> Zone de recherche inversée `10.16.172.in-addr.arpa` avec l'enregistrement PTR pointant vers `srv-dns.wilders.lan`.

---

## 3. Ping vers le nom A — `srv-dns.wilders.lan`

![Ping srv-dns]()

> Ping depuis le client vers l'enregistrement A du serveur DNS.

---

## 4. Ping vers le CNAME — `dns.wilders.lan`

![Ping CNAME]()

> Ping depuis le client vers l'alias CNAME du serveur DNS.

---

## 5. nslookup depuis le client

![nslookup]()

> Résolution DNS directe et inverse depuis le client en interrogeant `172.16.10.5`.
