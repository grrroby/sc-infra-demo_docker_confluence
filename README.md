## Confluence Demo Data Center

- Runs on Atlassian/Confluence
- Postgres
- Caddy, ssl self signed
- and additional metabase for sql/reporting

  ### Start

  `docker-compose -f docker-compose-atlassian.yml up -d`

  Please use a `.env` to configure the version and the URL name. To customize use the `Caddyfile`.
  The sql is for my own testing with a broken team-calendar.
  Pllease keep in mind to use a postgres and conflunece version that is compatible.
