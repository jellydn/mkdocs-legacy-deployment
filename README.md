<h1 align="center">How to Deploy Legacy Documentation with MkDocs 👋</h1>
<p>This guide will show you how to convert markdown files to an HTML page and deploy old documentation with MkDocs.</p>

## Motivation

As the homepage has changed and only the latest version (e.g. TypeORM v0.3) is available on typeorm.com, it can be useful to deploy old documentation for reference.

## Usage

### ✨ [Demo](https://typeorm-0238.vercel.app/)

To deploy the markdown docs from the typeorm/typeorm repository on GitHub to Vercel, follow these steps:

1. Clone the `typeorm/typeorm` repository using the `npx degit` command.

```sh
mkdir typeorm
cd typeorm
npx degit typeorm/typeorm#0.2.38
```

This will create a new directory called typeorm in your current directory. The directory will contain the source code for the TypeORM project, including the `docs` folder.

2. Install `mkdocs`

```sh
pip install mkdocs
```

3. Setup theme for document page

Create a `mkdocs.yml` with below configuration

```yml
site_name: TypeORM v0.2.38
site_url: https://typeorm-legacy.productsway.com/
theme: readthedocs
```

Then run

```sh
mkdocs build
npx vercel site
```

This will build a document site and deploy the markdown docs to Vercel, creating a live URL for you.

Here is an example of the output of the `vercel deploy` command:

```
Deployment complete!

Your project is now live at:

https://your-project-name.vercel.app/
```

Once the docs have been deployed, you can view them at the URL that was provided.

Sure, here is a reference section for the demo "How to Deploy Old Legacy Documentation with MkDocs 👋":

### References

- MkDocs Documentation: https://www.mkdocs.org/
- How to Install Python: https://www.python.org/downloads/

## Author

👤 **Huynh Duc Dung**

- Website: https://productsway.com/
- Twitter: [@jellydn](https://twitter.com/jellydn)
- Github: [@jellydn](https://github.com/jellydn)

## Show your support

[![kofi](https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/dunghd)
[![paypal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/dunghd)
[![buymeacoffee](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/dunghd)

Give a ⭐️ if this project helped you!
