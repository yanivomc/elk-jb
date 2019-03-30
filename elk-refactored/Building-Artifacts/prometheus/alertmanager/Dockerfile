FROM        prom/alertmanager:latest
COPY ./config/alertmanager.yml /etc/alertmanager/alertmanager.yml
ENTRYPOINT [ "/bin/alertmanager" ]
CMD        [ "--config.file=/etc/alertmanager/alertmanager.yml", \
             "--storage.path=/alertmanager", "--web.listen-address=:9118", "--log.level=debug"]

             #,"--web.external-url=promlb.roojoom.net:9118"