# Trust Boundary Checklist

## Check Inputs

- what enters from users, files, browsers, APIs, or external tools
- what is trusted without proof

## Check Secrets

- where tokens, cookies, credentials, or private config may appear
- whether any secret can leak into logs, commits, prompts, or generated files

## Check Authority

- what file, network, execution, or messaging authority the change enables
- whether the change can operate with less privilege

## Check Defaults

- whether the new path is safe when configuration is missing or malformed
- whether failure modes degrade safely
