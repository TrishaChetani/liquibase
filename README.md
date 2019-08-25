'''How to run ?'''


liquibase --driver=com.mysql.cj.jdbc.Driver \
	      --classpath="/Users/chetatri/Library/Preferences/IntelliJIdea2019.1/jdbc-drivers/MySQL Connector/J 8/8.0.15/mysql-connector-java-8.0.15.jar" \
          --changeLogFile=src/main/resources/db.changelog.xml \
          --url="jdbc:mysql://localhost:3306/example?serverTimezone=UTC" \
          --username=root \
          --password=1234 \
            migrate

driver: com.mysql.jdbc.Driver
classpath: lib/mysql-connector-java-5.1.29-bin.jar
url: 
username: root
password: root


liquibase --username=root  --password=1234   migrate

How to populate data on elastic search as liquibase is not supported
liquibase  --username=root --password=1234 --contexts=test  migrate