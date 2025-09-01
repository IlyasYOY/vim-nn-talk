# format code

Это мало кто знает, но **Vim** из коробки поддерживает форматирование кода
через `gq` (есть еще `gw`, но это другое).

Можно переопределять программу, которая форматирует код. Все это работает,
потому что текст в буфере доступен как *STDIN*.

Это можно настроить под себя!

## Example

Простой случай:

> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Вот еще: `./013-00-format-using-cli.go`.
