# Artemis II Live Transcript Archive

Este repositório reúne arquivos de transcrição e tradução gerados a partir de transmissões ao vivo relacionadas à missão **Artemis II**.

O objetivo deste projeto é **capturar áudio, transcrever em inglês, traduzir para português do Brasil e preservar o contexto técnico da missão** para que, mesmo à distância e mesmo depois da transmissão ao vivo, seja possível entender com clareza tudo o que aconteceu durante esse momento histórico da exploração humana rumo à Lua.

## Propósito

Durante eventos ao vivo, muitas informações importantes passam rápido demais: comunicações de cabine, confirmações do controle da missão, anomalias, procedimentos, mudanças de plano e marcos operacionais.

Este projeto foi desenvolvido para:

- registrar a comunicação operacional da missão em tempo quase real;
- manter uma linha do tempo fiel dos acontecimentos;
- facilitar a compreensão técnica do evento;
- permitir revisão posterior por pesquisadores, entusiastas e equipes técnicas;
- preservar um registro histórico acessível em inglês e em português.

## O que este repositório contém

Os arquivos principais normalmente seguem este padrão:

- `ddmmyyyy-hhmm-transcricao.txt`
  - contém a **transcrição original em inglês**;
- `ddmmyyyy-hhmm-traducao.txt`
  - contém a **tradução para português do Brasil**;
- `ddmmyyyy-hhmm-analise.txt`
  - contém uma **análise técnica e de riscos** baseada na linha do tempo capturada.

## Formato dos arquivos

### Transcrição em inglês

Cada linha representa uma entrada da timeline:

```txt
[22:46:36] and growing closer to our lunar neighbor, now 222,000 miles away from the Moon.
[22:46:39] Integrity, for your information, toilet is a go for use.
```

### Tradução em português

A tradução segue o mesmo timestamp da transcrição original:

```txt
[22:46:36] e se aproximando cada vez mais do nosso vizinho lunar, agora a 222.000 milhas da Lua.
[22:46:39] Integrity, para sua informação, o toalete está liberado para uso.
```

### Análise técnica

O arquivo de análise resume:

- fase atual mais provável da missão;
- sucessos observados;
- sucessos com desafios;
- riscos e anomalias;
- próximos marcos prováveis.

## Como esses arquivos foram gerados

Os registros deste repositório foram produzidos por uma aplicação em Python criada para:

1. conectar-se ao áudio de uma live do YouTube;
2. detectar trechos de fala;
3. segmentar o áudio por pausas;
4. enviar os trechos para transcrição automática;
5. armazenar o histórico em arquivos `.txt`;
6. traduzir o conteúdo para PT-BR;
7. gerar análise técnica consolidada.

## Valor histórico

A Artemis II representa um passo central no retorno da humanidade ao espaço profundo e no caminho de volta à Lua.

Este repositório busca servir também como **arquivo documental** de um período histórico, permitindo revisitar comunicações, decisões e eventos operacionais de forma organizada e legível.

## Organização sugerida

```txt
.
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── FILE_FORMATS.md
│   └── PROJECT_OVERVIEW.md
├── transcricoes/
│   ├── 02042026-1742-transcricao.txt
│   └── ...
├── traducoes/
│   ├── 02042026-1742-traducao.txt
│   └── ...
└── analises/
    ├── 02042026-1742-analise.txt
    └── ...
```

## Observações

- As transcrições podem conter trechos truncados, especialmente em momentos de ruído, sobreposição de voz ou limitações do reconhecimento automático.
- Siglas técnicas, nomes próprios e códigos de missão podem aparecer sem normalização completa.
- O objetivo principal é **preservação contextual e histórica**, com o máximo de fidelidade possível ao áudio transmitido.

## Autor

Projeto desenvolvido para registrar e compreender, com maior riqueza de detalhes, comunicações relacionadas à missão Artemis II, ajudando a tornar esse momento histórico mais acessível mesmo para quem acompanha remotamente.
