# drf-editable

A django app for integrating django rest framework into js

## Install via pip

    pip install git+https://github.com/raiderrobert/drf-vue-editable/
    
## Add to installed apps
    INSTALLED_APPS = [
        ...
        'drf_editable',
    ]
    
    
## Load the css_grid library and place the template tags appropriately
    # polls/templates/polls/list.html
    {% load drfe %}
    <!DOCTYPE html>

    <html>
        <head>
            <title>Hello World!</title>
            <meta charset="utf-8">
            {% drfe_js %}
        </head>
        <body>
            {% drfe resource='rest_framework:polls:list' %}
        </body>
    </html>
