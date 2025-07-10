Este plugin é uma adaptação do New Relic Cordova Plugin, permitindo fácil monitoramento de performance e erros em aplicações híbridas Android e iOS.

## 🚀 Instalação
Adicione o plugin no seu config.xml da seguinte forma:
<plugin name="cordova-plugin-newrelic-market4u" spec="^7.0.9">
    <variable name="IOS_APP_TOKEN" value="SEU_IOS_APP_TOKEN" />
    <variable name="ANDROID_APP_TOKEN" value="SEU_ANDROID_APP_TOKEN" />
</plugin>

Ou instale via CLI:
cordova plugin add cordova-plugin-newrelic-market4u \
  --variable IOS_APP_TOKEN=SEU_IOS_APP_TOKEN \
  --variable ANDROID_APP_TOKEN=SEU_ANDROID_APP_TOKEN

## ✅ Compatível com o Volt.Build — funciona tanto com config.xml quanto via instalação CLI.

## 📲 Plataformas Suportadas
- Android
- iOS

## 🛠 Como funciona
Este plugin inicializa o New Relic assim que o aplicativo é iniciado. Ele monitora automaticamente:
- Tempo de carregamento da aplicação
- Interações com a UI
- Erros de JavaScript
- Solicitações de rede
- Traces customizados (com uso da API New Relic JS)

## 📦 Requisitos
- Cordova 10+
- Android SDK ou Xcode configurados
- Conta ativa na New Relic

## 📘 API New Relic JavaScript
- Você pode usar a API JavaScript da New Relic dentro do seu app, por exemplo:
```
   newrelic.setUserId("usuario123");
   newrelic.recordBreadcrumb("Navegou para tela X");
   newrelic.noticeError(new Error("Erro inesperado"));
```

## 🔗 Links úteis
- [📘 New Relic para Cordova (documentação oficial)](https://docs.newrelic.com/docs/mobile-monitoring/new-relic-mobile-cordova/)
- [📊 New Relic Dashboard](https://one.newrelic.com/)
