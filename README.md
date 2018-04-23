# 文因经



> 我们通过选择自己的神明，来选择自己的命运。

## 这是什么？



- 一个开源宗教，使用MIT协议；
- 一个知识管理结构示范，从一切知识的源头出发，零假设，然后逐渐增加认知需要的脚手架，直到我们生活中的柴米油盐；
- MEME，你也可以把这看成我的第47条染色体，期待有一天我们可以等位基因交换。


## 结构是什么？

结构分为两部分。

1. 条款。如同法律中的条款，每一条都是我们生活中很重要的知识，也可以按顺序从上到下串成一个完整的故事。这是经文的主干。作用是指导我们的生活实践、成为了解他人生活原则的标识，甚至在未来的建国中用算法从「个人宪法」生成国家宪法，或者指导群体从末日灾难中恢复文明。
2. 正典。通俗解读条款，是支撑条款的依据，也是家庭教育的读本范围。

条款和正典都是可能改的，根据时代中公共知识、个人知识的变迁。

## 其他




链接中的文档部分从互联网下载来的，侵权请联系删除。

Jekyll主题是从[这个主题](http://pages-themes.github.io/modernist)改过来的，主要改 _sass 的 jekyll-theme-modernist.scss 文件。

欢迎邮件联系：lixvow@foxmail.com

或加入QQ群：230905405

## Usage

To use the Modernist theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    theme: jekyll-theme-modernist
    ```

2. Optionally, if you'd like to preview your site on your computer, add the following to your site's `Gemfile`:

    ```ruby
    gem "github-pages", group: :jekyll_plugins
    ```

## Customizing

### Configuration variables

Modernist will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
```

Additionally, you may choose to set the following optional variables:

```yml
show_downloads: ["true" or "false" to indicate whether to provide a download URL]
google_analytics: [Your Google Analytics tracking ID]
```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:
    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```
3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

*Note: If you'd like to change the theme's Sass variables, you must set new values before the `@import` line in your stylesheet.*

### Layouts

If you'd like to change the theme's HTML layout:

1. [Copy the original template](https://github.com/pages-themes/modernist/blob/master/_layouts/default.html) from the theme's repository<br />(*Pro-tip: click "raw" to make copying easier*)
2. Create a file called `/_layouts/default.html` in your site
3. Paste the default layout content copied in the first step
4. Customize the layout as you'd like

### Overriding GitHub-generated URLs

Templates often rely on URLs supplied by GitHub such as links to your repository or links to download your project. If you'd like to override one or more default URLs:

1. Look at [the template source](https://github.com/pages-themes/modernist/blob/master/_layouts/default.html) to determine the name of the variable. It will be in the form of `{{ site.github.zip_url }}`.
2. Specify the URL that you'd like the template to use in your site's `_config.yml`. For example, if the variable was `site.github.url`, you'd add the following:
    ```yml
    github:
      zip_url: http://example.com/download.zip
      another_url: another value
    ```
3. When your site is built, Jekyll will use the URL you specified, rather than the default one provided by GitHub.

*Note: You must remove the `site.` prefix, and each variable name (after the `github.`) should be indent with two space below `github:`.*

For more information, see [the Jekyll variables documentation](https://jekyllrb.com/docs/variables/).

## Roadmap

See the [open issues](https://github.com/pages-themes/modernist/issues) for a list of proposed features (and known issues).

## Project philosophy

The Modernist theme is intended to make it quick and easy for GitHub Pages users to create their first (or 100th) website. The theme should meet the vast majority of users' needs out of the box, erring on the side of simplicity rather than flexibility, and provide users the opportunity to opt-in to additional complexity if they have specific needs or wish to further customize their experience (such as adding custom CSS or modifying the default layout). It should also look great, but that goes without saying.

## Contributing

Interested in contributing to Modernist? We'd love your help. Modernist is an open source project, built one contribution at a time by users like you. See [the CONTRIBUTING file](docs/CONTRIBUTING.md) for instructions on how to contribute.

### Previewing the theme locally

If you'd like to preview the theme locally (for example, in the process of proposing a change):

1. Clone down the theme's repository (`git clone https://github.com/pages-themes/modernist`)
2. `cd` into the theme's directory
3. Run `script/bootstrap` to install the necessary dependencies
4. Run `bundle exec jekyll serve` to start the preview server
5. Visit [`localhost:4000`](http://localhost:4000) in your browser to preview the theme

### Running tests

The theme contains a minimal test suite, to ensure a site with the theme would build successfully. To run the tests, simply run `script/cibuild`. You'll need to run `script/bootstrap` one before the test script will work.
