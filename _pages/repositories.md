---
layout: page
permalink: /repositories/
title: GitHub (+ Replication codes)
description: A list of my `GitHub` repositories and replication codes
nav: false
nav_order: 4
---

{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
{% if site.data.repositories.github_users.size > 1 %}

  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.liquid username=user %}
  </div>

---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_repos %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}

## Replication codes

Replication materials for my published papers:
 
<div class="table-responsive">
  <table class="table table-sm">
    <thead>
      <tr>
        <th>Paper</th>
        <th>Description</th>
        <th>Files</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Generalized Latent Variable Models for Location, Scale, and Shape parameters</strong></td>
        <td>R code</td>
        <td>
          <a href="{{ '/assets/replication/glvmlss_replication_files.zip' | relative_url }}" class="btn btn-sm z-depth-0">Code</a>
        </td>
      </tr>
      <tr>
        <td><strong>A Generalized Additive Partial-Mastery Cognitive Diagnostic Model</strong></td>
        <td>R code </td>
        <td>
          <a href="{{ '/assets/replication/pmCDM_replication_files.zip' | relative_url }}" class="btn btn-sm z-depth-0">Code</a>
        </td>
      </tr>
      <!-- Add more papers as needed -->
      <!--
      <tr>
      <td><strong>Paper Title</strong></td>
      <td>Brief description</td>
      <td>
      <a href="{{ '/assets/replication/filename.zip' | relative_url }}" class="btn btn-sm z-depth-0">Code</a>
      </td>
      </tr>
      -->
    </tbody>
  </table>
</div>

