# vim-nn-talk

## Overview

Слайды доклада: "Vim — это метаредактирование".

## Getting Started

Откройте любой файл markdown в вашем любимом редакторе, начиная с
`000-00-title.md`.

Чтобы запустить пример на Go (необязательно):

```bash
go run 013-00-format-using-cli.go
```

## Contributing

Не стесняйтесь открывать issue'ы или присылать pull‑request'ы. При добавлении
новых глав следуйте числовой схеме именования (например,
`019-00-new-topic.md`).

## Slides with Marp

Любой markdown‑файл из этого репозитория можно превратить в набор слайдов с
помощью **Marp**.

```bash
# Install Marp CLI (if not already installed)
brew install marp-cli

# Concat slides
setopt extended_glob
files=(*.md~README.md~slides.md)

for i in {1..$#files}; do
    (( i > 1 )) && echo "\n---\n"
    awk '
        /^## Example$/ { exit }   # stop before printing the line
        { print }
    ' "${files[i]}"
done > slides.md

# Generate HTML slides from a markdown file
marp slides.md -o slides.pdf

# Open PDF with presentation
open slides.pdf
```

Сгенерированные слайды будут использовать тему **Marp** по умолчанию. Вы можете
настроить тему, добавив блок front‑matter в начале markdown‑файла:

```markdown
---
marp: true
theme: default
paginate: true
---
```
