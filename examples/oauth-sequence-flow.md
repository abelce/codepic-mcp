# OAuth Sequence Flow

## Prompt

```text
Draw a sequence diagram for OAuth login with PKCE between browser, app server, identity provider, and database.
```

## What to Expect

The diagram should show:

- Browser starting login
- App server creating a code verifier and challenge
- Identity provider handling authorization
- Browser returning with an authorization code
- App server exchanging the code for tokens
- Database storing or updating the user session

## Why This Demo Works

OAuth PKCE is hard to explain in prose. A sequence diagram makes the responsibility split clearer: what happens in the browser, what happens on the server, and what is handled by the identity provider.

## Community Short Description

CodePic MCP can turn an OAuth PKCE explanation into an editable sequence diagram that your team can refine.

## Links

- Try CodePic MCP: https://codepic.cc/tools/mcp
- Sequence diagram guide: https://codepic.cc/blog/sequence-diagram-guide

