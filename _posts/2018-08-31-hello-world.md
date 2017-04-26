---
layout: post
title: Hello World
subtitle: First post of this blog
---

This is the first blog post.

This is some ruby:
```ruby
  def create_shell_runner(cmd) # :nodoc:
    show_command = sh_show_command cmd
    show_command = show_command[0, 42] + "..." unless $trace

    lambda do |ok, status|
      ok or
        fail "Command failed with status (#{status.exitstatus}): " +
        "[#{show_command}]"
    end
  end
  private :create_shell_runner

```

