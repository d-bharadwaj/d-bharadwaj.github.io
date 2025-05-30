---
Title:  My classes as a Physics major
Date: 2025-01-30 
Category: personal 
thumbnail: "images/bloch.png"
Summary: >
  A page listing my coursework at UW-Madison.  
---


In college, I majored in Physics but mixed it up with some CS courses through my Data Science minor. I designed my coursework to build up the technical skills I’d need for research and SWE internships. I liked the interesection of Physics and CS so it made perfect sense to keep that momentum going into the research I’m working on now.

**MATH 321** (Vector & Complex Analysis) and **ART 100** (Introduction to Art) were my top picks. MATH 321 was tough ([apparently](https://www.reddit.com/r/UWMadison/comments/zxrr8q/what_is_the_hardest_class_youve_taken_at_uw/) the hardest course @ Wisconsin) but rewarding, deepening my understanding of linear algebra. ART 100 was quite fun, especially since I took it with my best friend. We explored museums and concerts, which made the course engaging and memorable.

!TEMPLATE!
{% set schedule = [
    [
        ("Fall 2020", [
            ("MATH 221", "Calculus & Analytic Geometry 1"),
            ("ECON 100", "Economics for Non-Majors"),
            ("ASTRON 104", "Our Exploration of the Solar System"),
            ("INTER-LS 250 ", "Required for Undergraduate Research Scholars Program")

        ]),
        ("Spring 2021", [
            ("PHY 207", "General Physics 1"),
            ("CS 220", "Data Science Programming 1"),
            ("MATH 222", "Calculus & Analytic Geometry 2"),
            ("LIT TRANS 275", "The Tales of Hans Christian Andersen"),
            ("INTER-LS 250", "Required for Undergraduate Research Scholars Program")
        ]),
    ],
    [
        ("Fall 2021", [
            ("PHY 208", "General Physics 2"),
            ("MATH 234", "Multivariable Calculus "),
            ("ART 100", "Introduction to Art"),
            ("LIS 202", "Informational Divides & Differences in a Multicultural Society"),
            ("EMA 599", "Supervised Research"),    
            ]),

        ("Spring 2022", [
            ("PHY 241", "Introduction to Modern Physics"),
            ("PHY 307", "Laboratory for Modern Physics"),
            ("MATH 320", "Linear Algebra & Differential Equations"),
            ("LIS 461", "Data & Algorithms: Ethics & Policy"),
            ("RPSE 100", "Disability & Society"),
            ("EMA 599", "Supervised Research")
        ]),
    ],
    [       
        ("Fall 2022", [
            ("PHY 311", "Classical Mechanics"),
            ("CS 320", "Data Science Programming 2"),
            ("STAT 240", "Data Science Modeling 1"),
            ("ENGL 153", "Literature & the Environment"),
            ("EMA 599", "Supervised Research"),    
            ]),

        ("Spring 2023", [
            ("PHY 322", "Electromagnetic Fields"),
            ("MATH 321", "Applied Vector & Complex Analysis"),
            ("PHY 325", " Classical & Modern Optics"),
            ("LIS 351", "Introduction to Digital Information"),
            ("EMA 599", "Supervised Research")
        ]),
    ],
    [       
        ("Fall 2023", [
            ("PHY 448", "Quantum Mechanics 1"),
            ("CS 532", "Matrix Methods in Machine Learning"),
            ("BIOCHEM 104", "Molecules to Life & Nature of Science"),
            ("EMA 599", "Supervised Research"),    
            ]),

        ("Spring 2024", [
            ("PHY 449", "Quantum Mechanics 2"),
            ("PHY 415", "Thermal Physics"),
            ("PHY 407", "Advanced Laboratory in Modern Physics"),
            ("INTER-LS 260", "Required research credits for Hilldale Fellowship")
        ]),
    ]
] 
%}

{%- for year in schedule -%}
<div class="row">
    {%- for term in year -%}
    <div class="col-sm-12 col-md-6 d-md-flex-row p-2 align-items-stretch">
        <div class="card">
        <div class="card-body">
            <h5 class="card-title">{{ term[0] }}</h5>
            <table class="table mb-0">
                {% for course in term[1] %}
                <tr>
                    <td><b>{{ course[0]}}</b>&nbsp;&nbsp;&nbsp;<div style="font-size:13px">{{ course[1] }}</div></td>
                </tr>
                {%- endfor -%}
            </table>
        </div>
        </div>
    </div>
    {%- endfor -%}
</div>
{% endfor %}

!TEMPLATE!