# RTX Spark 搭載 PC の比較

NVIDIA RTX Spark (N1X) を積んだ Windows PC を、統合メモリ・帯域・国内価格で並べ、GB10 搭載機と Apple に照らす

> 📅 作成: 2026-11-03 / 更新: 2026-11-11

[^^](../../README.md)

## 1. RTX Spark とは

NVIDIA と Microsoft が 2026-05-31 に発表した、Windows のノート PC と小型デスクトップ向けの SoC です。Grace CPU (Arm) と Blackwell 世代の RTX GPU を 1 つにまとめ、CPU と GPU が統合メモリを共有します。OS は Windows 11 の Arm 版です。国内では 2026 年 10 月中旬から搭載機が出ています。

| 構成 | CPU | GPU | 統合メモリ | 帯域 | 電力 | AI 性能 (FP4) |
|---|---|---|---|---:|---|---|
| N1X 上位 (ノート・デスクトップ) | Grace 20コア | 6,144コア | 最大 128GB | 300.8 GB/s | 45〜80W (デスクトップ 140W) | 1 PFLOPS |
| N1X 下位 (ノート) | Grace 18コア | 5,120コア | 最大 32GB | 300.8 GB/s | 45〜80W | 827 TFLOPS |

帯域は NVIDIA の仕様ページに書かれていません。表の値は、仕様ページの 256bit と、各社の資料にある LPDDR5X-9400 から計算したものです (9,400 MT/s × 256bit ÷ 8)。

> [!NOTE]
> <strong>メモリ構成は CPU/GPU の構成に縛られます。</strong>64GB 以上を選べるのは、どの機種も 20コアCPU / 6,144コアGPU の構成だけです。また Microsoft の注記によれば、**GPU が使える容量は統合メモリの合計より少なくなります**。128GB 機でも、128GB をそのまま GPU で使えるわけではありません。

## 2. 128GB 構成の国内価格

2026-11-10 に確認した、統合メモリ 128GB の構成です。価格はすべて税込で、安い順に並べています。

