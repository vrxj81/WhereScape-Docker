FROM az82/docker-derby

HEALTHCHECK CMD nc -z localhost 1527 || exit 1

CMD ["java", "-Dderby.stream.error.field=java.lang.System.out", "org.apache.derby.drda.NetworkServerControl", "start", "-h", "0.0.0.0"]
