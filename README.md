# Automação de Operações de Refinanciamento no Bradesco

Este repositório contém um script Python que utiliza a biblioteca Selenium para automatizar operações de refinanciamento no site do Bradesco. O objetivo principal do script é facilitar a consulta e gestão de operações de refinanciamento disponíveis, utilizando técnicas de automação para melhorar a eficiência e reduzir a necessidade de interação manual.

## Características Principais

- **Uso de Proxies:** Para evitar bloqueios por parte do site alvo, o script configura proxies, mascarando o endereço IP real do usuário.

- **Automação de Login:** Realiza login automático no site do Bradesco utilizando credenciais armazenadas em um arquivo de configuração separado, aumentando a segurança.

- **Navegação e Seleção Automatizada:** Após o login, o script navega até a seção de refinanciamento, selecionando as opções adequadas para consulta de operações disponíveis.

- **Captura de Informações:** Extrai informações detalhadas sobre as operações de refinanciamento, como valores, status e dados para novas operações.

- **Manuseio de Captchas:** Utiliza a API do TwoCaptcha para resolver automaticamente captchas que possam surgir durante a navegação, garantindo continuidade no processo de automação.

## Funcionalidades Implementadas

1. **Configuração de Proxies:** Inicializa a navegação configurando proxies através de uma extensão dinâmica criada em tempo de execução.

2. **Login Automático:** Acessa o site do Bradesco, inserindo as credenciais de usuário para login de forma automatizada.

3. **Seleção de Opções de Refinanciamento:** Navega pelas páginas necessárias, selecionando automaticamente as opções relacionadas ao refinanciamento.

4. **Extração de Dados:** Captura e organiza os dados das operações de refinanciamento disponíveis, como valor da operação, valor da parcela, saldo devedor e status.

5. **Resolução de Captchas:** Integra com o serviço TwoCaptcha para resolver desafios de captcha, essenciais para a continuação da navegação no site.

## Segurança

O script faz uso de um arquivo de configuração externo (`config.py`) para armazenar credenciais sensíveis, como logins e senhas, separando essas informações do código principal. Esta prática aumenta a segurança e facilita a manutenção do código.
