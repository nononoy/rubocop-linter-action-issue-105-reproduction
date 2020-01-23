# README

Template repository for reproducing bugs from [rubocop-linter-action](https://github.com/andrewmcodes/rubocop-linter-action).

## Dependencies

- Ruby: `2.7.0`
- Bundler: `2.1.4`
- Rails: `6.0.2.1`
- SQLite (see [this article](https://www.daveferrara1.com/ruby-in-rails-switch-from-sqlite3-to-postgres/) for instructions for changing to Postgres if needed)

## Setup

1. Click `Use this template` button on GitHub. See more instructions about using templates [here](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template)
2. Name the repo with a helpful name e.g. `rubocop-linter-action-issue-00-reproduction`, `rubocop-linter-action-bundler-bug-reproduction`
3. Clone the repo
4. cd into your local copy and run `bin/setup`

### Create reproduction

You may need to do one or more of the below steps to reproduce your issue:

1. Update/delete action config file at `./.github/config/rubocop_linter_config.yml`
2. Update workflow (or create a new one) at `./.github/workflows/rubocop.yml`
3. Update Gemfile at `./Gemfile`
4. Update/delete RuboCop config at `./.rubocop.yml`

## Running the app

You can run this app provided you have run `bin/setup`. Just start the Rails server `bin/rails s` and go to `localhost:3000`
