<h1>Commands:</h1>
<ul>
  <li>sudo apt update && sudo apt upgrade -y</li>
  <li>to  check java-->whereis java</li> 
</ul>
<h1>Install mySQL in ubuntu</h1>
<ul>
  <li>fetch the latest version of package list ->sudo apt update</li>
  <li>install mysql -> sudo apt install mysql-server -y</li>
  <li>check mysql daemon running -> sudo systemctl status mysql</li>
  <li>or using this command -->sudo service mysql status</li>
  <li>alternatively you can run --> systemctl is-active mysql</li>
  <li>to enable mysql on the system restart -> sudo systemctl enable mysql</li>
</ul>
<h2>Secure mysql</h2>
<ul>
  <li>run this ->sudo mysql_secure_installation</li>
  <li>if you want password authentication, ctrl c and come out and run -->sudo mysql </li>
  <li>alter user command in sql prompt--> ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';</li>
  <li>run the following command --> FLUSH PRIVILEGES;</li>
  <li>no password change for root, and for all the other options yes</li>
  <li>login with root user ->sudo mysql -u root -p</li>
  <li>create user -->CREATE USER 'nemali'@'localhost' IDENTIFIED BY 'nemali';</li>
  <li>give permissions to nemali user-->GRANT ALL PRIVILEGES ON *.* TO 'nemali'@'localhost' WITH GRANT OPTION;</li>
  <li>flush privileges-->FLUSH PRIVILEGES</li>
  <li>exit</li>
  <li>login and check nemali-->mysql -u nemali -p</li>
  <li>stop mysql -> sudo service mysql stop</li>
  <li>restart mysql -> sudo service mysql stop</li>
</ul>
<h2>my sql workbench installation</h2>
<ul>
  <li>install command -->sudo snap install mysql-workbench-community</li>
</ul>
<h2>My Sql users</h2>
<ul>
  <li>root user password is root</li>
</ul>
