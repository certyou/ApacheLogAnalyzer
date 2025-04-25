FROM httpd:2.4

# Créer un utilisateur sans privilèges
RUN addgroup --system apachegroup && \
    adduser --system --ingroup apachegroup --home /home/apacheuser apacheuser

# Copier la configuration d'Apache et le contenu de public-html
COPY httpd.conf /usr/local/apache2/conf/httpd.conf
COPY public-html/ /usr/local/apache2/htdocs/

# Assurez-vous que le bon module mpm est activé
RUN sed -i 's/LoadModule mpm_event_module/#LoadModule mpm_event_module/' /usr/local/apache2/conf/httpd.conf && \
    echo 'LoadModule mpm_prefork_module modules/mod_mpm_prefork.so' >> /usr/local/apache2/conf/httpd.conf

# Donne les permissions à apacheuser
RUN chown -R apacheuser:apachegroup /usr/local/apache2/htdocs /usr/local/apache2/logs || true

# Lancer Apache en mode foreground
CMD ["httpd", "-D", "FOREGROUND"]
