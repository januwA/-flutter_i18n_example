# flutter_i18n_example

使用intl库，来做本地化

1. 安装插件
  ```
dependencies:
  flutter_localizations:
    sdk: flutter
  intl:
  intl_translation
  ```
  
2. 拷贝 lib/main.dart
3. 创建 lib/l18n 文件夹
4. 编写.arb文件
5. 运行脚本
  ```
  $ flutter pub run intl_translation:extract_to_arb --output-dir=lib/l10 n lib/main.dart

  $ flutter pub run intl_translation:generate_from_arb --output-dir=lib/l10n --no-use-deferred-loading lib/main.dart lib/l10n/intl_*.arb
  ```

  6. 运行`flutter run`
  7. 切换手机语言，并返回app，文本将会自动切换


  ## 更多
  - [internationalization example](https://github.com/flutter/website/tree/master/examples/internationalization)
  - [flutter_localizations](https://github.com/flutter/flutter/tree/master/packages/flutter_localizations/lib/src/l10n)
  - [development internationalization](https://flutter.dev/docs/development/accessibility-and-localization/internationalization)
  - [intl](https://pub.flutter-io.cn/packages/intl)
  - [intl_translation](https://pub.flutter-io.cn/packages/intl_translation)
