# buffer-as-STDIO

Любой текст буфера, это потенциальный *STDIN*, который может стать *STDOUT*.

> [!note] STDOUT
> Можно легко сохранить вывод команды прям в буфер.

## Example

```json
{"name":"John Doe","age":35,"email":"johndoe@example.com","isSubscribed":true,"address":{"street":"123 Main St","city":"Anytown","state":"CA","postalCode":"90210"},"phoneNumbers":[{"type":"home","number":"555-555-1234"},{"type":"work","number":"555-555-5678"}],"hobbies":["reading","hiking","photography"]}
```

### Solution

Запустить в *Visual Mode*: `:!jq -c`.
