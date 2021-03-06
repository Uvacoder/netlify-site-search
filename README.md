<h1> Netlify Site Search
<a href="https://app.netlify.com/start/deploy?repository=https://github.com/davidwells/netlify-site-search">
  <img align="right" src="https://camo.githubusercontent.com/be2eb66bb727e25655f1dcff88c2fdca82a77513/68747470733a2f2f7777772e6e65746c6966792e636f6d2f696d672f6465706c6f792f627574746f6e2e737667" class="deploy-button" alt="deploy to netlify">
</a>
<a href='https://app.netlify.com/sites/netlify-site-search
/deploys'><img align="right" src='https://api.netlify.com/api/v1/badges/6545ecf6-4540-477d-8655-c4771b2fa027/deploy-status'/></a>
</h1>

Better Netlify site search UI. [Demo](https://twitter.com/i/status/1104099114608816128)

🌪 Filter by: 

- Last published
- Site creation date
- Team
- Function count
- Repo url

Man detective Search by:

- Site name
- Site url
- Repo
- Site ID

## How it works

![Netlify OAuth + Functions](https://user-images.githubusercontent.com/532272/54178445-106c0600-4453-11e9-998f-564a521dfc6b.png)

## Setup

1. **Create and Deploy a new Netlify site**

    You can use an [this repo](https://app.netlify.com/start/deploy?repository=https://github.com/davidwells/netlify-site-search)

2. **[Create OAuth application](https://app.netlify.com/account/applications)**

    Create your OAuth application in the Netlify admin UI.

    Add in your callback URL. This can be changed later.

    ![image](https://user-images.githubusercontent.com/532272/53382433-3066da00-3929-11e9-978a-74d802c212db.png)

3. **After creating your OAuth app, Click on show credentials**

    Save these credentials for the next step

    ![image](https://user-images.githubusercontent.com/532272/53382437-3957ab80-3929-11e9-9cbf-b812cd04c2c7.png)

4. **Take your OAuth credentials and add them to your OAuth app site**

    Set `NETLIFY_OAUTH_CLIENT_ID` and `NETLIFY_OAUTH_CLIENT_SECRET` environment variables in your site

    ![image](https://user-images.githubusercontent.com/532272/53382472-53918980-3929-11e9-9d24-598247b5f2c6.png)

5. **Then trigger a new deploy**

    ![image](https://user-images.githubusercontent.com/532272/53382490-6015e200-3929-11e9-9f6b-92be59d78e59.png)


6. **Visit your site and verify the OAuth flow is working**