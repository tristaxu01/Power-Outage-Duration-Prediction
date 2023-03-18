# US Major Power Outage Duration Prediction Model

*Between January 2000 to July 2016, there were total of 1534 number power outrage that impacted at least 50,000 customers or caused an unplanned firm load loss of atleast 300 MW occured in United State. The largest power outage affected approximately 3.5 million people, and a maximum of 41,788 MW Peak Demand Power was lost during a single outage event. The focus of our website is to investigate the relationship between monthly electricity prices in the residential sector (labeled as "RES.PRICE" in the dataset) and power outages caused by intentional attacks. Specifically, we aim to determine whether regions with a top 25% residential electricity price are more likely to experience power outages caused by intentional attacks.

-----

# Framing the Problem 

*Power outages are a common occurrence in the power network, and various factors can contribute to these events. As previously mentioned, power outages can result in significant financial losses and negatively impact people's lives. Predicting power outages can help local organizations and individuals take preventative actions to minimize losses before an unexpected event occurs. Our website explores data on major power outage events in the US continental and investigates the relationship between outage duration and factors such as US state, state population, outage occurrence time, climate region, and more using regression analysis. (The data cleaning process has been thoroughly documented on a [separate website](https://github.com/tristaxu01/Intentional-Power-Outage) that explores electricity prices and power outage causes.)

*Our team aims to predict the quantitative data of the power outage duration in minutes based on external factors such as climate, geography, and local electricity information. To measure the ability of our model to predict quantitative data, we will use mean squared error. By doing so, we hope to provide accurate and useful information to help individuals and organizations prepare and prevent significant losses resulting from power outages.



* [Hyde](https://hyde.getpoole.com)
* [Lanyon](https://lanyon.getpoole.com)

Individual theme feedback and bug reports should be submitted to the theme's individual repository.


## Contents

- [Usage](#usage)
- [Development](#development)
- [Author](#author)
- [License](#license)


## Usage

### 1. Install dependencies

Poole is built on Jekyll and uses its built-in SCSS compiler to generate our CSS. Before getting started, you'll need to install the Jekyll gem and related dependencies:

```bash
$ gem install jekyll jekyll-gist jekyll-sitemap jekyll-seo-tag
```

**Windows users:** Windows users have a bit more work to do, but luckily [@juthilo](https://github.com/juthilo) has your back with his [Run Jekyll on Windows](https://github.com/juthilo/run-jekyll-on-windows) guide.

**Need syntax highlighting?** Poole includes support for Pygments or Rouge, so install your gem of choice to make use of the built-in styling. Read more about this in the [Jekyll docs](https://jekyllrb.com/docs/liquid/tags/#code-snippet-highlighting).

### 2a. Quick start

To help anyone with any level of familiarity with Jekyll quickly get started, Poole includes everything you need for a basic Jekyll site. To that end, just download Poole and start up Jekyll.

### 2b. Roll your own Jekyll site

Folks wishing to use Jekyll's templates and styles can do so with a little bit of manual labor. Download Poole and then copy what you need (likely `_layouts/`, `*.html` files, `atom.xml` for RSS, and `assets/` for CSS, JS, etc.).

### 3. Running locally

To see your Jekyll site with Poole applied, start a Jekyll server. In Terminal, from `/poole` (or whatever your Jekyll site's root directory is named):

```bash
$ jekyll serve
```

Open <http://localhost:4000> in your browser, and voilà.

### 4. Serving it up

If you host your code on GitHub, you can use [GitHub Pages](https://pages.github.com) to host your project.

1. Fork this repo and switch to the `gh-pages` branch.
  1. If you're [using a custom domain name](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages), modify the `CNAME` file to point to your new domain.
  2. If you're not using a custom domain name, **modify the `baseurl` in `_config.yml`** to point to your GitHub Pages URL. Example: for a repo at `github.com/username/poole`, use `http://username.github.io/poole/`. **Be sure to include the trailing slash.**
3. Done! Head to your GitHub Pages URL or custom domain.

No matter your production or hosting setup, be sure to verify the `baseurl` option file and `CNAME` settings. Not applying this correctly can mean broken styles on your site.

## Development

Poole has two branches, but only one is used for active development.

- `master` for development.  **All pull requests should be to submitted against `master`.**
- `gh-pages` for our hosted site, which includes our analytics tracking code. **Please avoid using this branch.**

CSS is handled via Jeykll's built-in Sass compiler. Source Sass files are located in `_sass/`, included into `styles.scss`, and compile to `styles.css`.

## Author

**Mark Otto**
- <https://github.com/mdo>
- <https://twitter.com/mdo>


## License

Open sourced under the [MIT license](LICENSE.md).

<3
