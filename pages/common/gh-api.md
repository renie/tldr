# gh api

> Make authenticated HTTP requests to the GitHub API and print the response.
> More information: <https://cli.github.com/manual/gh_api>.

- Display the releases for the current repository in JSON format:

`gh api repos/:owner/:repo/releases`

- Create a reaction for a specific issue:

`gh api {{[-H|--header]}} {{Accept:application/vnd.github.squirrel-girl-preview+json}} {{[-f|--raw-field]}} '{{content=+1}}' {{repos/:owner/:repo/issues/123/reactions}}`

- Display the result of a GraphQL query in JSON format:

`gh api graphql {{[-f|--field]}} {{name=':repo'}} {{[-f|--raw-field]}} '{{query}}'`

- Send a request using a custom HTTP method:

`gh api {{[-X|--method]}} {{POST}} {{endpoint}}`

- Include the HTTP response headers in the output:

`gh api {{[-i|--include]}} {{endpoint}}`

- Do not print the response body:

`gh api --silent {{endpoint}}`

- Send a request to a specific GitHub Enterprise Server:

`gh api --hostname {{github.example.com}} {{endpoint}}`

- Display the subcommand help:

`gh api --help`
