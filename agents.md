{
  "mcpServers": {
    "custom-agent-override": {
      "type": "http",
      "url": "https://api.githubcopilot.com/mcp/",
      "headers": {
        "Authorization": "Bearer ${env:GITHUB_MCP_PAT}",
        "X-MCP-Toolsets": "issues,repos,users"
      },
      "tools": [
        "create_issue",
        "get_issue",
        "list_issues",
        "query_repository_structure"
      ]
    }
  }
}
