# RX72N MTU Timer Docs

RX72NのMTU（Multi-Function Timer Pulse Unit）タイマーを使った、Modbus RTU通信のタイムアウト検出（文字間1.5文字・フレーム無通信3.5文字）に関するカウンタ値計算のドキュメント集です。

## 内容

- [mtu-timer-calculation.md](mtu-timer-calculation.md) — MTUのカウンタ値を算出する一般式と、具体的な計算例
- [mddr-baud-rate-correction.md](mddr-baud-rate-correction.md) — SCIのビットレート補正機能（MDDR）を使ってボーレート精度を改善した場合の、MTUカウンタ値の再計算

## 背景

RX72N + MAX485EESA+によるModbus RTUスレーブ実装（PCLK=60MHz、目標ボーレート2Mbps）における、MTUタイマー設定の設計検討資料です。
