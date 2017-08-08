FROM   tommylau/php-5.2:latest 


#####################################
# MCRYPT:
#####################################

ARG INSTALL_MCRYPT=true
RUN if [ ${INSTALL_MCRYPT} = true ]; then \
    # Install the mcrypt extension
    apt-get update -yqq && \
    apt-get -y install libmcrypt-dev libreadline-dev php5-mcrypt && \
    docker-php-ext-install mcrypt \
;fi