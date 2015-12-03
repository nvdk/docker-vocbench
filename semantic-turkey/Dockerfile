FROM java:7
ADD https://bitbucket.org/art-uniroma2/vocbench/downloads/VOCBENCH_2.3.zip /VOCBENCH.zip
RUN apt-get update && apt-get install unzip && mkdir /vocbench /semantic-turkey && unzip /VOCBENCH.zip -d /vocbench/ && unzip -o /vocbench/semanticturkey*.zip -d /semantic-turkey  && chmod +x /semantic-turkey/semanticturkey-0.11/bin/karaf
WORKDIR /semantic-turkey/semanticturkey-0.11/bin
EXPOSE 1979
CMD ["./karaf", "server"]