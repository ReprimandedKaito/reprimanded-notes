# Network cloaking
#Wireless #Networking

**Network cloaking** is an attempt to provide wireless security by hiding the SSID from being broadcast publicly. -- Wikipedia

What I wanted to learn is _technically_ how the SSID of "hidden networks" ([[Wifi]]) can be discovered.

---

> Some examples of these sniffing programs include the following:
>
> **Passive**:
>   - \[...]
>   - [Kismet](https://en.wikipedia.org/wiki/Kismet_(software))
>       * https://www.KismetWireless.net
>       * [ ] KAITO: The same program whose UX I loved from BackTrack? Try it (again)!
>       * [ ] KAITO: List all BackTrack 5 programs that have a GUI or a TUI!
>
> **Active**:
>   - \[...]
>   - [inSSIDer](https://en.wikipedia.org/wiki/InSSIDer)
>       * [ ] KAITO: Used by that CBT Nuggets wifi dude. Try it!
>
> These programs are then able to discover the cloaked networks and their SSIDs through picking through frames of information such as:
> 
>   - **Probe request frames**.
>     Probe request frames are sent unencrypted by the client computer when trying to connect to a network. This unprotected frame of information, which can easily be intercepted and read by someone willing, will contain the SSID.
>
>   - **Probe response frames**.
>     In response to the probe request, the requested station will send back a frame of information also containing the SSID as well as other details about the network.
>
>   - **Association request frames**.
>     An association request frame is what begins the process of initializing a relationship between the computer and the access point. Once associated properly, the AP will be able to assign some of its resources to the network interface controller (NIC). Once again, through this process, the SSID is transmitted.
>
>   - **Re-association request frames**.
>     Re-association request frames are transmitted when a NIC notices a stronger signal from another access point and switches over from the previous one. This new access point will then "take over" and handle the data that may still be caught up in the previous session. The request of a new connection to a new beacon signal will of course require the transmission of a new SSID.
>
> Because of these multiple ways the network name is still being broadcast while the network is "cloaked," it is not completely hidden from persistent hackers.
> Worse still, because a station must probe for a hidden SSID, a fake access point can offer a connection. Programs that act as fake access points are freely available; e.g. airbase-ng and Karma.
>
> -- [Network cloaking &sect; "Disadvantages"](https://en.wikipedia.org/wiki/Network_cloaking)

---

_#linesilike_ about security:

> \[...]
>
> So there you have it, simple SSID discovery. The old axiom remains true: security by obscurity is no security at all. Hiding an SSID will not hide a wireless network, so ignore any such advice -- and it's amazing how often I continue to see this. By the way, also ignore any advice that says to use MAC address filtering. It's amazingly trivial to spoof the MAC address of an allowed supplicant -- simply sniff the traffic, look at the MAC addresses, and \[...] change your MAC to one that's permitted.
>
> -- [Myth vs. reality: Wireless SSIDs - Steve Riley on Security - TechNet Blogs `[archived]`](http://web.archive.org/web/20100605232458/http://blogs.technet.com/b/steriley/archive/2007/10/16/myth-vs-reality-wireless-ssids.aspx)

(Referenced by Wikipedia.)

---

FIN.
