---
layout: wide                        
title: Logs
permalink: /logs
---
This is a record of most [**music**](/music), [**films**](/films) and [**books**](/books) I've invested time on. Everything I consider worth your time is highlighted and is recommended.

<script type="text/javascript">
    function showHideDiv(ele) {
        var srcElement = document.getElementById(ele);
        if (srcElement != null) {
            if (srcElement.style.display == "block") {
                srcElement.style.display = 'none';
            }
            else {
                srcElement.style.display = 'block';
            }
            return false;
        }
    }
</script>
<div class="content-grid">
    <div class="content-grid-item">
        <input type="button" class="button" style="width: 100%;" value="Records" onClick="showHideDiv('log-music')"/>
        <div id="log-music" style="display: none;">
            {% for album in site.data.albums limit:25 %}
            <p>
                {% if album.rating > "7" %}
                <img class="log-icon" src="images/vinyl-fav.svg"><b>{{ album.title }} [{{ album.year }}]</b><br />
                {{ album.artist }}{% else %}
                <img class="log-icon" src="images/vinyl.svg">{{ album.title }} [{{ album.year }}]<br />
                {{ album.artist }}
                {% endif %}
            </p>
            {% endfor %}
            <a href="/music"><button class="button-alt" style="margin-bottom:20px;">View All Records</button></a>
        </div>
    </div>
    <div class="content-grid-item">
        <input type="button" class="button" style="width: 100%;" value="Films & TV" onClick="showHideDiv('log-films')"/>
        <div id="log-films" style="display: none;">
            {% for film in site.data.films limit:25 %}
            <p>
            {% if film.tv == "1" %}<img class="log-icon" src="images/tv.svg">{% elsif film.rating > "3.5" %}
            <img class="log-icon" src="images/cinema-fav.svg"><b>{{ film.name }} [{{ film.year }}]</b>{% else %}<img class="log-icon" src="images/cinema.svg">{{ film.name }} [{{ film.year }}]{% endif %}<br />
            {{ film.date }}</p>
            {% endfor %}
            <a href="/films"><button class="button-alt" style="margin-bottom:20px;">View All Films</button></a>
        </div>
    </div>
    <div class="content-grid-item">
       <input type="button" class="button" style="width: 100%;" value="Books" onClick="showHideDiv('log-books')"/>
        <div id="log-books" style="display: none;">
            {% for book in site.data.books limit:25 %}
            <p>
                {% if book.rating > "4" %}
                <span><i class="fas fa-bookmark"></i></span><b>{{ book.name }}</b><br />
                {{ book.author }}{% else %}
                <span><i class="far fa-bookmark"></i></span>{{ book.name }}<br />
                {{ book.author }}
                {% endif %} 
            </p>
            {% endfor %}
            <a href="/books"><button class="button-alt" style="margin-bottom:20px;">View All Books</button></a>
        </div>    
    </div>
</div>
<a href="/timeline"><button class="button-alt" style="width: 100%;">Back to Timeline</button></a>