# GameList

Este é o **GameList**, evolução do app anterior, com:

- Coleção / backlog de jogos
- Dispositivos (PC, Odin, TV, Quest 3s, Outro...)
- Metas simples de jogatina
- Busca em API (RAWG) para preencher título/capa/sinopse automaticamente
- Visual mais próximo do iOS (segmented control por dispositivo)
- Edição em lote (selecionar vários jogos e definir status/dispositivos)
- Backup/restore via JSON
- 100% offline para uso normal (API só é usada quando você toca em "Buscar online")

## Como gerar o APK pelo GitHub

1. Crie um repositório (pode ser privado) no GitHub.
2. Descompacte este `.zip` no seu computador.
3. Envie **todo o conteúdo da pasta `gamelist/`** para o seu repositório.
4. No GitHub, entre na aba **Actions** e habilite os workflows.
5. Rode o workflow **"Android APK"** (ou faça um push e ele roda sozinho).
6. Ao finalizar, baixe o artefato `app-debug.apk` na página da execução.

Se você já tem um workflow `.github/workflows/main.yml` com o conteúdo que usamos antes, pode mantê-lo. Este projeto também traz um workflow de exemplo em `.github/workflows/android.yml`.
