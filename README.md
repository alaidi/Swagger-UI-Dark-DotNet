# Swagger UI Dark
Customize the UI
The default UI is both functional and presentable. However, API documentation pages should represent your brand or theme. Branding the Swashbuckle components requires adding the resources to serve static files and building the folder structure to host those files.

## Enable Static File Middleware:
```
app.UseStaticFiles();
```
## To inject CSS stylesheets
add css file to the project's `wwwroot` folder and specify the relative path in the middleware options:

```
 app.UseSwaggerUI(options =>
    {
        options.InjectStylesheet("/assets/swagger_ui_dark.css");
    });
```

![Alt text](dark.png?raw=true "swagger dark theme ")
