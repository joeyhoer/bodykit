# Bodykit

Bodykit improves frontend web development by providing abstractions of frequently used styling patterns.

## Some Assembly Required
Bodykit is a Sass library, designed to be style agnostic, providing developers with pieces to assemble and paint as they see fit.

## Adding a Mixin

After adding a new mixin, create a test in the `test/sass` directory and run the following command to generate an output file:

    echo $new-mixin | xargs -I% sass --scss --sourcemap=none test/sass/%.scss:test/css/%.css

**Note:** `$new-mixin` is the filename of the new mixin.

Once the output has been generated, validate that the output is correct before commiting your changes.

## Running Tests

The test suite requires [minitest](https://github.com/seattlerb/minitest), which can be installed with:

    gem install minitest

Tests can be run with:

    ruby test.rb

## Documentation

Bodykit uses [SassDoc](https://github.com/SassDoc/).
