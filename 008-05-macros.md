# macros

Можно записать любой набор действий, и повторить его.

Получается полноценная программа на языке **Vim**.

## Example

Тут может быть вообще пример любой сложности. Буквально, что
угодно можно сделать через **macros**.

```go
// make errors local
// this code does not compile

err := some1(x)
if err != nil {
    return err
}

err := some2(x)
if err != nil {
    return err
}

err := some3(x)
if err != nil {
    return err
}

err := some4(x)
if err != nil {
    return err
}

// want 

if err := some1(x); err != nil {
    return err
}

if err := some2(x); err != nil {
    return err
}

if err := some3(x); err != nil {
    return err
}

if err := some4(x); err != nil {
    return err
}
```

### Solution

Команда: `Jwciw<Bcsp>;<Esc>Iif`
