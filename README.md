# 🤖 Automação de Testes com Robot Framework

Este projeto tem como objetivo demonstrar o uso do **Robot Framework** para automação de testes de forma simples, legível e eficiente.

---

## 📌 O que é o Robot Framework?

O **Robot Framework** é uma estrutura de automação de testes de código aberto, escrita em Python, que utiliza uma sintaxe simples baseada em palavras-chave (keywords). Ele é especialmente útil para testes de aceitação e testes de comportamento (ATDD/BDD).

Com o Robot, é possível escrever casos de teste em formato de tabela (usando arquivos `.robot`) de forma muito intuitiva, mesmo para quem não tem experiência com programação.

---

## 🚀 Vantagens do Robot Framework

- ✅ Sintaxe legível por humanos
- 🔌 Suporte a bibliotecas externas (SeleniumLibrary, RequestsLibrary, etc)
- 🧩 Fácil integração com ferramentas CI/CD
- 🧪 Excelente para testes end-to-end e APIs
- 📊 Geração automática de relatórios e logs detalhados

---

## 📁 Estrutura do Projeto

```
tests/
│   login_tests.robot
│   cadastro_tests.robot
resources/
│   keywords.robot
│   variables.robot
results/
│   (relatórios gerados automaticamente)
```

---

## ▶️ Executando os Testes

Certifique-se de ter o Python instalado e instale as dependências com pip:

```bash
pip install robotframework
pip install robotframework-seleniumlibrary
```

Para rodar os testes:

```bash
robot tests/
```

Após a execução, os relatórios serão gerados automaticamente nas pastas:

- `log.html`
- `report.html`
- `output.xml`

---

## 📚 Exemplos de Keywords

```robot
*** Test Cases ***
Login com sucesso
    [Tags]    login    positivo
    Abrir navegador    https://meusite.com
    Preencher campo    usuário    admin
    Preencher campo    senha      123456
    Clicar botão       Entrar
    Verificar texto    Bem-vindo, admin

*** Keywords ***
Abrir navegador
    [Arguments]    ${url}
    Open Browser    ${url}    chrome
    Maximize Browser Window
```

---

## 🛠 Tecnologias e Bibliotecas Utilizadas

- [Robot Framework](https://robotframework.org/)
- [SeleniumLibrary](https://github.com/robotframework/SeleniumLibrary)
- [Python](https://www.python.org/)

---

## 🤝 Contribuindo

Sinta-se à vontade para contribuir com melhorias, novos testes ou sugestões. Pull requests são sempre bem-vindos! 🚀

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

📌 **Dica:** Use o VSCode com a extensão do Robot Framework para uma melhor experiência de escrita e execução dos testes.

---
