# Source code for the [AUR Deploy] website

## Test with Jekyll locally

In order to test the website without having a webserver running and also see
the changes in real time use the `setup.sh` script to run [Jekyll] locally from
the repository directory.

It requires [ruby] to be installed, the rest will be installed locally in a
`.bundle` directory.

The current Gemfile configuration is set to use the same
Jekyll version as [GitHub pages].

The website will be available at <http://localhost:4000/>.

If using another webserver you'll need to point it to the built `_site` directory.

## Development notes

- Please use an [EditorConfig] compatible editor to avoid indentation,
  whitespaces and missing lines at EOF issues.
- Desired line length maximum is 82 columns.
- See above to how to test page's changes with Jekyll.
- For further information please refer to the [Jekyll manual].


[AUR Deploy]:    https://archlive.github.io/aur/
[Jekyll]:        https://jekyllrb.com/
[Jekyll manual]: https://jekyllrb.com/docs/
[ruby]:          https://www.ruby-lang.org/en/
[GitHub pages]:  https://pages.github.com/versions/
