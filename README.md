# ID.me jQuery Sample Code #

This is jQuery sample code to make API requests with ID.me using OAuth 2.0.

## Setup ##

In order to run the example you need to include `jquery` and ID.me's JavaScript dependencies in your application.

### jQuery Dependency ###

```html
<script type="text/javascript" src="https://code.jquery.com/jquery-3.2.0.min.js"></script>
```

### ID.me Dependency ###

```html
<script src="https://s3.amazonaws.com/idme/developer/idme-buttons-2.0.1/assets/js/idme-modal.min.js" type="text/javascript"></script>
```

### Include Sample Code ###

Include `idme.js` in your application after the required dependencies.

### Use ID.me Button Code Generator ###

Utilize the button code generator available in your Application dashboard at [https://developer.id.me](http://developer.id.me).

Be sure your button code is updated with the correct parameters:

  * data-scope=`military`, `responder`, `student`, `teacher`, and/or `government`
    * A parameter that defines the group affiliation you are requesting permission to access.
  * data-client-id=`YOUR_CLIENT_ID`
    * The client identifier received during app registration. It is automatically generated and located in your application dashboard.
  * data-redirect=`YOUR_REDIRECT_URI`
    * Where the user gets redirected after authorizing an application. Set by the developer within the application dashboard.
  * data-response=`code` or `token`
    * The client informs the authorization server of the desired grant type with this parameter.
  * data-op=`signin` or `signup`
    * A parameter that determines which experience, sign-in or sign-up, a user will encounter upon entering ID.me.
  * data-text=`OFFER_DESCRIPTION_TEXT`
    * A custom recommended parameter used to display the offer description within the ID.me Button Widget.
  * data-display=`popup` or `link`
    * A parameter to determine whether a flow will use a full-page redirect or a pop-up. Defaults to `link`
  * data-show-verify=`true` or `false`
    * A parameter that allows the client to display the "Verification by ID.me" text. Defaults to `true`

### Testing the sample code ###

In order to test the sample code you need to start a server. We suggest doing the following:

1. Install [node](https://docs.npmjs.com/getting-started/installing-node)
2. Run `npm install -g serve`
3. Run `serve -p 3000` in the directory of the sample code.

Go to `http://localhost:3000` and you'll see the app running.
