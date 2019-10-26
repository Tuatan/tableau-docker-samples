FROM openjdk:8

ADD https://downloads.tableau.com/esdalt/2019.3.1/tableau-tabcmd-2019-3-1_all.deb //tableau-tabcmd-2019-3-1_all.deb

RUN apt-get install ./tableau-tabcmd-2019-3-1_all.deb
RUN ./opt/tableau/tabcmd/bin/tabcmd --accepteula > /dev/null

ENV PATH="/opt/tableau/tabcmd/bin:${PATH}"

CMD [ "bash" ]
