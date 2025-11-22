# `[redacted]` company technical tests

### overview

This GitHub organization was created with the solely purpose of store and organize the technical tests being taken at the company `[redacted]`.

The goal here is organization and grouping of information for easier access to all parties involved in these tests, and not to share publicly any possible sensitive information about the `[redacted]` company or the `[redacted]` testee, which in this case is yours truly.

Given that there are two tests, one for frontend and one for backend, the environment will be set up so that they can be run either simultaneously or individually, while meeting the requirements in both cases.

### running asgard applications

To run the applications simultaneously, the first thing needed is to create an docker network, so that their dockerfiles can communicate.

```sh
docker create asgard
```

Then fill the envfiles on each of the projects, instructions on how to do so can be found in their README files:

[THOR](https://github.com/technical-test-energy-company/thor)
[LOKI](https://github.com/technical-test-energy-company/loki)

And at last run the docker command on the root of both the projects:

```sh
docker compose up
```

> [!TIP]
> You may also run them locally, without the need for docker.

### documentation

There is a file put together with information about the decisions taken during this accessment, the technical choices made and what I would do with more time and/or previous experience with the stack and tools.

You may find the [file here](../technical-report.pdf), please take some time to read it throughly.
