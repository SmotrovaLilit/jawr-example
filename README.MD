# Пример JAWR
- Заупск tomcat
```
docker run -it --rm -p 8888:8080 -v ./webs:/usr/local/tomcat/webapps tomcat:8.0
```
- Сборка проекта
```
mvn package
```
- Перенос архива в tomcat
```
cp ./target/combine-js-css-1.0.0-SNAPSHOT.war ./webs/example.war
```
- Просмотр
```
http://localhost:8888/example/
```