# コントリビューションガイドライン

このプロジェクトへの貢献に興味を持っていただきありがとうございます！

## 貢献の方法

### Issue の報告

- バグを見つけた場合や新機能の提案がある場合は、Issue を作成してください
- 既存の Issue を確認し、重複がないかご確認ください
- Issue には以下の情報を含めてください：
  - 問題の明確な説明
  - 再現手順（バグの場合）
  - 期待される動作
  - 実際の動作
  - 使用環境（OS、Python バージョンなど）

### Pull Request の作成

1. リポジトリをフォークしてください
2. 新しいブランチを作成してください（`git checkout -b feature/amazing-feature`）
3. 変更をコミットしてください（`git commit -m 'Add some amazing feature'`）
4. ブランチにプッシュしてください（`git push origin feature/amazing-feature`）
5. Pull Request を作成してください

### コーディング規約

- Python コードは [PEP 8](https://pep8-ja.readthedocs.io/ja/latest/) に準拠してください
- Jupyter Notebook のセルには適切なコメントやマークダウンを含めてください
- 新しいアルゴリズムを追加する場合は、以下を含めてください：
  - 数式の説明（マークダウンセル）
  - scikit-learn などの既存ライブラリでの実装（比較用）
  - PuLP を使った数理最適化での実装
  - 結果の可視化

### コミットメッセージ

コミットメッセージは以下の形式で記述してください：

```
<type>: <subject>

<body>
```

**type の種類：**
- `feat`: 新機能
- `fix`: バグ修正
- `docs`: ドキュメントのみの変更
- `style`: コードの意味に影響しない変更（空白、フォーマットなど）
- `refactor`: バグ修正や機能追加ではないコードの変更
- `test`: テストの追加や修正
- `chore`: ビルドプロセスやツールの変更

## 開発環境のセットアップ

```bash
# リポジトリのクローン
git clone https://github.com/your-username/ml-or-or.git
cd ml-or-or

# 仮想環境の作成
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# 依存関係のインストール
pip install -r requirements.txt
```

## 質問がある場合

Issue を作成するか、リポジトリのメンテナーにお問い合わせください。

ご協力ありがとうございます！

