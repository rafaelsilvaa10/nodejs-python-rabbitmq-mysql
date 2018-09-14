FROM mysql:5.7
COPY setup.sh /mysql/setup.sh
COPY setup.sql /mysql/setup.sql
RUN /mysql/setup.sh

#!/bin/bash
set -e
service mysql start
mysql < /mysql/setup.sql
