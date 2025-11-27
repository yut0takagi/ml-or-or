# ML or OR（機械学習 vs 数理最適化）

[![CI](https://github.com/your-username/ml-or-or/actions/workflows/ci.yml/badge.svg)](https://github.com/your-username/ml-or-or/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.12+](https://img.shields.io/badge/python-3.12+-blue.svg)](https://www.python.org/downloads/)

> 機械学習アルゴリズムを数理最適化で実装することで、アルゴリズムの性質を可視化・理解することを目的としたプロジェクトです。

## 📖 概要

このプロジェクトでは、一般的に機械学習ライブラリ（scikit-learn など）で実装されるアルゴリズムを、数理最適化ライブラリ（PuLP など）を使って再実装します。これにより：

- **目的関数**と**制約条件**の観点から問題を捉え直せる
- 機械学習と数理最適化の**関係性**を学べる

## 📁 プロジェクト構成

```
ml-or-or/
├── data/                    # データファイル
│   ├── simple_linear_data.csv
│   └── multi_linear_data.csv
├── img/                     # 画像ファイル
├── notebook/                # Jupyter Notebook
│   ├── 01_create_sample_data.ipynb  # サンプルデータ生成
│   └── 02_linear_regression.ipynb   # 線形回帰
├── .github/workflows/   # CI設定
│   └── ci.yml
├── .gitignore
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── pyproject.toml       # ツール設定
├── README.md
├── requirements.txt
└── requirements-dev.txt # 開発用依存関係
```

## 🚀 クイックスタート

### 必要条件

- Python 3.12 以上
- pip

### インストール

```bash
# リポジトリのクローン
git clone https://github.com/your-username/ml-or-or.git
cd ml-or-or

# 仮想環境の作成（推奨）
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# 依存関係のインストール
pip install -r requirements.txt
```

### 使い方

1. **サンプルデータの生成**

   ```bash
   jupyter notebook notebook/01_create_sample_data.ipynb
   ```

   ノートブックを実行して `data/` ディレクトリにサンプルデータを生成します。

2. **アルゴリズムの実行**

   ```bash
   jupyter notebook notebook/02_linear_regression.ipynb
   ```

   線形回帰を scikit-learn と PuLP の両方で実装・比較します。

## 📚 実装済みアルゴリズム

| アルゴリズム | scikit-learn | PuLP (数理最適化) | ノートブック |
|-------------|:------------:|:-----------------:|-------------|
| 単回帰分析 | ✅ | ✅ (LAD回帰) | `02_linear_regression.ipynb` |

### 今後の予定

- [ ] 重回帰分析
- [ ] ロジスティック回帰
- [ ] サポートベクターマシン (SVM)
- [ ] k-means クラスタリング

## 🔧 技術スタック

- **Python**: メイン言語
- **pandas**: データ操作
- **NumPy**: 数値計算
- **matplotlib**: 可視化
- **scikit-learn**: 機械学習
- **PuLP**: 線形計画法・整数計画法

## 📝 ライセンス

このプロジェクトは [MIT ライセンス](LICENSE) の下で公開されています。

## 🤝 コントリビューション

貢献は大歓迎です！詳細は [CONTRIBUTING.md](CONTRIBUTING.md) をご覧ください。

## 📧 お問い合わせ

質問やフィードバックがありましたら、Issue を作成してください。
