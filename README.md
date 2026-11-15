# observatorio-radar

Caixa de entrada do Radar do Observatório de Compósitos.

Uma tarefa agendada do Claude Code roda aqui uma vez por dia, busca notícias públicas do
setor de compósitos e grava `radar/entrada.json` no ramo `claude/radar`. Este repositório
existe para isolar a tarefa: ela só tem acesso a ele.

O arquivo é tratado como dado não confiável. O observatório lê só esse arquivo, como texto,
e confere cada notícia por código antes de publicar: formato, datas, nada de links ou HTML
nos textos, repetidas, e se o link abre e o título aparece na página.

Não guarde nada sensível aqui: o repositório é público.
