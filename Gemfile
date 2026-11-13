source "https://rubygems.org"

ruby file: ".ruby-version"

# ponytail: production is built by GitHub Pages' legacy builder (pinned github-pages versions);
# this Gemfile only drives local builds. We list the gems the site uses instead of the
# `github-pages` meta-gem, whose jekyll-remote-theme pins a vulnerable rubyzip (< 3.0).
gem "jekyll", "3.10.0"
gem "kramdown-parser-gfm", "1.1.0"

group :jekyll_plugins do
  gem "jekyll-redirect-from", "0.16.0"
  gem "jekyll-paginate", "1.1.0"
  # Plugins GitHub Pages enables by default
  gem "jekyll-github-metadata", "2.16.1"
  gem "jekyll-optional-front-matter", "0.3.2"
  gem "jekyll-readme-index", "0.3.0"
  gem "jekyll-titles-from-headings", "0.5.3"
  gem "jekyll-relative-links", "0.6.1"
  gem "jekyll-default-layout", "0.1.5"
  gem "jekyll-gist", "1.5.0"
  gem "jekyll-coffeescript", "1.2.2"
end
