# テクノロジー（藤原）12/6授業

## Bashの実行ログ

```
kogadoom:~/workspace $  cd ~/workspace
kogadoom:~/workspace $ git clone git@github.com:kogatoshi/lecture-1206.git
Cloning into 'lecture-1206'...
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
remote: Counting objects: 95, done.
remote: Compressing objects: 100% (79/79), done.
remote: Total 95 (delta 2), reused 95 (delta 2), pack-reused 0
Receiving objects: 100% (95/95), 38.69 KiB | 220.00 KiB/s, done.
Resolving deltas: 100% (2/2), done.
kogadoom:~/workspace $ cd lecture-1206/asagao
kogadoom:~/workspace/lecture-1206/asagao (master) $ bundle install
The latest bundler is 1.16.0, but you are currently running 1.15.4.
To update, run `gem install bundler`
The git source `git://github.com/flori/json.git` uses the `git` protocol, which transmits data without encryption. Disable this warning with `bundle config git.allow_insecure true`, or switch to the `https` protocol to keep your data secure.
Warning: the running version of Bundler (1.15.4) is older than the version that created the lockfile (1.16.0). We suggest you upgrade to the latest version of Bundler by running `gem install bundler`.
Using rake 12.2.1
Using concurrent-ruby 1.0.5
Using minitest 5.10.3
Using thread_safe 0.3.6
Using builder 3.2.3
Using erubis 2.7.0
Using mini_portile2 2.3.0
Using crass 1.0.2
Using rack 1.6.8
Using mini_mime 0.1.4
Using arel 6.0.4
Using debug_inspector 0.0.3
Using bundler 1.15.4
Using byebug 9.1.0
Using coffee-script-source 1.8.0
Using execjs 2.7.0
Using thor 0.20.0
Using ffi 1.9.18
Using multi_json 1.12.2
Using json 1.8.6 from git://github.com/flori/json.git (at v1.8@7f4cfd8)
Using rb-fsevent 0.10.2
Using rdoc 4.3.0
Using tilt 2.0.8
Using sqlite3 1.3.13
Using turbolinks-source 5.0.3
Using i18n 0.9.1
Using tzinfo 1.2.4
Using nokogiri 1.8.1
Using rack-test 0.6.3
Using sprockets 3.7.1
Using mail 2.7.0
Using binding_of_caller 0.7.3
Using coffee-script 2.4.1
Using uglifier 3.2.0
Using rb-inotify 0.9.10
Using sdoc 0.4.2
Using turbolinks 5.0.1
Using activesupport 4.2.10
Using loofah 2.1.1
Using sass-listen 4.0.0
Using rails-deprecated_sanitizer 1.0.3
Using globalid 0.4.1
Using activemodel 4.2.10
Using jbuilder 2.7.0
Using spring 2.0.2
Using rails-html-sanitizer 1.0.3
Using sass 3.5.3
Using rails-dom-testing 1.0.8
Using activejob 4.2.10
Using activerecord 4.2.10
Using actionview 4.2.10
Using actionpack 4.2.10
Using actionmailer 4.2.10
Using railties 4.2.10
Using sprockets-rails 3.2.1
Using coffee-rails 4.1.1
Using jquery-rails 4.3.1
Using rails 4.2.10
Using sass-rails 5.0.6
Using web-console 2.3.0
Bundle complete! 15 Gemfile dependencies, 60 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:create
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:create RAILS_ENV=production
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:create
db/development.sqlite3 already exists
db/test.sqlite3 already exists
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails g model member
      invoke  active_record
      create    db/migrate/20171206004649_create_members.rb
      create    app/models/member.rb
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:migrate
rake aborted!
NameError: undefined local variable or method `t' for main:Object
/home/ubuntu/workspace/lecture-1206/asagao/db/migrate/20171206004649_create_members.rb:2:in `<top (required)>'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:274:in `require'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:274:in `block in require'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:240:in `load_dependency'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:274:in `require'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:777:in `load_migration'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:773:in `migration'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:768:in `disable_ddl_transaction'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:1076:in `use_transaction?'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:986:in `rescue in block in migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:983:in `block in migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:980:in `each'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:980:in `migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:823:in `up'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:801:in `migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/tasks/database_tasks.rb:139:in `migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/railties/databases.rake:44:in `block (2 levels) in <top (required)>'

Caused by:
NameError: undefined local variable or method `t' for main:Object
/home/ubuntu/workspace/lecture-1206/asagao/db/migrate/20171206004649_create_members.rb:2:in `<top (required)>'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:274:in `require'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:274:in `block in require'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:240:in `load_dependency'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/dependencies.rb:274:in `require'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:777:in `load_migration'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:773:in `migration'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:768:in `disable_ddl_transaction'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:1076:in `use_transaction?'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:1068:in `ddl_transaction'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:1022:in `execute_migration_in_transaction'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:984:in `block in migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:980:in `each'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:980:in `migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:823:in `up'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/migration.rb:801:in `migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/tasks/database_tasks.rb:139:in `migrate'
/usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/railties/databases.rake:44:in `block (2 levels) in <top (required)>'
Tasks: TOP => db:migrate
(See full trace by running task with --trace)
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails c
Loading development environment (Rails 4.2.10)
2.4.0 :001 > Member.count
ActiveRecord::StatementInvalid: Could not find table 'members'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:501:in `table_structure'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:375:in `columns'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/schema_cache.rb:43:in `columns'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/attributes.rb:93:in `columns'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/model_schema.rb:260:in `column_names'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:232:in `aggregate_column'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:258:in `execute_simple_calculation'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:227:in `perform_calculation'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:133:in `calculate'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:48:in `count'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:13:in `count'
        from (irb):1
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :002 > Member.count
ActiveRecord::StatementInvalid: Could not find table 'members'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:501:in `table_structure'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:375:in `columns'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/schema_cache.rb:43:in `columns'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/attributes.rb:93:in `columns'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/model_schema.rb:260:in `column_names'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:232:in `aggregate_column'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:258:in `execute_simple_calculation'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:227:in `perform_calculation'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:133:in `calculate'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/calculations.rb:48:in `count'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:13:in `count'
        from (irb):2
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :003 > member.number = 1
NameError: undefined local variable or method `member' for main:Object
        from (irb):3
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :004 > member.name = "Taro"
NameError: undefined local variable or method `member' for main:Object
        from (irb):4
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :005 > member.save
NameError: undefined local variable or method `member' for main:Object
        from (irb):5
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :006 > Member.first
  Member Load (0.7ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
ActiveRecord::StatementInvalid: SQLite3::SQLException: no such table: members: SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `initialize'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `new'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `prepare'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:284:in `block in exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:484:in `block in log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/notifications/instrumenter.rb:20:in `instrument'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:478:in `log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:281:in `exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:356:in `select'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:32:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/query_cache.rb:70:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:39:in `find_by_sql'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:639:in `exec_queries'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:515:in `load'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:243:in `to_a'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:500:in `find_nth_with_limit'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:484:in `find_nth'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:127:in `first'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:3:in `first'
        from (irb):6
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :007 > pp Member.first
  Member Load (1.1ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
ActiveRecord::StatementInvalid: SQLite3::SQLException: no such table: members: SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `initialize'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `new'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `prepare'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:284:in `block in exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:484:in `block in log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/notifications/instrumenter.rb:20:in `instrument'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:478:in `log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:281:in `exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:356:in `select'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:32:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/query_cache.rb:70:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:39:in `find_by_sql'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:639:in `exec_queries'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:515:in `load'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:243:in `to_a'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:500:in `find_nth_with_limit'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:484:in `find_nth'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:127:in `first'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:3:in `first'
        from (irb):7
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :008 > member = Member.first
  Member Load (3.1ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
ActiveRecord::StatementInvalid: SQLite3::SQLException: no such table: members: SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `initialize'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `new'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `prepare'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:284:in `block in exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:484:in `block in log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/notifications/instrumenter.rb:20:in `instrument'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:478:in `log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:281:in `exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:356:in `select'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:32:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/query_cache.rb:70:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:39:in `find_by_sql'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:639:in `exec_queries'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:515:in `load'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:243:in `to_a'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:500:in `find_nth_with_limit'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:484:in `find_nth'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:127:in `first'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:3:in `first'
        from (irb):8
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :009 > member.number = 41
NoMethodError: undefined method `number=' for nil:NilClass
        from (irb):9
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :010 > member.save
NoMethodError: undefined method `save' for nil:NilClass
        from (irb):10
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :011 > Member.first
  Member Load (0.6ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
ActiveRecord::StatementInvalid: SQLite3::SQLException: no such table: members: SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `initialize'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `new'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `prepare'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:284:in `block in exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:484:in `block in log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/notifications/instrumenter.rb:20:in `instrument'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:478:in `log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:281:in `exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:356:in `select'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:32:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/query_cache.rb:70:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:39:in `find_by_sql'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:639:in `exec_queries'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:515:in `load'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:243:in `to_a'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:500:in `find_nth_with_limit'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:484:in `find_nth'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:127:in `first'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:3:in `first'
        from (irb):11
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :012 >
kogadoom:~/workspace/lecture-1206/asagao (master) $ mkdir -p db/seeds/development
kogadoom:~/workspace/lecture-1206/asagao (master) $ touch db/seeds/development/members.rb
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:reset
/home/ubuntu/workspace/lecture-1206/asagao/db/schema.rb doesn't exist yet. Run `rake db:migrate` to create it, then try again. If you do not intend to use a database, you should instead alter /home/ubuntu/workspace/lecture-1206/asagao/config/application.rb to limit the frameworks that will be loaded.
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:seed
You have 1 pending migration:
  20171206004649 CreateMembers
Run `rake db:migrate` to update your database then try again.
kogadoom:~/workspace/lecture-1206/asagao (master) $ Member.count
bash: Member.count: command not found
kogadoom:~/workspace/lecture-1206/asagao (master) $ Member .count
bash: Member: command not found
kogadoom:~/workspace/lecture-1206/asagao (master) $ Member.count
bash: Member.count: command not found
kogadoom:~/workspace/lecture-1206/asagao (master) $ Member .countbin/rails c
bash: Member: command not found
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails c
Loading development environment (Rails 4.2.10)
2.4.0 :001 > pp Member.first
  Member Load (0.5ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
ActiveRecord::StatementInvalid: SQLite3::SQLException: no such table: members: SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `initialize'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `new'
        from /usr/local/rvm/gems/ruby-2.4.0/gems/sqlite3-1.3.13/lib/sqlite3/database.rb:91:in `prepare'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:284:in `block in exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:484:in `block in log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activesupport-4.2.10/lib/active_support/notifications/instrumenter.rb:20:in `instrument'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract_adapter.rb:478:in `log'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/sqlite3_adapter.rb:281:in `exec_query'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:356:in `select'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/database_statements.rb:32:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/connection_adapters/abstract/query_cache.rb:70:in `select_all'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:39:in `find_by_sql'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:639:in `exec_queries'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:515:in `load'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation.rb:243:in `to_a'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:500:in `find_nth_with_limit'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:484:in `find_nth'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/relation/finder_methods.rb:127:in `first'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/activerecord-4.2.10/lib/active_record/querying.rb:3:in `first'
        from (irb):1
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :002 >
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails db
SQLite version 3.8.2 2013-12-06 14:53:30
Enter ".help" for instructions
Enter SQL statements terminated with a ";"
sqlite> .tables
schema_migrations
sqlite> .schema members
sqlite> SELECT * from members;
Error: no such table: members
sqlite> SELECT * from members;
Error: no such table: members
sqlite> .schema members
sqlite> SELECT * from members;
Error: no such table: members
sqlite> quit                                                                                                                                        
   ...> .quit
   ...> bin/rails c
   ...> 
Error: incomplete SQL: quitT * from member
.quit
bin/rails c
kogadoom:~/workspace/lecture-1206/asagao (master) $ in/rails c
bash: in/rails: No such file or directory
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:migrate
== 20171206004649 CreateMembers: migrating ====================================
-- create_table(:members)
   -> 0.0020s
== 20171206004649 CreateMembers: migrated (0.0023s) ===========================

kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails c
Loading development environment (Rails 4.2.10)
2.4.0 :001 > Member.count
   (0.4ms)  SELECT COUNT(*) FROM "members"
 => 0 
2.4.0 :002 > 0 
 => 0 
2.4.0 :003 > member = Member.new
 => #<Member id: nil, number: nil, name: nil, full_name: nil, email: nil, birthday: nil, gender: 0, administrator: false, created_at: nil, updated_at: nil> 
2.4.0 :004 > member.number = 1
 => 1 
2.4.0 :005 > member.name = "Taro"
 => "Taro" 
2.4.0 :006 > member.save
   (0.2ms)  begin transaction
  SQL (0.6ms)  INSERT INTO "members" ("number", "name", "created_at", "updated_at") VALUES (?, ?, ?, ?)  [["number", 1], ["name", "Taro"], ["created_at", "2017-12-06 02:02:46.055493"], ["updated_at", "2017-12-06 02:02:46.055493"]]
   (12.2ms)  commit transaction
 => true 
2.4.0 :007 > Member.first
  Member Load (0.5ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
 => #<Member id: 1, number: 1, name: "Taro", full_name: nil, email: nil, birthday: nil, gender: 0, administrator: false, created_at: "2017-12-06 02:02:46", updated_at: "2017-12-06 02:02:46"> 
2.4.0 :008 > pp Member.first
  Member Load (0.6ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
#<Member:0x0000000348a528
 id: 1,
 number: 1,
 name: "Taro",
 full_name: nil,
 email: nil,
 birthday: nil,
 gender: 0,
 administrator: false,
 created_at: Wed, 06 Dec 2017 11:02:46 JST +09:00,
 updated_at: Wed, 06 Dec 2017 11:02:46 JST +09:00>
 => #<Member id: 1, number: 1, name: "Taro", full_name: nil, email: nil, birthday: nil, gender: 0, administrator: false, created_at: "2017-12-06 02:02:46", updated_at: "2017-12-06 02:02:46"> 
2.4.0 :009 > member = Member.first
  Member Load (0.7ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
 => #<Member id: 1, number: 1, name: "Taro", full_name: nil, email: nil, birthday: nil, gender: 0, administrator: false, created_at: "2017-12-06 02:02:46", updated_at: "2017-12-06 02:02:46"> 
2.4.0 :010 > member.number = 41
 => 41 
2.4.0 :011 > member.save
   (0.5ms)  begin transaction
  SQL (0.5ms)  UPDATE "members" SET "number" = ?, "updated_at" = ? WHERE "members"."id" = ?  [["number", 41], ["updated_at", "2017-12-06 02:03:33.570644"], ["id", 1]]
   (12.7ms)  commit transaction
 => true 
2.4.0 :012 > Member.first
  Member Load (0.6ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
 => #<Member id: 1, number: 41, name: "Taro", full_name: nil, email: nil, birthday: nil, gender: 0, administrator: false, created_at: "2017-12-06 02:02:46", updated_at: "2017-12-06 02:03:33"> 
2.4.0 :013 > 
kogadoom:~/workspace/lecture-1206/asagao (master) $ ^C
kogadoom:~/workspace/lecture-1206/asagao (master) $ mkdir -p db/seeds/development
kogadoom:~/workspace/lecture-1206/asagao (master) $ touch db/seeds/development/members.rb
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:reset
-- create_table("members", {:force=>:cascade})
   -> 0.0160s
-- initialize_schema_migrations_table()
   -> 0.0568s
-- create_table("members", {:force=>:cascade})
   -> 0.0140s
-- initialize_schema_migrations_table()
   -> 0.0267s
Creating members...
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rake db:seed
Creating members...
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails c
Loading development environment (Rails 4.2.10)
2.4.0 :001 > pp Member.first
  Member Load (0.2ms)  SELECT  "members".* FROM "members"  ORDER BY "members"."id" ASC LIMIT 1
#<Member:0x000000021fbe20
 id: 1,
 number: 10,
 name: "Taro",
 full_name: "佐藤 太郎",
 email: "Taro@example.com",
 birthday: Tue, 01 Dec 1981,
 gender: 0,
 administrator: true,
 created_at: Wed, 06 Dec 2017 11:04:29 JST +09:00,
 updated_at: Wed, 06 Dec 2017 11:04:29 JST +09:00>
 => #<Member id: 1, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29"> 
2.4.0 :002 > 
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails db
SQLite version 3.8.2 2013-12-06 14:53:30
Enter ".help" for instructions
Enter SQL statements terminated with a ";"
sqlite>  .tables
   ...> .schema members
   ...> SELECT * from members;
Error: near ".": syntax error
sqlite>  .tables
   ...> .schema members
   ...> SELECT * from members;
Error: near ".": syntax error
sqlite> .tables
members            schema_migrations
sqlite> .schema members
CREATE TABLE "members" ("id" INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL, "number" integer NOT NULL, "name" varchar NOT NULL, "full_name" varchar, "email" varchar, "birthday" date, "gender" integer DEFAULT 0 NOT NULL, "administrator" boolean DEFAULT 'f' NOT NULL, "created_at" datetime NOT NULL, "updated_at" datetime NOT NULL);
sqlite> SELECT * from members;
1|10|Taro|佐藤 太郎|Taro@example.com|1981-12-01|0|t|2017-12-06 02:04:29.853866|2017-12-06 02:04:29.853866
2|11|Jiro|鈴木 次郎|Jiro@example.com|1981-12-01|0|f|2017-12-06 02:04:29.869856|2017-12-06 02:04:29.869856
3|12|Hana|高橋 花子|Hana@example.com|1981-12-01|1|f|2017-12-06 02:04:29.883617|2017-12-06 02:04:29.883617
4|13|John|田中 太郎|John@example.com|1981-12-01|0|f|2017-12-06 02:04:29.898607|2017-12-06 02:04:29.898607
5|14|Mike|佐藤 次郎|Mike@example.com|1981-12-01|0|f|2017-12-06 02:04:29.912073|2017-12-06 02:04:29.912073
6|15|Sophy|鈴木 花子|Sophy@example.com|1981-12-01|1|f|2017-12-06 02:04:29.923868|2017-12-06 02:04:29.923868
7|16|Bill|高橋 太郎|Bill@example.com|1981-12-01|0|f|2017-12-06 02:04:29.938485|2017-12-06 02:04:29.938485
8|17|Alex|田中 次郎|Alex@example.com|1981-12-01|0|f|2017-12-06 02:04:29.951220|2017-12-06 02:04:29.951220
9|18|Mary|佐藤 花子|Mary@example.com|1981-12-01|1|f|2017-12-06 02:04:29.964127|2017-12-06 02:04:29.964127
10|19|Tom|鈴木 太郎|Tom@example.com|1981-12-01|0|f|2017-12-06 02:04:29.978807|2017-12-06 02:04:29.978807
11|10|Taro|佐藤 太郎|Taro@example.com|1981-12-01|0|t|2017-12-06 02:04:36.464618|2017-12-06 02:04:36.464618
12|11|Jiro|鈴木 次郎|Jiro@example.com|1981-12-01|0|f|2017-12-06 02:04:36.484127|2017-12-06 02:04:36.484127
13|12|Hana|高橋 花子|Hana@example.com|1981-12-01|1|f|2017-12-06 02:04:36.501942|2017-12-06 02:04:36.501942
14|13|John|田中 太郎|John@example.com|1981-12-01|0|f|2017-12-06 02:04:36.516497|2017-12-06 02:04:36.516497
15|14|Mike|佐藤 次郎|Mike@example.com|1981-12-01|0|f|2017-12-06 02:04:36.533149|2017-12-06 02:04:36.533149
16|15|Sophy|鈴木 花子|Sophy@example.com|1981-12-01|1|f|2017-12-06 02:04:36.550391|2017-12-06 02:04:36.550391
17|16|Bill|高橋 太郎|Bill@example.com|1981-12-01|0|f|2017-12-06 02:04:36.568044|2017-12-06 02:04:36.568044
18|17|Alex|田中 次郎|Alex@example.com|1981-12-01|0|f|2017-12-06 02:04:36.587789|2017-12-06 02:04:36.587789
19|18|Mary|佐藤 花子|Mary@example.com|1981-12-01|1|f|2017-12-06 02:04:36.602955|2017-12-06 02:04:36.602955
20|19|Tom|鈴木 太郎|Tom@example.com|1981-12-01|0|f|2017-12-06 02:04:36.616774|2017-12-06 02:04:36.616774
sqlite> .quit
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails c
Loading development environment (Rails 4.2.10)
2.4.0 :001 > Members.ids
NameError: uninitialized constant Members
        from (irb):1
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :002 > Members.id
NameError: uninitialized constant Members
        from (irb):2
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :003 > 
kogadoom:~/workspace/lecture-1206/asagao (master) $ bin/rails c
Loading development environment (Rails 4.2.10)
2.4.0 :001 > Members.id
NameError: uninitialized constant Members
        from (irb):1
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :002 > Member.ids
   (0.3ms)  SELECT "members"."id" FROM "members"
 => [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20] 
2.4.0 :003 > member = Members.find(3)
NameError: uninitialized constant Members
        from (irb):3
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:110:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/console.rb:9:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:68:in `console'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands/commands_tasks.rb:39:in `run_command!'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/railties-4.2.10/lib/rails/commands.rb:17:in `<top (required)>'
        from bin/rails:4:in `require'
        from bin/rails:4:in `<main>'
2.4.0 :004 > member = Member.find(3)
  Member Load (0.5ms)  SELECT  "members".* FROM "members" WHERE "members"."id" = ? LIMIT 1  [["id", 3]]
 => #<Member id: 3, number: 12, name: "Hana", full_name: "高橋 花子", email: "Hana@example.com", birthday: "1981-12-01", gender: 1, administrator: false, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29"> 
2.4.0 :005 > member.email
 => "Hana@example.com" 
2.4.0 :006 > member = Member.find_by(name: "Taro")
  Member Load (0.7ms)  SELECT  "members".* FROM "members" WHERE "members"."name" = ? LIMIT 1  [["name", "Taro"]]
 => #<Member id: 1, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29"> 
2.4.0 :007 > member = Member.find_by(gender: 0, administrator: false)
  Member Load (0.5ms)  SELECT  "members".* FROM "members" WHERE "members"."gender" = ? AND "members"."administrator" = ? LIMIT 1  [["gender", 0], ["administrator", "f"]]
 => #<Member id: 2, number: 11, name: "Jiro", full_name: "鈴木 次郎", email: "Jiro@example.com", birthday: "1981-12-01", gender: 0, administrator: false, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29"> 
2.4.0 :008 > member = Member.find_by(gender: 1, administrator: true)
  Member Load (0.4ms)  SELECT  "members".* FROM "members" WHERE "members"."gender" = ? AND "members"."administrator" = ? LIMIT 1  [["gender", 1], ["administrator", "t"]]
 => nil 
2.4.0 :009 > member = Member.where(name: "Taro")
  Member Load (0.6ms)  SELECT "members".* FROM "members" WHERE "members"."name" = ?  [["name", "Taro"]]
 => #<ActiveRecord::Relation [#<Member id: 1, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29">, #<Member id: 11, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:36", updated_at: "2017-12-06 02:04:36">]> 
2.4.0 :010 > puts member.to_sql
SELECT "members".* FROM "members" WHERE "members"."name" = 'Taro'
 => nil 
2.4.0 :011 > members = Member.where(name: "Taro")
  Member Load (0.5ms)  SELECT "members".* FROM "members" WHERE "members"."name" = ?  [["name", "Taro"]]
 => #<ActiveRecord::Relation [#<Member id: 1, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29">, #<Member id: 11, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:36", updated_at: "2017-12-06 02:04:36">]> 
2.4.0 :012 > members = member.where("number < 20")
  Member Load (0.4ms)  SELECT "members".* FROM "members" WHERE "members"."name" = ? AND (number < 20)  [["name", "Taro"]]
 => #<ActiveRecord::Relation [#<Member id: 1, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29">, #<Member id: 11, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:36", updated_at: "2017-12-06 02:04:36">]> 
2.4.0 :013 > members = Member.where(name: "Taro").where("number < 20")
  Member Load (0.3ms)  SELECT "members".* FROM "members" WHERE "members"."name" = ? AND (number < 20)  [["name", "Taro"]]
 => #<ActiveRecord::Relation [#<Member id: 1, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29">, #<Member id: 11, number: 10, name: "Taro", full_name: "佐藤 太郎", email: "Taro@example.com", birthday: "1981-12-01", gender: 0, administrator: true, created_at: "2017-12-06 02:04:36", updated_at: "2017-12-06 02:04:36">]> 
2.4.0 :014 > members = Member.where(gender: 1).order("number")
  Member Load (0.6ms)  SELECT "members".* FROM "members" WHERE "members"."gender" = ?  ORDER BY number  [["gender", 1]]
 => #<ActiveRecord::Relation [#<Member id: 3, number: 12, name: "Hana", full_name: "高橋 花子", email: "Hana@example.com", birthday: "1981-12-01", gender: 1, administrator: false, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29">, #<Member id: 13, number: 12, name: "Hana", full_name: "高橋 花子", email: "Hana@example.com", birthday: "1981-12-01", gender: 1, administrator: false, created_at: "2017-12-06 02:04:36", updated_at: "2017-12-06 02:04:36">, #<Member id: 6, number: 15, name: "Sophy", full_name: "鈴木 花子", email: "Sophy@example.com", birthday: "1981-12-01", gender: 1, administrator: false, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29">, #<Member id: 16, number: 15, name: "Sophy", full_name: "鈴木 花子", email: "Sophy@example.com", birthday: "1981-12-01", gender: 1, administrator: false, created_at: "2017-12-06 02:04:36", updated_at: "2017-12-06 02:04:36">, #<Member id: 9, number: 18, name: "Mary", full_name: "佐藤 花子", email: "Mary@example.com", birthday: "1981-12-01", gender: 1, administrator: false, created_at: "2017-12-06 02:04:29", updated_at: "2017-12-06 02:04:29">, #<Member id: 19, number: 18, name: "Mary", full_name: "佐藤 花子", email: "Mary@example.com", birthday: "1981-12-01", gender: 1, administrator: false, created_at: "2017-12-06 02:04:36", updated_at: "2017-12-06 02:04:36">]> 
2.4.0 :015 > 