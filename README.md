# rubocop-configs

A collection of reusable [RuboCop](https://rubocop.org) configuration files for inclusion in other Ruby projects.

## Usage

Add the following to your project's `Gemfile` and run `bundle install`:

```ruby
gem "rubocop"
gem "rubocop-performance"
gem "rubocop-rails"
gem "rubocop-rake"
gem "rubocop-rspec"
```

Add the following to your project's `.rubocop.yml`:

```yaml
inherit_from:
  - https://github.com/jgarber623/rubocop-configs/raw/main/.rubocop.yml
  - https://github.com/jgarber623/rubocop-configs/raw/main/.rubocop-rails.yml
  - https://github.com/jgarber623/rubocop-configs/raw/main/.rubocop-rspec.yml
```

## Dependencies

As noted above, the configurations in this project require one or more of the following RuboCop extensions:

- [rubocop-performance](https://rubygems.org/gems/rubocop-performance)
- [rubocop-rails](https://rubygems.org/gems/rubocop-rails) (`.rubocop-rails.yml` only)
- [rubocop-rake](https://rubygems.org/gems/rubocop-rake)
- [rubocop-rspec](https://rubygems.org/gems/rubocop-rspec) (`.rubocop-rspec.yml` only)

[rubocop-packaging](https://rubygems.org/gems/rubocop-packaging) is also recommended but not required. When using this extension, add the following to your project's `.rubocop.yml`:

```yaml
require:
  - rubocop-packaging
```

## License

rubocop-configs is freely available under the MIT License. Use it, learn from it, fork it, improve it, change it, tailor it to your needs.
