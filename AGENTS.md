# Instruções obrigatórias do projeto Pesca2

Estas instruções pertencem exclusivamente a este repositório. Antes de investigar, planejar ou alterar qualquer parte do jogo, leia também a skill principal local: [`skills/pesca2-workflow/SKILL.md`](skills/pesca2-workflow/SKILL.md).

## Antes de qualquer alteração

1. O MCP do roblox para que você tenha controle total sobre o projeto dentro do roblox já está condigurado, então é só usar.
2. Leia `ServerStorage.CheckList`. A descrição é a fonte de verdade para entender o jogo e o contexto de cada pedido; o checklist define o que ainda falta para o jogo ficar pronto.
3. Inspecione os scripts, a hierarquia e as convenções que a alteração toca antes de editar.
4. Faça alterações no projeto pelo MCP do Roblox, já configurado no Codex e no Antigravity para a instância aberta `Pesca2`.

## Regras de implementação

- Construa sistemas em ModuleScripts focados. Nunca concentre toda uma funcionalidade em apenas um script de servidor e outro de cliente.
- Mantenha autoridade do servidor e apresentação do cliente separadas.
- Ao concluir trabalho, atualize automaticamente `ServerStorage.CheckList`: marque o item concluído e registre de forma breve o que foi entregue, quando a estrutura do checklist permitir.
- Para interfaces, leia e siga a skill local [`skills/pesca2-interface/SKILL.md`](skills/pesca2-interface/SKILL.md) antes de editar.
- Para cenário, criação ou manipulação de qualquer objeto 3D, leia e siga a skill local [`skills/pesca2-3d/SKILL.md`](skills/pesca2-3d/SKILL.md) antes de editar.
- Nunca grave, exponha ou faça commit de chaves de API, tokens ou outras credenciais.

## Localização das skills

Todas as skills do Pesca2 ficam versionadas neste próprio repositório, em `skills/`. Um `git clone` ou `git pull` traz `AGENTS.md` e as três skills junto; não existe dependência de `~/.codex/skills` nem de qualquer pasta pessoal de outro computador.
