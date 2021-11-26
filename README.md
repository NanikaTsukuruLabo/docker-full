## MySQL

### 操作方法

#### ログイン

1. mysqlのcontainerのcontainer id を取得

```
docker container ps -a
```

2. containerの中にはいる

```sh
docker container exec -it {container id} bin/bash
```

3. mysqlにログイン

```sh
mysql -u root -p
```

4. パスワードの入力

```
root
```

#### テーブルの作成(メモ)


```mysql
CREATE TABLE
	user
(
	id int
	, name varchar(10)
);
```

```mysql
CREATE TABLE
	product
(
	id int
	, name varchar(10)
	, col varchar(10)
);
```
#### データの挿入(メモ)

```mysql
INSERT
	user
VALUES
(
	1
	, "shiota"
);
```


