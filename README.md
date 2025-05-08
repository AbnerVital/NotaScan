# 📄 Extração de Dados de Notas Fiscais em PDF com PyMuPDF

Este projeto tem como objetivo extrair informações de notas fiscais eletrônicas (NFS-e, NF-e, NFC-e) de arquivos PDF utilizando a biblioteca PyMuPDF (fitz). O código foi desenvolvido para extrair dados de um formato específico de nota fiscal, e pode ser adaptado para outros formatos de documentos fiscais. Os dados extraídos são exportados para um arquivo Excel, facilitando o processamento e análise posterior.

O código serve como **exemplo** para outros projetos que envolvem a extração de dados de PDFs de notas fiscais, sendo possível customizar as expressões regulares para diferentes padrões de documentos fiscais.

## 📌 Sobre o Projeto

O script foi desenvolvido em Python e utiliza a biblioteca **PyMuPDF** para processar arquivos PDF e buscar informações específicas, como:

- Número da Nota
- CNPJ do Tomador
- Valor dos Serviços
- Valor Líquido
- Total de Retenções

As informações extraídas são organizadas em um DataFrame do **pandas** e exportadas para um arquivo Excel, facilitando o processamento e análise posterior.

## 🚀 Como Executar o Projeto

### 1. Instale as dependências

Certifique-se de ter a biblioteca **PyMuPDF** instalada. Caso não tenha, você pode instalá-la usando o seguinte comando:

```bash
pip install pymupdf
````

### 2. Suba os arquivos PDF

O script permite o upload de múltiplos arquivos PDF através do **Google Colab**, que serão processados para extrair as informações.

### 3. Execute o Script

Basta executar o script no ambiente **Google Colab**. O código irá:

1. Processar os arquivos PDF enviados.
2. Buscar as informações das notas fiscais.
3. Gerar um arquivo Excel com as informações extraídas.

### 4. Download do Arquivo Excel

Após a execução, o arquivo **Excel** com os dados extraídos será disponibilizado para download.

## 🧱 Estrutura do Projeto

```plaintext
📁 extracao-notas-fiscais/
├── 📄 extracao_notas_fiscais.py        # Script Python para extrair dados de PDFs
└── 📄 README.md                        # Documentação do projeto
```

## 🔍 Funcionalidades

* **Extração de dados de PDFs**: O script busca e extrai informações específicas, como número da nota, CNPJ do tomador, valores de serviços e retenções.
* **Processamento de múltiplos arquivos**: O script suporta o upload de vários PDFs e processa cada um deles individualmente.
* **Exportação para Excel**: Os dados extraídos são organizados em uma planilha Excel para fácil análise.
* **Limpeza de arquivos**: Após a extração, os arquivos PDF enviados são removidos automaticamente.

## 📸 Captura de Tela

* Exemplo de estrutura de dados extraídos:

| Arquivo   | Número da Nota  | CNPJ Tomador       | Valor dos Serviços (R\$) | Valor Líquido (R\$) | Total Retenções (R\$) |
| --------- | --------------- | ------------------ | ------------------------ | ------------------- | --------------------- |
| nota1.pdf | 123456789012345 | 12.345.678/0001-99 | 100,00                   | 90,00               | 10,00                 |
| nota2.pdf | 987654321098765 | 98.765.432/0001-88 | 200,00                   | 180,00              | 20,00                 |

## 📈 Melhorias Futuras

* Implementar a extração de mais campos das notas fiscais, como dados do prestador de serviços.
* Integrar com sistemas de API para automatizar o envio de dados extraídos.
* Melhorar o tratamento de exceções e erros para arquivos mal formatados.

## 👨‍💻 Autor

| [<img src="https://avatars.githubusercontent.com/u/102125924?v=4" width=115><br><sub>Abner Vital</sub>](https://github.com/AbnerVital) |
| :------------------------------------------------------------------------------------------------------------------------------------: |

## 📫 Contato

* **GitHub**: [@AbnerVital](https://github.com/AbnerVital)
* **LinkedIn**: [@Abner Vital](https://www.linkedin.com/in/abner-vital-233730141/)

---

