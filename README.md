> This is my assignment for Week 4 - My Portfolio 

# Connecting your domain to Cloudflare and deploying to Netlify: A Tutorial

In this tutorial, I will guide you through the process of connecting your domain to Cloudflare and deploying your website to Netlify. By the end of this tutorial, you will have a website that is fast, secure, and scalable.

## Step 1: Sign up for Cloudflare

To start, go to the Cloudflare website and [Sign Up](http://dash.cloudflare.com/sign-up) for a free account. After signing up, add your domain to Cloudflare by following the on-screen instructions.

### add your domain to Cloudflare

Enter the domain name you want to set up, click Add site to continue.
![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675725561/wee4-revou/homepage-cloudflare_vg1ek3.png "Logo Title Text 1")

On the next page, select a package that fits your domain needs. For this tutorial, I use the Free Plan only, then click the Confirm Plan button
![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675729193/wee4-revou/freeplan_bjmvbn.png "Logo Title Text 1")

## Step 2: Change your nameservers

Next, you will need to change your domain’s nameservers to Cloudflare’s. This is done through your domain registrar’s website. The process for doing this will vary depending on the registrar you use, but you should be able to find instructions by searching for “change nameservers on [registrar name]". For this tutorial, we will use *JagoanHosting* as an example.

### Nameservers Configuration

Change your domain nameserver to match the nameserver provided by Cloudflare. For example, like the picture shown below.

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675728504/wee4-revou/Cloudflare_nameserver_uifbu9.png "Logo Title Text 1")

Go to the Jagoanhosting member area, click on the Domains section and select your domain name. Then, click the three dots and choose Manage Domain.

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675727532/wee4-revou/manage_domain_dmdbwz.png "Logo Title Text 1")

Next, in the Setting NS (Nameservers) tab, change the nameserver to match the nameserver provided by Cloudflare, and then click Change Nameserver to save the changes.
![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675728228/wee4-revou/configure_name_server_eou7an.png "Logo Title Text 1")

## Step 3: Sign up for Netlify

Next, go to the Netlify website and sign up for a free account.

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675738866/wee4-revou/signup-netlify_yyxv2q.png "Logo Title Text 1")

Once you have signed up, create a new site by connecting your Git repository or uploading your website files. For this tutorial, I will use the Git repository option.
![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675741599/wee4-revou/import_git_echfvg.png "Logo Title Text 1")

On this page, you can adjust your settings. Ensure that your publish directory is the location where your public site files will be stored after building, and your build command is the command you run to build the site (e.g. npm run build). Once you have confirmed these details, click the Deploy Site button to proceed.

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675742129/wee4-revou/site-settings_nkrwm9.png "Logo Title Text 1")

## Step 4: Deploy your website

Finally, deploy your website to Netlify. Netlify will automatically build and deploy your website each time you push changes to your Git repository or upload updated files.

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675742275/wee4-revou/deploy_site_xov1qv.png "Logo Title Text 1")

## Step 5: Connect your Cloudflare to Netlify

For the next step, you will need to configure it to work with your website hosted on Netlify. Start by going to the “DNS” section of the Cloudflare dashboard and adding CNAME records for your domain. The specific records you will need will depend on your setup, but you should be able to find examples by searching for “Cloudflare DNS records for Netlify.”

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675753576/wee4-revou/add_cname_2_wkj34z.png "Logo Title Text 1")

In the “Custom domains” tab, add your new custom domain name to Netlify by following the on-screen instructions.

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675753280/wee4-revou/add_custom_domain_seu5qz.png "Logo Title Text 1")
![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675753036/wee4-revou/add_custom_domain_in_netlify_hspghb.png "Logo Title Text 1")

## Step 6: Verify the connection

Finally, verify that the connection between your custom domain and Netlify is working properly by visiting your website through your new custom domain name. If everything is working correctly, you should see your website.

![Cloudflare homepage](https://res.cloudinary.com/djudfrj8s/image/upload/v1675780283/wee4-revou/verify_domain_w5dv2o.png "Logo Title Text 1")

That’s it! By following these steps, you will have successfully connected your domain to Cloudflare and deployed your website to Netlify. Your website will now be secure and scalable, giving you the confidence to grow your online presence.

**Visit My Website:** https://generalist.my.id 

---

_Disclaimer: Using both Cloudflare's CDN and Netlify at the same time for one site is not recommended by either company. Netlify's web service works best without an additional CDN in front of it. Proxying through Netlify is not supported and may not give the best results. Cloudflare also does not recommend this setup. [Source](https://answers.netlify.com/t/how-do-i-use-cloudflare-dns-with-a-netlify-custom-domain/1557)_
