---
title: Welcome
permalink: /docs/home/
redirect_from: /docs/index.html
---

## Getting started

[GitHub Pages](https://pages.github.com) can automatically generate and serve the website for you.
Let's say you have a username/organisation `my-org` and project `my-proj`; if you locate Jekyll source under `docs` folder of master branch in your repo `github.com/my-org/my-proj`, the website will be served on `my-org.github.io/my-proj`.
The good thing about coupling your documentation with the source repo is, whenever you merge features with regarding content to master branch, it will also be published on the webpage instantly.

1. Just [download the source](https://github.com/aksakalli/jekyll-doc-theme/archive/gh-pages.zip) into your repo under `docs` folder.
2. Edit site settings in  `_config.yml` file according to your project. !!! `baseurl` should be your website's relative URI like `/my-proj` !!!
3. Replace `favicon.ico` and `assets/img/logonav.png` with your own logo.

[GitHub Pages](https://pages.github.com)는 자동으로 웹사이트를 생성하여 제공할 수 있습니다. 사용자 이름/조직이 `my-org` 이고 프로젝트가 `my-proj` 라고 가정할 때, `master` 브랜치의 문서 폴더 아래에 있는 지킬 소스를 리포지토리 `github.com/my-org/my-proj`에서 찾으면 웹사이트가 `my-org.github.io/my-proj`에 서비스됩니다. 문서를 소스 리포지토리에 연결하면 좋은 점은 마스터 브랜치에 관련 콘텐츠를 병합할 때마다 웹페이지에도 즉시 게시된다는 것입니다.

1. `docs` 폴더 아래의 리포지토리에 [소스를 다운로드](https://github.com/aksakalli/jekyll-doc-theme/archive/gh-pages.zip) 하기만 하면 됩니다.
2. 프로젝트에 따라 `_config.yml` 파일에서 사이트 설정을 편집합니다. !!! `baseurl`은 `/my-proj`와 같은 웹사이트의 상대 URI여야 합니다 !!!
3. `favicon.ico` 및 `assets/img/logonav.png`를 고유 로고로 바꿉니다.

## Writing content

### Docs

Docs are [collections](https://jekyllrb.com/docs/collections/) of pages stored under `_docs` folder. To create a new page:

**1.** Create a new Markdown as `_docs/my-page.md` and write [front matter](https://jekyllrb.com/docs/frontmatter/) & content such as:

```
---
title: My Page
permalink: /docs/my-page/
---

Hello World!
```

**2.** Add the pagename to `_data/docs.yml` file in order to list in docs navigation panel:

```
- title: My Group Title
  docs:
  - my-page
```

### Blog posts

Add a new Markdown file such as `2017-05-09-my-post.md` and write the content similar to other post examples.

### Pages

The homepage is located under `index.html` file. You can change the content or design completely different welcome page for your taste. (You can use [bootstrap components](http://getbootstrap.com/components/))

In order to add a new page, create a new `.html` or `.md` (markdown) file under root directory and link it in `_includes/topnav.html`.
