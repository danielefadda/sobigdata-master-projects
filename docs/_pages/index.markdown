---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "Home"
show_sidetoc: true
subtitle: "LBDAI - SoBigData Master course 2024"
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
        {% for image in site.data.home-cards %}
            <a href="{{image.path}}" target="_blank">
                <div class="row py-3 my-3 project" >
                        <div class="col-md-4">
                            <div class="project-img"><img src="{{site.baseurl}}{{ image.img_url}}" alt="{{ image.name }}" style="width:100%"></div>
                        </div>
                        <div class="col-md-8">
                            <div class="project-body">
                                <h5>{{ image.group }}. {{ image.name }}</h5>
                                <p>{{ image.description }}</p>
                                {% assign students = image.students | split: "," %}
                                <p class="students">

                                <em><strong>Students</strong>:
                                    {% for student in students %}
                                        {% if forloop.last %}
                                            <span>{{ student | strip |  replace: '[', ''  |  replace: ']', '' |  replace: '"', '' }}.</span>
                                        {% else %}
                                            <span>{{ student | strip |  replace: '[', ''  |  replace: ']', '' |  replace: '"', '' }}, </span>
                                        {% endif %}
                                    {% endfor %}
                                </em></p>
                            </div>
                        </div>
                </div>
            </a>
        {% endfor %}
</div>


<div class="container py-1">
    <div class="row">
        <div class="col-md-12">
            <hr>
            <h3>Courses involved</h3>
            <ul>
                <li>BDSCCS – Big Data Sources, crowdsourcing, crowdsensing</li>
                <li>DMML – Data Mining and Machine Learning</li>
                <li>IR – Information Retrieval</li>
                <li>DDI – Data Driven Innovation</li>
                <li>DVDJ – Data Visualization and Data Journalism</li>
                <li>TAWM – Text Analysis & Web Mining</li>
            </ul>
        </div>
    </div>
</div>