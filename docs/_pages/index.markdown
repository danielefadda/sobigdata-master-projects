---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "Home"
show_sidetoc: true
subtitle: "LBDAI - SoBigData Master course"
header_type: base #base, post, hero,image, splash
header_img: assets/images/header.svg
header_title: "SoBigData Master projects"
---

<div class="container py-1">
<div class="row">
        <div class="col-md-12">
            <p class="lead" style="text-align:justify">The SoBigData Master projects aim to teach students how to observe and represent phenomena from various perspectives, drawing on the knowledge gained from different master's courses: from data collection to the final delivery. The students will employ in the project methods, techniques and tools studied in the other modules. The duration of this module, differently from the others, will span across several months until the end of the lectures when the results of the project will be presented in front of a committee.</p>
        </div>
    </div>
</div>

<div class="container py-3" id="projects-container">
    <a href="{{site.baseurl}}/2025.html">
        <div class="row py-3 my-3 project">
                <div class="col-md-4" >
                    <div class="project-img"><img src="{{site.baseurl}}/assets/images/g1_videogame.png" alt="2025"></div>
                </div>
                <div class="col-md-8">
                    <h2>YEAR 2025</h2>
                    <p class="students">
                        <strong>Teachers:</strong> Roberto Trasarti, Anna Monreale, Riccardo Guidotti, Daniele Fadda
                    </p>
                </div>
        </div>
    </a>
</div>

<div class="container py-3" id="projects-container">
    <a href="{{site.baseurl}}/2024.html">
        <div class="row py-3 my-3 project">
                <div class="col-md-4" >
                    <div class="project-img"><img src="{{site.baseurl}}/assets/images/g1_spot_tv.png" alt="2024"></div>
                </div>
                <div class="col-md-8">
                    <h2>YEAR 2024</h2>
                    <p class="students">
                        <strong>Teachers:</strong> Roberto Trasarti, Anna Monreale, Riccardo Guidotti, Paolo Ferragina, Daniele Fadda
                    </p>
                </div>
        </div>
    </a>
</div>

---

### Search for projects

{% include search-lunr.html %}