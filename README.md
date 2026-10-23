[vercel.json](https://github.com/user-attachments/files/33887582/vercel.json)
{
  "rewrites": [
    { "source": "/", "destination": "/reflow-web/index.html" },
    { "source": "/:path((?!reflow-web/).*)", "destination": "/reflow-web/:path" }
  ],
  "headers": [
    { "source": "/sw.js", "headers": [{ "key": "Cache-Control", "value": "no-cache" }] },
    { "source": "/app.js", "headers": [{ "key": "Cache-Control", "value": "no-cache" }] }
  ]
}
