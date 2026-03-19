# useful

## Anki Cards

```plaintext
создай 50 anki карточек по теме, если что-то не учтено в pdf, дополни
в качестве разделителя используй |
выдай их в формате кода
```

## Bash commands

**Duplicate one file into several:**

```bash
tee < source.file destination{0..9}.file > /dev/null
```

**List files in lines count sort by extension:**

```bash
find . -type f -name '*.md' | xargs wc -l | sort -n
```

**List files in update time order:**

```bash
ls -larth
```

**Remove all\* docker containers:**

```bash
docker container ls -aq | awk '{print $1}' | xargs docker container rm
```

**Remove all\* docker images:**

```bash
docker images -q | awk '{print $1}' | xargs docker image rm
```

**Remove all\* docker volumes:**

```bash
docker volume ls -q | xargs docker volume rm
```
