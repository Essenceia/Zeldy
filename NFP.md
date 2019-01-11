# Notes for posterity

This is a small reminder of this projects challenges for posterity and giggles.

## The 11 of january bug

In the projects the MCU is communicating with an influxDB database. All was
going great, we had finished our testing round on the 10 and our final presentation
was on the 11th. We gathered for the final test about an hour before and
ran for some final tests, and then ... **Error 500** for invalide utf-8 encoding. We triggered an internal
server error on our influxDB backend. Turned out a new version of influxDB
was released that night version `1.6.5`.

> Fun times