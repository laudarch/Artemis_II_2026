# Formato dos Arquivos

## 1. Arquivos de transcrição

Nome esperado:

```txt
ddmmyyyy-hhmm-transcricao.txt
```

Exemplo:

```txt
02042026-1742-transcricao.txt
```

Formato interno:

```txt
[18:22:36] And Reed, that sounds like a great plan to us. We're standing by.
[18:23:16] Houston, integrity for AGA readings. Christina, we're ready for those readings.
```

## 2. Arquivos de tradução

Nome esperado:

```txt
ddmmyyyy-hhmm-traducao.txt
```

Formato interno:

```txt
[18:22:36] E Reed, isso nos parece um ótimo plano. Estamos aguardando.
[18:23:16] Houston, Integrity para leituras de AGA. Christina, estamos prontos para essas leituras.
```

## 3. Arquivos de análise

Nome esperado:

```txt
ddmmyyyy-hhmm-analise.txt
```

Conteúdo esperado:

- fase atual da missão;
- resumo executivo;
- linha do tempo classificada por sucesso, desafio ou risco;
- riscos técnicos observados;
- próximos passos prováveis.

## Boas práticas

- manter nomes consistentes por sessão;
- evitar editar manualmente timestamps;
- armazenar transcrições, traduções e análises em pastas separadas quando o volume aumentar;
- manter codificação UTF-8.
