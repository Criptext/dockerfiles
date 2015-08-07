FROM mysql

RUN usermod -u 1000 mysql
RUN usermod -G staff mysql

RUN chown -R mysql:staff /var/lib/mysql
RUN chown -R mysql:staff /var/run/mysqld
RUN chmod -R 770 /var/lib/mysql
RUN chmod -R 770 /var/run/mysqld
