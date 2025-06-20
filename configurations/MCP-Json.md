
# MCP Json Configuration
This document provides an overview of the MCP (Microsoft Copilot) JSON configuration file format.

## Shell File
Basic format of the mcp.json file

```json
{
   "inputs": [
   
   ],
   "servers": {
    
   }
}
```

## GitHub MCP Server Example
You will need to create a GitHub token with the `repo` scope and replace `<your_github_token>` with your actual token (DO NOT COMMIT THIS TO GIT).
You can create a token by going to your GitHub account settings, navigating to Developer settings, and then Personal access tokens. Make sure to copy the token as you won't be able to see it again after you create it. 

```json
{
   "inputs": [
      {
         "name": "github",
         "type": "github",
         "url": "https://api.github.com"
      }
   ],
   "servers": {
      "github": {
         "type": "github",
         "url": "https://api.github.com",
         "token": "<your_github_token>"
      }
   }
}

```
## Azure MCP Server Example
You will be prompted for the Azure DevOps organization name when you run the MCP server. Use `Netchex Rewrite`

You will likley need to do an `az login` first to authenticate your Azure DevOps account via the CLI.

```json
{
   "inputs": [
     {
         "id": "ado_org",
         "type": "promptString",
         "description": "Azure DevOps organization name  (e.g. 'contoso')"
     }
   ],
   "servers": {
     "ado": {
         "type": "stdio",
         "command": "npx",
         "args": [
             "-y",
             "@azure-devops/mcp",
             "${input:ado_org}"
         ]
      }
   }
}
```