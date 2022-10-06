# REQUIREMENTS
1. PHP >= 7.4
2. console access

# PARAMETERS
1. `baseURL`: Mandatory! The base url of your website (i.e. `'https://mywebsite.com'`)
2. `targetDir`: Optional! The directory which you're going to scan relative to the execution folder (i.e. `plugins`). Default if omitted: `plugins` 
3. `downloadBasePath`: Optional! The directory where the fonts will be downloaded to, relative to your execution folder. Make sure this is part of the public facing folder structure! (i.e. `'uploads/font-cache'`). Default if omitted: `wp-content/uploads/font-cache`. 
4. `basePath`: Optional! Only needed if the `downloadBasePath` is not relative to the current execution directory or parts of the path would not be public facing (i.e. `public`). Default if omitted: `` (empty).

# USAGE
1. copy the script somewhere you know (i.e. `~/bin` or the application's webroot)
2. `chmod +x gfontreplacer.php` 
3. execution with at least first parameter (the BaseURL). like `php gfontreplacer.php 'https://mywebsite.com` or `php gfontreplacer.php 'https://mywebsite.com' plugins 'uploads/font-cache' public`