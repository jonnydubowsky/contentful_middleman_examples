# Multiple Content Types Example

## How to Run

Paste the following command inside your terminal:

```bash
echo "Checkout Repository"         && git clone git@github.com:contentful/contentful_middleman_examples.git && \
echo "Go to This Example's Folder" && cd contentful_middleman_examples/examples/multiple_content_types && \
echo "Install Dependencies"        && bundle install && \
echo "Create Catalogue Space"      && bundle exec contentful_bootstrap create_space my_catalogue --json-template bootstrap_templates/catalogue.json && \
echo "Fetch Contentful Data"       && bundle exec middleman contentful && \
echo "Start Middleman Server"      && bundle exec middleman server
```

Then open your browser and go to: [localhost:4567](http://localhost:4567)

## Configuration

For reference of basic configuration, you can look into [single_content_type example](../single_content_type/README.md)

In this example we'll be using [Contentful Bootstrap](https://github.com/contentful/contentful-bootstrap.rb) for setting up our own Space with multiple Content Types, and fetching
the configuration from `~/.contentfulrc`

The template used is located [here](./bootstrap_templates/catalogue.json)
