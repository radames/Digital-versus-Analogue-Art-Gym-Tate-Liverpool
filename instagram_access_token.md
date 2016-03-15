##How to get your Instagram App and Access token

###The easy way
1. Go to http://instagram.pixelunion.net/
2. Then Generate Access Token

###The medium

1. Go to https://apigee.com/embed/console/instagram
2. Click on the dropdown list **Authentication** and select **OAuth 2**
3. Login in on Instagram account and give access to the app
4. **Request URL GET** and type `tag` then **SEND**
5. You'll see the your access token in the Request Box



###The hard way
1. Create an Developer account [Developers at Instagram](https://www.instagram.com/developer/)
2. **Register new Client**
3. You need an **Application Name** and a **Description**
4. For **Website URL** and **Valid redirect URIs** you can use your website, don't forget to put **http or https**, if you don't have a website you can use **https://www.example.com**
5. In the tab **Security** toggle off the option **Disable implicit OAuth**
6. Now you have your **Client ID** go to the folloe website replacing **CLIENT-ID** with the your sequence, and **REDIRECT-URI** with your valid URIs website
https://api.instagram.com/oauth/authorize/?client_id=CLIENT-ID&redirect_uri=REDIRECT-URI&response_type=token
  
7. Authorize with your Instagram Account then you'll be redirect to the **REDIRECT-URI** address you put on your app
8. You Access token will be as a parameter in the address bar, save that sequence. **#access_token=YOUR_ACCESS_TOKEN**



###Revoking acesss

You can revoke apps access anytime going to https://www.instagram.com/accounts/manage_access/
