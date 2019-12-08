# adventcalendar-postgres-2019-9

## これは何のレポジトリ？

これは [PostgreSQL Advent Calendar 2019](https://qiita.com/advent-calendar/2019/postgresql) の9日目のエントリーで使用した EC2上に構築する PostgreSQL + PGroonga のレポジトリです。 

## 起動方法

```
# git clone git@github.com:TakahashiIkki/adventcalendar-postgres-2019-9.git
# cd adventcalendar-postgres-2019-9

# docker-compose up --build -d
```

## 復元方法

※ 作業ディレクトリは このレポジトリをクローンした後のルートディレクトリを想定しています。

```
# docker-compose exec postgres bash
# pg_restore -U adv_user -d adv_demo -Fc pg_schema.dump
```

# 注意事項

動作確認してるのは EC2 の `Ubuntu 18.04.3 LTS (GNU/Linux 4.15.0-1056-aws x86_64)` です。

- 
