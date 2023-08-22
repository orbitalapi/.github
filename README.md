![Header](./github-banner.png)

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

Then visit https://localhost:9022 in your browser.

## What is Orbital?
Orbital is a data gateway that automates the integration, transformation and discovery of data from data sources (API’s, databases, message brokers) across your enterprise.

Orbital integrates on-the-fly, automatically adjusting as your data sources change.

This is powered [Taxi](https://github.com/taxilang/taxilang) which adds rich [Semantic Metadata](https://orbitalhq.com/blog/2023-05-22-semantic-metadata-101) to your exist API specs, that describes how data relates between your data sources.

![Network Diagram](network-diagram.png)

## Taxi
Under the hood, Orbital is a [TaxiQL](https://docs.taxilang.org/language-reference/querying-with-taxiql/) query server.

### Links
 * [Taxi](https://taxilang.org)
 * [TaxiQL](https://docs.taxilang.org/language-reference/querying-with-taxiql/) 


## FAQ's

### How does this relate to GraphQL?
Orbital gives you many of the benefits of GraphQL (API federation, custom response schemas), without having to move your tech stack over to GraphQl - instead working with your existing tech stack(s).

The key differences are:

#### Technology agnostic
GraphQL works great when you have GraphQL everywhere.  For everything else, you have to maintain a seperate shim layer to adapt your RESTful API / Database / Message Queue etc., to GraphQL.

Orbital and Taxi work by embedding metatdata in your existing API specs (OpenAPI / Protobuf / Avro / JsonSchema, etc), so that you don't need to change the underlying tech you're using.

#### Decentralized, spec-first federation
Orbital is built for decentralized teams, so that teams can ship changes independently, without having to build and maintain a seperate integration layer.

#### Resolver-free
Resolvers in GraphQL are integration code that has to be maintated - often by a dedicated GraphQL / middleware team.  This means teams that own services have to co-ordinate changes with a seperate integration team.

Instead, Orbital uses Taxi metadata embedded in API specs to define how data relates semantically.  From here, most integration can be created automatically.

### Does this mean all my systems have to have the same ID schemes and request/response models?
Nope. Taxi is designed to encourage teams to evolve independently, without sharing common models.  Instead, semantic scalars are used to compose models together automatically.

We talk more about that in [Why we built Taxi](https://orbitalhq.com/blog/2023-05-12-why-we-created-taxi)

## Doc links

 * [Semantic Integration 101](https://orbitalhq.com/blog/2023-05-22-semantic-metadata-101)
 * [Why we built Taxi](https://orbitalhq.com/blog/2023-05-12-why-we-created-taxi)
 * [Using Semantic Metadata to automate integration](https://orbitalhq.com/blog/2023-01-16-using-semantic-metadata)
 * [Querying for data](https://orbitalhq.com/docs/querying/writing-queries)
 * 