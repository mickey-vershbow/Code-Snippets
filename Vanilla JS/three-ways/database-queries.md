# 3 ways to write database queries:

Using a callback

```
app.get ("/", (req, res) => {
  Model.create(req.body, (err, data) => {
   res.json(data);
  })
};
```

Using .then

```
app.get ("/", (req, res) => {
  Model.create(req.body);
  .then(data => res.json(data));
};
```

Using Async Await

```
app.get ("/", async (req, res) => {
  const data = await Model.create(req.body);
  res.json(data);
};
```
