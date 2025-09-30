# docker-mcp-gateway
Docker MCP Gateway using Docker Compose wtih sample custom docker and with remote access

# Setup
```
git clone https://github.com/miko550/docker-mcp-gateway.git
cd docker-mcp-gateway
curl -s https://desktop.docker.com/mcp/catalog/v2/catalog.yaml -o mcp/official-catalog.yml
docker compose up -d
```

# On MCP CLient
```
{
  "mcpServers": {
    "docker-mcp-gateway": {
      "type": "streamable",          // or "sse" if you set --transport=sse
      "url": "http://<SERVER IP>:8811/mcp"
    }
  }
}
```
