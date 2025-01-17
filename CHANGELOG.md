# Changelog

## 1.2.3
- Flake8 tests are now executed at the end of the test session
- Flake8 result caching is now disabled by default (re-enable with `--flake8-enable-result-caching`)

## 1.2.2
- Added `flake8-cli-arguments` pytest config parameter to pass through pytest cli arguments explicitly
- Marked `flake8-max-line-length`, `flake8-max-complexity`, `flake8-show-source`, `flake8-statistics`
    as deprecated (please use flake8 config file or `flake8-cli-arguments` instead)

## 1.2.1
- pyproject.toml is no longer implicitly passed through to flake8 (issue #7)

## 1.2.0
- DROPPED flake8 v3 support
- DROPPED pytest v6 support
- fixed various pytest v7 compatibility warnings

## 1.1.0 - 1.1.2
- branched from the original tholo version
- updated the code base to work with flake8 v4

## 1.0.7

- Implement collect() for Flake8Item; from @thomascobb
- Document skipping behavior in README; from @jpyams

## 1.0.6

- Fix compatibility with flake8 >= 3.8, from @marc

## 1.0.5

- Fix deprecation warning; from @jonasundderwolf

## 1.0.4

- Support flake8 3.7+ by checking existence of "app.make_notifier";
  from jirikuncar@github
- More fixes for Travis CI -- properly specify Python versions, in
  particular for pypy (and fix a typo)

## 1.0.3

- Don't use long deprecated functions from pytest, broke with pytest 4.1.0
- Fix typo that caused some tests to not run as expected
- Run Travis CI tests against Python 3.7, and fix some issues with current tox

## 1.0.2

- Test on Python 3.7
- Escape a regex tring with r""

## 1.0.1

- Correct junit XML output for pytest 3.5.x

## 1.0.0

- Honor ignore settings in default flake8 config section; from
  brianbruggeman@github
- Improve junit XML output; from Struan Judd

## 0.9.1

- Do continuous integration with Travis; from alex-dr@github
- Declare compatibility with Python 3.6

## 0.9

- Extend options already loaded instead of replacing them; from
  mforbes@github
- Correct some issues preventing proper operation with flake8 3.5.0;
  from jezdez@github
- Register pytest marker for flake8; from alex-dr@github

## 0.8, 0.8.1

- Allow running with no cacheprovider
- Modernize use of fixtures in tests

## 0.7

- Added new options "flake8-max-complexity", "flake8-show-source"
  and "flake8-statistics"

## 0.6

- Update for flake8 3.x

## 0.5

- Fix rendering of rST; from Ken Dreyer

## 0.4

- Really fix cache usage; had a comparison between tuple and
  list which always failed

## 0.3

- Use integrated pytest cache instead of separate pytest-cache
  module (which is now integrated)
- Use documented hooks for start and end of a test run

## 0.2

- Added ability to override maximum line length

## 0.1

- initial release
