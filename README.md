# Project

Public WiFi hotspots in a hotel, restaurant or train are generally unsafe. There is a risk of being eavesdropped or tracked by someone on the same network or by malicious software. A virtual private network (VPN) sends all data over an encrypted connection and offers a safe and secure path to the internet. There are hardly any Internet Service Providers (ISP) that provide VPN services to their customers and setting it up yourself is rather cumbersome. The few ones that do offer VPN haven’t been able to offer a modern and user-friendly experience to their users. There are a lot of other VPN solutions around, but most of them do not provide sufficient security en privacy to their users.

Let’s Connect! provides an open source VPN solution allowing ISPs, hosters and bussinesses to easily setup a secure VPN service. Even security minded people will be able to deploy it in a home environment. After deployment, users have a safe path from all generic devices.
Development

# Development
Let’s Connect! is being developed by SURFnet (the Dutch NREN) in collaboration with XS4ALL (a Dutch ISP). Everything is open source and the progress can be followed on GitHub. As of now we are starting so there are no packages available yet. We will post future updates on this website. SIDN Fonds provided the project with additional funding so user friendly apps can be developed for Let’s Connect!.

# Install

Since Let’s Connect! actually started out as eduVPN (our open source VPN service for the (higher) education and research in The Netherlands) the two projects are still quite intertwined. After finalising eduVPN we will make dedicated Let’s Connect! packages and applications and fill this GitHub repository. Of course you can already test eduVPN for yourself, since it will be very much the same as the final Let’s Connect! releases.


Below are the basic steps needed to install eduVPN on your hardware or VM.

### Requirements ###
* Practically any hardware (or VM) will do
* Clean Debian 9 Stretch, CentOS 7 or Fedora 26+
* SELinux has to be enabled on CentOS
* A working Internet connection
* Open ports tcp/80, tcp/443, udp/1194 and tcp/1194

### How to install ### 
Download the documentation repository on the host where you want to deploy:

    $ curl -L -O https://github.com/eduvpn/documentation/archive/master.tar.gz
Decompress the archive:

    $ tar -xzf master.tar.gz
Go to the document-master directory ($ cd documentation-master) and choose one of the following deploy scripts:

    deploy_debian.sh on Debian 9
    deploy_centos.sh on CentOS 7
    deploy_fedora.sh on Fedora 26+
Then run the script as root:

    $ sudo -s

    # ./deploy_distro.sh

And answer the questions in the script with something that makes sense for your deployment. After running the deploy script, it is time to configure Let’s Connect!. More on this is documented in the deploy documentation on Debian, CentOS and Fedora.


For detailed information and the source code, visit our [GitHub](https://github.com/eduVPN/documentation).


# Security Contact

If you find a security problem in the Let’s Connect! code, the deployed service(s) and want to
report it responsibly, contact [fkooman@tuxed.net](mailto:fkooman@tuxed.net). 
You can use PGP. My key is `0x9C5EDD645A571EB2`. The full fingerprint is 
`6237 BAF1 418A 907D AA98  EAA7 9C5E DD64 5A57 1EB2`.
