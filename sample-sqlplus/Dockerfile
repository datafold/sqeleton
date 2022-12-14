FROM oraclelinux:8

ARG release=19
ARG update=10

RUN  dnf -y install oracle-release-el8 && \
     dnf -y install oracle-instantclient${release}.${update}-basic \
         oracle-instantclient${release}.${update}-devel \
         oracle-instantclient${release}.${update}-sqlplus \
     && rm -rf /var/cache/dnf

CMD ["sqlplus", "-v"]

