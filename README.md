# Sprint name tool (sname)

Sprint name tool helps to choose an interesting name for a sprint.
At the moment it uses a database of 655 programming languages as
a source of inspiration.

**WARNING:** it's a prototype project. Everything is unstable.

## Install

```shell
git clone git@github.com:soulim/sname.git
cd sname
```

## Usage

```shell
# list all names
bin/list

# if you have FZF installed
bin/list | fzf --preview "bin/preview {}"
```

## Data source

The database of programming languages is built using information provided
on Wikipedia.

## Contributing

Please see [CONTRIBUTING](docs/CONTRIBUTING.md) for details.

## License

Please see [LICENSE](LICENSE) for licensing details.
