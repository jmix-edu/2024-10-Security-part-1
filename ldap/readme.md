### How to configure OpenLDAP server.

1. Setup: 
   - docker and docker compose
   - or podman and podman compose. How to install podman compose see https://podman-desktop.io/blog/getting-started-with-compose
2. Download OpenLDAP image: - https://hub.docker.com/r/osixia/openldap/
   or use `docker-compose.yml` from **ldap** folder.
3. Download Apache Directory Studio: https://directory.apache.org/studio/
4. Start OpenLDAP container
5. Setup new connection to ldap in ADS
    -  Note, that we need connection with authentication.  
       Default **username**: "cn=admin,dc=example,dc=org"  
       Default **password**: "admin"
6. Import LDAP users and groups from `ldap-configuration-**.ldif`.
    - Users have the same username and password.