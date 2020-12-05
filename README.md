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

# select one with fuzzy search and preview
bin/list | fzf --preview="bin/preview {}" --preview-window=up:wrap

# select one from three random options
bin/list | shuf | head -n 3 | fzf --preview="bin/preview {}" --preview-window=up:wrap
```

## Data source

The database of programming languages is built using information provided
on Wikipedia.

## Contributing

Please see [CONTRIBUTING](docs/CONTRIBUTING.md) for details.

## License

Please see [LICENSE](LICENSE) for licensing details.
