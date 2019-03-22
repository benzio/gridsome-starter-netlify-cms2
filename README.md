# Netlify CMS starter for Gridsome

## Install
`gridsome create my-gridsome-project netlify-cms`

## Guide

Add your git repository to the `config.yml`.

```yml

backend:
  name: github # Source provider, github, gitlab, etc
  repo: your_name/repo_name # repository name

media_folder: "uploads"
public_folder: "../uploads"

collections:
  - name: "posts"
    label: "Posts"
    folder: "posts"
    create: true
    slug: "{{slug}}"
    fields:
      - {label: "Title", name: "title", widget: "string"}
      - {label: "Excerpt", name: "excerpt", widget: "string"}
      - {label: "Body", name: "content", widget: "markdown"}

```

## Included templates

This starter includes basic template for blogging, for more info read the guide about [Add Netlify CMS](https://gridsome.org/docs/guide-netlify-cms).
