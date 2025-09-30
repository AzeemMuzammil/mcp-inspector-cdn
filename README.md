# MCP Inspector CDN

🔍 **Model Context Protocol Inspector** - Ready for CDN deployment

This repository contains the production-ready build of the MCP Inspector, optimized for CDN hosting and website integration.

## 🚀 Live Demo

Access the MCP Inspector directly from this CDN:
- **Main App**: `https://azeemmuzammil.github.io/mcp-inspector-cdn/`
- **Integration Example**: `https://azeemmuzammil.github.io/mcp-inspector-cdn/integration-example.html`

## 📦 What's Included

- **`index.html`** - Main MCP Inspector application
- **`assets/`** - Optimized JavaScript and CSS bundles
- **`mcp.svg`** - Application icon
- **`integration-example.html`** - Example integration page
- **`deployment-info.txt`** - Deployment details

## 🌐 CDN Integration

### Simple Iframe
```html
<iframe 
    src="https://azeemmuzammil.github.io/mcp-inspector-cdn/" 
    width="100%" 
    height="800px"
    frameborder="0"
    title="MCP Inspector">
</iframe>
```

### Modal Integration
```html
<button onclick="openInspector()">Open MCP Inspector</button>

<div id="modal" style="display:none; position:fixed; z-index:1000; left:0; top:0; width:100%; height:100%; background:rgba(0,0,0,0.5);">
    <div style="background:white; margin:2% auto; width:95%; height:90%; border-radius:8px;">
        <iframe src="https://azeemmuzammil.github.io/mcp-inspector-cdn/" width="100%" height="100%"></iframe>
    </div>
</div>

<script>
function openInspector() {
    document.getElementById('modal').style.display = 'block';
}
</script>
```

### Direct Asset Loading
```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" href="https://azeemmuzammil.github.io/mcp-inspector-cdn/assets/index-CkIb6udC.css">
</head>
<body>
    <div id="root" class="w-full"></div>
    <script type="module" src="https://azeemmuzammil.github.io/mcp-inspector-cdn/assets/index-DjScrj8s.js"></script>
</body>
</html>
```

## 🔧 Features

- **Tools Management** - Test and debug MCP tools
- **Resources Browser** - Browse and read MCP resources  
- **Prompts Library** - Test prompts with streaming responses
- **Connection Manager** - Support for stdio, SSE, streamable-HTTP
- **Authentication** - Bearer tokens, OAuth, custom headers
- **Real-time Monitoring** - Request history and notifications

## 📊 Bundle Information

- **Main Bundle**: `assets/index-DjScrj8s.js` (1.48MB)
- **Stylesheet**: `assets/index-CkIb6udC.css` (56KB)
- **Total Size**: 1.5MB
- **Built from**: `@modelcontextprotocol/inspector@0.16.8`

## 🛠️ Local Development

To serve locally:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000`

## 🔗 Related Links

- [MCP Inspector Source](https://github.com/modelcontextprotocol/inspector)
- [Model Context Protocol](https://modelcontextprotocol.io)
- [MCP Documentation](https://modelcontextprotocol.io/docs)

## 📄 License

This is a redistributed build of the MCP Inspector, originally licensed under MIT by Anthropic, PBC.

---

**Built on**: $(date)  
**Version**: 0.16.8  
**CDN Ready**: ✅