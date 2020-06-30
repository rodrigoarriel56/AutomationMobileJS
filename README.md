
## 1-) Rodar o Sh com as Dependencias:

Acessar o diretório por terminal e rodar o seguinte comando:
$ sh install_dependencies.sh

## 2-) Configurar seu Bash Profile:

Adicionar isso no seu ~/.bash_profile
```
export ANDROID_HOME=/Users/$(whoami)/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH/:$ANDROID_HOME/platform-tools
export JAVA_HOME=$(/usr/libexec/java_home)
#export PATH=${JAVA_HOME}/bin:$PATH
```

## 3-) Rodar o comando para salvar o bash profile:
Run: `$ source ~/.bash_profile`


Se rodar o appium-doctor e aparecer problema no bin, por favor descomentar a ultima linha do bin e rodar o comando do passo 3 novamente.


## 4-) Json para configurar o Appium Desktop:
{
  "platformName": "Android",
  "deviceName": "920110594119334a",
  "app": "C:\\GitMobile\\FrameworkMobile\\automationMobile\\App\\Android\\app-qa-release0.64.0.apk",
  "automationName": "uiautomator2"
}`

IOS: `{
  "app": "C:\\GitMobile\\FrameworkMobile\\automationMobile\\App\\iOS\\.ipa"",
  "platformName": "iOS",
  "platformVersion": "12.2",
  "deviceName": "iPhone X"
}`
