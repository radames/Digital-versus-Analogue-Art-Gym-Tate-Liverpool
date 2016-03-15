##How to get your Instagram App and Access token

###The easy way
1. Go to http://instagram.pixelunion.net/
2. Then Generate Access Token

###The medium

1. Go to https://apigee.com/embed/console/instagram
2. Click on the dropdown list **Authentication** and select **OAuth 2**
![](https://cloud.githubusercontent.com/assets/102277/13771339/e6ce6552-ea84-11e5-80c3-a358ccc2c17a.png)
3. Login in on Instagram account and give access to the app
![](https://cloud.githubusercontent.com/assets/102277/13771338/e6c97ef2-ea84-11e5-8f4f-5dbd6102f91a.png)
4. **Request URL GET** and type `tag` then **SEND**
![](https://cloud.githubusercontent.com/assets/102277/13771336/e6beec3a-ea84-11e5-8934-e2223f31b79c.png)
5. You'll see the your access token in the Request Box



###The hard way
1. Create an Developer account [Developers at Instagram](https://www.instagram.com/developer/)
2. **Register new Client**

![](https://cloud.githubusercontent.com/assets/102277/13771337/e6bf8ece-ea84-11e5-95ce-e327e5fca0a5.png)

3. You need an **Application Name** and a **Description**
4. For **Website URL** and **Valid redirect URIs** you can use your website, don't forget to put **http or https**, if you don't have a website you can use **https://www.example.com**

![](https://cloud.githubusercontent.com/assets/102277/13771335/e6be9636-ea84-11e5-8af4-ef64f4b03d1f.png)

5. In the tab **Security** toggle off the option **Disable implicit OAuth**

![](https://cloud.githubusercontent.com/assets/102277/13771334/e6bced22-ea84-11e5-9d1c-4dda5469f091.png)

6. Now you have your **Client ID** go to the following website replacing **CLIENT-ID** with the your sequence, and **REDIRECT-URI** with your valid URIs website

https://api.instagram.com/oauth/authorize/?client_id=CLIENT-ID&redirect_uri=REDIRECT-URI&response_type=token
![](https://cloud.githubusercontent.com/assets/102277/13771333/e6bc1960-ea84-11e5-9a29-b3d7733b03e5.png)

  
7. Authorize with your Instagram Account then you'll be redirect to the **REDIRECT-URI** address you put on your app

![](https://cloud.githubusercontent.com/assets/102277/13771332/e6b04ef0-ea84-11e5-8273-9d8d1d3a2dc4.png)

8. You Access token will be as a parameter in the address bar, save that sequence. **#access_token=YOUR_ACCESS_TOKEN**

![](https://cloud.githubusercontent.com/assets/102277/13771331/e69be604-ea84-11e5-9d9a-701409641bca.png)


###Revoking acesss

You can revoke apps access anytime going to https://www.instagram.com/accounts/manage_access/
