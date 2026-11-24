# 🎬 Onde publicar meu drama de IA

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![Onde publicar meu drama de IA](guia/assets/banner.jpg)](https://inematds.github.io/drama-ia-onde-publicar/guia/)

📖 Guia de uso: **https://inematds.github.io/drama-ia-onde-publicar/guia/**

Você fez (ou vai fazer) uma série de drama com IA e não sabe a quem mostrar nem quem paga. Este kit tira o chute: você diz sua rota, ele lista as 26 portas que conhecemos com a fonte oficial de cada uma, põe as abertas na frente, avisa as que já fecharam e escreve o e-mail de pitch.

## O que é
Uma lista conferida (19/11/2026) de 26 plataformas e programas, com link da página oficial e data, mais uma ferramenta de linha de comando e uma skill para o Claude Code. Serve a quem cria dramas verticais com IA. Resolve "para onde mando" e "o que escrevo". Precisa só de Python 3.

## Instalação técnica
```bash
git clone https://github.com/inematds/drama-ia-onde-publicar && cd drama-ia-onde-publicar
python3 -m drama rotas
python3 -m drama escolher --rota criador
python3 -m drama vencidos
python3 -m drama pitch --titulo "..." --historia "..." --episodios 30 --duracao "90 s" --idioma English --amostra "<link privado>" --canal "<seu canal>" --ferramentas "<ferramentas de IA>"
python3 -m unittest discover -s testes   # 10 testes: 26 linhas, fonte em toda linha, ordem, prazos, pitch
```
Os textos completos (o que cada uma paga, a pegadinha, e o checklist de pitch) estão em `docs/` e em `drama escolher --detalhe`.
Skill: copie `skill/onde-publicar-meu-drama` para `~/.claude/skills/`.

## O processo, do início ao fim
1. 🧠 Você diz a rota (`drama rotas`).
2. ⚙️ `drama escolher --rota X` lista, abertas primeiro, encerradas por último.
3. 🧠 Você abre a fonte de cada uma e confere país, conta, duração, direitos.
4. ⚙️ `drama pitch …` escreve o e-mail.
5. 🧠 Você envia (o kit nunca envia) e guarda a cópia com a data.

## Limites
Os valores "até US$ X" são o teto, não o comum. Algumas linhas vêm só de notícia e dizem isso. Nada aqui é promessa de ganho.

## Lista, casos reais e exemplo

- A lista das 26 plataformas, uma a uma, está no guia (seção "A lista") e em `docs/1-platform-map.md`.
- "Casos reais": dois criadores com resultados opostos e o caso da personagem de IA que não recebeu.
- `exemplos/episodio-exemplo.mp4`: mini-episódio vertical de 24 s feito com o Kling 4.0 Flash (3 cenas), para mostrar o formato. A marca do Kling fica de propósito.
