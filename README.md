# drf-vue-editable

A django app for integrating django rest framework into vue.js

## Install via pip

    pip install git+https://github.com/raiderrobert/drf-vue-editable/
    
## Add to installed apps
    INSTALLED_APPS = [
        ...
        'drf_vue_editable',
    ]
    
    
## Load the css_grid library and place the template tags appropriately
    # polls/templates/polls/list.html
    {% load drf_vue %}
    <!DOCTYPE html>

    <html>
        <head>
            <title>Hello World!</title>
            <meta charset="utf-8">
            <script src="http://unpkg.com/vue/dist/vue.js"></script>
            <script src="http://cdn.jsdelivr.net/vue.resource/1.3.0/vue-resource.min.js"></script>
        </head>
        <body>
            {% drf_vue resource='rest_framework:polls:list' %}
        </body>
    </html>
