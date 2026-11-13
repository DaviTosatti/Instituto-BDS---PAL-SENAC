# Instituto BdS · PAL Senac

**Versão original do projeto escolar, preservada na branch `legacy`.**

Projeto desenvolvido no curso técnico em informática do Senac Lapa Tito para conscientizar trabalhadores, especialmente jovens entrando no mercado de trabalho, sobre direitos trabalhistas e condições dignas de trabalho.

O site reúne conteúdo informativo, cadastro e login de usuários e empresas, perfis de empresas, avaliações e rankings. Foi construído com **PHP, MySQL, HTML e CSS**, usando **XAMPP** como ambiente local.

## Versões do projeto

| Branch | Conteúdo |
| --- | --- |
| [`main`](https://github.com/DaviTosatti/Instituto-BDS---PAL-SENAC/tree/main) | Versão com código organizado em `src/` e scripts SQL em `database/`. |
| [`legacy`](https://github.com/DaviTosatti/Instituto-BDS---PAL-SENAC/tree/legacy) | Estrutura original do projeto escolar, incluindo arquivos SQL e o pacote da época. |

Esta cópia foi publicada por **Davi Tosatti**, integrante e colaborador do projeto, a partir de [PHenrique07/Instituto-BdS](https://github.com/PHenrique07/Instituto-BdS). O histórico de commits foi preservado. O código foi desenvolvido em equipe; os autores dos commits representam quem realizou os envios ao GitHub. Nesta branch, apenas a apresentação deste README foi atualizada.

## Estrutura original

```text
PALBDSDEFINITIVO/
├── BDS 16 11.sql
├── BDS DEFINITIVO.sql
└── PALBDS xampp/
    ├── PALBDS.rar
    └── PALBDS/
        ├── Listas/         # Páginas administrativas
        └── PAL/            # Páginas PHP, estilos, imagens e conexão
```

## Ambiente local

1. Instale o [XAMPP](https://www.apachefriends.org/) e inicie **Apache** e **MySQL**.
2. Clone esta versão:

   ```bash
   git clone --branch legacy https://github.com/DaviTosatti/Instituto-BDS---PAL-SENAC.git Instituto-BDS-legacy
   ```

3. Copie a pasta `PALBDSDEFINITIVO/PALBDS xampp/PALBDS/` para `C:\xampp\htdocs\PALBDS\` no Windows, ou para o `htdocs` da sua instalação.
4. Revise os scripts SQL antes de importá-los pelo phpMyAdmin. Eles pertencem à versão escolar e incluem comandos de desenvolvimento: `BDS DEFINITIVO.sql`, por exemplo, termina com `DROP TABLE Avaliacao`. Para manter essa tabela, remova esse comando na cópia local usada na importação. O script já contém `CREATE DATABASE BDS` e deve ser usado em um ambiente local separado.
5. Ajuste `PAL/conexao-bds.php` com os dados do seu MySQL local. O arquivo original usa a configuração padrão de desenvolvimento do XAMPP.
6. Abra [localhost/PALBDS/PAL/index.php](http://localhost/PALBDS/PAL/index.php).

Esta branch registra a implementação da época. Para consultar a estrutura reorganizada e seu arquivo de exemplo de conexão, use a branch [`main`](https://github.com/DaviTosatti/Instituto-BDS---PAL-SENAC/tree/main).

## Equipe

- [Pedro Henrique Santos da Silva](https://www.linkedin.com/in/pedro-henrique-santos-da-silva-40b521349/)
- [Davi Tosatti](https://www.linkedin.com/in/davi-tosatti-042b7519a/)
- [Gabriel Vaz Ferreira](https://www.linkedin.com/in/gabriel-vaz-284608351/)
- Lucas Henrique Furtado da Rosa Pio
- [Igor Costa](https://www.linkedin.com/in/igor-costa-417405355/)
- [Carlos Augusto Pires](https://www.linkedin.com/in/carlos-pires01/)
