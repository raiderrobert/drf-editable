# drf-editable

A django app for integrating django rest framework into js

## Install via pip

    pip install git+https://github.com/raiderrobert/drf-vue-editable/
    
## Add to installed apps
    INSTALLED_APPS = [
        ...
        'drf_editable',
    ]
    
    
## Load the drf_edtiable library and place the template tags appropriately
    # some_html.html
    {% load drfe %}
    <!DOCTYPE html>

    <html>
        <head>
            <title>Hello World!</title>
            <meta charset="utf-8">
            {% drfe_js %}
        </head>
        <body>
            {% drfe resource='rest_framework:polls:detail' action='PATCH' %}
        </body>
    </html>
