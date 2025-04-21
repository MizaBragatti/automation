# Documentação:

---

Playlist do youtube:
[Link](https://www.youtube.com/playlist?list=PL4GZKvvcjS3vAPWLqWbKZogkL5cD71yrT)

## Robot Framework And Appium - Install Environment On Windows

1. Instalar Java JDK
   - [Link](https://www.oracle.com/th/java/technologies/downloads/#jdk24-windows)
   - Configurar Variáveis Locais
     - JAVA_HOME | C:\Program Files\Java\jdk-24
     - pasta PATH
       - %JAVA_HOME%\bin
2. Instalar Android Studio  
   - [Link](https://developer.android.com/studio?hl=pt-br)
   - Configurar Variáveis Locais
     - ANDROID_HOME | C:\Users\\\<user>\AppData\Local\Android\Sdk
     - pasta PATH
       - %ANDROID_HOME%\tools
       - %ANDROID_HOME%\tools\bin
       - %ANDROID_HOME%\build-tools
       - %ANDROID_HOME%\emulator
3. Instalar Node
   - [Link](https://nodejs.org/pt)
4. Instalar Appium  
   ```bash
   npm install -g appium  
   ```
   ```bash
   appium --version 
   ```
5. Instalar Appium Doctor
    ```bash
   npm install -g appium-doctor  
   ```
      ```bash
   appium-doctor 
   ```
6. Instalar Robot Framework
    ```bash
   pip install robotframework-appiumlibrary  
   ```
   ```bash
   pip list 
   ```
   
## Robot Framework And Appium - Configure Devices And Emulators

1. Conectar o Dispositivo físico
   - Executar o comando para verificar se conectou  
    ```bash
     adb devices  
    ```
2. Baixar um programa para espelhar a tela do celular
   - [Vysor](https://www.vysor.io/) 
   - [scrcopy](https://github.com/Genymobile/scrcpy)

3. Criar um Emulador
   - Criar no Device Manager
     - Ex. Pixel 3a | 5.6" | 1080x2220 | 440dpi
   - Escolher Imagem do Sistema
     - Ex. Q | 29 | x86 | Android 10.0 (Google Play)
   - Cria um nome para o Emulador
     - Ex. Pixel_3a_Android_10
   - Inicia o Emulador
     