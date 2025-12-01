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
  
## Structure

```bash
.
├── Caddyfile # Setup Reverse Proxy
├── docker-compose-atlassian.yml # docker setup 
├── README.md 
├── sql_files # Fix problems in the team-calendar
│   ├── backup_team_calendar.sql
│   ├── drop_backup_team_calendar.sql
│   ├── drop_team_calendar.sql
│   ├── restore_team_calendar.sql
│   └── team_calendar.tar.gz
└── team_calendar.zip # just the zip

```
