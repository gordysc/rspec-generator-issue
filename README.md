# Example

## Developer Notes

This codebase was generated using the following command:

```sh
rails new --css=bootstrap --database=postgresql example
```

## Postgres Setup

```sh
# Jump into the Postgres shell
psql postgres
# Create a user for the database
CREATE ROLE example WITH LOGIN PASSWORD 'password';
# Promote the user to a super user
ALTER ROLE example WITH Superuser;
# Leave the shell
\q
```

## Reproduce Bug

```sh
# Note: This works on rspec-rails 5.1.2
rails g model user email password_digest
```
