---
title: "Creating Your Site"
date: 2025-09-28
weight: 3
---

#### Creating Your First Site
Now we have our local development environment ready to go, let's create our first site!
{{< tabs groupid="a" >}}
{{% tab title="_**MacOS**_" %}}
 - Search for 'Herd' in Spotlight or Finder, and open the application.
 - Click the **Let's Get Started** button. If this is the first time you have opened Herd, a bunch of things will likely install in the background. Accept any prompts until setup is complete.
 - Open the Herd Dashboard once setup has completed.
 
 **Important Note:**  
 If prompted to enter a license key for Herd Pro, choose **Skip for now**. You do not need Herd Pro!

![Screenshot of Skip for Now button to bypass Herd Pro prompt](images/HerdProOptionSkipForNow.png)

 - On the left hand side, choose **Sites**
 - If prompted to choose a sites folder, we recommend using the default folder recommended by Herd.
 - Click the **Add Site** button.

![Screenshot of Laravel Herd showing the button to Add Site](images/HerdDashboardAddSite.png)

- Choose **New Laravel Project**
- Choose **Livewire** as your starter kit
- Enter details as per the below screenshot:

<!-- Kate to add screenshot - copy details from Windows -->
![Screenshot of new site details - Mac](images/NewLaravelProjectDetails-Mac.png)

- Once the site creation is complete, click **Open in Browser** to view the home page of your new site!

{{% /tab %}}
{{% tab title="_**Windows**_" %}}
 - Open Laravel Herd from the Start menu
 - Click the **Let's Get Started** button. If this is the first time you have opened Herd, a bunch of things will likely install in the background. 
 - If prompted, allow access to public and private networks.

 ![Screenshot of prompt to bypass Firewall](images/OpeningHerdPerms.png)

 - Open the Herd Dashboard once setup has completed.
 
 **Important Note:**  
 If prompted to enter a license key for Herd Pro, choose **Skip for now**. You do not need Herd Pro!

![Screenshot of Skip for Now button to bypass Herd Pro prompt](images/HerdProOptionSkipForNow.png)

 - On the left hand side, choose **Sites**
 - If prompted to choose a sites folder, we recommend using the default folder recommended by Herd.
 - Click the **Add Site** button.

![Screenshot of Laravel Herd showing the button to Add Site](images/HerdDashboardAddSite.png)

- Choose **New Laravel Project**
- Choose **Livewire** as your starter kit
- Enter details as per the below screenshot:

![Screenshot of new site details](images/NewLaravelProjectDetails.png)

- Once the site creation is complete, click **Open in Browser** to view the home page of your new site!

{{% /tab %}}
{{% tab title="_**Linux**_" %}}
The best way to create a new application on a Linux machine is from the command line.

In your terminal of choice, run `laravel new my-app`.

After creating your Laravel application, you only need to install its frontend dependencies via NPM and start the Laravel development server:

```
cd my-app
npm install && npm run build
composer run dev
```

{{% /tab %}}
{{< /tabs >}}

{{% notice info %}}
You should now have a home page that looks like this - if not don't worry, we'll troubleshoot in the next step!
{{% /notice %}}

![Default Starter Kit Home Page](images/StarterKitDefaultHomePage.png)

Next: [Testing your local environment](/laravel/testing-your-environment/)

