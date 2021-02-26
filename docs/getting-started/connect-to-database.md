---
layout: default
title: Connect to the database
parent: Getting Started
nav_order: 4
last_modified_date: 2021-02-26T17:03
---

# Connect to the database

---

The Blindata Data Governance and Compliance Platform stands on a PostgreSQL database.

You can connect to the database from your EC2 instance with the PostgreSQL client tool using the default username `postgres`:

```sh
sudo su - postgres -c psql
```

---

**Related pages:**

- [Connect to the server using SSH]({{ site.baseurl }}{% link docs/getting-started/connect-to-server.md %})