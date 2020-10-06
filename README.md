# Vscode Remote Containers for ActiveRecord

ActiveRecordのバグ報告テンプレートをVSCodeのリモートコンテナーで使えるように移植したコードです。

* [SQLite3用](https://github.com/mh-mobile/vscode_remote_containers_for_active_record/tree/master/containers/sqlite)
* [PostgreSQL用](https://github.com/mh-mobile/vscode_remote_containers_for_active_record/tree/master/containers/postgres)

# 使い方

## リモートコンテナの起動

.devcontainerが配置されたディレクトリをVSCodeで読み込みます。
VSCodeの起動後、ダイアログの`Reopen in Container`ボタンを選択します。
明示的に、ディレクトリを指定する場合は、VSCodeのパレットから `Remote Containers: Open Folder in Container...`を選択します。

## active_record_gem.rbの実行

リモートコンテナの起動後、コンテナ上のターミナルから`ruby active_record_gem.rb`を実行します。
※ workspaceディレクトリは、.devcontainerのあるホストOSのディレクトリがマウントされます

```bash
root ➜ /workspace $ ruby active_record_gem.rb 
```