| 機種 | 画面 | ストレージ | 価格 | 入手先 | 状態 |
|---|---|---|---:|---|---|
| [Microsoft Surface Laptop Ultra](https://www.microsoft.com/ja-jp/surface/devices/surface-laptop-ultra) | 15型 | 1TB | **1,094,280 円** | Microsoft Store | ⚠️ **在庫なし** 構成ページで選べるが、在庫が無い |
| [ASUS ProArt P14 (H7407)](https://www.asus.com/jp/laptops/for-creators/proart/proart-p14-h7407/) | 14型 | 1TB | 1,198,000 円 | 通販 (価格.com 最安) | ✅ **販売中** 2026-10-23 発売 |
| [ASUS ProArt P16 (H7607)](https://www.asus.com/jp/laptops/for-creators/proart/proart-p16-h7607/) | 16型 | 1TB | 1,248,000 円 | 通販 (価格.com 最安) | ✅ **販売中** 2026-10-23 発売 |
| HP OmniBook Ultra 16 AI PC (エクストリームプロ) | 16型 | 2TB | 1,294,700 円〜 | 日本HP (希望販売価格) | ⬜ **未発売** 2026 年 11 月以降に発売 |
| [MSI Prestige N16 Flip AI+](https://jp.msi.com/news/detail/Prestige-N16-Flip-AI--C1XM-150007) (C1XMT-3100JP) | 16型 2-in-1 | 2TB | 1,301,877 円 | ソフマップ (価格.com 最安) | ✅ **販売中** 2026-10-23 発売 |

<strong>最安は 128GB でも約 109 万円で、すべてノート PC です。</strong>国内で 128GB を選べる RTX Spark 機は、この 5 機種だけでした。最安の Surface は在庫が無いため、いま買える最安は ASUS ProArt P14 の 1,198,000 円になります。

### 国内で 128GB を買えないもの

| 機種 | 理由 |
|---|---|
| Dell XPS 16 Creator Edition | ❌ **構成なし** 国内で出ているのは 32GB・512GB の構成だけ (価格.com 最安 799,598 円) |
| HP OmniBook X 14 | ❌ **日本未発表** 米国のみ |
| Lenovo Yoga Pro 9n ・ Yoga 9n 2-in-1 | ❌ **日本未発表** 米国のみ。Yoga 9n 2-in-1 は最大 64GB |
| Microsoft Surface RTX Spark Dev Box | ❌ **日本未発表** 128GB・2TB の小型デスクトップ。米国での価格は 6,000 ドルと報じられている |

### メモリが少ない構成

64GB 以下でよければ、価格は大きく下がります。

| 機種 | メモリ / ストレージ | 価格 | 入手先 |
|---|---|---:|---|
| HP OmniBook Ultra 16 (エクストリームプラス) | 64GB / 1TB | 796,400 円〜 | 日本HP (希望販売価格)・2026-10-29 発売 |
| Microsoft Surface Laptop Ultra | 64GB / 1TB | 812,680 円 | Microsoft Store |
| ASUS ProArt P14 (H7407) | 48GB / 1TB | 949,800 円 | ASUS (発表価格)・11 月中旬発売 |
| MSI Prestige N16 Flip AI+ (C1XMT-3200JP) | 64GB / 2TB | 989,820 円 | 通販 (価格.com 最安) |
| ASUS ProArt P16 (H7607) | 48GB / 1TB | 999,800 円 | ASUS (発表価格)・11 月中旬発売 |

## 3. GB10 搭載機・Apple との比較

128GB 構成どうしで比べます。GB10 搭載機と Apple の価格は、[ローカルLLM 機種比較 2026](r260916-01-ローカルLLM機種比較.md) の 2026-11-10 の値です (MacBook Pro 16インチ M5 Max だけは 2026-11-03 の値)。

| 機種 | 形態 / OS | 帯域 | ストレージ | 価格 | 1GB あたり | 帯域 1GB/s あたり |
|---|---|---:|---|---:|---:|---:|
| Mac Studio M5 Max | 据置 / macOS | 614 GB/s | 2TB | 1,031,800 円 | **8,061 円** | **1,681 円** |
| Surface Laptop Ultra (RTX Spark) | ノート / Windows | 300.8 GB/s | 1TB | 1,094,280 円 | 8,549 円 | 3,638 円 |
| ASUS ProArt P14 (RTX Spark) | ノート / Windows | 300.8 GB/s | 1TB | 1,198,000 円 | 9,359 円 | 3,983 円 |
| MacBook Pro 16インチ M5 Max | ノート / macOS | 614 GB/s | 2TB | 1,209,800 円 | 9,452 円 | 1,971 円 |
| ASUS ProArt P16 (RTX Spark) | ノート / Windows | 300.8 GB/s | 1TB | 1,248,000 円 | 9,750 円 | 4,149 円 |
| HP OmniBook Ultra 16 (RTX Spark) | ノート / Windows | 300.8 GB/s | 2TB | 1,294,700 円 | 10,115 円 | 4,304 円 |
| HP ZGX Nano G1n (GB10) | 据置 / Linux (DGX OS) | 273 GB/s | 4TB | 1,299,100 円 | 10,149 円 | 4,759 円 |
| MSI Prestige N16 Flip AI+ (RTX Spark) | ノート / Windows | 300.8 GB/s | 2TB | 1,301,877 円 | 10,171 円 | 4,328 円 |

<strong>RTX Spark 機は、GB10 搭載機とほぼ同じ価格・同じ帯域のノート PC です。</strong>帯域は GB10 搭載機の 273 GB/s より約 1 割広いだけで、Apple の M5 Max (614 GB/s) の半分以下です。LLM の生成速度は帯域でほぼ決まるため、同じモデルなら M5 Max の約半分の速度になる見込みです (実測はしていません)。

<strong>128GB を持ち運ぶなら、MacBook Pro 16インチと比べることになります。</strong>2TB どうしでは MacBook Pro が 1,209,800 円で、HP・MSI の RTX Spark 機より 8.5〜9.2 万円安く、帯域は 2 倍です。RTX Spark 機を選ぶ理由は、Windows で NVIDIA の GPU を使うことにあります。

> [!NOTE]
> <strong>GB10 搭載機とは OS が違います。</strong>GB10 搭載機は Linux (DGX OS) で CUDA の開発環境がそろった状態で届きますが、RTX Spark 機は Windows 11 の Arm 版です。同じ道具がそのまま動くとは限りません。買う前に、使うソフトが Windows の Arm 版で動くかを確かめてください。

## 4. 出典

- [NVIDIA RTX Spark 仕様](https://www.nvidia.com/en-us/products/rtx-spark/specifications/) (構成・メモリ・電力・AI 性能)
- [Wikipedia: Nvidia RTX Spark](https://en.wikipedia.org/wiki/Nvidia_RTX_Spark) (発表日・OEM 各社)
- [PC Watch: ASUS ProArt P14 / P16 の予約開始 (2026-10-14)](https://pc.watch.impress.co.jp/docs/news/2147835.html) (構成別の価格・LPDDR5X-9400)
- [日本HP: OmniBook Ultra 16 AI PC 発表 (2026-10-15)](https://www.gdm.or.jp/pressrelease/2026/1015/656269) (構成別の希望販売価格)
- [Microsoft Store: Surface Laptop Ultra の構成](https://www.microsoft.com/ja-jp/store/configure/surface-laptop-ultra/8wg5vqp0x4b8) (構成別の価格・在庫)
- [価格.com: RTX Spark の検索結果](https://search.kakaku.com/RTX%20Spark/) (ASUS・MSI・Dell の通販価格)
- [RTX Spark 搭載ノート PC 9 製品のまとめ](https://thehikaku.net/pc/newpc/newpc-20261011-rtx-spark.html) (国外モデル・発売予定)
- [Surface RTX Spark Dev Box の報道](https://korben.info/ja/microsoft-surface-rtx-spark-dev-box-mini-pc-local-ai.html) (米国での価格)

[^^](../../README.md)
