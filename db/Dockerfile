FROM mysql:8.0.19

MAINTAINER lengleng(wangiegie@gmail.com)

ENV TZ=Asia/Shanghai

RUN ln -sf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

COPY ./1schema.sql /docker-entrypoint-initdb.d

COPY ./2pigxx.sql /docker-entrypoint-initdb.d

COPY ./3pigxx_ac.sql /docker-entrypoint-initdb.d

COPY ./4pigxx_job.sql /docker-entrypoint-initdb.d

COPY ./5pigxx_mp.sql /docker-entrypoint-initdb.d

COPY ./6pigxx_config.sql /docker-entrypoint-initdb.d

COPY ./7pigxx_pay.sql /docker-entrypoint-initdb.d

COPY ./8pigxx_codegen.sql /docker-entrypoint-initdb.d