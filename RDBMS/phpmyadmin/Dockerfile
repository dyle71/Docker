FROM phpmyadmin:latest

RUN apt-get update && apt-get install -y wget unzip

RUN wget https://files.phpmyadmin.net/themes/boodark/1.1.0/boodark-1.1.0.zip && \
  unzip boodark-1.1.0.zip && \
  mv boodark /var/www/html/themes && \
  chown -R root: /var/www/html/themes/boodark && \
  rm boodark-1.1.0.zip

RUN wget https://files.phpmyadmin.net/themes/darkwolf/5.2/darkwolf-5.2.zip && \
  unzip darkwolf-5.2.zip && \
  mv darkwolf /var/www/html/themes && \
  chown -R root: /var/www/html/themes/darkwolf && \
  rm darkwolf-5.2.zip 
RUN rm -rf /var/lib/apt/lists/*
