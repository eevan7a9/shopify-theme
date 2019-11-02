# Shopify theme

## Requirements:

Theme Kit is a command line tool for shopify themes. Download the application and with a tiny bit of setup you’re off to the theme creation races.

### Installation

#### Windows

    choco install themekit

- To verify that Theme Kit has been installed, open cmd.exe and type in theme.

#### Linux

python 2 required

    curl -s https://shopify.github.io/themekit/scripts/install.py | sudo python

- Ensure that it works as expected by running theme version

## Connecting to theme store

You will need to set up an API key to add to our configuration and create a connection between your store and Theme Kit. The API key allows Theme Kit to talk.

### **Shopify App setup**

- log into the Shopify store, In the Shopify Admin, go to **Apps** and click on **Manage private apps**, and then select the **app** or you can **Create a New app**.

in **ADMIN API PERMISSIONS**

> **Theme templates and theme assets** to have "Read and write access".

### **Local setup**

- create copy config(sample) and rename it to "config.yml"
  ```
  theme-folder/config.yml
  ```
- add the following requirements:

  ```
  *use your own password-theme_id-store

  development:
    password: 23hg123g2h3g123ghj123g23123   <---password
    theme_id: "3j213213k12j3mk123"          <---theme_id
    store: store.myshopify.com              <---store

  ```

- Run

in the terminal navigate to **theme-folder/** run the command

```
    theme watch
```
