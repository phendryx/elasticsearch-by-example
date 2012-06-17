ElasticSearch by Example
========================

_ElasticSearch by Example_ is a simple framework to learn and play with
[ElasticSearch](http://elasticsearch.org).

It will help you get started in [ElasticSearch](http://elasticsearch.org)
and provide a sandbox for experimentation and comparison of features.

Each example contains a readme file with the key information on the feature,
sample data, a mapping file and a search query. You can see the output directly
into the console.

It is important that the program is kept as simple as possible.
A [ElasticSearch](http://elasticsearch.org) beginner should easily understand each step.

I have deliberately used raw [JSON](http://www.json.org/) structures to facilitate communication with [ElasticSearch](http://elasticsearch.org) using the
[REST](http://en.wikipedia.org/wiki/Representational_state_transfer) API to make
it clear. There are no abstractions to hide details.


Installation
------------

Clone the project repository from [GitHub](http://github.com/):

    git clone git://github.com/rmoszczynski/elasticsearch-by-example.git
    cd elasticsearch-by-example
    bundle install

If you have already installed [ElasticSearch](http://elasticsearch.org) local
or on a remote machine you're done.

To install [ElasticSearch](http://elasticsearch.org) on Mac with
[Homebrew](http://mxcl.github.com/homebrew/) type:

    brewdle install


Configuration
-------------

_ElasticSearch by Example_ uses its own [ElasticSearch](http://elasticsearch.org) configuration file stored in `config/elasticsearch.yml`.

To use a remote [ElasticSearch](http://elasticsearch.org) installation
please customize the `host` and `port` constants in the `bin/run` script.


Usage
-----

To use _ElasticSearch by Example_ open two console windows.

Console 1:

    foreman start

Console 2:

    bin/run queries/text

As you can see the `bin/run` script takes one parameter, a path to a selected
example directory relative to the `examples` directory in the root of this project.

You can list all examples by using the `list` parameter:

    bin/run list


Links
-----
* [Project Home](https://github.com/rmoszczynski/elasticsearch-by-example)
* [ElasticSearch Home](http://www.elasticsearch.org/)
