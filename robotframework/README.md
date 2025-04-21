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