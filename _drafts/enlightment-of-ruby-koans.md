---
layout: post
title: "Enlightment of Ruby Koans"
categories: Programming
tags: ruby
---

Enlightment of [Ruby Koans](http://rubykoans.com/).

{% include toc %}

## Asserts

Ruby doesn't provide standard `assert`, but we can use `raise` to accomplish the same job.

```ruby
module Assertions
    FailedAssertionError = Class.new(StandardError)

    def flunk(msg)
      raise FailedAssertionError, msg
    end

    def assert(condition, msg=nil)
      msg ||= "Failed assertion."
      flunk(msg) unless condition
      true
    end

    def assert_equal(expected, actual, msg=nil)
      msg ||= "Expected #{expected.inspect} to equal #{actual.inspect}"
      assert(expected == actual, msg)
    end
end
```

## Nil

Everything in Ruby is an object, even `nil` is an object. This sentence means that `nil` has methods.

```ruby
nil.is_a?(Object) # => true
nil.nil?          # => true
nil.to_s          # => ""
nil.inspect       # => "nil"
```