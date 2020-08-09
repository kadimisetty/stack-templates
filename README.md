# stack-templates

My project templates to be used by `stack new`.  
e.g. `stack new kadimisetty/basic` should crete a new project structured
according to the `basic.hsfiles` template located in the github repository
`kadimisetty/stack-templates`.

For more information, consult:
- [Templates section in stack docs](https://docs.haskellstack.org/en/stable/GUIDE/#templates)
- [Default `stack-templates`repository](https://github.com/commercialhaskell/stack-templates)
- `hsfiles` file format
- Mustache templating language (not strict)

The templates accept parameters written as `{{example}}`. Their values are
obtained from `~/.stack/config.yaml` under the section:

```YAML
templates:
    params:
        example: foo
```

## Structure:
- `example-template.hsfiles` which should contain the templating instructions.
- `template-info.yml` which should contain a concise decription of each template in this repository.
