- `.then` is the promise and `.catch` will catch the errors

- dummy connection (base)

```
mongodb.connect('mongodb+srv://test_user:12345@cluster0.ibrvy.mongodb.net/shop?retryWrites=true&w=majority')
  .then(client => {
    console.log('Connected!');
    client.close();
  })
  .catch(err => {
    console.log(err);
  });
```

- store products to db by creating collection

```
MONGO SHELL CONNECTION
------------------------
 mongo --host "mongodb+srv://cluster0.ibrvy.mongodb.net/test" --username admin
```