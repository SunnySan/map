context.xml �� JDBC �]�w

    <Resource name="jdbc/map" auth="Container" type="javax.sql.DataSource"

    username="sa" password="P@ssw0rdtiis" driverClassName="com.microsoft.sqlserver.jdbc.SQLServerDriver"

    url="jdbc:sqlserver://172.19.85.211:1433;databaseName=APC" maxActive="1" maxIdle="1"/>

web.xml �� JDBC �]�w

  <resource-ref>
      <description>DB Connection</description>
      <res-ref-name>jdbc/map</res-ref-name>
      <res-type>javax.sql.DataSource</res-type>
      <res-auth>Container</res-auth>
  </resource-ref>

Tomcat/lib �ݦ� mssql-jdbc-7.2.2.jre8.jar
