---
title: "Lição 12 - Publique o site com o GitHub Pages"
description: "Configure o fluxo de trabalho do Pages com o app GitHub Copilot, revise a pull request e verifique o Space Quiz publicado."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publique o Space Quiz com o GitHub Pages para que qualquer pessoa possa acessá-lo. O Copilot pode preparar o fluxo de trabalho e orientar a implantação, mas você precisa revisar as alterações e confirmar que o site foi publicado.

Nesta lição, você vai:

- Pedir ao Copilot para configurar a implantação no GitHub Pages.
- Revisar o fluxo de trabalho e a pull request antes de fazer o merge.
- Acompanhar a implantação e verificar o site publicado.

## Cenário

O Space Quiz já está em um repositório do GitHub, mas ainda não há uma forma simples de acessá-lo. Publicar o site de um único arquivo com o GitHub Pages disponibiliza uma URL pública sem adicionar um servidor ou dependências de runtime.

## Peça ao Copilot para publicar o site

Na sessão do app Copilot para `space-quiz`, envie este prompt:

```plaintext
Ative o GitHub Pages para este repositório. Se necessário, crie um fluxo de trabalho do GitHub Actions para compilar e implantar o site no GitHub Pages. Se ainda não houver um README, adicione um que descreva o app e como executá-lo localmente. Crie uma pull request com as alterações e faça o merge quando as verificações obrigatórias forem aprovadas. Monitore a implantação até que ela seja bem-sucedida e, em seguida, informe a URL final do site. Se você não tiver permissão para ativar o Pages ou fazer o merge, diga exatamente o que preciso aprovar ou fazer. Não informe que a implantação foi concluída até que o site esteja realmente publicado.
```

![Diagrama em três etapas mostrando o merge da pull request do Space Quiz, uma execução do GitHub Actions bem-sucedida com as etapas Build website, Upload artifact e Deploy to Pages e o Space Quiz aberto em yourname.github.io/space-quiz/](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este prompt pede que o agente crie e faça o merge de uma pull request e altere as configurações do Pages do repositório. Antes de continuar, revise o diff, as permissões de implantação e as solicitações de aprovação do GitHub.

## Revise o fluxo de trabalho e verifique a implantação

1. Confirme se um README foi adicionado somente quando o repositório ainda não tinha um.
2. Revise as alterações da pull request, incluindo as etapas de compilação e implantação do fluxo de trabalho.
3. Faça o merge somente depois que as verificações obrigatórias da pull request forem aprovadas.
4. Confirme que a execução de implantação do GitHub Actions foi concluída com sucesso.
5. Abra a URL informada e confirme que o Space Quiz carrega.

Se o agente não puder ativar o Pages ou fazer o merge da pull request, siga as instruções específicas fornecidas. Não considere o trabalho concluído até que a implantação seja bem-sucedida e o site real esteja carregando.

## Resumo e próximos passos

Você publicou o Space Quiz como um site real e verificou a implantação em vez de confiar apenas no relato do agente. Continue para a [Lição 13: Revisão e próximos passos][next-lesson].

[next-lesson]: ../13-review/
