![Header](profile/github-banner.png)

<div align="center">


[![Docker Pulls](https://img.shields.io/docker/pulls/orbitalhq/orbital?style=for-the-badge)](https://hub.docker.com/r/orbitalhq/orbital)
![Latest Version](https://img.shields.io/badge/dynamic/xml.svg?label=Latest&url=http%3A%2F%2Frepo.orbitalhq.com%2Frelease%2Fio%2Fvyne%2Fplatform%2Fmaven-metadata.xml&query=%2F%2Frelease&colorB=green&prefix=v&style=for-the-badge&)

</div>

<div align="center">

[![Join us on Slack](https://img.shields.io/badge/Slack-chat%20with%20us-%235865F2?style=for-the-badge&logo=slack&logoColor=%23fff)](https://join.slack.com/t/orbitalapi/shared_invite/zt-697laanr-DHGXXak5slqsY9DqwrkzHg)
[![Follow us on Twitter](https://img.shields.io/badge/Follow-@orbitalapi-%235865F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/orbitalapi)

</div>

<div align="center">

[Website](https://orbitalhq.com)&nbsp;&nbsp;&nbsp;•&nbsp;&nbsp;&nbsp;
[Docs](https://orbitalhq.com/docs)&nbsp;&nbsp;&nbsp;•&nbsp;&nbsp;&nbsp;
[Blog](https://orbitalhq.com/blog)&nbsp;&nbsp;&nbsp;

</div>

Orbital automates integration for your microservices.

Get started right now, by spinning up Orbital on your machine

```bash
docker run -p 9022:9022 orbitalhq/orbital
```

Then visit http://localhost:9022 in your browser.

## What is Orbital?
Orbital is a data gateway that automates the integration, transformation and discovery of data from data sources (API’s, databases, message brokers) across your enterprise.

Orbital integrates on-the-fly, automatically adjusting as your data sources change.

This is powered [Taxi](https://github.com/taxilang/taxilang) which adds rich [Semantic Metadata](https://orbitalhq.com/blog/2023-05-22-semantic-metadata-101) to your exist API specs, that describes how data relates between your data sources.
