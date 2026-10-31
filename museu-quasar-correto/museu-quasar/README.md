# Museu Quasar — projeto HTML5

Portal fictício de um museu digital, feito somente com HTML5, sem CSS, JavaScript ou backend. O tema reúne três exposições: **Quasares e galáxias**, **Oceanos profundos** e **Invenções que mudaram rotinas**.

## Abrir o projeto

Extraia a pasta `museu-quasar` e abra `index.html` no navegador. Os caminhos das páginas e das mídias são relativos; mantenha a estrutura de pastas ao mover os arquivos.

## Páginas

- `index.html`: apresentação, motivos para visitar, passos de exploração e links para exposições.
- `paginas/exposicoes.html`: as três exposições, curiosidades, áudio, vídeo legendado e FAQ expansível.
- `paginas/programacao.html`: tabela semântica com seis atividades fictícias.
- `paginas/agendamento.html`: formulário de demonstração com validação HTML nativa.
- `paginas/sobre.html`: desafio extra com a história fictícia do museu.

## Recursos novos pesquisados e aplicados

1. **`scope` em `th`** — em `paginas/programacao.html`, relaciona cada cabeçalho aos dados da coluna (`scope="col"`) ou da linha (`scope="row"`), melhorando a compreensão da tabela por tecnologias assistivas.
2. **`track` e WebVTT** — em `paginas/exposicoes.html`, associa a faixa `midias/videos/visita-quasar.vtt` ao vídeo para oferecer legendas em português.
3. **`datalist`** — em `paginas/agendamento.html`, sugere nomes de instituições ou grupos, mas permite digitar outra opção. Também foram praticados `figure`/`figcaption`, `details`/`summary`, `time datetime` e `caption` na tabela.

## Dificuldades e soluções

- **Caminhos relativos entre diretórios:** links e mídias nas páginas de `paginas/` usam `../` para voltar à pasta principal antes de acessar `midias/` ou `index.html`.
- **Validação do formulário:** os campos usam tipos nativos, `required`, limites e `pattern` para o convite; os radios compartilham o mesmo `name` para permitir somente uma escolha.

## Fontes e licenças

- As imagens de quasar, oceano e oficina de invenções foram criadas para este projeto com geração de imagem por IA; estão incluídas localmente e não dependem de links externos.
- `paisagem-espacial.wav` é uma paisagem sonora sintetizada originalmente para o projeto.
- `visita-quasar.mp4` e as legendas WebVTT foram produzidos para este projeto.
- Os textos sobre o museu, as exposições, curiosidades e programação são fictícios e não apresentam dados científicos específicos.
- Links externos opcionais para consulta: [NASA — Universe](https://science.nasa.gov/universe/), [NOAA Ocean Service](https://oceanservice.noaa.gov/) e [Smithsonian Institution](https://www.si.edu/). As páginas externas não são necessárias para o funcionamento do site.
- O HTML foi elaborado com base em elementos e atributos padrão do HTML Living Standard; documentação de apoio: [MDN Web Docs — HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML).

## Funcionalidades e limites

A navegação entre páginas, âncoras, controles de mídia e validação básica do formulário funcionam no navegador. O formulário é apenas uma simulação: não tem `action`, método configurado, armazenamento nem envio para um servidor. A agenda, o museu e as atividades não são reais.
