# Guia de Edição do Portfólio (Atualizado)

Este documento contém instruções sobre como editar e personalizar seu site de portfólio com a nova estrutura de páginas individuais para matérias.

## Estrutura do Site

O site de portfólio foi desenvolvido com uma estrutura organizada, contendo as seguintes seções:

1. **Início (Hero)** - Apresentação inicial com seu nome e curso
2. **Sobre Mim** - Informações acadêmicas, habilidades e biografia
3. **Matérias** - Cards com links para páginas individuais de cada matéria
4. **Contato** - Formulário e informações de contato

### Páginas Individuais de Matérias
Cada matéria possui sua própria página com:
- Informações do professor
- Resumo da matéria
- Lista de conteúdos com links para páginas específicas

### Páginas de Conteúdo
Cada conteúdo possui sua própria página com:
- Detalhes do conteúdo
- Botão para repositório no GitHub
- Navegação de retorno para a página da matéria

## Como Editar o Conteúdo

### Página Principal (index.html)

1. Abra o arquivo `index.html` em um editor de texto ou IDE
2. Edite as informações pessoais na seção Hero
3. Atualize a seção "Sobre Mim" com suas informações acadêmicas
4. Personalize os cards de matérias com os nomes corretos das disciplinas
5. Atualize as informações de contato

### Páginas de Matérias (materias/materia1.html, etc.)

1. Abra cada arquivo de matéria em um editor
2. Substitua "Nome da Matéria" pelo nome real da disciplina
3. Adicione informações do professor na seção correspondente
4. Escreva um resumo sobre a matéria
5. Personalize os itens de conteúdo com títulos e descrições relevantes
6. Atualize os links para os repositórios GitHub específicos de cada conteúdo

### Páginas de Conteúdo (materias/materia1/conteudos/conteudo1.html, etc.)

1. Abra cada arquivo de conteúdo em um editor
2. Substitua "Nome do Conteúdo" pelo título real
3. Atualize a data e outras informações meta
4. Preencha as seções de introdução, desenvolvimento e conclusão
5. Atualize o link para o repositório GitHub específico deste conteúdo

## Áreas Editáveis

Todas as áreas com a classe `editable-content` foram projetadas para serem facilmente identificáveis e editáveis. Ao passar o mouse sobre essas áreas no navegador, elas exibirão uma borda tracejada para indicar que são editáveis.

## Personalização Visual

### Cores

As cores principais do site estão definidas como variáveis CSS no arquivo `css/styles.css`:

```css
:root {
  --primary: #6c5ce7;      /* Cor primária (roxo suave) */
  --secondary: #00cec9;    /* Cor secundária (turquesa) */
  --background: #1e272e;   /* Cor de fundo (escuro) */
  --text-primary: #f5f6fa; /* Cor de texto principal */
  --text-secondary: #dcdde1; /* Cor de texto secundário */
  --accent: #00b894;       /* Cor de destaque (verde menta) */
}
```

Para alterar a paleta de cores, basta modificar esses valores.

### Fontes

O site utiliza as fontes Montserrat (para títulos) e Roboto (para textos), carregadas do Google Fonts. Para alterar as fontes:

1. Escolha novas fontes no [Google Fonts](https://fonts.google.com/)
2. Atualize o link no cabeçalho HTML
3. Modifique as referências às fontes no CSS

## Adicionando Novos Conteúdos

### Adicionar Novo Conteúdo a uma Matéria

1. Duplique um arquivo de conteúdo existente (ex: `conteudo1.html`)
2. Renomeie-o para `conteudo2.html`, `conteudo3.html`, etc.
3. Atualize o título, descrição e links
4. Adicione um novo item na lista de conteúdos na página da matéria correspondente

### Adicionar Imagens

Para adicionar suas próprias imagens:
1. Crie uma pasta `images` dentro da pasta `public`
2. Adicione suas imagens a esta pasta
3. Referencie-as no HTML usando o caminho relativo: `<img src="../images/sua-imagem.jpg">`

## Navegação Entre Páginas

O site foi estruturado com uma navegação intuitiva:
- A barra de navegação principal está presente em todas as páginas
- Breadcrumbs (navegação em trilha) ajudam a localizar a página atual
- Botões de "Voltar" permitem retornar à página anterior
- Links para GitHub levam diretamente aos repositórios de projetos

## Responsividade

O site foi projetado para funcionar perfeitamente em dispositivos de todos os tamanhos:
- Desktop e laptops
- Tablets
- Smartphones

Arquivos CSS adicionais (`responsive.css`) contêm ajustes específicos para garantir que todos os elementos se adaptem corretamente a diferentes tamanhos de tela.

## Dicas para Manutenção

1. **Backup**: Sempre faça uma cópia de segurança antes de realizar alterações significativas
2. **Teste em Dispositivos**: Verifique como o site se comporta em diferentes tamanhos de tela
3. **Validação**: Use ferramentas como o [W3C Validator](https://validator.w3.org/) para verificar seu HTML
4. **Otimização de Imagens**: Comprima imagens antes de adicioná-las ao site

## Hospedagem

Para disponibilizar seu portfólio online, você pode usar serviços como:
- GitHub Pages (gratuito)
- Netlify (gratuito)
- Vercel (gratuito)
- InfinityFree (gratuito)
- Hostinger (pago)

## Suporte

Este portfólio foi desenvolvido para ser facilmente editável e expansível. Se precisar de ajuda adicional, consulte recursos online sobre HTML, CSS e JavaScript básico.
