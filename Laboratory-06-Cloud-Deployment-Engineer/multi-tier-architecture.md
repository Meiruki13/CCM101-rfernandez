# Multi-Tier Architecture: Two-Tier Deployment

## The Web/Application Tier
This tier (the Nextcloud `app` container) is the part that users
directly interact with. It provides the web interface, receives HTTP
requests through port 8080, and manages tasks such as file uploads,
user logins, and sharing actions before sending the necessary data to
the database tier.

## The Database Tier
This tier (the `database` container running MariaDB) handles the
persistent information used by the application. This includes user
accounts, login credentials, file metadata, and sharing permissions.
It is not directly accessible from the public internet and only
responds to requests coming from the application tier.

## Why Separate Them?
Keeping the web application and database in separate containers allows
each component to be managed independently. They can be updated,
restarted, secured, or scaled without directly affecting the other
component. For example, the Nextcloud application can be updated
without stopping the database. This setup also improves security
because the database is not exposed directly to the internet and can
only be accessed through the internal Docker network used by the
application tier.
