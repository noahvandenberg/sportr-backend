# Sportr backend

Express/PostgreSQL API for users, sports events, and user-event participation.
Routes are under `routes/`; Knex migrations and seed fixtures are under `db/`.

## Local development

Install with `npm ci`, copy `.env.example` to `.env`, and configure a disposable
PostgreSQL database with the `DB_HOST`, `DB_USER`, `DB_PASS`, and `DB_NAME` values
used by `knexfile.js`. Run `npm run db:migrate`, optionally `npm run db:seed`, then
`npm start`. The existing `db:reset` script rolls back all migrations and seeds again;
use it only for disposable local data.

The companion web project is [LHL-Final-Sportr](https://github.com/noahvandenberg/LHL-Final-Sportr).
This repository retains its separate API history and three branches. No migration,
seed, live server, or deployment was run by this documentation cleanup.
