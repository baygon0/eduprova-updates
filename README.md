# EduProva Updates

Repositório público usado como canal de atualizações do EduProva para Windows.

Este repositório não guarda o código-fonte do aplicativo. Ele serve apenas para publicar releases com os arquivos que o atualizador automático do EduProva consulta.

## Arquivos necessários em cada release

Para cada nova versão, anexe estes arquivos gerados na pasta `release` do projeto:

- `EduProva-Setup-X.Y.Z.exe`
- `EduProva-Setup-X.Y.Z.exe.blockmap`
- `latest.yml`

O arquivo `latest.yml` precisa apontar para o mesmo nome do instalador anexado na release.

## Como publicar uma atualização

1. Aumente a versão no `package.json` do projeto principal, por exemplo de `1.0.1` para `1.0.2`.
2. Rode `npm run desktop:build`.
3. Entre em `https://github.com/baygon0/eduprova-updates/releases/new`.
4. Crie uma tag no formato `vX.Y.Z`, por exemplo `v1.0.2`.
5. Anexe os três arquivos da pasta `release`.
6. Publique a release.

Depois disso, os usuários podem abrir o EduProva e acessar:

`Configurações > Atualizações do software > Verificar atualizações`
