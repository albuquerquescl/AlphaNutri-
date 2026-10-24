AlphaNutri — pacote preparado para GitHub Actions

Estrutura:
- www/index.html: interface web da aplicação
- package.json: dependências Capacitor
- capacitor.config.json: configuração da aplicação Android
- .github/workflows/android-apk.yml: workflow para compilar um APK no GitHub Actions

IMPORTANTE:
Este pacote não contém um APK já compilado. O GitHub Actions tenta compilar a aplicação depois de os ficheiros e pastas serem enviados para um repositório GitHub.

Como o envio por telemóvel pode não preservar pastas, confirme que o repositório tem esta estrutura:
- package.json
- capacitor.config.json
- www/index.html
- .github/workflows/android-apk.yml

Depois, no GitHub, abra Actions, escolha “Build AlphaNutri Android APK” e carregue em “Run workflow”. Quando terminar, abra a execução e descarregue o artefacto “AlphaNutri-debug-apk”.

O APK debug serve para testes e não é uma versão assinada para publicação na Play Store.
