FROM node:20-alpine

WORKDIR /nextjs

# package.jsonとpackage-lock.jsonをコピー
COPY package*.json ./

# 依存関係をインストール
RUN npm ci

# ソースコードをコピー
COPY . .

# 開発サーバーを起動
CMD ["npm", "run", "dev"]

# ポート3000を公開
EXPOSE 3000