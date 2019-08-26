context.xml 的 JDBC 設定

    <Resource name="jdbc/map" auth="Container" type="javax.sql.DataSource"

    username="sa" password="P@ssw0rdtiis" driverClassName="com.microsoft.sqlserver.jdbc.SQLServerDriver"

    url="jdbc:sqlserver://172.19.85.211:1433;databaseName=APC" maxActive="1" maxIdle="1"/>

web.xml 的 JDBC 設定

  <resource-ref>
      <description>DB Connection</description>
      <res-ref-name>jdbc/map</res-ref-name>
      <res-type>javax.sql.DataSource</res-type>
      <res-auth>Container</res-auth>
  </resource-ref>

Tomcat/lib 需有 mssql-jdbc-7.2.2.jre8.jar
