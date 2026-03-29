# Remote Repository Setup

## Current Remotes
```
backup  git@github.com:y8r1k/techstart-api-backup.git (fetch)
backup  git@github.com:y8r1k/techstart-api-backup.git (push)
origin  git@github.com:y8r1k/techstart-api.git (fetch)
origin  git@github.com:y8r1k/techstart-api-backup.git (push)
origin  git@github.com:y8r1k/techstart-api.git (push)
```

## Tracking Branches
```
* main bbea539 [backup/main] Merge remote-tracking branch 'origin/main'
```

## Fork Workflow Summary
- Original repository: [\[URL\]](https://github.com/y8r1k/techstart-api)
- Fork repository: [\[URL\]](https://github.com/y8r1k/techstart-api-backup)
- Upstream configuration: `git remote add upstream git@github.com:y8r1k/techstart-api.git`

## Backup Strategy
- Primary remote: origin
- Backup remote: backup
- Sync command: git remote set-url --add --push git@github.com:y8r1k/techstart-api-backup.git

## Lessons Learned
1. Всегда настраивайте upstream для форка — это позволяет синхронизировать ваш репозиторий с оригиналом.
2. Используйте разные remote для разных целей: origin — ваш форк, upstream — оригинал, backup — резервная копия.
3. Перед внесением изменений в форк обновляйте локальную main через upstream, чтобы избежать конфликтов.
