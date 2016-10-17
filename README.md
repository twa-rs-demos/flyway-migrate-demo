# Flyway gradle
####运行环境
1.Java 6+
2.A working Gradle install  (https://gradle.org/gradle-download/)

####运行方式

Creates an H2 DB populated with the migration scripts in src/main/resources/db/migration
####版本迁移
```
gradle flywayMigrate -i
```
####版本回退
```
gradle flywayClean -i(谨慎使用，删除所有创建的数据库对象，包括用户、表、视图等，回退到初始化数据库时的状态)
```
