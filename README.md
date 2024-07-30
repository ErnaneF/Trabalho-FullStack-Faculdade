# Trabalho-FullStack-Faculdade
Acesse o site: *https://ernanef.github.io/Trabalho-FullStack-Faculdade/* 
**Membros do grupo**: 
- Ernane Manoel da Silva Filho
- Brunno Zara Bolognisi
- Jhonnatan

# Estrutura e Requisitos

## Pagina principal

### Introdução
O site "Fernanda Esteticista" foi desenvolvido para promover os serviços de uma renomada esteticista facial e corporal. O objetivo é fornecer uma plataforma informativa e interativa onde os clientes possam conhecer os serviços oferecidos, visualizar resultados anteriores e agendar sessões facilmente.

### Requisitos

1. **HTML5 Semântico**: Utilização de tags semânticas para melhor organização e acessibilidade do conteúdo.
2. **Responsividade**: Uso do sistema de grid do Bootstrap para garantir que o site seja responsivo e adaptável a diferentes tamanhos de tela.
3. **Estilização**: Utilização do Bootstrap e CSS customizado para estilização dos componentes.
4. **Interatividade**: Uso de jQuery para adicionar funcionalidades interativas, como rolagem suave e máscaras de input.
5. **Componentes do Bootstrap**: Uso de no mínimo 10 componentes do Bootstrap, como Navbar, Cards, Carousel, Forms, etc.
6. **Formulários**: Inclusão de formulários para cadastro de usuários e login.
7. **Eventos do jQuery**: Implementação de no mínimo 3 eventos do jQuery.

### Estrutura do Código

#### HTML

1. **Cabeçalho (`<head>`)**
    - Metadados e links para estilos e scripts externos.
    - Inclusão do Bootstrap, jQuery, Popper.js, Font Awesome e outros recursos.
    
2. **Corpo (`<body>`)**
    - **Header**: Contém a Navbar fixa no topo com links para seções do site.
    - **Seções Principais**:
        - **Home**: Seção inicial com o banner.
        - **Sobre**: Informações sobre a esteticista Fernanda Farias e os serviços oferecidos.
        - **Serviços**: Detalhes dos serviços oferecidos, organizados em um carousel.
        - **Resultados**: Exemplos de resultados de tratamentos anteriores.
        - **Contato**: Formulário para agendamento de sessões e mapa de localização.

3. **Footer**
    - Informações de contato, endereço e links para redes sociais.

#### CSS

- **Bootstrap**: Utilizado para estilização base e componentes responsivos.
- **Custom CSS** (`ajustes.css`): Estilos personalizados para ajustes específicos do site.

#### JavaScript

1. **jQuery**: Usado para adicionar interatividade, como rolagem suave e máscaras de input.
2. **Máscaras de Input**: Plugin jQuery Mask para formatação do campo de telefone.
3. **Bootstrap JS**: Scripts para componentes do Bootstrap como o carousel e dropdown.

### Detalhamento das Seções

1. **Header**
    - Navbar com logo e links para navegação suave entre as seções do site.
    - Botão de toggler para navegação em dispositivos móveis.

2. **Home**
    - Seção inicial que pode conter um banner ou imagem de destaque.

3. **Sobre**
    - Texto detalhado sobre a esteticista Fernanda Farias e os serviços que ela oferece.
    - Imagem ilustrativa.

4. **Serviços**
    - Carousel com cards detalhando os serviços faciais, corporais e especiais como Banho de Lua e Hydra Gloss Lips.
    - Cada card contém uma lista detalhada dos tratamentos oferecidos.

5. **Resultados**
    - Cards com exemplos de resultados de tratamentos anteriores.
    - Imagens e descrições dos tratamentos com datas e links para agendamento.

6. **Contato**
    - Formulário para agendamento de sessões com campos para nome, telefone e seleção do tipo de serviço.
    - Mapa de localização embutido com a localização da esteticista.

7. **Footer**
    - Informações de endereço e contatos.
    - Links para redes sociais como Instagram e Facebook.

### Scripts

1. **jQuery Smooth Scroll**
    ```javascript
    $(document).ready(function() {
        $('.smooth-scroll').on('click', function(event) {
            event.preventDefault();
            var target = $(this).attr('href');
            $('html, body').animate({
                scrollTop: $(target).offset().top
            }, 800);
        });
    });
    ```

2. **jQuery Mask para Telefone**
    ```javascript
    $(document).ready(function(){
        $('#phone').mask('(00) 00000-0000');
    });
    ```

### Favicons

- Favicons em vários formatos (ico, png) para diferentes dispositivos.


## Pagina de Login

## Introdução
Esta página de login foi criada para autenticação de usuários no site "Fernanda Esteticista". Ela contém campos para inserção de email e senha, opções de lembrar a senha e um link para recuperação de senha esquecida.

## Estrutura do Código

### HTML

1. **Cabeçalho (`<head>`)**
    - Metadados e links para estilos externos.
    - Inclusão do arquivo CSS customizado (`login.css`).

2. **Corpo (`<body>`)**
    - **Div `login-wrapper`**: Contém o formulário de login.
    - **Formulário**:
        - **Título**: `h2` com o texto "Login".
        - **Campo de Email**: `input` de texto com label "Digite seu email".
        - **Campo de Senha**: `input` de senha com label "Digite sua senha".
        - **Opções de Senha**:
            - Checkbox para lembrar a senha.
            - Link para recuperação de senha.
        - **Botão de Envio**: Botão para submeter o formulário.
        - **Opções de Conta**: Texto e link para criar uma nova conta.


### CSS

1. **Arquivo: Login**
    - **Objetivo**: Estilização personalizada dos campos de login, botões e opções.





## Pagina de Administrador

## Introdução
Esta página administrativa foi criada para gerenciar os administradores do site "Fernanda Esteticista". Inclui funcionalidades para adicionar novos administradores, exportar dados, filtrar administradores e visualizar suas permissões.

## Estrutura do Código

### HTML

1. **Cabeçalho (`<head>`)**
    - Metadados e links para estilos externos.
    - Título da página.
    - Inclusão dos arquivos CSS do Bootstrap e ajustes personalizados.

2. **Corpo (`<body>`)**
    - **Div `container`**: Contém o conteúdo principal da página.
    - **Título**: `h2` com o texto "Administradores".
    - **Botões de Ação**: Botões para adicionar e exportar administradores.
    - **Campo de Pesquisa**: Input para adicionar filtros.
    - **Tabela de Administradores**: Tabela listando os administradores com colunas de ID, Nome, Usuário, Status e Ações.
    - **Rodapé**: Informações de suporte técnico e links úteis.
