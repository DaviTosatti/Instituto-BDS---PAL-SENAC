# Instituto BdS · PAL Senac

Projeto desenvolvido em equipe no curso técnico em Informática do **Senac Lapa Tito**, voltado à conscientização sobre direitos trabalhistas e boas condições de trabalho, especialmente para jovens que estão ingressando no mercado.

O site reúne cadastros de usuários e empresas, avaliações, rankings e relatos sobre o ambiente de trabalho.

**Tecnologias:** PHP · MySQL · HTML · CSS · XAMPP

## Origem e versões

Esta é uma cópia de colaborador do projeto [PHenrique07/Instituto-BdS](https://github.com/PHenrique07/Instituto-BdS), publicada por Davi Tosatti com o histórico Git e os créditos da equipe preservados.

O código foi desenvolvido em equipe; os autores dos commits representam quem realizou os envios ao GitHub.

| Branch | Conteúdo |
| --- | --- |
| [`main`](https://github.com/DaviTosatti/Instituto-BDS---PAL-SENAC/tree/main) | Versão organizada em `src/` e `database/`, com exemplo de configuração da conexão. |
| [`legacy`](https://github.com/DaviTosatti/Instituto-BDS---PAL-SENAC/tree/legacy) | Estrutura original do projeto, preservada para consulta histórica. |

## Estrutura da branch main

```text
src/
├── pages/     # Páginas PHP e lógica da aplicação
├── admin/     # Área administrativa
├── css/       # Estilos
└── img/       # Imagens
database/
├── schema.sql
└── schema-v1.sql
```

## Preparação do ambiente local

Use o [XAMPP](https://www.apachefriends.org/) com Apache e MySQL ativos.

1. Abra o terminal na pasta `htdocs` do XAMPP — no Windows, normalmente `C:\xampp\htdocs` — e clone o projeto diretamente nela:

   ```bash
   git clone https://github.com/DaviTosatti/Instituto-BDS---PAL-SENAC.git Instituto-BDS
   cd Instituto-BDS
   ```

2. Crie a configuração local a partir do exemplo:

   ```bash
   cp src/pages/conexao-bds.example.php src/pages/conexao-bds.php
   ```

   No PowerShell, use `Copy-Item` no lugar de `cp`. Edite `src/pages/conexao-bds.php` com as credenciais do seu MySQL e mantenha esse arquivo apenas no ambiente local.

3. Revise `database/schema.sql` antes de importar. Ele é um script histórico e termina com `DROP TABLE Avaliacao;`, que exclui a tabela de avaliações após sua criação. Prepare uma cópia revisada para testes; o SQL original foi preservado neste repositório.

4. No [phpMyAdmin local](http://localhost/phpmyadmin), importe a cópia revisada em um ambiente de testes. O próprio script contém `CREATE DATABASE BDS` e `USE BDS`: não crie o banco previamente. Se já existir um banco `BDS`, use uma instância de testes separada.

5. Com a configuração e o banco preparados, o endereço de entrada é [localhost/Instituto-BDS/src/pages/index.php](http://localhost/Instituto-BDS/src/pages/index.php).

## Equipe

- [Pedro Henrique Santos da Silva](https://www.linkedin.com/in/pedro-henrique-santos-da-silva-40b521349/)
- [Davi Tosatti](https://www.linkedin.com/in/davi-tosatti-042b7519a/)
- [Gabriel Vaz Ferreira](https://www.linkedin.com/in/gabriel-vaz-284608351/)
- Lucas Henrique Furtado da Rosa Pio
- [Igor Costa](https://www.linkedin.com/in/igor-costa-417405355/)
- [Carlos Augusto Pires](https://www.linkedin.com/in/carlos-pires01/)
