# GitHub Recon:

## Specific Org search:
- "Org_name" password
- "org_name" key
- "org_name" api
- "org_name" “filename:vim_settings.xml”
- "org_name" "Authorization: Bearer"
- "org_name" "Language: PHP"

## Sensitive Files search:

- filename:manifest.xml
- filename:travis.yml
- filename:vim_settings.xml
- filename:database
- filename:secrets.yml password
- filename:.esmtprc password
- filename:passwd path:etc
- filename:dbeaver-data-sources.xml
- path:sites databases password
- filename:config.php dbpasswd

## Specific Language based search:

- language:python username
- language:php username
- language:sql username
- language:html password
- language:perl password
- language:shell username
- language:java api
- HOMEBREW_GITHUB_API_TOKEN language:shell

## API keys, Token & Hard-Coded Password search:
 
- SecretKey / Secrect_key / skey
- privatekey / private_key / pkey
- user_secret / userSecret
- admin_passwd / adminpasswd / adminPass etc
- “api keys”
- authorization_bearer:
- oauth
- auth
- authentication
- client_secret
- api_token:
- “api token”
- client_id
- password
- user_password
- user_pass
- passcode
- client_secret
- secret
- password hash
- OTP
- user auth

## Username search:

- user:name (user:admin)
- org:name (org:google type:users)
- in:login (<username> in:login)
- in:name (<username> in:name)
- fullname:firstname lastname (fullname:<name> <surname>)
- in:email (data in:email)

## GitHub Dorks for Finding Information using Dates:

- created:<2012–04–05
- created:>=2011–06–12
- created:2016–02–07 location:iceland
- created:2011–04–06..2013–01–14 <user> in:username

## Extension based search:

- extension:pem private
- extension:ppk private
- extension:sql mysql dump
- extension:sql mysql dump password
- extension:json api.forecast.io

## Automated Tools:

1. [TruffleHog](https://github.com/dxa4481/truffleHog)
2. [WatchTower](https://radar.nightfall.ai/)

## NOTE :
If you find any API key or credentials or any other sensitive information under test directory then do not report it because that is an intended behaviour.

## Author:
[Mr._fr3qu3n533](https://twitter.com/mr_fr3qu3n533)

GitHub dorks for AWS, Jira, Okta .. secrets

By @hunter0x7, @GodfatherOrwa
Source: link1, link2

Here are some useful GitHub dorks shared by @hunter0x7 for identifying sensitive information related to Amazon AWS cloud:

org:Target "bucket_name"
org:Target "aws_access_key"
org:Target "aws_secret_key"
org:Target "S3_BUCKET"
org:Target "S3_ACCESS_KEY_ID"
org:Target "S3_SECRET_ACCESS_KEY"
org:Target "S3_ENDPOINT"
org:Target "AWS_ACCESS_KEY_ID"
org:Target "list_aws_accounts"

Here’s another list of GitHub dorks shared by @GodfatherOrwa for identifying various other credentials and secrets:

"target.com" password or secret
"target.atlassian" password
"target.okta" password
"corp.target" password
"jira.target" password
"target.onelogin" password
target.service-now password
some time only "target"

Protip: While you are doing GitHub dorking, try also GitDorker (made by @obheda12) which automates the whole process and which contains 400+ dorks in total, for easy bug bounty wins.

Detailed information about GitDorker can be found here.

Also check related tip BBT5-8.

 GitHub dorks for finding secrets

By @impratikdabhi
Source: link

Here’s a list of 10 Github dorks to find secret and access tokens:

    “target.com” send_keys
    “target.com” password
    “target.com” api_key
    “target.com” apikey
    “target.com” jira_password
    “target.com” root_password
    “target.com” access_token
    “target.com” config
    “target.com” client_secret
    “target.com” user auth
