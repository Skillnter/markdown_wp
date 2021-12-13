# Public

This section contains all the public-facing functionality.

## Folder Structure

- `css`  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - Contains all the style sheets available in the public section.
- `js` &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - Contains all the script files available in the public section.
- `partials` &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - Contains all the view files available in the public section.
- `check.json` &nbsp; &nbsp; &nbsp; &nbsp;- Contain the ZOHO tokens.
- `kyc_submit.php` - AJAX to send selected package details.

## Javascript 

- **submit_package.js** : Send the selected package or not interested information to the backend.
- **logout.js** : Logout user on closing of the website (all tabs or redirected to other website).
- **test.js** : Update, check and validate forms. Also, Autocheck radios buttons and Autoselect select options.

## PHP

- **aqugen_startSession** : Start PHP session.
- **replace_string** : Replace string on the RESEND OTP text with the anchor tag.
- **replace_wrong_test** : Replace string on the WRONG NUMBER text with the anchor tag.
- **replace_POST_variable** : Replace placeholders with POST variable values.
- **replace_dynamic_variable** : Replace placeholders with the provided variable object values.
- **replace_pipes_variable** : Replace pipe placeholders with pipe functions values. e.g, `split`.
- **replace_variable** : Replace placeholders with the provided object values.
- **add_form_onsubmit** : Add submit button to form.
- **Request_GET** : Wrapper for WordPress GET request.
- **Request_POST** : Wrapper for WordPress POST request.
- **get_json_from_query** : Convert query variables to json object.
- **console_log** : Log the message in the browser console.
- **testt_Demo** : Generate the form dynamically by taking form id from the shortcode variable and return the form.
- **send_otp** : Fetch `sms` configurations from the form and send the OTP on the provided number.
- **resend_otp** : Fetch `sms` configurations from the form and resend the OTP on the provided number.
- **verify_otp** : Fetch `sms` configurations from the form, verify the OTP on the provided number and update the `entries` table.
- **wrong_number** : Clear the session data.
- **business_input** : Update the `entries` table for the business entries.
- **str_replace_first** : Replace the first occurence of the subject in the string.
- **generateRandomString** : Generate random string of specified length. By default it use length of 10.
- **throwException** : Throw exception with provided message.
- **check_logout** : Logout user.
- **hook_logout** : Hook to register logout.
- **check_query_parameters** : Check the query pan, gst & iec parameters.
- **count_query_parameters** : Count the query pan, gst & iec parameters
- **packages** : Load the service provider packages section.
- **filter_array_combo** : Filter the service provider combo packages.
- **filter_array_gst** : Filter the service provider gst packages.
- **filter_array_pan** : Filter the service provider pan packages.
- **filter_array_iec** : Filter the service provider iec packages.
- **check_send_package** : AJAX call to send the service provider packages to the backend.
- **hook_send_package** : Hook to register AJAX call to send the service provider packages to the backend.
- **get_token** : Wrapper for WordPress POST request to return json body for ZOHO token API.
- **insert_lead** : Wrapper for WordPress POST request to return json body for ZOHO Insert API.
- **query_to_array** : Convert query string to associative array.
- **update_access_token** : Update the ZOHO token to json file.
- **footer_link** : Generate footer link HTML for shortcode.
- **erase_user_data** : Generate GDPR section for shortcode.
- **erase_mobile_otp** : Fetch `sms` configurations from the form and send the OTP on the provided number.
- **erase_mobile_verify** : Fetch `sms` configurations from the form and verify the OTP on the provided number.
- **delete_data** : Delete the user data from the `entries` & `lead` table and update the `delete` table.
