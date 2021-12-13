# wordpres_plugin

The goal of this project is to save & build dynamic forms for client KYC, then process the data using APIs from ZOHO, VOXOMOS, and VENDOR.

- The boilerplate is generated with [WordPress Plugin Boilerplate]

# Installation

### Upload

- Login to your WordPress Dashboard.
- In your WordPress Admin Menu, go to **Plugins** > **Add New**.
- Click on Upload Plugin button found on top left corner of page.
- Click on Browse, Select the `.zip` file of your plugin in your computer, and click **Install Now** button.

### FTP
- Log in to your **FTP** service.
- Add the plugin folder to the folder labeled `wp-content/plugins` folder in your WordPress directory.
- Go to WordPress admin area and click on the **Plugins**
- Click on the **Activate** link below the plugin to start using it.


# Notes

### Updated `class-plugin-name-loader.php` to incorporate shortcodes.

- Private variable `$shortcodes` added.
- `__construct()` is updated to initial `$shortcodes` also with empty array.
- Added a new function to register shortcodes `add_shortcode`.
- Updated `run()` function to incorporate `$shortcodes`.

## Application Structure

- `includes/class-plugin-name.php` - Register all of the hooks related to the public/admin-facing functionality.
- `installer.php` &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;- If the tables do not exist when the application is activated, it will construct them; otherwise, it will check the version and make the necessary changes to the table.

- [`admin/`] &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp; &nbsp;- This folder will include views and actions that will be done inside WordPress Admin.
- [`public/`] &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp;- This folder will include views and actions that will be done on the public website.



[WordPress Plugin Boilerplate]:https://wppb.me/
[`admin/`]: /admin.md
[`public/`]: /public.md
