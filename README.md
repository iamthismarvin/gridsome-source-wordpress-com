# gridsome-source-wordpress-com

WordPress.com Source for Gridsome. Based on @gridsome/source-wordpress.

## Install

- `npm install git+https://github.com/iamthismarvin/gridsome-source-wordpress-com.git`

## Usage

```js
module.exports = {
  plugins: [
    {
      use: "gridsome-source-wordpress-com",
      options: {
        baseUrl: "WEBSITE_URL", // required
        apiBase: "wp-json",
        typeName: "WordPress",
        perPage: 100,
        concurrent: 10,
        routes: {
          post: "/:year/:month/:day/:slug",
          post_tag: "/tag/:slug"
        }
      }
    }
  ]
};
```
