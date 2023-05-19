Exemplos de RSYNC

RSync para host remoto

rsync -lrpPta --stats <usuário>@:

Criando arquivo de log

rsync -lrpPtah --log-file= <usuário>@:

Rsync dos arquivos dos ultimos 10 dias

rsync -lrpPtah --stats --files-from=<(find /path/origem -mtime -10 -type f -exec basename {} ;) <usuário>@:

Opção --dry-run. Simula os envio e erros, mas não o executa de fato.

rsync -lrpPta --stats --dry-run <usuário>@: