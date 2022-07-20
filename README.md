# olog
OAuth2 credentials flow tool written in Go

# configuration
Create a configuration file at `~/.olog/config.toml` with the following structure:

# usage

This tool leverages the Go AWS SDK to retrieve Cognito user pool information. It currently only
supports the environment-based AWS credentials. Make sure they are exported before using it.

[envs.dev]
token_url = "https://your.token.url/oauth2/token"
user_pool_id = "your-user-pool-id"
client_id = "your-client-id"

[envs.stg]
token_url = "https://your.token.url/oauth2/token"
user_pool_id = "your-user-pool-id"
client_id = "your-client-id"