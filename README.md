# Testing Remote Websites With Cucumber and Mechanize

This is a minimal example of how to use [cucumber](http://cukes.info/) and
[mechanize](http://mechanize.rubyforge.org/) to test a remote website.

## Usage

    $ gem install bundler   # ...if you haven't done so already
    $ bundle                # make sure the proper gems are installed
    $ cucumber              # run the tests

You should see something like this:

    Using the default profile...
    Feature: Google Search
      In order to learn something
      As an internet user
      I want to search for information on Google

      Scenario: Learn about Iran                    
        When I Google for "Iran"                    
        Then I should see search results about Iran 

    1 scenario (1 passed)
    2 steps (2 passed)
    0m0.437s

## Origin

Here is the original [blog post](http://surgeworks.com/blog/general/using-cucumber-and-webrat-for-remote-web-testing)
that introduced this code.
