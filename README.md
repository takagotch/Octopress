### octopress
---
https://github.com/octopress/octopress

```
gem install octopress
gem 'octopress', '~> 3.0'
bundle
gem install bundler

octopress init <PATH> [options]
octopress new page some-page
octopress new page about.md
octopress new page docs/
octopress new page _legal/tems
octopress new draft "My Title"
octopress publish _drafts/some-cool-post.md
octopress publish cool
octopress unpublish _posts/2018-11-08-some-post.md
octopress unpublish some post
octpress new post "Some title" --template linkpost
octopress new post "Some title" -tm _templates/linkpost
octopress isolate
octopress isolate _posts/2018-11-08-kittens.md
octopress isolate kittens
octopress deploy
octopress deploy init s3
octopress deploy init rsync
octopress deploy init git git@github.com:user/project
octopress deploy init s3 --help
octopress deploy init rsync --config_stagining.yml
octopress deploy --config_staging.yml
octopress deploy pull [DIR]
```

```ruby
source 'https://rubygems.org'
gem 'octopress', '~> 3.0'


```

```
post_ext: markdown
page_ext: html

post_layout: post
page_layout: page

titlecase: true

post_template: post
page_template: page
draft_template: draft


access_key_id: <%= ENV['AWS_ACCESS_KEY'] %>
secret_access_key: <%= ENV['AWS_SECRET_KEY'] %>

headers:
  - filename: 'assets.*\.js$'
    expires: '+3 years'
    cache_control: 'max-age=94680000'
    content_type: 'application/javascript'
  - filename: '^assets.*\.css$'
    expires: '+3 years'
    cache_control: 'max-age=9468000'
    content_type: 'text/css'

```
