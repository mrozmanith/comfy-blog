# ComfyBlog

ComfyBlog is a simple blog management engine for [ComfortableMexicanSofa](https://github.com/comfy/comfortable-mexican-sofa)

[![Gem Version](https://img.shields.io/gem/v/comfy_blog.svg?style=flat)](http://rubygems.org/gems/comfy_blog)
[![Gem Downloads](https://img.shields.io/gem/dt/comfy_blog.svg?style=flat)](http://rubygems.org/gems/comfy_blog)
[![Build Status](https://img.shields.io/travis/comfy/comfy-blog.svg?style=flat)](https://travis-ci.org/comfy/comfy-blog)
[![Dependency Status](https://img.shields.io/gemnasium/comfy/comfy-blog.svg?style=flat)](https://gemnasium.com/comfy/comfy-blog)
[![Code Climate](https://img.shields.io/codeclimate/maintainability/comfy/comfy-blog.svg?style=flat)](https://codeclimate.com/github/comfy/comfy-blog)
[![Coverage Status](https://img.shields.io/coveralls/comfy/comfy-blog.svg?style=flat)](https://coveralls.io/r/comfy/comfy-blog?branch=master)

## Dependencies

Make sure that you have [ComfortableMexicanSofa](https://github.com/comfy/comfortable-mexican-sofa) installed first.

## Installation

Add gem definition to your Gemfile:

```ruby
gem 'comfy_blog', '~> 2.0.0'
```

Then from the Rails project's root run:

    bundle install
    rails generate comfy:blog
    rake db:migrate

Take a look inside your `config/routes.rb` file and you should see following lines there:

```ruby
comfy_route :blog_admin, path: 'admin'
comfy_route :blog, path: 'blog'
```

You should also find view templates in `/app/views/blog` folder. Feel free to adjust them as you see fit.

---

Copyright 2009-2017 Oleg Khabarov
