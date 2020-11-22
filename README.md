# flutter_i18n_example

使用intl库，来做本地化

1. 编辑pubspec.yaml文件
```yaml
dependencies:
  flutter:
    sdk: flutter
  flutter_localizations: # add
    sdk: flutter
  intl: # add

flutter:
  generate: true # add
  uses-material-design: true
```

2. 添加l10n.yaml的配置文件
```yaml
arb-dir: lib/l10n
template-arb-file: app_en.arb
output-localization-file: app_localizations.dart
```

3. 在lib/l10n中创建arb翻译模板
4. 在app中使用(见lib/main.dart)，运行app
5. 切换手机语言，并返回app，文本将会自动切换


  ## 更多
  - [官方文档](https://flutter.dev/docs/development/accessibility-and-localization/internationalization)
  - [intl](https://pub.flutter-io.cn/packages/intl)
