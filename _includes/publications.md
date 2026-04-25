<h2 id="publications" class="pub-section-title">Publications <span class="pub-ext-links"><a href="{{ site.google_scholar }}" target="_blank" rel="noopener">Google Scholar</a></span></h2>

<div class="publications">
  <ol class="bibliography">
    {% for link in site.data.publications.main %}
      <li>
        <div class="pub-row">
          <div class="col-sm-3 abbr">
            <img src="{{ link.image | default: '/assets/img/teaser_example.png' | relative_url }}" class="teaser img-fluid z-depth-1" alt="">
            {% if link.conference_short %}
            <abbr class="badge" data-venue="{{ link.conference_short }}">{{ link.conference_short }}</abbr>
            {% endif %}
          </div>
          <div class="col-sm-9">
            <div class="title">
              {% if link.pdf %}
                <a href="{{ link.pdf }}" target="_blank" rel="noopener">{{ link.title }}</a>
              {% else %}
                {{ link.title }}
              {% endif %}
            </div>
            <div class="author">{{ link.authors }}</div>
            {% if link.conference %}
            <div class="periodical"><em>{{ link.conference }}</em></div>
            {% endif %}
            <div class="links">
              {% if link.pdf %}
              <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">PDF</a>
              {% endif %}
              {% if link.doi %}
              <a href="{{ link.doi }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">DOI</a>
              {% endif %}
              {% if link.code %}
              <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Code</a>
              {% endif %}
              {% if link.page %}
              <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Project Page</a>
              {% endif %}
              {% if link.notes %}
              <strong><i>{{ link.notes }}</i></strong>
              {% endif %}
            </div>
          </div>
        </div>
      </li>
    {% endfor %}
  </ol>
</div>
