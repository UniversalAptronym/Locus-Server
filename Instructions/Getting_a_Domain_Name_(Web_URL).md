to-do:
- I'm pretty sure the current configuration I have leaves traffic readable by Cloudflare. Check if there's a way around this other than getting both parties to go through the hassle of Tailscale.  
- We might also need to change the Zero Trust instructions for dietpi.

These instructions will get you a web domain, with a unique URL, which as of 2024 costs ~$10/yr, along with the services of an organization known as Cloudflare to route web traffic through it.

Note: Updates to Cloudflare's user interface may cause the website's layout to be different than the following pictures. Hopefully they will still be a helpful visual aid if so.

## __Instructions__

First, go to [IPchicken](https://ipchicken.com/) to find your router's **global IP address**. It should be of the form **XX.XXX.XXX.XX**. Save this.

Second, go to [Cloudflare's website](https://www.cloudflare.com/) and click the `Sign Up` to make an account. Select the `Free` option.

Once you have an account, go to your [Cloudflare dashboard](https://dash.cloudflare.com). You should be at `Account Home`. If not, click that tab on the left. Click `Add A New Domain`, then `Or register a new domain ->`. Enter your desired URL into the search bar to see if it's available. We recommend selecting a **.org** or **.com** address, as these are open to anyone to register. `Confirm` your desired URL and purchase it. 

<img src="../Media_Repository/Cloudflare_Account_Home.png" alt="Cloudflare account home" title="Cloudflare account home" width="35%"/> <img src="../Media_Repository/Cloudflare_New_Domain_1.png" alt="Cloudflare new domain 1" title="Cloudflare new domain 1" width="25%"/> <img src="../Media_Repository/Cloudflare_New_Domain_2.png" alt="Cloudflare new domain 2" title="Cloudflare new domain 2" width="30%"/> 

**NOTE:** If you do not renew your URL when your payment period is finished, you will lose it. If you are using this for secure communication that is a security risk, as someone else could take the URL and pretend to be your secure server.

Return to Cloudflare's `Account Home`. Click the `DNS` (Domain Name System) tab on the left, then click `Add A Record` (you may have to scroll down to find this). Make sure the `Type` field is **A**, the `Name` field is **@**, and the `Proxy Status` is **Proxied**. Enter the global IP address you found above into the `IPv4 address` field. Then click `Save`.



Note: If you move your equipment so that it is connected to a different internet router, during a home move for example, you will need to use [IPchicken](https://ipchicken.com/) to find your new global IP address and change the `IPv4 address` field here to that new value.

Next we will set up a "tunnel", which allows encryption and decrytion of information which passes through your web domain to occur safely within you self-hosted server. 

Return to `Account Home` (there is a back arrow in the top left which will take you there). Click `Zero Trust` on the left. Click `Networks` on the left. Click `Create a tunnel`. Select `Cloudflared`. Enter a tunnel name and click `Save Tunnel`. You do not have to record this name and it will be here on your Cloudflare account if you ever need it again. Select `Docker` (this is the operating software 

