source 'https://rubygems.org'

# Jekyll core
gem 'jekyll', '~> 4.3'

# Use the SassC-based converter (jekyll-sass-converter 2.x) because
# jekyll-sass-converter 3.x pulls in sass-embedded which requires
# rubygems >= 3.3.22 — newer than what ships with Debian/Ubuntu's Ruby 3.0.
gem 'jekyll-sass-converter', '~> 2.0'

group :jekyll_plugins do
  gem 'jekyll-gist'
  gem 'jekyll-paginate'
  gem 'jekyll-asciidoc'
  gem 'jekyll-feed'
end

gem 'asciidoctor', '~> 2.0'
gem 'coderay', '~> 1.1'

# Webrick is no longer bundled with Ruby 3+
gem 'webrick'
