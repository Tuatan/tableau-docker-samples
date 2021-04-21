FROM openjdk:8-jre

ADD https://downloads.tableau.com/esdalt/2020.3.7/tableau-tabcmd-2020-3-7_all.deb /tableau-tabcmd.deb

RUN apt-get update \
  && apt-get -y install ./tableau-tabcmd.deb \
  && ./opt/tableau/tabcmd/bin/tabcmd --accepteula > /dev/null

ENV PATH="/opt/tableau/tabcmd/bin:${PATH}"

CMD [ "bash" ]
