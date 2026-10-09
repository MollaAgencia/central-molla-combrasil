# Central do Cliente · Combrasil

Portal de entregáveis da Combrasil no padrão Central do Cliente Molla (De > para da Central Vetoquinol Pets).

## Publicação

Arquivo único, sem build. Basta subir o `index.html` na branch principal: o Vercel (preset Other) republica a cada push.

- URL sugerida: https://central-molla-combrasil.vercel.app (a confirmar; o guia de acesso e o QR Code já apontam para ela)
- Login: nome livre + senha de grupo do projeto (ver guia de acesso)
- Não confundir com o portal de cronograma, que segue em https://portal-molla-crono-combrasil.vercel.app

## Conteúdo atual

- Planejamentos: em breve
- Relatórios mensais: em breve

Para publicar um material, inclua o HTML em base64 no objeto `DOCS` do `index.html` e troque o card "Em breve" da seção por um card com `data-doc` e `data-pdf` apontando para a mesma chave (mesmo modelo da Central Vetoquinol). O documento abre no visualizador interno, com download em PDF pelo navegador.

## Arquivos

| Arquivo | Para quê |
|---|---|
| `index.html` | Portal completo (login + central + visualizador) |
| `guia-de-acesso.html` | Fonte do guia do cliente (A5, 4 páginas) |
| `Guia_Acesso_Central_do_Cliente_Combrasil.pdf` | Guia enviado à Combrasil (sem senha) |
| `assets/logos/` | Logos Combrasil e Molla, paleta Molla |
| `assets/icones-plataformas/` | Instagram, Meta Ads, Google Ads, YouTube, WhatsApp, para reports e planejamentos |

## Senha

A senha fica na variável `PASS` do `index.html`. Ela é enviada ao cliente por mensagem, separada do guia.

Aviso: a senha é validada no navegador e visível no código fonte. Ela organiza o acesso, não protege conteúdo sigiloso.
