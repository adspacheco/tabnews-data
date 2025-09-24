# TabNews Data Collection

Este repositório contém uma coleção estruturada de dados do projeto **TabNews** em formato markdown, otimizada para alimentar agentes de codificação e sistemas de inteligência artificial.

## 📋 Visão Geral

Os arquivos markdown neste repositório foram processados e compactados com tags específicas para facilitar o consumo por modelos de linguagem e ferramentas de análise de código. Todos os dados são apresentados em formato estruturado para maximizar a eficiência no processamento automatizado.

## 📁 Descrição dos Arquivos

### `codebase.md` (1.6MB)
**Representação completa do código-fonte do TabNews**

- Contém todo o código-fonte do repositório TabNews empacotado em um único documento
- Processado pela ferramenta Repomix com verificação de segurança desabilitada
- Inclui estrutura de diretórios, arquivos de configuração, e código fonte completo
- Organizado com tags estruturadas para fácil navegação por IA
- Exclui arquivos binários, fontes e diretórios públicos
- Arquivos ordenados por contagem de mudanças Git (mais alterados no final)
- Ideal para análise de código, revisão automatizada e compreensão da arquitetura

**Formato:**
```
<file_summary>...</file_summary>
<directory_structure>...</directory_structure>
<file path="...">conteúdo do arquivo</file>
```

### `pull_requests.md` (1.2MB)  
**Histórico completo de Pull Requests**

- Coleção estruturada de todos os Pull Requests mergeados do projeto TabNews
- Inclui descrições, comentários de review, e feedback inline no código
- Dados extraídos diretamente da API do GitHub
- Títulos sanitizados para evitar caracteres problemáticos
- Ideal para análise de padrões de desenvolvimento, geração de changelogs, e insights sobre contribuidores

**Formato:**
```
<pull_{número}_{título_sanitizado}>
Descrição do PR
> > Review de {usuário} ({estado}):
> > Comentário de review
> > Comentário inline
</pull_{número}_{título_sanitizado}>
```

### `issues.md` (0B)
**Arquivo de Issues (atualmente vazio)**

- Preparado para conter o histórico de issues do repositório TabNews
- Formato estruturado similar aos Pull Requests
- Será povoado com dados de bugs, feature requests e discussões

### `prompt.md` (1KB)
**Template de Prompt para Agente TabNews**

- Prompt especializado para criar um agente de IA expert no projeto TabNews
- Define o contexto, responsabilidades e estilo de comunicação do agente
- Foco no entendimento e aprendizado, não em gerar código automaticamente
- Configurado para usar os dados estruturados deste repositório como base de conhecimento
- Inclui diretrizes para manter a consistência com a filosofia e padrões do projeto

### `README.md` (este arquivo)
**Documentação e guia de uso**

## 🎯 Casos de Uso

### Para Agentes de IA e Aprendizado
- **Mentor Técnico Especializado**: Use `prompt.md` para criar um assistente expert focado no entendimento do TabNews
- **Análise Arquitetural**: Compreenda decisões técnicas e padrões através do histórico de PRs
- **Orientação para Contribuições**: Aprenda a filosofia do projeto e como propor melhorias alinhadas
- **Context Window Otimizado**: Arquivos estruturados para maximizar o aproveitamento em LLMs
- **Code Review Educativo**: Análise baseada em padrões históricos para aprendizado

### Para Análise de Projeto
- **Evolução do Código**: Histórico completo via Pull Requests
- **Padrões de Desenvolvimento**: Análise de reviews e comentários
- **Documentação Automatizada**: Geração de docs baseada no código
- **Métricas de Qualidade**: Análise de práticas de desenvolvimento

## 🔧 Como Usar

### Criando um Agente TabNews
**Método recomendado com Claude Projects (ou similar):**

1. **Crie um novo projeto/agente** na sua plataforma de IA preferida
2. **Adicione os arquivos de dados** como knowledge base:
   - `codebase.md` - código completo do projeto
   - `pull_requests.md` - histórico de PRs e reviews  
   - `issues.md` - issues e discussões (quando disponível)
3. **Configure as instruções** usando o conteúdo do `prompt.md`

O agente estará pronto para ajudar no entendimento do projeto, explicar decisões arquiteturais, e orientar contribuições alinhadas com a filosofia do TabNews.

### Uso Programático
```bash
# Carregar código completo
cat codebase.md | your-ai-tool

# Analisar histórico de PRs
cat pull_requests.md | your-analysis-tool
```

### Processamento de Tags
Os arquivos usam tags XML-like para estruturação:
- `<file_summary>`: Metadados e instruções
- `<directory_structure>`: Estrutura de pastas
- `<file path="...">`: Conteúdo individual de arquivos
- `<pull_*>`: Pull Requests individuais

## ⚠️ Considerações Importantes

- **Somente Leitura**: Arquivos são snapshots, alterações devem ser feitas no repositório original
- **Informações Sensíveis**: Verificação de segurança foi desabilitada, trate com cuidado
- **Tamanho**: Arquivos grandes otimizados para processamento em lote
- **Atualização**: Dados refletem estado específico no tempo, não são atualizados automaticamente

## 📊 Estatísticas

| Arquivo | Tamanho | Conteúdo |
|---------|---------|----------|
| `codebase.md` | 1.6MB | Código completo do TabNews |
| `pull_requests.md` | 1.2MB | PRs mergeados e reviews |
| `issues.md` | 0B | Issues (a ser povoado) |
| `prompt.md` | 1KB | Template de prompt para agente |

---

> 💡 **Dica**: Para melhor performance com LLMs, considere dividir arquivos grandes em chunks baseados nas tags estruturais.
