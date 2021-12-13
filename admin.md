# Admin

This section contains all the admin-facing functionality.

## Folder Structure

- `css`  &nbsp;  &nbsp;  &nbsp;  &nbsp; - Contains all the style sheets available in the admin section.
- `images` &nbsp;  &nbsp;- Contains all the images available in the admin section.
- `js` &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  - Contains all the script files available in the admin section.
- `partials` - Contains all the view files available in the admin section.

## Javascript 

- **replace_ITI** : Check if form name already exist.
- **open_popup** : Open popup and set `data-id`.
- **close_popup** : Close popup and remove `data-id`.
- **delete_form** : Delete form and remove `data-id`.
- **delete_provider** : Delete Service provider and remove `data-id`.
- **delete_package** : Delete Service packages and remove `data-id`.
- **delete_api** : Delete Service provider API and remove `data-id`.
- **check_required** : Check the required API fields.
- **subsections_required** : Check the required subsections of API fields.
- **check_if_valid** : Check if the API fields are valid.
- **check_if_HTML_verified** : Check to verify the initial format of the HTML.
- **admin_autochecked** : Automatically check the checkboxes in the admin section forms.
- **change_display_post_body** : Toggle the visibility of POST TYPE request body on type change.
- **form_error** : Log form errors in console.
- **update_refresh** : Event listener for change event.
- **changeRefresh** : Toggle REFRESH TYPE form fields.

## PHP

- **test_plugin_setup_menu** : Setup menu section.
- **remove_submenu_list** : Remove submenu list from the menu section.
- **load_admin_page_placeholder** : Load placeholder page.
- **load_admin_page_content** : Load form list page.
- **load_admin_page_add** : Load form add page.
- **load_admin_page_edit** : Load form edit page and require form id as query parameter to access.
- **load_admin_page_help** : Load help section page.
- **load_admin_page_provider** : Load service provider list page.
- **load_admin_provider_add** : Load service provider add page.
- **load_admin_provider_edit** : Load service provider edit page.
- **load_admin_page_package** : Load packages list page.
- **load_admin_package_add** : Load packages add page.
- **load_admin_package_edit** : Load packages edit page.
- **load_admin_page_api** : Load service provider API list page.
- **load_admin_api_add** : Load service provider add API page.
- **load_admin_api_edit** : Load service provider edit API page.
- **load_whatspp_key** : Load whatsapp section page.
- **load_whatspp_bot_add** : Load VOXOMOS Whatsapp Bot Configuration page.
- **add_form** : Format the entered data and insert into forms table.
- **add_provider** : Add provider name to the provider table.
- **edit_provider** : Edit provider name in the provider table.
- **add_package** : Add package details to the package table.
- **edit_package** : Edit package details in the package table.
- **add_api** : Add provider APIs to the API table.
- **edit_api** : Edit provider APIs in the API table.
- **update_form** : Edit form configurations in the form table.
- **check_validator_ajax** : AJAX call to check for the form name.
- **hook_validator_ajax** : Hook to register AJAX call to check for the form name.
- **check_form_delete_ajax** : AJAX call to delete form.
- **hook_form_delete_ajax** : Hook to register AJAX call to delete form.
- **check_provider_delete_ajax** : AJAX call to delete service provider.
- **hook_provider_delete_ajax** : Hook to register AJAX call to delete service provider.
- **check_api_delete_ajax** : AJAX call to delete service provider APIs.
- **hook_api_delete_ajax** : Hook to register AJAX call to delete service provider APIs.
- **check_package_delete_ajax** : AJAX call to delete service provider packages.
- **hook_package_delete_ajax** : Hook to register AJAX call to delete service provider packages.
- **encrypt_decrypt** : Encrypt and decrypt strings using `sha256`.
- **generate_key** : Generate API keys.
- **whatsapp_web_webhook** : Register API Endpoint for whatsapp to capture feeds provider by Voxomos team.
- **replace_dynamic_variable** : Replaces the placeholders with the provided variable object values.
- **whatsapp_feed** : Process the feed provided by the Voxomos team to match the data and update lead and entries table.
- **getPrefix** : Matches the questions and get the table column name.
- **aq_whatsapp_wp_cron** : Set a cron to run the Voxomos API to feed Whatsapp Bot configurations and data at a specific time regularly.
- **aq_whatsapp_run_now_wp_cron** : Set a cron to one time run the Voxomos API to feed Whatsapp Bot configurations and data at the current time.
