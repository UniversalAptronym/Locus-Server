To-do:
I'm pretty sure the current configuration I have leaves traffic readable by Cloudflare. Check if there's a way around this other than getting both parties to go through the hassle of Tailscale.  

These instructions will get you a web domain, with a unique URL, which as of 2024 costs ~$10/yr, along with the services of an organization known as Cloudlare to route web traffic through it.

First, go to [Cloudflare's website](https://www.cloudflare.com/) and click the `Sign Up` to make an account. Select the `Free` option.

Once you have an account, go to your [Cloudflare dashboard](https://dash.cloudflare.com). You should be at `Account Home`. If not, click that tab on the left. Click `Add A New Domain`, then `Or register a new domain ->`. Enter your desired URL into the search bar to see if it's available. We recommend selecting a **.org** or **.com** address, as these are open to anyone to register. `Confirm` your desired URL and purchase it. 

<img src="../Media_Repository/Cloudflare_Account_Home.png" alt="Cloudflare account home" title="Cloudflare account home" width="35%"/> <img src="../Media_Repository/Cloudflare_New_Domain_1.png" alt="Cloudflare new domain 1" title="Cloudflare new domain 1" width="25%"/> <img src="../Media_Repository/Cloudflare_New_Domain_2.png" alt="Cloudflare new domain 2" title="Cloudflare new domain 2" width="30%"/> 

**NOTE:** If you do not renew your URL when your payment period is finished, you will lose it. If you are using this for secure communication that is a security risk, as someone else could take the URL and pretend to be your secure server.
