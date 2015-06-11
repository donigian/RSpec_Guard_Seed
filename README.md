RSpec Guard Seed
===================

This is a seed project which demonstrates how to use RSpec with Guard to unit test Ruby projects.
CI is done using Travis.

Two ways to run:
-------------------
1) `rspec spec`

This is the most concise and fastest way to execute unit tests.

2) `bundle exec rake spec`

Instead of running rspec to execute your test suite, you could optionally run rake spec.
When you execute rake spec from the command line, the Rails environment is loaded to support the
rake task with the development profile **(RAILS_ENV=dev)**. In order to run with a proper test environment,
rake spec spawns off rspec in a child process with the test profile **(RAILS_ENV=test)**.
This means that the Rails environment gets loaded twice is slower than executing rspec by itself.


