source "https://rubygems.org"
# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!
gem "jekyll", "~> 4.2"

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

group :jekyll_plugins do
  gem "jekyll-theme-anu", :git => "git@gitlab.anu.edu.au:jekyll-anu/gems/jekyll-theme-anu.git", :tag => "v2.1.0"
  gem "jekyll-plugins-anu", :git => "git@gitlab.anu.edu.au:jekyll-anu/gems/jekyll-plugins-anu.git",  :tag => "v2.1.0"
  gem "jekyll-revealify-plugin", :git => "git@gitlab.anu.edu.au:jekyll-anu/gems/jekyll-revealify-plugin.git", :branch => "master"
  gem "jekyll-paginate-v2", :git => "https://github.com/viv-li/jekyll-paginate-v2.git", :branch => "develop"
  gem "jekyll-sitemap"
end

# Add webrick as a dependency for Ruby 3.0, as it's no longer a bundles gem
gem "webrick", "~> 1.7"
