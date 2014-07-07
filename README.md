This is a sample project known to work with RSense.  Clone this and try
doing some simple edits in lib/sample.rb.  Should be good for creating
test-cases from, too.

```bash
$ git clone https://github.com/rsense/sample.git
$ cd sample
$ bundle install
$ bundle exec rsense start --path ~/path/to/sample
$ atom/subl/etc . #ie. use whichever editor you are trying out
```
After opening up lib/sample.rb in your editor of choice, try getting completions on `sample` at the bottom by typing a `.s` after it. Like so:

```ruby
require "sample/version"

module Sample
  class Sample
    def sample_method
      "Test"
    end
  end
end
sample = Sample::Sample.new
sample.s
```
