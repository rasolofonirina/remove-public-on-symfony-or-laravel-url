# Remove "public" on Symfony or Laravel URL

EN : When you create your website or web application with the Symfony or Laravel framework and deploy it on shared hosting, the access address becomes `http(s)://example.com/public`.<br>
To remove the `public` from URLs you can add these instructions to the `.htaccess` file at the root of the site.`<br>

FR : Lorsque vous créez votre site ou application web avec le framework Symfony ou Laravel et le déployez sur un hébergement mutualisé, l'adresse d'accès devient `http(s)://example.com/public`.<br>
Pour enlever le `public` sur les URLs vous pouvez ajouter ces instructions sur le fichier `.htaccess` à la racine du site.<br>

```
RewriteEngine On
RewriteCond %{REQUEST_URI} !^/public/
RewriteRule ^(.*)$ /public/$1 [L,QSA]
```
<br>
<br>
<p align="center">
<a href="https://www.buymeacoffee.com/rasolofonirina"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=rasolofonirina&button_colour=BD5FFF&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00" /></a>
</p>
