# rs485HAT

Raspberry Pi用RS485通信HAT基板のKiCadデータです。回路図・基板・自作部品ライブラリを公開しています。

[製品情報・お問い合わせ](https://raspikoubou.theshop.jp/items/103737327)

## 概要

- GPIO14（TX）、GPIO15（RX）、GPIO4（送受信切替）を使用します。
- 半二重通信に対応し、GPIO4がHIGHで送信、LOWで受信します。
- 対応機種はRaspberry Pi 5シリーズ、Raspberry Pi 4 Model B、Raspberry Pi 3 Model B+です（製品ページ記載）。
- 終端抵抗は、RS485のA・B間にアキシャルリード抵抗を取り付けられます。

詳細な仕様・接続方法・注意事項は、製品ページをご確認ください。

## データの版・作成環境

- データの版：ver1.0.0
- 作成環境：Windows / KiCad 8.0.6

## ファイル構成

| ファイル | 内容 |
| --- | --- |
| `RS485_HAT_PCB_ver1.0.0.kicad_pro` | KiCadプロジェクト設定 |
| `RS485_HAT_PCB_ver1.0.0.kicad_sch` | 回路図 |
| `RS485_HAT_PCB_ver1.0.0.kicad_pcb` | 基板レイアウト |
| `000_RS485HAT.kicad_sym` | 自作シンボルライブラリ |
| `000_RS485HAT.pretty/` | 自作フットプリントライブラリ（4点） |
| `sym-lib-table` / `fp-lib-table` | プロジェクト内ライブラリの参照設定 |
| `fabrication-toolkit-options.json` | Fabrication Toolkit用の設定 |

リポジトリを一式ダウンロードし、KiCadで `RS485_HAT_PCB_ver1.0.0.kicad_pro` を開いてください。ライブラリ参照にはプロジェクト相対パス（`${KIPRJMOD}`）を使用しています。

自動バックアップ・キャッシュ・個人の表示設定は管理対象から除外しています。

## 利用条件

ライセンスは未設定です。現時点で、本リポジトリから追加の利用許諾は行っていません。改変・再配布・商用利用・本データによる製造などの許諾範囲については、製品ページからお問い合わせください。

ご使用にあたっては、ご利用者ご自身の責任においてご判断いただきますようお願いします。
