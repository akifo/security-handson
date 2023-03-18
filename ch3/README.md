ブラウザのコンソールで実行するコード

```
const response = await fetch("http://localhost:3000/api");
await response.json()
```

```
const response = await fetch("http://localhost:3000/api?message=hello");
await response.json()
```

```
await fetch("http://localhost:3000/api", {
  method: "POST",
  body: JSON.stringify({ message: "こんにちは" }),
  headers: { "Content-type": "application/json" }
});
```

```
const response = await fetch("http://localhost:3000/api?message=", {
  headers: { "X-Lang": "en" }
});
await response.json()
```