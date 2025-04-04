# Hermit buildkite plugin

Activate hermit environment to use and manage packages.

Will retry hermit activation up to `max_retries` times with a delay of
`retry_delay` seconds between retries. Set `max_retries` to `0` to disable
retries.

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: ls
    plugins:
      - elastic/hermit#v1.0.3
```

## Configuration

| Key | Description | Default |
|-----|-------------|---------|
| `max_retries` | The maximum number of retries for hermit activation | `3` |
| `retry_delay` | The number of seconds to wait between retries | `1` |
