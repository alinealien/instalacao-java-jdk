## Passo a Passo para Instalar o Java JDK no Windows

**Antes de tudo:**
* Verifique se você tem o java instalado na máquina: `java -version` ou `java --version`;

1. **Baixar o JDK**: Acesse o site oficial da Oracle para baixar o JDK. Você pode encontrar a página de downloads em: [Java SE Downloads](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html).

2. **Aceitar o Acordo de Licença**: Antes de baixar o JDK, você precisará aceitar o Acordo de Licença da Oracle.

3. **Escolher a Versão Correta**: Certifique-se de baixar a versão correta do JDK para o seu sistema operacional Windows (32-bit ou 64-bit). Escolha o arquivo executável (`.exe`) adequado.

4. **Iniciar o Instalador**: Após o download, clique duas vezes no arquivo executável para iniciar o instalador.

5. **Selecionar Local de Instalação**: Durante o processo de instalação, você poderá ser solicitado a selecionar o local de instalação. O padrão é geralmente em `C:\Program Files\Java\jdk-xx`. Caso não seja solicitado, o instalador criará uma pasta como `C:\Program Files\Common Files\` e `C:\Program Files\Java\`.

6. **Configurar Diretamente as Variáveis de Ambiente**:
   - **Variável de Ambiente `JAVA_HOME`**: Esta variável deve apontar para o diretório de instalação do JDK.
     - Clique com o botão direito em "Meu Computador" ou "Este Computador" e selecione "Propriedades".
     - Clique em "Configurações avançadas do sistema" (ou "Configurações avançadas do sistema" no Windows 10).
     - Na aba "Avançado", clique em "Variáveis de ambiente".
     - Em "Variáveis do sistema", clique em "Novo" e adicione uma nova variável de sistema chamada `JAVA_HOME` com o valor do diretório de instalação do JDK (por exemplo, `C:\Program Files\Java\jdk-xx`).
   - **Variável de Ambiente `PATH`**: Adicione o caminho para o diretório `bin` do JDK ao `PATH`.
     - Encontre a variável de sistema chamada `PATH` em "Variáveis do sistema".
     - Edite esta variável e adicione `;%JAVA_HOME%\bin` no final do valor existente. Certifique-se de incluir o ponto-e-vírgula (`;`) antes de `%JAVA_HOME%\bin`.
     
7. **Verificar a Instalação**: Abra o Prompt de Comando e digite `java -version`. Isso deve exibir a versão do Java instalada, confirmando que a instalação foi bem-sucedida.
