Internet Defense League Anti-Censorship Education
=================================================
**This repo contains the information we show to help people bypass government
censorship. Please help us keep it up to date! (Pull requests welcome :)**

Background
----------
As the Internet evolves, many governments are implementing hostile regimes of
censorship, blocking access to parts of the Internet with the goal of
suppressing the free exchange of information and ideas. This is a threat to the
very fabric of the Internet and a violation of the human right to free speech.
Now, site owners can fight back using the
[Internet Defense League (IDL) Anti-Censorship Widget][1]. By pasting a few
lines of JavaScript code into your site, you can participate in a global network
of anti-censorship education.

The idea is simple: whenever a user visits your site from a country like China
or Iran, where the Internet is censored, the IDL Anti-Censorship Widget pops up
gives them information about how to bypass government censorship and get
unrestricted access to the full Internet. [You can read more about it here.][2]

But there's a challenge: government censorship practices are constantly
evolving, and we need to keep our educational efforts up to date. That's why we
need help from the Internet community to maintain the information we show to
users around the world, and that's what this project is all about.

This is where the IDL Anti-Censorship Widget pulls its information from. It's
basic HTML and CSS, and easy to edit. Please help us keep it up to date!
(Pull requests are very welcome and we are happy to answer any questions you
have about getting involved)

How to participate
------------------
This project contains pairs of HTML and CSS files organized by country. So, for
example, there's a folder called `CN` containing a pair of HTML and CSS files.
That's where we store the anti-censorship info for China, educating users about
how to get around the Great Firewall. If one day the Chinese government blocks
one of our circumvention techniques, we will need to update this info to stay
current with the latest way of getting through to the full Internet.

**Basic steps:**

* Fork this project
* Make the change you need
* Submit a pull request
* We'll pull your changes in and push it out to the network!

### Editing the HTML

The anti-censorship information for each country is stored in the `info.html`
file in that country's directory. There are two main segments to the html file:
a modal (stored in the `<div class="_ac_c">` block), and a details page (stored
in `<div id="_ac_moar" ...`). Editing either of these should be as easy for
anyone with basic HTML skills. Fork this code, make the change you want, and
then submit a pull request. We'll review it and pull it in!

### Editing the CSS

This should not be ordinarily necessary, but the CSS is in the `info.css` file
in each country's directory. Testing changes to the CSS is a bit treacherous
right now, but we will try to add a guide soon.

### Adding images

It's complicated to add images. Because of the encryption layer of the widget
(which makes it harder for governments to block), we can't pull in any remote
resources. So any images have to be included as Base64-encoded binary data in
the CSS file for a given country. For an example, see `CN/info.css`.

This also means that images should be very optimized and compressed, no more
than a few kilobytes. We are actually decrypting this data in the client
browser, and too much data will create too much overhead and impact performance
when the widget appears.

### Adding a new country

Simply take one of the existing countries, copy it into a new directory with the
correct two character ISO code, and customize the HTML / CSS as needed. Once we
pull your changes into the main repo and encrypt the data, it will start working
automatically.

Getting in touch
----------------
If you have any questions, please email me at jeff@fightforthefuture.org, or hit
me up on Twitter [@rubbingalcohol](https://twitter.com/rubbingalcohol).

[1]: https://www.internetdefenseleague.org
[2]: https://www.internetdefenseleague.org/censorship