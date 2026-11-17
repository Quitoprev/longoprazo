# Placar de Hábitos

Controle de hábitos em formato de campeonato de pontos corridos. Cada dia é uma rodada:
vitória se tudo o que estava programado foi feito, empate se foi feita uma parte, derrota se nada foi feito.
A capa traz o lema "No longo prazo, ninguém me vence" e a meta de 100 dias, com uma casa por dia.

É um site estático: um único `index.html`, sem etapa de build e sem servidor.

## Publicar no Vercel

1. No Vercel, escolha **Add New → Project** e importe este repositório.
2. Em *Framework Preset*, deixe **Other**. Não preencha comando de build nem pasta de saída.
3. Clique em **Deploy**. A cada novo commit na branch principal, o Vercel publica de novo.

O `vercel.json` só define cabeçalhos de segurança e pede aos buscadores que não indexem o endereço.

## Usar no celular

Abra o endereço do Vercel no navegador do celular e use **Adicionar à Tela de Início**
(Safari: botão de compartilhar; Chrome: menu ⋮). O Placar passa a abrir como aplicativo, em tela cheia.

## Onde ficam os dados

Os hábitos e as marcações ficam salvos **neste navegador**, no aparelho em que você usa o site.
Nada é enviado a servidor algum, e este repositório não contém dado pessoal.

- Outro aparelho ou outro navegador começa vazio.
- Limpar os dados do navegador apaga o histórico.
- Em **Backup e dados**, no rodapé, dá para baixar um arquivo de backup e restaurá-lo em outro aparelho.

Arquivos de backup (`placar-habitos-AAAA-MM-DD.json`) estão no `.gitignore` e não devem ser enviados ao repositório.

## Arquivos

| Arquivo | Para que serve |
| --- | --- |
| `index.html` | O aplicativo inteiro: tela, estilo e regras |
| `manifest.webmanifest`, `icon-*.png` | Nome e ícone do atalho na tela de início |
| `vercel.json` | Cabeçalhos de segurança no Vercel |
