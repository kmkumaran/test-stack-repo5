<a href="https://github.com/new?stack=ghstack-nextjs-azure-appservice"><img src="./.github/stacks/use-this-stack.png"/></a>

<img src="https://upload.wikimedia.org/wikipedia/commons/8/8e/Nextjs-logo.svg" alt="Hugo" width="200" height ="100"/>   <img src="https://upload.wikimedia.org/wikipedia/commons/3/30/OCR-A_char_Plus_Sign.svg" alt="Hugo" width="100" height ="100"/>   <img src="https://upload.wikimedia.org/wikipedia/commons/a/a8/Microsoft_Azure_Logo.svg" alt="Azure" width="200" height ="100"/>

[![GitHub stars](https://img.shields.io/github/stars/github/fetch.svg?style=social&label=Star)](https://github.com/github/fetch) 
<a href="https://discord.gg/phoenix24"><img src="https://img.shields.io/badge/chat-discord-brightgreen.svg?logo=discord&style=flat"></a>
<a href="https://twitter.com/intent/follow?screen_name=phoenix24"><img src="https://img.shields.io/badge/Follow-phoenix24-blue.svg?style=flat&logo=twitter"></a>
<a href="https://eepurl.com/phoenix24"><img src="https://img.shields.io/badge/newsletter-subscribe-yellow.svg?style=flat"></a>


 <p>
    <img src="https://assets.vercel.com/image/upload/v1607554385/repositories/next-js/next-logo.png" height="20">
    <img src="https://avatars.githubusercontent.com/u/6844498?s=200&v=4" height="20">
    <b>Use this stack</b> to spin up a static website in seconds.
</p>


## Why should you use this stack?
You can spin up your own personal website in seconds. This stack uses nextjs to generate the contents. Next.js gives you the best developer experience with all the features you need for production: hybrid static & server rendering, TypeScript support, smart bundling, route pre-fetching, and more. No config needed. Read more about [next.js](https://nextjs.org/learn)

Deployment happens on Azure Cloud via a Azure Static Website. This stack uses an Azure Github app to help you with the Azure setup.

The stack also sets up a proper Github CI/CD environment by taing care of the following things
1. Branch Naming convention - You can use any branch prefixed with "dev" as your development environment. 
2. Branch Protection Setting - Developers working on this branch can work freely and push changes without a PR and a code reviewer. This facilitates quick development. However the `master` Branch is protected and it needs a Pull request to merge with 2 reviewers approving it. The Reviewers should be defined in CODEOWNERS file.
3. Enable Security alerts - A workflow will be setup for you to enable Dependabot alerts to detect vulnerabilities.
4. CodeQL Security Analysis - Discover vulnerabilities across a codebase with CodeQL, our industry-leading semantic code analysis engine

## What are the inputs to pass while setting up the stack?
```
# This is needed for stack initialization
- NODE_VERSION

# This is needed for stack initialization
- NEXTJS_VERSION

# This is needed for dependabot workflow
- NPM_PASSWORD

# created by github stack initialization to be used by sendgrid action
- SENDGRID_API_KEY

# You dont have to pass this. Azure OIDC app will set the secret 
- PROD_SPN_ID
```

#### Github apps installed with this stack
```Azure```

#### Version summary
```nextjs version (17.0.2)```

## How to setup local development server?
```
# to start a local development environment, and view in browser.
npm run dev
open http://localhost:3000 

# to run tests
npm test

# to generate a production build
npm run build
```

## Learn more 

### Nextjs
Learn more about [next.js](https://nextjs.org/learn) from the official tutorial.
Visit [https://nextjs.org/docs](https://nextjs.org/docs) to view the full documentation.

### Azure Cloud
Learn more about [azure](https://docs.microsoft.com/en-us/azure) from the official site.
Visit [azure static website](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-static-website) to view the official documentation.


## Other Useful links

#### Security guide
Please see our guide lines for reporting issues related to [security.md](/.github/stacks/security.md).

#### Contributor guide
Please see our guide lines for [contributing.md](/.github/stacks/contributing.md).

## Contributors 
- chaitanya sharma ([@phoenix24](https://twitter.com/phoenix24)) 
- atul malaviya ([@azooinmyluggage](https://twitter.com/azooinmyluggage))
- usha narayanabhatta ([@n-usha](https://twitter.com/n-usha))
- trilok ramakrishna ([@3loka](https://twitter.com/3loka))
