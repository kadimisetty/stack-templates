# stack-templates

My project templates to be used by `stack new`.  
e.g. `stack new kadimisetty/basic` should create a new project structured
according to the `basic.hsfiles` template located in the github repository
`kadimisetty/stack-templates`.

For more information, consult:
- [Templates section in stack docs](https://docs.haskellstack.org/en/stable/GUIDE/#templates)
- [Default `stack-templates`repository](https://github.com/commercialhaskell/stack-templates)
- `hsfiles` file format
- Mustache templating language (not strict)

The templates accept parameters (written as `{{example}}`) whose values are
obtained from the following section in`~/.stack/config.yaml`:

```YAML
templates:
    params:
        example: foo
```

## Notes:
- `template-info.yml` contains concise descriptions of templates within this repository.
