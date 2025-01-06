# Tuono benchmarks

> [!WARNING]
> This repo is a work in progress.
>
> [Go to tuono repository `benches` folder](https://github.com/tuono-labs/tuono/tree/main/benches)

This repo includes multiple setups to compare the HTTP performance against
tuono and other frameworks.

The main goal is to make the comparison as fair as possible enhancing each framework specific
performance improvements.

Any improvement to the benchmarks or implementation of a different framework is strongly appreciated.

Feel free also to try it with your hardware and open an issue in case you spot significant different results.

## Benchmark setup

In order to make each comparison as fair as possible each framework should contain a single server side
rendered page that requires data from the backend service.

The data returned by the backend service should be a JSON including a random number between 0 and 10.
