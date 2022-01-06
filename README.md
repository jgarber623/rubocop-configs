# rubocop-configs

A collection of [RuboCop](https://rubocop.org) configuration files for inclusion in other Ruby-based projects.

## Usage

For standard Ruby projects:

```yaml
# Your project's .rubocop.yml

inherit_from:
  - https://raw.githubusercontent.com/jgarber623/rubocop-configs/main/.rubocop.yml

# Any custom RuboCop configuration
```

For a Ruby gem project:

```yaml
# Your project's .rubocop.yml

inherit_from:
  - https://raw.githubusercontent.com/jgarber623/rubocop-configs/main/.rubocop.gem.yml

# Any custom RuboCop configuration
```

For a Ruby on Rails project:

```yaml
# Your project's .rubocop.yml

inherit_from:
  - https://raw.githubusercontent.com/jgarber623/rubocop-configs/main/.rubocop.rails.yml

# Any custom RuboCop configuration
```

## Additional Dependencies

Note that both the `.rubocop.gem.yml` and `.rubocop.rails.yml` configurations include additional gem dependencies via the `require` directive:

- [rubocop-packaging](https://rubygems.org/gems/rubocop-packaging) (`.rubocop.gem.yml` only)
- [rubocop-performance](https://rubygems.org/gems/rubocop-performance)
- [rubocop-rails](https://rubygems.org/gems/rubocop-rails) (`.rubocop.rails.yml` only)
- [rubocop-rake](https://rubygems.org/gems/rubocop-rake)
- [rubocop-rspec](https://rubygems.org/gems/rubocop-rspec)

Be sure to add the above to your project's `Gemfile` or `.gemspec` as appropriate.
