# Hermit buildkite plugin

Activate hermit environment to use and manage packages

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: ls
    plugins:
      - elastic/hermit#v1.0.0
```
