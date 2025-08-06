___
[[Cris Braun/Cris Braun|Cris Braun]]
[[Wado]]

___
## Prompts
```
O objeto no anexo é sua base de conhecimento para esta conversa. Toda esta conversa será baseada neste arquivo json com a seguinte interface:

{ 
	filePath: string;
	fileContent: string;
}[]

❗ Nunca assuma, infira ou simule a existência de arquivos, componentes, telas ou diretórios. Toda resposta deve se basear exclusivamente nos filePaths listados no JSON. Qualquer menção a algo inexistente é considerada erro grave.

Você deve:
- Carregar 100% da estrutura do JSON.
- Criar uma lista interna com todos os filePaths.
- Toda operação, leitura ou edição deve usar o filePath, nunca apenas o nome do arquivo.
- Toda edição deve reescrever o arquivo inteiro, manter o padrão original, usar inglês na criação de códigos (inclusive comentários), e respeitar o ESLint.
- Responder em português no chat
Essas regras são obrigatórias. Qualquer erro básico de leitura é falha grave. Não responda até confirmar leitura do JSON.
```

```
Dentre os `fileContent` do arquivo no anexo existem marcações `!!!TO-DO:` seguidas de instruções do que fazer ali. Retorne as respostas, uma a uma, as relacionando com suas respectivas `filePath`
```

```
Quero montar o mesmo projeto `wado.json`, com a mesma estrutura e seguindo exatamente os mesmos moldes de criação de conteúdo dos módulos e arquivos, mas para criar conteúdo para <nome_do_artistico_e_nome_real_completo_do_artista>. Quero que a entrega seja feita em arquivos .md separados por "filePath", não como um .json único
```