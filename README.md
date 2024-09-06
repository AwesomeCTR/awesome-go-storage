# Awesome Go Storage [![Awesome](https://cdn.jsdelivr.net/gh/sindresorhus/awesome@d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

Список удивительных проектов хранения и библиотек Go. Вдохновленный [awesome-go](https://x07.it/catalog/awesome/awesome-go).

### Contents

- [Awesome Go Storage](#awesome-go-storage)
    - [Storage Server](#storage-server)
    - [Key-Value Store](#key-value-store)
    - [File System](#file-system)
    - [Database](#database)
    - [Database Drivers](#database-drivers)


## Storage Server

*Серверы хранения данных, реализованные на Go.*

* [minio](https://github.com/minio/minio) - Minio - сервер объектного хранения с открытым исходным кодом, совместимый с API Amazon S3.
* [rclone](https://github.com/ncw/rclone) - «rsync для облачных хранилищ» - Google Drive, Amazon Drive, S3, Dropbox, Backblaze B2, One Drive, Swift, Hubic, Cloudfile...
* [perkeep](https://github.com/perkeep/perkeep) - Perkeep - это ваша персональная система хранения данных на всю жизнь: способ хранения, синхронизации, обмена, моделирования и резервного копирования контента.
* [s3git](https://github.com/s3git/s3git) - Git для облачного хранилища. Распределенный контроль версий для данных.
* [storj](https://github.com/storj/storj) - Децентрализованное облачное хранилище объектов, доступное, простое в использовании, приватное и безопасное. 
* [rook](https://github.com/rook/rook) - Открытое, облачное и универсальное распределенное хранилище.
* [longhorn](https://github.com/rancher/longhorn) - Longhorn - это сервер постоянного блочного хранения с открытым исходным кодом, поставляемый через контейнеры. 

## Key-Value Store

*Хранилище ключей-значений, реализованное на Go.*

* [Bitcask](https://git.mills.io/prologic/bitcask) - Bitcask - это встраиваемая, постоянная и быстрая база данных ключ-значение (KV), написанная на чистом Go, с предсказуемой производительностью чтения/записи, низкой задержкой и высокой пропускной способностью благодаря компоновке bitcask на диске (LSM+WAL).
* [Bitraft](https://git.mills.io/prologic/bitraft) - Bitraft - это распределенное хранилище ключей/значений на основе плота с протоколом, совместимым с Redis. Оно использует [Bitcask](https://git.mills.io/prologic/bitcask) для высокой производительности/проходимости и низкой задержки.
* [BadgerDB](https://github.com/dgraph-io/badger) - BadgerDB - это встраиваемая, постоянная, простая и быстрая база данных ключ-значение (KV), написанная на чистом Go. Она призвана стать производительной альтернативой не основанным на Go хранилищам ключевых значений, таким как RocksDB.
* [column](https://github.com/kelindar/column) - встраиваемое, столбцовое, in-memory хранилище с растровой индексацией, транзакциями и кверингом с нулевым распределением.
* [consul](https://github.com/hashicorp/consul) - Распределенное последовательное реплицируемое хранилище ключевых значений для обнаружения и настройки сервисов.
* [diskv](https://github.com/peterbourgon/diskv) - Хранилище ключевых значений с поддержкой диска.
* [etcd](https://github.com/coreos/etcd) - Распределенное надежное хранилище ключевых значений для наиболее важных данных распределенной системы.
* [go-cache](https://github.com/patrickmn/go-cache) - Библиотека in-memory key:value store/cache (аналогичная Memcached) для Go, подходит для одномашинных приложений.
* [IceFireDB](https://github.com/IceFireDB/IceFireDB) - Распределенная дисковая база данных, использующая протоколы Raft и Redis.
* [nutsdb](https://github.com/xujiajun/nutsdb) - Nutsdb - это простое, быстрое, встраиваемое, постоянное хранилище ключей/значений, написанное на чистом Go. Оно поддерживает полностью сериализуемые транзакции и многие структуры данных, такие как список, набор, сортированный набор.
* [pogreb](https://github.com/akrylysov/pogreb) - встраиваемое хранилище ключей-значений для рабочих нагрузок с высокой интенсивностью чтения.
* [rosedb](https://github.com/roseduan/rosedb) - Быстрая, стабильная и встроенная k-v база данных на чистом Golang, поддерживает строки, списки, хэши, наборы, сортированные наборы.
* [LotusDB](https://github.com/flower-corp/lotusdb) - Быстрое k/v хранилище, совместимое с lsm tree и b+tree.

## File System

*Файловые системы, реализованные в Go.*

* [afero](https://github.com/spf13/afero) - Система абстракции файловой системы для Go.
* [fsnotify](https://github.com/fsnotify/fsnotify) - Кроссплатформенная система уведомлений о файловой системе для Go.
* [juicefs](https://github.com/juicedata/juicefs) - Распределенная POSIX файловая система, построенная на базе Redis и S3.
* [gcsfuse](https://github.com/GoogleCloudPlatform/gcsfuse) - Файловая система пользовательского пространства для взаимодействия с Google Cloud Storage.
* [git-lfs](https://github.com/git-lfs/git-lfs) - расширение Git для версионирования больших файлов.
* [go-systemd](https://github.com/coreos/go-systemd) - Связки Go для активации сокетов systemd, журнала, D-Bus и юнит-файлов.
* [goofys](https://github.com/kahing/goofys) - Высокопроизводительная, POSIX-ish файловая система Amazon S3, написанная на Go.
* [minikeyvalue](https://github.com/geohot/minikeyvalue) - Распределенное хранилище ключевых значений на ~1000 строк.
* [seaweedfs](https://github.com/chrislusf/seaweedfs) - SeaweedFS - простая и высокомасштабируемая распределенная файловая система для небольших файлов.
* [svfs](https://github.com/ovh/svfs) - Виртуальная файловая система над Openstack Swift, построенная на основе fuse.

## Database

*Базы данных, реализованные на Go.*

* [BigCache](https://github.com/allegro/bigcache) - Эффективный кэш ключей/значений для гигабайтов данных.
* [bolt](https://github.com/boltdb/bolt) - низкоуровневая база данных ключей/значений для Go. Эта оригинальная версия, созданная Беном Джонсоном, была помечена как неподдерживаемая и развита на [etcd-io bbolt](https://github.com/etcd-io/bbolt).
* [buntdb](https://github.com/tidwall/buntdb) - Быстрая, встраиваемая, in-memory база данных ключей/значений для Go с пользовательской индексацией и пространственной поддержкой.
* [cache2go](https://github.com/muesli/cache2go) - Кэш in-memory ключ:значение, поддерживающий автоматическое аннулирование на основе таймаутов.
* [clover](https://github.com/ostafen/clover) - Легкая документо-ориентированная NoSQL база данных, написанная на чистом Golang.
* [cockroach](https://github.com/cockroachdb/cockroach) - Масштабируемое, геореплицируемое, транзакционное хранилище данных.
* [couchcache](https://github.com/codingsince1985/couchcache) - RESTful микросервис кэширования, поддерживаемый сервером Couchbase.
* [CovenantSQL](https://github.com/CovenantSQL/CovenantSQL) - База данных SQL с функциями блокчейна.
* [dgraph](https://github.com/dgraph-io/dgraph) - Масштабируемая, распределенная, с низкой задержкой и высокой пропускной способностью база данных графиков.
* [diskv](https://github.com/peterbourgon/diskv) - Отечественное хранилище ключевых значений с поддержкой дисков.
* [dolt](https://github.com/dolthub/dolt) - MySQL-совместимая база данных с контролем версий в стиле Git. Первая SQL-база данных, которую можно разветвлять и объединять.
* [eliasdb](https://github.com/krotik/eliasdb) - Независящая от зависимостей, транзакционная база данных графов с REST API, поиском по фразам и SQL-подобным языком запросов.
* [emitter](https://github.com/emitter-io/emitter) - Масштабируемая, распределенная и безопасная база данных pub/sub с низким уровнем задержек и хранением сообщений временных рядов, подходит для IoT, игр, приложений и веба в реальном времени.
* [forestdb](https://github.com/couchbase/goforestdb) - Связка Go для ForestDB.
* [frostdb](https://github.com/polarsignals/frostdb/) - Встраиваемая колоночная база данных, написанная на Go. 
* [GCache](https://github.com/bluele/gcache) - Библиотека кэша с поддержкой расширяемого кэша, LFU, LRU и ARC.
* [geocache](https://github.com/melihmucuk/geocache) - Кэш in-memory, который подходит для приложений, основанных на геолокации.
* [go-cache](https://github.com/pmylund/go-cache) - Библиотека in-memory key:value store/cache (аналогичная Memcached) для Go, подходит для одномашинных приложений.
* [godis](https://github.com/hdt3213/godis) - реализованный на Golang высокопроизводительный сервер и кластер Redis.
* [goleveldb](https://github.com/syndtr/goleveldb) - Реализация базы данных ключей/значений [LevelDB](https://github.com/google/leveldb) в Go.
* [groupcache](https://github.com/golang/groupcache) - Groupcache - это библиотека для кэширования и заполнения кэша, предназначенная для замены memcached во многих случаях.
* [immudb](https://github.com/codenotary/immudb) - База данных со встроенной криптографической проверкой и доказательством. Может работать как хранилище ключевых значений или как реляционная база данных (SQL).
* [influxdb](https://github.com/influxdb/influxdb) - Масштабируемое хранилище данных для метрик, событий и аналитики в реальном времени.
* [ledisdb](https://github.com/siddontang/ledisdb) - Ledisdb - высокопроизводительная NoSQL, подобная Redis, основанная на LevelDB.
* [levigo](https://github.com/jmhodges/levigo) - Levigo является оберткой Go для LevelDB.
* [moss](https://github.com/couchbase/moss) - Moss - простой LSM-движок для хранения ключевых значений, написанный на 100% Go.
* [noms](https://github.com/attic-labs/noms) - Версионная, вилочная, синхронизируемая база данных.
* [objectbox-go](https://github.com/objectbox/objectbox-go) - Встраиваемая объектная база данных (NoSQL) с Go API.
* [piladb](https://github.com/fern4lvarez/piladb) - Легкий RESTful движок баз данных, основанный на стековых структурах данных.
* [pREST](https://github.com/nuveo/prest) - Предоставление RESTful API из любой базы данных PostgreSQL.
* [prometheus](https://github.com/prometheus/prometheus) - Система мониторинга и база данных временных рядов.
* [rqlite](https://github.com/rqlite/rqlite) - Легкая, распределенная, реляционная база данных, построенная на SQLite.
* [scribble](https://github.com/nanobox-io/golang-scribble) - Крошечное плоское хранилище JSON-файлов.
* [SpiceDB](https://github.com/authzed/spicedb) - База данных, вдохновленная [Zanzibar](https://research.google/pubs/pub48190/), которая хранит, вычисляет и проверяет разрешения приложений с поддержкой нескольких бэкендов баз данных.
* [tidb](https://github.com/pingcap/tidb) - TiDB - распределенная база данных SQL. Вдохновлена дизайном Google F1.
* [tiedot](https://github.com/HouzuoGuo/tiedot) - Ваша NoSQL база данных на базе Golang.
* [Tile38](https://github.com/tidwall/tile38) - Геолокационная БД с пространственным индексом и геозоной в реальном времени.
  
*Миграция схем баз данных.*

* [darwin](https://github.com/GuiaBolso/darwin) - Библиотека эволюции схем баз данных для Go
* [goose](https://github.com/steinbacher/goose) - Инструмент миграции баз данных. Вы можете управлять эволюцией базы данных, создавая инкрементные SQL- или Go-скрипты.
* [gormigrate](https://github.com/go-gormigrate/gormigrate) - Помощник миграции схем баз данных для Gorm ORM.
* [migrate](https://github.com/golang-migrate/migrate) - обработка миграции баз данных в Golang с поддержкой MySQL, PostgreSQL, Cassandra и SQLite.
* [pravasan](https://github.com/pravasan/pravasan) - Простой инструмент миграции - в настоящее время для MySQL, но в скором времени планируется поддержка Postgres, SQLite, MongoDB и т.д.,
* [soda](https://github.com/markbates/pop/tree/master/soda) - Миграция баз данных, создание, ORM и т.д... для MySQL, PostgreSQL и SQLite.
* [sql-migrate](https://github.com/rubenv/sql-migrate) - Инструмент для миграции баз данных. Позволяет встраивать миграции в приложение с помощью go-bindata.

*Инструменты для работы с базами данных.*

* [go-mysql](https://github.com/siddontang/go-mysql) - Набор инструментов go для работы с протоколом MySQL и репликацией.
* [go-mysql-elasticsearch](https://github.com/siddontang/go-mysql-elasticsearch) - автоматическая синхронизация данных MySQL с Elasticsearch.
* [kingshard](https://github.com/flike/kingshard) - kingshard - это высокопроизводительный прокси для MySQL на базе Golang.
* [myreplication](https://github.com/2tvenom/myreplication) - Слушатель репликации бинарного журнала MySql. Поддерживает репликацию на основе операторов и строк.
* [orchestrator](https://github.com/openark/orchestrator) - Менеджер и визуализатор топологии репликации MySQL
* [pgweb](https://github.com/sosedoff/pgweb) - Веб-браузер баз данных PostgreSQL
* [vitess](https://github.com/youtube/vitess) - vitess предоставляет серверы и инструменты, которые облегчают масштабирование баз данных MySQL для крупномасштабных веб-сервисов.
* [usql](https://github.com/xo/usql) - универсальный интерфейс командной строки для баз данных SQL.

*Построитель SQL-запросов, библиотеки для построения и использования SQL.*

* [buildsqlx](https://github.com/arthurkushman/buildsqlx) - Библиотека построителя запросов к базам данных Go
* [dat](https://github.com/mgutz/dat) - Go Postgres Data Access Toolkit
* [Dotsql](https://github.com/gchaincl/dotsql) - библиотека Go, которая помогает хранить sql-файлы в одном месте и легко использовать их.
* [goqu](https://github.com/doug-martin/goqu) - Идиоматический SQL-конструктор и библиотека запросов.
* [grimoire](https://github.com/Fs02/grimoire) - Grimoire - это слой доступа к базам данных и валидации для golang. (Поддержка: MySQL, PostgreSQL и SQLite3).
* [igor](https://github.com/galeone/igor) - Уровень абстракции для PostgreSQL, поддерживающий расширенную функциональность и использующий gorm-подобный синтаксис.
* [ozzo-dbx](https://github.com/go-ozzo/ozzo-dbx) - Мощные методы поиска данных, а также возможности построения запросов, не зависящих от БД.
* [SQLBoiler](https://github.com/volatiletech/sqlboiler) - инструмент для генерации Go ORM, адаптированного под схему вашей базы данных. Это ORM «database-first», в отличие от «code-first», и вы должны сначала создать свою базу данных.
* [sqrl](https://github.com/elgris/sqrl) - построитель SQL-запросов, форк Squirrel с улучшенной производительностью.
* [Squirrel](https://github.com/Masterminds/squirrel) - библиотека Go, помогающая строить SQL-запросы.
* [xo](https://github.com/knq/xo) - Генерация идиоматического Go-кода для баз данных на основе существующих определений схем или пользовательских запросов с поддержкой PostgreSQL, MySQL, SQLite, Oracle и Microsoft SQL Server.


## Database Drivers

*Библиотеки для подключения и работы с базами данных.*

* Реляционные базы данных
    * [bgc](https://github.com/viant/bgc) - Подключение к хранилищу данных для BigQuery для Go.
    * [firebirdsql](https://github.com/nakagami/firebirdsql) - SQL-драйвер РСУБД Firebird для Go.
    * [go-adodb](https://github.com/mattn/go-adodb) - Драйвер Microsoft ActiveX Object DataBase для go, использующий базу данных/sql.
    * [go-bqstreamer](https://github.com/rounds/go-bqstreamer) - быстрая и параллельная потоковая вставка BigQuery.
    * [go-mssqldb](https://github.com/denisenkom/go-mssqldb) - Драйвер Microsoft MSSQL на языке go.
    * [go-oci8](https://github.com/mattn/go-oci8) - Драйвер Oracle для go, использующий базу данных/sql.
    * [go-sql-driver/mysql](https://github.com/go-sql-driver/mysql) - Драйвер MySQL для Go.
    * [go-sqlite3](https://github.com/mattn/go-sqlite3) - Драйвер SQLite3 для Go, использующий базу данных/sql.
    * [gofreetds](https://github.com/minus5/gofreetds) Драйвер Microsoft MSSQL. Обертка для Go над [FreeTDS](http://www.freetds.org).
    * [pgx](https://github.com/jackc/pgx) - драйвер PostgreSQL, поддерживающий функции, выходящие за рамки тех, что предоставляет database/sql.
    * [pq](https://github.com/lib/pq) - Чистый драйвер Go Postgres для database/sql.

* Базы данных NoSQL
    * [aerospike-client-go](https://github.com/aerospike/aerospike-client-go) - Клиент Aerospike на языке Go.
    * [arangolite](https://github.com/solher/arangolite) - Легкий golang-драйвер для ArangoDB.
    * [asc](https://github.com/viant/asc) - Подключение к хранилищу данных для Aerospike на языке Go.
    * [cayley](https://github.com/google/cayley) - Графовая база данных с поддержкой нескольких бэкендов.
    * [dsc](https://github.com/viant/dsc) - Возможность подключения к хранилищу данных для SQL, NoSQL, структурированных файлов.
    * [dynago](https://github.com/underarmour/dynago) - Dynago - клиент для DynamoDB, работающий по принципу наименьшего удивления.
    * [go-couchbase](https://github.com/couchbase/go-couchbase) - Клиент Couchbase на Go
    * [go-couchdb](https://github.com/fjl/go-couchdb) - Еще одна обертка CouchDB HTTP API для Go
    * [gocb](https://github.com/couchbase/gocb) - Официальный Couchbase Go SDK
    * [gocql](http://gocql.github.io) - Драйвер языка Go для Apache Cassandra.
    * [gomemcache](https://github.com/bradfitz/gomemcache/) - клиентская библиотека memcache для языка программирования Go.
    * [gorethink](https://github.com/GoRethink/gorethink) - Драйвер на языке Go для RethinkDB
    * [goriak](https://github.com/zegl/goriak) - драйвер языка Go для Riak KV   
    * [mongo-go-driver](https://github.com/mongodb/mongo-go-driver) - Go-драйвер для MongoDB
    * [neo4j](https://github.com/cihangir/neo4j) - Связка Neo4j Rest API для Golang
    * [Neo4j-GO](https://github.com/davemeehan/Neo4j-GO) - REST-клиент Neo4j на golang.
    * [neoism](https://github.com/jmcvetta/neoism) - Neo4j клиент для Golang
    * [redigo](https://github.com/gomodule/redigo) - Redigo - Go-клиент для базы данных Redis.
    * [redis](https://github.com/go-redis/redis) - Клиент Redis для Golang
    * [redis](https://github.com/hoisie/redis) - Простой, мощный клиент Redis для Go.
    * [redeo](https://github.com/bsm/redeo) - TCP-серверы/сервисы, совместимые с Redis-протоколом.

* Поисковые и аналитические базы данных
    * [bleve](https://github.com/blevesearch/bleve) - Современная библиотека индексации текста для Go.
    * [elastic](https://github.com/olivere/elastic) - Клиент Elasticsearch для Go.
    * [elastigo](https://github.com/mattbaird/elastigo) - Клиентская библиотека Elasticsearch.
    * [skizze](https://github.com/seiflotfy/skizze) - Сервис и хранилище вероятностных структур данных.

* Множество бэкендов
    * [Fiber Storage](https://github.com/gofiber/storage) - готовые драйверы хранилищ, реализующие интерфейс [Storage](https://github.com/gofiber/storage/blob/main/storage.go). 
    * [gokv](https://github.com/philippgille/gokv) - простой интерфейс хранилища ключевых значений и множество реализаций для Go (Redis, Consul, etcd, bbolt, BadgerDB, LevelDB, Memcached, DynamoDB, S3, PostgreSQL, MongoDB, CockroachDB и многие другие)
