# Documentation for ${{values.app_name}}

This application has two endpoints:
- `api/v1/info`
- `api/v1/details`

# How to access the app

You can access the application by going to: 

{%- if values.app_env == 'prod' %}
    * `${{ values.app_name }}.test.com/api/v1/info`
{%- else %}
    * `${{ values.app_name }}-${{ values.app_env }}.test.com/api/v1/info`
{%- endif %}
