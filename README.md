# I use Arch btw

I build and run websites and web apps for clients through my business, Virtual Vince.
Lately I've been moving toward embedded and backend systems work, which is where I want
to end up.

## Orpheus

Version control for music production. Git handles DAW projects badly because they are
large binary files, so changing one note looks like rewriting the whole thing. Orpheus
makes them properly diffable.

I work on the backend, the Convex schema and the track mutations, and the validation on
everything that gets written to the database.

## Elizabeth Gardens Creative Collective

A community arts organization running on a VPS I set up and administer. Bare Ubuntu
Server upward, HestiaCP, user accounts, DNS, firewall, and my own backups. It is
multi-tenant, hosting other artists alongside the main site.

I wrote 11 WordPress plugins for it. They create the pages, navigation, layouts, forms
and content programmatically, so the site structure lives in version control.

The coolest was the activity log. It makes its own database table, keeps a schema version
for migrations, lets you exclude accounts, and captures the exact diff of every content
edit along with plugin and publishing events. The board can see who changed what.

## ChironAI

The AI side of my business. Training teams to use AI properly, agent setup, and
automation for small businesses. Most of it is unglamorous, which is the point.
Businesses do not need a new model, they need the boring integration around it to be
reliable.

[chiron.virtualvince.ca](https://chiron.virtualvince.ca/)

## Client work

- [Radiant Roots Vitality](https://www.radiantrootsvitality.com/), a health practice.
  Next.js, TypeScript and Tailwind, with Google Maps and a Fullscript handoff. I host and
  maintain it on a monthly retainer.
- [My YAYBI Way](https://myyaybiway.me/). Next.js, TypeScript and Tailwind, pulling live
  products and images from a Shopify storefront into a custom front end.
- [K2E Canada](https://www.k2e.ca/), professional education. Shopify with custom Liquid.

## Arduino

[r3builds](https://github.com/VirtualVince/R3Builds) is ten small builds, ordered so each
one teaches something the next one needs. GPIO and timing, debounce, PWM, UART, ADC, I2C,
SPI, a sensor to actuator control loop, a state machine, and IR decode into actuation.
Next is PID and IMU work, SDR, and embedded Linux.

## Tools

Go, TypeScript, Python, C++, C#, Java, PHP, SQL, Lua. Linux, Ubuntu Server, HestiaCP, DNS
and firewalls. Node, Express, Next.js, React, Angular, ASP.NET. PostgreSQL, MongoDB,
MySQL, SQLite, Convex. AWS, Azure, GCP, Vercel. Arduino and C for microcontrollers. Arch,
fish, Neovim.

[virtualvince.ca](https://virtualvince.ca) ·
[LinkedIn](https://www.linkedin.com/in/vincente-sequeira-1824b4245/) ·
[YouTube](https://www.youtube.com/@virtualvincebuilds)
