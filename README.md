

# 初期開発時メモ
## 1. Next.jsアプリケーションを作成する
```bash
cd frontend
docker-compose run --rm frontend npx create-next-app . --ts
```

## 2. Ruby on Railsでサーバー環境を構築する
```bash
cd backend
$ docker-compose run --rm backend bundle exec rails new . --api -d mysql
```

## 3. Bundle InstallされていないものをDocker内でインストールする
```bash
docker-compose run --rm backend bash
bundle install
```

## 4. データベースを作成する
```bash
docker-compose run --rm backend rails db:create
```

## 5. コンテナを起動する
```bash
docker-compose up --build
```