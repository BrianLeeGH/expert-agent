# Expert Agent

Hermes Agent base distribution for administrator-defined experts.

## Install

```bash
hermes profile install \
  https://github.com/BrianLeeGH/expert-agent.git \
  --name expert-agent \
  --yes
```

Create a concrete expert from the installed base, then replace its SOUL through
the Hermes administration path:

```bash
hermes profile create n8n-expert --clone --clone-from expert-agent
```

The expert retains memory and skill growth but explicitly disables
`soul-manage`. ChatHub applications use concrete expert profiles in `Shared`
mode.

