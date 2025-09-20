# BoyScout UP! Install Link

BoyScout UP!アプリのインストールリンクページです。

## 機能

- **デバイス自動判定**: ユーザーのデバイス（iOS/Android）を自動判定
- **アプリ起動**: 既にアプリがインストールされている場合、アプリを直接起動
- **ストアリダイレクト**: アプリが未インストールの場合、適切なアプリストアへリダイレクト
  - iOS: App Store
  - Android: Google Play Store

## 動作仕様

### iOS
1. カスタムURLスキーム `scoutup://` でアプリ起動を試行
2. 2秒以内にアプリが起動しない場合、App Storeへリダイレクト

### Android
1. Intent URL `intent://open#Intent;scheme=scoutup;package=org.ScoutAssociationofJapan.scoutup;end` でアプリ起動を試行
2. 2秒以内にアプリが起動しない場合、Google Play Storeへリダイレクト

### その他のデバイス
- PC等のモバイル以外のデバイスには、スマートフォンからアクセスするよう案内メッセージを表示

## アプリストアリンク

- **iOS**: https://apps.apple.com/jp/app/id6744021399
- **Android**: https://play.google.com/store/apps/details?id=org.ScoutAssociationofJapan.scoutup

## ファイル構成

```
.
├── index.html    # メインページ
└── README.md     # このファイル
```

## デプロイ

このプロジェクトは静的サイトなので、任意のWebホスティングサービスにデプロイできます。